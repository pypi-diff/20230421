# Comparing `tmp/control-lab-ly-1.0.0b1.tar.gz` & `tmp/control-lab-ly-1.0.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "control-lab-ly-1.0.0b1.tar", last modified: Wed Apr 12 16:17:50 2023, max compression
+gzip compressed data, was "control-lab-ly-1.0.1a0.tar", last modified: Fri Apr 21 08:38:54 2023, max compression
```

## Comparing `control-lab-ly-1.0.0b1.tar` & `control-lab-ly-1.0.1a0.tar`

### file list

```diff
@@ -1,218 +1,218 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 16:17:50.171707 control-lab-ly-1.0.0b1/
--rw-rw-rw-   0        0        0     1093 2023-02-24 13:59:16.000000 control-lab-ly-1.0.0b1/LICENSE.md
--rw-rw-rw-   0        0        0       17 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b1/MANIFEST.in
--rw-rw-rw-   0        0        0    17453 2023-04-12 16:17:50.171707 control-lab-ly-1.0.0b1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-12 16:17:48.838090 control-lab-ly-1.0.0b1/docs/
--rw-rw-rw-   0        0        0     4263 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/docs/CHANGELOG.md
--rw-rw-rw-   0        0        0     5356 2023-02-24 14:06:11.000000 control-lab-ly-1.0.0b1/docs/CODE_OF_CONDUCT.md
--rw-rw-rw-   0        0        0       33 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0b1/docs/CONTRIBUTING.md
--rw-rw-rw-   0        0        0     1093 2023-02-24 13:59:16.000000 control-lab-ly-1.0.0b1/docs/LICENSE.md
--rw-rw-rw-   0        0        0    12070 2023-04-12 16:03:24.000000 control-lab-ly-1.0.0b1/docs/README.md
--rw-rw-rw-   0        0        0      108 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0b1/pyproject.toml
--rw-rw-rw-   0        0        0     1561 2023-04-12 16:17:50.179682 control-lab-ly-1.0.0b1/setup.cfg
--rw-rw-rw-   0        0        0       37 2023-03-10 02:02:34.000000 control-lab-ly-1.0.0b1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-12 16:17:48.471823 control-lab-ly-1.0.0b1/src/
-drwxrwxrwx   0        0        0        0 2023-04-12 16:17:48.876290 control-lab-ly-1.0.0b1/src/control_lab_ly.egg-info/
--rw-rw-rw-   0        0        0    17453 2023-04-12 16:17:48.000000 control-lab-ly-1.0.0b1/src/control_lab_ly.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7306 2023-04-12 16:17:48.000000 control-lab-ly-1.0.0b1/src/control_lab_ly.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 16:17:48.000000 control-lab-ly-1.0.0b1/src/control_lab_ly.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      214 2023-04-12 16:17:48.000000 control-lab-ly-1.0.0b1/src/control_lab_ly.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-12 16:17:48.000000 control-lab-ly-1.0.0b1/src/control_lab_ly.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-12 16:17:48.888031 control-lab-ly-1.0.0b1/src/controllably/
-drwxrwxrwx   0        0        0        0 2023-04-12 16:17:48.888531 control-lab-ly-1.0.0b1/src/controllably/Analyse/
-drwxrwxrwx   0        0        0        0 2023-04-12 16:17:48.900491 control-lab-ly-1.0.0b1/src/controllably/Analyse/Data/
-drwxrwxrwx   0        0        0        0 2023-04-12 16:17:48.913840 control-lab-ly-1.0.0b1/src/controllably/Analyse/Data/Database/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b1/src/controllably/Analyse/Data/Database/__init__.py
--rw-rw-rw-   0        0        0     3029 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b1/src/controllably/Analyse/Data/Database/database_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-12 16:17:48.969298 control-lab-ly-1.0.0b1/src/controllably/Analyse/Data/Types/
--rw-rw-rw-   0        0        0      277 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b1/src/controllably/Analyse/Data/Types/__init__.py
--rw-rw-rw-   0        0        0     6448 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b1/src/controllably/Analyse/Data/Types/circuit_datatype.py
--rw-rw-rw-   0        0        0    26583 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b1/src/controllably/Analyse/Data/Types/eis_datatype.py
--rw-rw-rw-   0        0        0      956 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b1/src/controllably/Analyse/Data/Types/eis_test_circuits.yaml
--rw-rw-rw-   0        0        0     1585 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b1/src/controllably/Analyse/Data/Types/eis_tests.json
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b1/src/controllably/Analyse/Data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 16:17:48.986690 control-lab-ly-1.0.0b1/src/controllably/Analyse/Visualisation/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b1/src/controllably/Analyse/Visualisation/__init__.py
--rw-rw-rw-   0        0        0      830 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b1/src/controllably/Analyse/Visualisation/visualisation_utils.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b1/src/controllably/Analyse/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.000168 control-lab-ly-1.0.0b1/src/controllably/Compound/
-drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.008764 control-lab-ly-1.0.0b1/src/controllably/Compound/LiquidMover/
-drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.032998 control-lab-ly-1.0.0b1/src/controllably/Compound/LiquidMover/Opentrons/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b1/src/controllably/Compound/LiquidMover/Opentrons/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b1/src/controllably/Compound/LiquidMover/Opentrons/opentrons_utils.py
--rw-rw-rw-   0        0        0      259 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Compound/LiquidMover/__init__.py
--rw-rw-rw-   0        0        0    14057 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Compound/LiquidMover/liquidmover_utils.py
--rw-rw-rw-   0        0        0      241 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Compound/__init__.py
--rw-rw-rw-   0        0        0     8733 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Compound/compound_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.041011 control-lab-ly-1.0.0b1/src/controllably/Control/
-drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.088431 control-lab-ly-1.0.0b1/src/controllably/Control/GUI/
--rw-rw-rw-   0        0        0      516 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Control/GUI/__init__.py
--rw-rw-rw-   0        0        0    30932 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b1/src/controllably/Control/GUI/_guibuilder.py
--rw-rw-rw-   0        0        0    17704 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Control/GUI/gui_utils.py
--rw-rw-rw-   0        0        0      886 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Control/GUI/loader_panel.py
--rw-rw-rw-   0        0        0     8608 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Control/GUI/measurer_panel.py
--rw-rw-rw-   0        0        0    15405 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Control/GUI/mover_panel.py
--rw-rw-rw-   0        0        0     3624 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Control/GUI/viewer_panel.py
-drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.104577 control-lab-ly-1.0.0b1/src/controllably/Control/Schedule/
--rw-rw-rw-   0        0        0      147 2023-04-11 14:01:57.000000 control-lab-ly-1.0.0b1/src/controllably/Control/Schedule/__init__.py
--rw-rw-rw-   0        0        0     1868 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Control/Schedule/schedule_utils.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b1/src/controllably/Control/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.138113 control-lab-ly-1.0.0b1/src/controllably/Make/
-drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.161937 control-lab-ly-1.0.0b1/src/controllably/Make/Heat/
--rw-rw-rw-   0        0        0      225 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Make/Heat/__init__.py
--rw-rw-rw-   0        0        0    10393 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Make/Heat/peltier_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.180861 control-lab-ly-1.0.0b1/src/controllably/Make/Light/
--rw-rw-rw-   0        0        0      218 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Make/Light/__init__.py
--rw-rw-rw-   0        0        0     9094 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Make/Light/led_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.192798 control-lab-ly-1.0.0b1/src/controllably/Make/Mixture/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b1/src/controllably/Make/Mixture/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.204931 control-lab-ly-1.0.0b1/src/controllably/Make/ThinFilm/
--rw-rw-rw-   0        0        0      268 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Make/ThinFilm/__init__.py
--rw-rw-rw-   0        0        0     9660 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Make/ThinFilm/spinner_utils.py
--rw-rw-rw-   0        0        0      217 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Make/__init__.py
--rw-rw-rw-   0        0        0     3956 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Make/make_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.242247 control-lab-ly-1.0.0b1/src/controllably/Measure/
-drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.258192 control-lab-ly-1.0.0b1/src/controllably/Measure/Electrical/
-drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.297193 control-lab-ly-1.0.0b1/src/controllably/Measure/Electrical/Keithley/
--rw-rw-rw-   0        0        0      314 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Measure/Electrical/Keithley/__init__.py
--rw-rw-rw-   0        0        0    18015 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Measure/Electrical/Keithley/keithley_device.py
--rw-rw-rw-   0        0        0     7492 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Measure/Electrical/Keithley/keithley_lib.py
--rw-rw-rw-   0        0        0     2102 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Measure/Electrical/Keithley/keithley_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.347618 control-lab-ly-1.0.0b1/src/controllably/Measure/Electrical/Keithley/programs/
--rw-rw-rw-   0        0        0      401 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Measure/Electrical/Keithley/programs/__init__.py
--rw-rw-rw-   0        0        0    10256 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Measure/Electrical/Keithley/programs/base_programs.py
--rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b1/src/controllably/Measure/Electrical/__init__.py
--rw-rw-rw-   0        0        0      298 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Measure/Electrical/electrical_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.364957 control-lab-ly-1.0.0b1/src/controllably/Measure/Mechanical/
-drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.400897 control-lab-ly-1.0.0b1/src/controllably/Measure/Mechanical/PiezoRobotics/
--rw-rw-rw-   0        0        0      334 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Measure/Mechanical/PiezoRobotics/__init__.py
--rw-rw-rw-   0        0        0    10329 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_device.py
--rw-rw-rw-   0        0        0     3163 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_lib.py
--rw-rw-rw-   0        0        0     2093 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.427094 control-lab-ly-1.0.0b1/src/controllably/Measure/Mechanical/PiezoRobotics/programs/
--rw-rw-rw-   0        0        0      350 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Measure/Mechanical/PiezoRobotics/programs/__init__.py
--rw-rw-rw-   0        0        0     3973 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Measure/Mechanical/PiezoRobotics/programs/base_programs.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b1/src/controllably/Measure/Mechanical/__init__.py
--rw-rw-rw-   0        0        0      298 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Measure/Mechanical/mechanical_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.439540 control-lab-ly-1.0.0b1/src/controllably/Measure/Physical/
--rw-rw-rw-   0        0        0      249 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Measure/Physical/__init__.py
--rw-rw-rw-   0        0        0     7972 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Measure/Physical/balance_utils.py
--rw-rw-rw-   0        0        0      535 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Measure/__init__.py
--rw-rw-rw-   0        0        0     5398 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Measure/instrument_utils.py
--rw-rw-rw-   0        0        0    13804 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Measure/measure_utils.py
--rw-rw-rw-   0        0        0     4176 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Measure/program_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.453245 control-lab-ly-1.0.0b1/src/controllably/Move/
-drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.488972 control-lab-ly-1.0.0b1/src/controllably/Move/Cartesian/
--rw-rw-rw-   0        0        0      346 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Move/Cartesian/__init__.py
--rw-rw-rw-   0        0        0     9049 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Move/Cartesian/cartesian_utils.py
--rw-rw-rw-   0        0        0     3402 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Move/Cartesian/ender_utils.py
--rw-rw-rw-   0        0        0     2853 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Move/Cartesian/primitiv_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.497074 control-lab-ly-1.0.0b1/src/controllably/Move/Jointed/
-drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.528975 control-lab-ly-1.0.0b1/src/controllably/Move/Jointed/Dobot/
--rw-rw-rw-   0        0        0      336 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Move/Jointed/Dobot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.543968 control-lab-ly-1.0.0b1/src/controllably/Move/Jointed/Dobot/dobot_api/
--rw-rw-rw-   0        0        0       62 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b1/src/controllably/Move/Jointed/Dobot/dobot_api/__init__.py
--rw-rw-rw-   0        0        0    24262 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b1/src/controllably/Move/Jointed/Dobot/dobot_api/dobot_api.py
--rw-rw-rw-   0        0        0    15851 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Move/Jointed/Dobot/dobot_utils.py
--rw-rw-rw-   0        0        0     7030 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Move/Jointed/Dobot/m1pro_utils.py
--rw-rw-rw-   0        0        0     4325 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Move/Jointed/Dobot/mg400_utils.py
--rw-rw-rw-   0        0        0      233 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Move/Jointed/__init__.py
--rw-rw-rw-   0        0        0    10507 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Move/Jointed/jointed_utils.py
--rw-rw-rw-   0        0        0      217 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Move/__init__.py
--rw-rw-rw-   0        0        0    32152 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Move/move_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.563012 control-lab-ly-1.0.0b1/src/controllably/Transfer/
-drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.594517 control-lab-ly-1.0.0b1/src/controllably/Transfer/Liquid/
-drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.612438 control-lab-ly-1.0.0b1/src/controllably/Transfer/Liquid/Pumps/
-drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.637624 control-lab-ly-1.0.0b1/src/controllably/Transfer/Liquid/Pumps/TriContinent/
--rw-rw-rw-   0        0        0      255 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Transfer/Liquid/Pumps/TriContinent/__init__.py
--rw-rw-rw-   0        0        0     3460 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_lib.py
--rw-rw-rw-   0        0        0    29831 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_utils.py
--rw-rw-rw-   0        0        0      332 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Transfer/Liquid/Pumps/__init__.py
--rw-rw-rw-   0        0        0     9064 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Transfer/Liquid/Pumps/peristaltic_utils.py
--rw-rw-rw-   0        0        0     3097 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Transfer/Liquid/Pumps/pump_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.669182 control-lab-ly-1.0.0b1/src/controllably/Transfer/Liquid/Sartorius/
--rw-rw-rw-   0        0        0      252 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Transfer/Liquid/Sartorius/__init__.py
--rw-rw-rw-   0        0        0     3210 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Transfer/Liquid/Sartorius/sartorius_lib.py
--rw-rw-rw-   0        0        0    30582 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Transfer/Liquid/Sartorius/sartorius_utils.py
--rw-rw-rw-   0        0        0      364 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Transfer/Liquid/__init__.py
--rw-rw-rw-   0        0        0    13126 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Transfer/Liquid/liquid_utils.py
--rw-rw-rw-   0        0        0     3413 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Transfer/Liquid/syringe_lib.py
--rw-rw-rw-   0        0        0    14619 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Transfer/Liquid/syringe_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.677392 control-lab-ly-1.0.0b1/src/controllably/Transfer/Powder/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b1/src/controllably/Transfer/Powder/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.691909 control-lab-ly-1.0.0b1/src/controllably/Transfer/Substrate/
-drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.709325 control-lab-ly-1.0.0b1/src/controllably/Transfer/Substrate/Dobot/
--rw-rw-rw-   0        0        0      348 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Transfer/Substrate/Dobot/__init__.py
--rw-rw-rw-   0        0        0     8255 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Transfer/Substrate/Dobot/dobot_attachments.py
--rw-rw-rw-   0        0        0      238 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Transfer/Substrate/__init__.py
--rw-rw-rw-   0        0        0     1032 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Transfer/Substrate/substrate_utils.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b1/src/controllably/Transfer/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b1/src/controllably/Transfer/transfer_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.726902 control-lab-ly-1.0.0b1/src/controllably/View/
-drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.789816 control-lab-ly-1.0.0b1/src/controllably/View/Classifiers/
--rw-rw-rw-   0        0        0      333 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/View/Classifiers/__init__.py
--rw-rw-rw-   0        0        0     2586 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/View/Classifiers/classifier_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.807821 control-lab-ly-1.0.0b1/src/controllably/View/Optical/
--rw-rw-rw-   0        0        0      219 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/View/Optical/__init__.py
--rw-rw-rw-   0        0        0     3163 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/View/Optical/optical_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.822632 control-lab-ly-1.0.0b1/src/controllably/View/Optical/placeholders/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b1/src/controllably/View/Optical/placeholders/__init__.py
--rw-rw-rw-   0        0        0    15567 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0b1/src/controllably/View/Optical/placeholders/optical_camera.png
-drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.840468 control-lab-ly-1.0.0b1/src/controllably/View/Thermal/
-drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.840468 control-lab-ly-1.0.0b1/src/controllably/View/Thermal/Flir/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0b1/src/controllably/View/Thermal/Flir/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.892068 control-lab-ly-1.0.0b1/src/controllably/View/Thermal/Flir/ax8/
--rw-rw-rw-   0        0        0       33 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0b1/src/controllably/View/Thermal/Flir/ax8/__init__.py
--rw-rw-rw-   0        0        0    10147 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0b1/src/controllably/View/Thermal/Flir/ax8/ax8.py
--rw-rw-rw-   0        0        0     3821 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0b1/src/controllably/View/Thermal/Flir/ax8/ax8_camera_feed.py
--rw-rw-rw-   0        0        0      636 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0b1/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_regs.py
--rw-rw-rw-   0        0        0      819 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0b1/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_utils.py
--rw-rw-rw-   0        0        0      219 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/View/Thermal/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.901301 control-lab-ly-1.0.0b1/src/controllably/View/Thermal/placeholders/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0b1/src/controllably/View/Thermal/placeholders/__init__.py
--rw-rw-rw-   0        0        0   148660 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0b1/src/controllably/View/Thermal/placeholders/infrared_camera.png
--rw-rw-rw-   0        0        0     2983 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/View/Thermal/thermal_utils.py
--rw-rw-rw-   0        0        0      294 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/View/__init__.py
--rw-rw-rw-   0        0        0    15729 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/View/image_utils.py
--rw-rw-rw-   0        0        0    17366 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/View/view_utils.py
--rw-rw-rw-   0        0        0       98 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.953432 control-lab-ly-1.0.0b1/src/controllably/misc/
--rw-rw-rw-   0        0        0      586 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/misc/__init__.py
--rw-rw-rw-   0        0        0     2522 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/misc/decorators.py
--rw-rw-rw-   0        0        0    10014 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/misc/factory.py
--rw-rw-rw-   0        0        0     6551 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/misc/helper.py
--rw-rw-rw-   0        0        0    17274 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/misc/layout.py
--rw-rw-rw-   0        0        0     2867 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/misc/logger.py
--rw-rw-rw-   0        0        0     4576 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/misc/misc_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.961830 control-lab-ly-1.0.0b1/src/controllably/misc/templates/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0b1/src/controllably/misc/templates/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.970917 control-lab-ly-1.0.0b1/src/controllably/misc/templates/configs/
--rw-rw-rw-   0        0        0        0 2023-02-23 14:08:10.000000 control-lab-ly-1.0.0b1/src/controllably/misc/templates/configs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.996091 control-lab-ly-1.0.0b1/src/controllably/misc/templates/configs/plugins/
--rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b1/src/controllably/misc/templates/configs/plugins/__init__.py
--rw-rw-rw-   0        0        0     1091 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/misc/templates/configs/plugins/plugin_template.py
--rw-rw-rw-   0        0        0      439 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/misc/templates/configs/registry.yaml
-drwxrwxrwx   0        0        0        0 2023-04-12 16:17:50.018630 control-lab-ly-1.0.0b1/src/controllably/misc/templates/setup/
--rw-rw-rw-   0        0        0      772 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/misc/templates/setup/__init__.py
--rw-rw-rw-   0        0        0     1434 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/misc/templates/setup/config.yaml
--rw-rw-rw-   0        0        0      987 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/misc/templates/setup/layout.json
-drwxrwxrwx   0        0        0        0 2023-04-12 16:17:50.163669 control-lab-ly-1.0.0b1/tests/
--rw-rw-rw-   0        0        0      189 2023-04-11 09:35:43.000000 control-lab-ly-1.0.0b1/tests/test_camera_optical.py
--rw-rw-rw-   0        0        0      230 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b1/tests/test_camera_thermal.py
--rw-rw-rw-   0        0        0      509 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b1/tests/test_cartesian_ender.py
--rw-rw-rw-   0        0        0      429 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b1/tests/test_cartesian_primitiv.py
--rw-rw-rw-   0        0        0      585 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b1/tests/test_compound_liquidmover.py
--rw-rw-rw-   0        0        0      801 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b1/tests/test_compound_spin_printer.py
--rw-rw-rw-   0        0        0      616 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b1/tests/test_dobot_m1pro.py
--rw-rw-rw-   0        0        0      651 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b1/tests/test_dobot_mg400.py
--rw-rw-rw-   0        0        0      324 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b1/tests/test_electrical_keithley.py
--rw-rw-rw-   0        0        0      392 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b1/tests/test_film_spin.py
--rw-rw-rw-   0        0        0      587 2023-04-11 09:21:52.000000 control-lab-ly-1.0.0b1/tests/test_heat_peltier.py
--rw-rw-rw-   0        0        0      349 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b1/tests/test_light_led_array.py
--rw-rw-rw-   0        0        0      362 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b1/tests/test_liquid_sartorius.py
--rw-rw-rw-   0        0        0      412 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b1/tests/test_liquid_syringe_assembly.py
--rw-rw-rw-   0        0        0      538 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/tests/test_liquid_tricontinent.py
--rw-rw-rw-   0        0        0      239 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b1/tests/test_mechanical_piezorobotics.py
--rw-rw-rw-   0        0        0      268 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b1/tests/test_panels.py
--rw-rw-rw-   0        0        0      273 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b1/tests/test_physical_balance.py
--rw-rw-rw-   0        0        0      337 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b1/tests/test_pump_peristaltic.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:38:54.105082 control-lab-ly-1.0.1a0/
+-rw-rw-rw-   0        0        0     1093 2023-02-24 13:59:16.000000 control-lab-ly-1.0.1a0/LICENSE.md
+-rw-rw-rw-   0        0        0       17 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a0/MANIFEST.in
+-rw-rw-rw-   0        0        0    17492 2023-04-21 08:38:54.109880 control-lab-ly-1.0.1a0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-21 08:38:52.207903 control-lab-ly-1.0.1a0/docs/
+-rw-rw-rw-   0        0        0     4263 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/docs/CHANGELOG.md
+-rw-rw-rw-   0        0        0     5356 2023-02-24 14:06:11.000000 control-lab-ly-1.0.1a0/docs/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0        0        0       33 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a0/docs/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0     1093 2023-02-24 13:59:16.000000 control-lab-ly-1.0.1a0/docs/LICENSE.md
+-rw-rw-rw-   0        0        0    12109 2023-04-21 06:54:10.000000 control-lab-ly-1.0.1a0/docs/README.md
+-rw-rw-rw-   0        0        0      108 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a0/pyproject.toml
+-rw-rw-rw-   0        0        0     1559 2023-04-21 08:38:54.150031 control-lab-ly-1.0.1a0/setup.cfg
+-rw-rw-rw-   0        0        0       37 2023-03-10 02:02:34.000000 control-lab-ly-1.0.1a0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:38:51.822740 control-lab-ly-1.0.1a0/src/
+drwxrwxrwx   0        0        0        0 2023-04-21 08:38:52.236169 control-lab-ly-1.0.1a0/src/control_lab_ly.egg-info/
+-rw-rw-rw-   0        0        0    17492 2023-04-21 08:38:51.000000 control-lab-ly-1.0.1a0/src/control_lab_ly.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7306 2023-04-21 08:38:51.000000 control-lab-ly-1.0.1a0/src/control_lab_ly.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 08:38:51.000000 control-lab-ly-1.0.1a0/src/control_lab_ly.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      214 2023-04-21 08:38:51.000000 control-lab-ly-1.0.1a0/src/control_lab_ly.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-21 08:38:51.000000 control-lab-ly-1.0.1a0/src/control_lab_ly.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 08:38:52.239957 control-lab-ly-1.0.1a0/src/controllably/
+drwxrwxrwx   0        0        0        0 2023-04-21 08:38:52.242946 control-lab-ly-1.0.1a0/src/controllably/Analyse/
+drwxrwxrwx   0        0        0        0 2023-04-21 08:38:52.253273 control-lab-ly-1.0.1a0/src/controllably/Analyse/Data/
+drwxrwxrwx   0        0        0        0 2023-04-21 08:38:52.267345 control-lab-ly-1.0.1a0/src/controllably/Analyse/Data/Database/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a0/src/controllably/Analyse/Data/Database/__init__.py
+-rw-rw-rw-   0        0        0     3029 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a0/src/controllably/Analyse/Data/Database/database_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:38:52.301990 control-lab-ly-1.0.1a0/src/controllably/Analyse/Data/Types/
+-rw-rw-rw-   0        0        0      277 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a0/src/controllably/Analyse/Data/Types/__init__.py
+-rw-rw-rw-   0        0        0     6448 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a0/src/controllably/Analyse/Data/Types/circuit_datatype.py
+-rw-rw-rw-   0        0        0    26583 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a0/src/controllably/Analyse/Data/Types/eis_datatype.py
+-rw-rw-rw-   0        0        0      956 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a0/src/controllably/Analyse/Data/Types/eis_test_circuits.yaml
+-rw-rw-rw-   0        0        0     1585 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a0/src/controllably/Analyse/Data/Types/eis_tests.json
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a0/src/controllably/Analyse/Data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:38:52.321851 control-lab-ly-1.0.1a0/src/controllably/Analyse/Visualisation/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a0/src/controllably/Analyse/Visualisation/__init__.py
+-rw-rw-rw-   0        0        0      830 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a0/src/controllably/Analyse/Visualisation/visualisation_utils.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a0/src/controllably/Analyse/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:38:52.333070 control-lab-ly-1.0.1a0/src/controllably/Compound/
+drwxrwxrwx   0        0        0        0 2023-04-21 08:38:52.340050 control-lab-ly-1.0.1a0/src/controllably/Compound/LiquidMover/
+drwxrwxrwx   0        0        0        0 2023-04-21 08:38:52.361819 control-lab-ly-1.0.1a0/src/controllably/Compound/LiquidMover/Opentrons/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a0/src/controllably/Compound/LiquidMover/Opentrons/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a0/src/controllably/Compound/LiquidMover/Opentrons/opentrons_utils.py
+-rw-rw-rw-   0        0        0      259 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Compound/LiquidMover/__init__.py
+-rw-rw-rw-   0        0        0    16608 2023-04-21 08:35:19.000000 control-lab-ly-1.0.1a0/src/controllably/Compound/LiquidMover/liquidmover_utils.py
+-rw-rw-rw-   0        0        0      241 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Compound/__init__.py
+-rw-rw-rw-   0        0        0     8151 2023-04-21 07:30:47.000000 control-lab-ly-1.0.1a0/src/controllably/Compound/compound_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:38:52.374884 control-lab-ly-1.0.1a0/src/controllably/Control/
+drwxrwxrwx   0        0        0        0 2023-04-21 08:38:52.448785 control-lab-ly-1.0.1a0/src/controllably/Control/GUI/
+-rw-rw-rw-   0        0        0      516 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Control/GUI/__init__.py
+-rw-rw-rw-   0        0        0    30932 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a0/src/controllably/Control/GUI/_guibuilder.py
+-rw-rw-rw-   0        0        0    17704 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Control/GUI/gui_utils.py
+-rw-rw-rw-   0        0        0      886 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Control/GUI/loader_panel.py
+-rw-rw-rw-   0        0        0     8608 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Control/GUI/measurer_panel.py
+-rw-rw-rw-   0        0        0    15405 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Control/GUI/mover_panel.py
+-rw-rw-rw-   0        0        0     3624 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Control/GUI/viewer_panel.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:38:52.462459 control-lab-ly-1.0.1a0/src/controllably/Control/Schedule/
+-rw-rw-rw-   0        0        0      147 2023-04-11 14:01:57.000000 control-lab-ly-1.0.1a0/src/controllably/Control/Schedule/__init__.py
+-rw-rw-rw-   0        0        0     1868 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Control/Schedule/schedule_utils.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a0/src/controllably/Control/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:38:52.491092 control-lab-ly-1.0.1a0/src/controllably/Make/
+drwxrwxrwx   0        0        0        0 2023-04-21 08:38:52.531957 control-lab-ly-1.0.1a0/src/controllably/Make/Heat/
+-rw-rw-rw-   0        0        0      225 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Make/Heat/__init__.py
+-rw-rw-rw-   0        0        0    10517 2023-04-21 07:30:47.000000 control-lab-ly-1.0.1a0/src/controllably/Make/Heat/peltier_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:38:52.547863 control-lab-ly-1.0.1a0/src/controllably/Make/Light/
+-rw-rw-rw-   0        0        0      218 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Make/Light/__init__.py
+-rw-rw-rw-   0        0        0     9094 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Make/Light/led_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:38:52.569861 control-lab-ly-1.0.1a0/src/controllably/Make/Mixture/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a0/src/controllably/Make/Mixture/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:38:52.600664 control-lab-ly-1.0.1a0/src/controllably/Make/ThinFilm/
+-rw-rw-rw-   0        0        0      268 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Make/ThinFilm/__init__.py
+-rw-rw-rw-   0        0        0     9660 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Make/ThinFilm/spinner_utils.py
+-rw-rw-rw-   0        0        0      217 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Make/__init__.py
+-rw-rw-rw-   0        0        0     3956 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Make/make_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:38:52.659207 control-lab-ly-1.0.1a0/src/controllably/Measure/
+drwxrwxrwx   0        0        0        0 2023-04-21 08:38:52.665311 control-lab-ly-1.0.1a0/src/controllably/Measure/Electrical/
+drwxrwxrwx   0        0        0        0 2023-04-21 08:38:52.711248 control-lab-ly-1.0.1a0/src/controllably/Measure/Electrical/Keithley/
+-rw-rw-rw-   0        0        0      314 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Measure/Electrical/Keithley/__init__.py
+-rw-rw-rw-   0        0        0    18015 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Measure/Electrical/Keithley/keithley_device.py
+-rw-rw-rw-   0        0        0     7492 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Measure/Electrical/Keithley/keithley_lib.py
+-rw-rw-rw-   0        0        0     2102 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Measure/Electrical/Keithley/keithley_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:38:52.755782 control-lab-ly-1.0.1a0/src/controllably/Measure/Electrical/Keithley/programs/
+-rw-rw-rw-   0        0        0      401 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Measure/Electrical/Keithley/programs/__init__.py
+-rw-rw-rw-   0        0        0    10256 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Measure/Electrical/Keithley/programs/base_programs.py
+-rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a0/src/controllably/Measure/Electrical/__init__.py
+-rw-rw-rw-   0        0        0      298 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Measure/Electrical/electrical_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:38:52.767824 control-lab-ly-1.0.1a0/src/controllably/Measure/Mechanical/
+drwxrwxrwx   0        0        0        0 2023-04-21 08:38:52.820453 control-lab-ly-1.0.1a0/src/controllably/Measure/Mechanical/PiezoRobotics/
+-rw-rw-rw-   0        0        0      334 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Measure/Mechanical/PiezoRobotics/__init__.py
+-rw-rw-rw-   0        0        0    10329 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_device.py
+-rw-rw-rw-   0        0        0     3163 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_lib.py
+-rw-rw-rw-   0        0        0     2093 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:38:52.861104 control-lab-ly-1.0.1a0/src/controllably/Measure/Mechanical/PiezoRobotics/programs/
+-rw-rw-rw-   0        0        0      350 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Measure/Mechanical/PiezoRobotics/programs/__init__.py
+-rw-rw-rw-   0        0        0     3973 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Measure/Mechanical/PiezoRobotics/programs/base_programs.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a0/src/controllably/Measure/Mechanical/__init__.py
+-rw-rw-rw-   0        0        0      298 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Measure/Mechanical/mechanical_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:38:52.902106 control-lab-ly-1.0.1a0/src/controllably/Measure/Physical/
+-rw-rw-rw-   0        0        0      249 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Measure/Physical/__init__.py
+-rw-rw-rw-   0        0        0     8271 2023-04-21 07:30:47.000000 control-lab-ly-1.0.1a0/src/controllably/Measure/Physical/balance_utils.py
+-rw-rw-rw-   0        0        0      535 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Measure/__init__.py
+-rw-rw-rw-   0        0        0     5398 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Measure/instrument_utils.py
+-rw-rw-rw-   0        0        0    13804 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Measure/measure_utils.py
+-rw-rw-rw-   0        0        0     4176 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Measure/program_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:38:52.939190 control-lab-ly-1.0.1a0/src/controllably/Move/
+drwxrwxrwx   0        0        0        0 2023-04-21 08:38:52.984490 control-lab-ly-1.0.1a0/src/controllably/Move/Cartesian/
+-rw-rw-rw-   0        0        0      346 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Move/Cartesian/__init__.py
+-rw-rw-rw-   0        0        0     9049 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Move/Cartesian/cartesian_utils.py
+-rw-rw-rw-   0        0        0     3402 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Move/Cartesian/ender_utils.py
+-rw-rw-rw-   0        0        0     2853 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Move/Cartesian/primitiv_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:38:53.000839 control-lab-ly-1.0.1a0/src/controllably/Move/Jointed/
+drwxrwxrwx   0        0        0        0 2023-04-21 08:38:53.034499 control-lab-ly-1.0.1a0/src/controllably/Move/Jointed/Dobot/
+-rw-rw-rw-   0        0        0      336 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Move/Jointed/Dobot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:38:53.062642 control-lab-ly-1.0.1a0/src/controllably/Move/Jointed/Dobot/dobot_api/
+-rw-rw-rw-   0        0        0       62 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a0/src/controllably/Move/Jointed/Dobot/dobot_api/__init__.py
+-rw-rw-rw-   0        0        0    24262 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a0/src/controllably/Move/Jointed/Dobot/dobot_api/dobot_api.py
+-rw-rw-rw-   0        0        0    15851 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Move/Jointed/Dobot/dobot_utils.py
+-rw-rw-rw-   0        0        0     7030 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Move/Jointed/Dobot/m1pro_utils.py
+-rw-rw-rw-   0        0        0     4325 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Move/Jointed/Dobot/mg400_utils.py
+-rw-rw-rw-   0        0        0      233 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Move/Jointed/__init__.py
+-rw-rw-rw-   0        0        0    10507 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Move/Jointed/jointed_utils.py
+-rw-rw-rw-   0        0        0      217 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Move/__init__.py
+-rw-rw-rw-   0        0        0    32152 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Move/move_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:38:53.071616 control-lab-ly-1.0.1a0/src/controllably/Transfer/
+drwxrwxrwx   0        0        0        0 2023-04-21 08:38:53.130251 control-lab-ly-1.0.1a0/src/controllably/Transfer/Liquid/
+drwxrwxrwx   0        0        0        0 2023-04-21 08:38:53.179331 control-lab-ly-1.0.1a0/src/controllably/Transfer/Liquid/Pumps/
+drwxrwxrwx   0        0        0        0 2023-04-21 08:38:53.229287 control-lab-ly-1.0.1a0/src/controllably/Transfer/Liquid/Pumps/TriContinent/
+-rw-rw-rw-   0        0        0      255 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Transfer/Liquid/Pumps/TriContinent/__init__.py
+-rw-rw-rw-   0        0        0     3460 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_lib.py
+-rw-rw-rw-   0        0        0    29831 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_utils.py
+-rw-rw-rw-   0        0        0      332 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Transfer/Liquid/Pumps/__init__.py
+-rw-rw-rw-   0        0        0     9064 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Transfer/Liquid/Pumps/peristaltic_utils.py
+-rw-rw-rw-   0        0        0     3097 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Transfer/Liquid/Pumps/pump_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:38:53.279847 control-lab-ly-1.0.1a0/src/controllably/Transfer/Liquid/Sartorius/
+-rw-rw-rw-   0        0        0      252 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Transfer/Liquid/Sartorius/__init__.py
+-rw-rw-rw-   0        0        0     3210 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Transfer/Liquid/Sartorius/sartorius_lib.py
+-rw-rw-rw-   0        0        0    30605 2023-04-21 07:30:47.000000 control-lab-ly-1.0.1a0/src/controllably/Transfer/Liquid/Sartorius/sartorius_utils.py
+-rw-rw-rw-   0        0        0      364 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Transfer/Liquid/__init__.py
+-rw-rw-rw-   0        0        0    13126 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Transfer/Liquid/liquid_utils.py
+-rw-rw-rw-   0        0        0     3451 2023-04-21 08:27:57.000000 control-lab-ly-1.0.1a0/src/controllably/Transfer/Liquid/syringe_lib.py
+-rw-rw-rw-   0        0        0    14619 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Transfer/Liquid/syringe_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:38:53.302152 control-lab-ly-1.0.1a0/src/controllably/Transfer/Powder/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a0/src/controllably/Transfer/Powder/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:38:53.333781 control-lab-ly-1.0.1a0/src/controllably/Transfer/Substrate/
+drwxrwxrwx   0        0        0        0 2023-04-21 08:38:53.364389 control-lab-ly-1.0.1a0/src/controllably/Transfer/Substrate/Dobot/
+-rw-rw-rw-   0        0        0      348 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Transfer/Substrate/Dobot/__init__.py
+-rw-rw-rw-   0        0        0     8255 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Transfer/Substrate/Dobot/dobot_attachments.py
+-rw-rw-rw-   0        0        0      238 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Transfer/Substrate/__init__.py
+-rw-rw-rw-   0        0        0     1032 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/Transfer/Substrate/substrate_utils.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a0/src/controllably/Transfer/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a0/src/controllably/Transfer/transfer_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:38:53.407515 control-lab-ly-1.0.1a0/src/controllably/View/
+drwxrwxrwx   0        0        0        0 2023-04-21 08:38:53.437394 control-lab-ly-1.0.1a0/src/controllably/View/Classifiers/
+-rw-rw-rw-   0        0        0      333 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/View/Classifiers/__init__.py
+-rw-rw-rw-   0        0        0     2586 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/View/Classifiers/classifier_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:38:53.462892 control-lab-ly-1.0.1a0/src/controllably/View/Optical/
+-rw-rw-rw-   0        0        0      219 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/View/Optical/__init__.py
+-rw-rw-rw-   0        0        0     3163 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/View/Optical/optical_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:38:53.493863 control-lab-ly-1.0.1a0/src/controllably/View/Optical/placeholders/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a0/src/controllably/View/Optical/placeholders/__init__.py
+-rw-rw-rw-   0        0        0    15567 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a0/src/controllably/View/Optical/placeholders/optical_camera.png
+drwxrwxrwx   0        0        0        0 2023-04-21 08:38:53.520526 control-lab-ly-1.0.1a0/src/controllably/View/Thermal/
+drwxrwxrwx   0        0        0        0 2023-04-21 08:38:53.532489 control-lab-ly-1.0.1a0/src/controllably/View/Thermal/Flir/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a0/src/controllably/View/Thermal/Flir/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:38:53.613079 control-lab-ly-1.0.1a0/src/controllably/View/Thermal/Flir/ax8/
+-rw-rw-rw-   0        0        0       33 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a0/src/controllably/View/Thermal/Flir/ax8/__init__.py
+-rw-rw-rw-   0        0        0    10147 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a0/src/controllably/View/Thermal/Flir/ax8/ax8.py
+-rw-rw-rw-   0        0        0     3821 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a0/src/controllably/View/Thermal/Flir/ax8/ax8_camera_feed.py
+-rw-rw-rw-   0        0        0      636 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a0/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_regs.py
+-rw-rw-rw-   0        0        0      819 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a0/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_utils.py
+-rw-rw-rw-   0        0        0      219 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/View/Thermal/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:38:53.642110 control-lab-ly-1.0.1a0/src/controllably/View/Thermal/placeholders/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a0/src/controllably/View/Thermal/placeholders/__init__.py
+-rw-rw-rw-   0        0        0   148660 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a0/src/controllably/View/Thermal/placeholders/infrared_camera.png
+-rw-rw-rw-   0        0        0     2983 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/View/Thermal/thermal_utils.py
+-rw-rw-rw-   0        0        0      294 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/View/__init__.py
+-rw-rw-rw-   0        0        0    15729 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/View/image_utils.py
+-rw-rw-rw-   0        0        0    17366 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/View/view_utils.py
+-rw-rw-rw-   0        0        0       98 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:38:53.741266 control-lab-ly-1.0.1a0/src/controllably/misc/
+-rw-rw-rw-   0        0        0      586 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/misc/__init__.py
+-rw-rw-rw-   0        0        0     2522 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/misc/decorators.py
+-rw-rw-rw-   0        0        0    10014 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/misc/factory.py
+-rw-rw-rw-   0        0        0     6551 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/misc/helper.py
+-rw-rw-rw-   0        0        0    17440 2023-04-21 07:30:47.000000 control-lab-ly-1.0.1a0/src/controllably/misc/layout.py
+-rw-rw-rw-   0        0        0     2867 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/misc/logger.py
+-rw-rw-rw-   0        0        0     4576 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/misc/misc_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:38:53.753241 control-lab-ly-1.0.1a0/src/controllably/misc/templates/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a0/src/controllably/misc/templates/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:38:53.781965 control-lab-ly-1.0.1a0/src/controllably/misc/templates/configs/
+-rw-rw-rw-   0        0        0        0 2023-02-23 14:08:10.000000 control-lab-ly-1.0.1a0/src/controllably/misc/templates/configs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:38:53.809974 control-lab-ly-1.0.1a0/src/controllably/misc/templates/configs/plugins/
+-rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a0/src/controllably/misc/templates/configs/plugins/__init__.py
+-rw-rw-rw-   0        0        0     1091 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/misc/templates/configs/plugins/plugin_template.py
+-rw-rw-rw-   0        0        0      439 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/misc/templates/configs/registry.yaml
+drwxrwxrwx   0        0        0        0 2023-04-21 08:38:53.863295 control-lab-ly-1.0.1a0/src/controllably/misc/templates/setup/
+-rw-rw-rw-   0        0        0      772 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/misc/templates/setup/__init__.py
+-rw-rw-rw-   0        0        0     1434 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/misc/templates/setup/config.yaml
+-rw-rw-rw-   0        0        0      987 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/src/controllably/misc/templates/setup/layout.json
+drwxrwxrwx   0        0        0        0 2023-04-21 08:38:54.098861 control-lab-ly-1.0.1a0/tests/
+-rw-rw-rw-   0        0        0      189 2023-04-11 09:35:43.000000 control-lab-ly-1.0.1a0/tests/test_camera_optical.py
+-rw-rw-rw-   0        0        0      230 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a0/tests/test_camera_thermal.py
+-rw-rw-rw-   0        0        0      509 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a0/tests/test_cartesian_ender.py
+-rw-rw-rw-   0        0        0      429 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a0/tests/test_cartesian_primitiv.py
+-rw-rw-rw-   0        0        0      585 2023-04-21 08:33:59.000000 control-lab-ly-1.0.1a0/tests/test_compound_liquidmover.py
+-rw-rw-rw-   0        0        0      801 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a0/tests/test_compound_spin_printer.py
+-rw-rw-rw-   0        0        0      616 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a0/tests/test_dobot_m1pro.py
+-rw-rw-rw-   0        0        0      651 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a0/tests/test_dobot_mg400.py
+-rw-rw-rw-   0        0        0      324 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a0/tests/test_electrical_keithley.py
+-rw-rw-rw-   0        0        0      392 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a0/tests/test_film_spin.py
+-rw-rw-rw-   0        0        0      587 2023-04-11 09:21:52.000000 control-lab-ly-1.0.1a0/tests/test_heat_peltier.py
+-rw-rw-rw-   0        0        0      349 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a0/tests/test_light_led_array.py
+-rw-rw-rw-   0        0        0      362 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a0/tests/test_liquid_sartorius.py
+-rw-rw-rw-   0        0        0      412 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a0/tests/test_liquid_syringe_assembly.py
+-rw-rw-rw-   0        0        0      538 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a0/tests/test_liquid_tricontinent.py
+-rw-rw-rw-   0        0        0      239 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a0/tests/test_mechanical_piezorobotics.py
+-rw-rw-rw-   0        0        0      268 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a0/tests/test_panels.py
+-rw-rw-rw-   0        0        0      273 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a0/tests/test_physical_balance.py
+-rw-rw-rw-   0        0        0      337 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a0/tests/test_pump_peristaltic.py
```

### Comparing `control-lab-ly-1.0.0b1/LICENSE.md` & `control-lab-ly-1.0.1a0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/PKG-INFO` & `control-lab-ly-1.0.1a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: control-lab-ly
-Version: 1.0.0b1
+Version: 1.0.1a0
 Summary: Lab Equipment Automation Package
 Home-page: https://github.com/kylejeanlewis/control-lab-le
 Author: Chang Jie Leong
 Author-email: changjie.leong@outlook.com
 License: MIT
 Project-URL: GitHub, https://github.com/kylejeanlewis/control-lab-le
 Project-URL: Documentation, https://github.com/kylejeanlewis/control-lab-le/blob/main/docs/README.md
@@ -292,20 +292,22 @@
 lab.Factory.register(myClass, "Make.Something.Good")
 ```
 
 #### 5.2 Registering a Python module
 Alternatively, you can automatically register all Classes and Functions in a Python module just by importing it.\
 Declare a `__where__` global variable to indicate where to register the module.
 ```python
-### my_module.py
+### my_module.py ###
 __where__ = "Make.Something.Good"                 # Where to register this module to
+# ==========
 def myClass:                                      # Main body of code goes here
   ...
-from controllably import include_this_module
-include_this_module()                             # Registers only the Classes and Functions defined above in this .py file
+# ==========
+from controllably import include_this_module      # Registers only the Classes and Functions
+include_this_module()                             # defined above in this .py file
 ```
 At the end of the .py file, import and call  the `include_this_module()` function.
 
 ---
 
 ## Dependencies
 - Dash (>=2.7.1)
```

### Comparing `control-lab-ly-1.0.0b1/docs/CHANGELOG.md` & `control-lab-ly-1.0.1a0/docs/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/docs/CODE_OF_CONDUCT.md` & `control-lab-ly-1.0.1a0/docs/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/docs/LICENSE.md` & `control-lab-ly-1.0.1a0/docs/LICENSE.md`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/docs/README.md` & `control-lab-ly-1.0.1a0/docs/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -267,20 +267,22 @@
 lab.Factory.register(myClass, "Make.Something.Good")
 ```
 
 #### 5.2 Registering a Python module
 Alternatively, you can automatically register all Classes and Functions in a Python module just by importing it.\
 Declare a `__where__` global variable to indicate where to register the module.
 ```python
-### my_module.py
+### my_module.py ###
 __where__ = "Make.Something.Good"                 # Where to register this module to
+# ==========
 def myClass:                                      # Main body of code goes here
   ...
-from controllably import include_this_module
-include_this_module()                             # Registers only the Classes and Functions defined above in this .py file
+# ==========
+from controllably import include_this_module      # Registers only the Classes and Functions
+include_this_module()                             # defined above in this .py file
 ```
 At the end of the .py file, import and call  the `include_this_module()` function.
 
 ---
 
 ## Dependencies
 - Dash (>=2.7.1)
```

### Comparing `control-lab-ly-1.0.0b1/setup.cfg` & `control-lab-ly-1.0.1a0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,98 +1,98 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2063 6f6e 7472 6f6c 2d6c 6162 2d6c   = control-lab-l
 00000020: 790d 0a76 6572 7369 6f6e 203d 2031 2e30  y..version = 1.0
-00000030: 2e30 2d62 2e31 0d0a 6465 7363 7269 7074  .0-b.1..descript
-00000040: 696f 6e20 3d20 4c61 6220 4571 7569 706d  ion = Lab Equipm
-00000050: 656e 7420 4175 746f 6d61 7469 6f6e 2050  ent Automation P
-00000060: 6163 6b61 6765 0d0a 6c6f 6e67 5f64 6573  ackage..long_des
-00000070: 6372 6970 7469 6f6e 203d 2066 696c 653a  cription = file:
-00000080: 2064 6f63 732f 5245 4144 4d45 2e6d 642c   docs/README.md,
-00000090: 2064 6f63 732f 4348 414e 4745 4c4f 472e   docs/CHANGELOG.
-000000a0: 6d64 0d0a 6c6f 6e67 5f64 6573 6372 6970  md..long_descrip
-000000b0: 7469 6f6e 5f63 6f6e 7465 6e74 5f74 7970  tion_content_typ
-000000c0: 6520 3d20 7465 7874 2f6d 6172 6b64 6f77  e = text/markdow
-000000d0: 6e0d 0a61 7574 686f 7220 3d20 4368 616e  n..author = Chan
-000000e0: 6720 4a69 6520 4c65 6f6e 670d 0a61 7574  g Jie Leong..aut
-000000f0: 686f 725f 656d 6169 6c20 3d20 6368 616e  hor_email = chan
-00000100: 676a 6965 2e6c 656f 6e67 406f 7574 6c6f  gjie.leong@outlo
-00000110: 6f6b 2e63 6f6d 0d0a 7572 6c20 3d20 6874  ok.com..url = ht
-00000120: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000130: 2f6b 796c 656a 6561 6e6c 6577 6973 2f63  /kylejeanlewis/c
-00000140: 6f6e 7472 6f6c 2d6c 6162 2d6c 650d 0a70  ontrol-lab-le..p
-00000150: 726f 6a65 6374 5f75 726c 7320 3d20 0d0a  roject_urls = ..
-00000160: 0947 6974 4875 6220 3d20 6874 7470 733a  .GitHub = https:
-00000170: 2f2f 6769 7468 7562 2e63 6f6d 2f6b 796c  //github.com/kyl
-00000180: 656a 6561 6e6c 6577 6973 2f63 6f6e 7472  ejeanlewis/contr
-00000190: 6f6c 2d6c 6162 2d6c 650d 0a09 446f 6375  ol-lab-le...Docu
-000001a0: 6d65 6e74 6174 696f 6e20 3d20 6874 7470  mentation = http
-000001b0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6b  s://github.com/k
-000001c0: 796c 656a 6561 6e6c 6577 6973 2f63 6f6e  ylejeanlewis/con
-000001d0: 7472 6f6c 2d6c 6162 2d6c 652f 626c 6f62  trol-lab-le/blob
-000001e0: 2f6d 6169 6e2f 646f 6373 2f52 4541 444d  /main/docs/READM
-000001f0: 452e 6d64 0d0a 0943 6861 6e67 656c 6f67  E.md...Changelog
-00000200: 203d 2068 7474 7073 3a2f 2f67 6974 6875   = https://githu
-00000210: 622e 636f 6d2f 6b79 6c65 6a65 616e 6c65  b.com/kylejeanle
-00000220: 7769 732f 636f 6e74 726f 6c2d 6c61 622d  wis/control-lab-
-00000230: 6c65 2f62 6c6f 622f 6d61 696e 2f64 6f63  le/blob/main/doc
-00000240: 732f 4348 414e 4745 4c4f 472e 6d64 0d0a  s/CHANGELOG.md..
-00000250: 0954 7261 636b 6572 203d 2068 7474 7073  .Tracker = https
-00000260: 3a2f 2f67 6974 6875 622e 636f 6d2f 6b79  ://github.com/ky
-00000270: 6c65 6a65 616e 6c65 7769 732f 636f 6e74  lejeanlewis/cont
-00000280: 726f 6c2d 6c61 622d 6c65 2f69 7373 7565  rol-lab-le/issue
-00000290: 730d 0a6c 6963 656e 7365 203d 204d 4954  s..license = MIT
-000002a0: 0d0a 6b65 7977 6f72 6473 203d 200d 0a09  ..keywords = ...
-000002b0: 7079 7468 6f6e 0d0a 096c 6162 2061 7574  python...lab aut
-000002c0: 6f6d 6174 696f 6e0d 0a63 6c61 7373 6966  omation..classif
-000002d0: 6965 7273 203d 200d 0a09 4465 7665 6c6f  iers = ...Develo
-000002e0: 706d 656e 7420 5374 6174 7573 203a 3a20  pment Status :: 
-000002f0: 3320 2d20 416c 7068 610d 0a09 496e 7465  3 - Alpha...Inte
-00000300: 6e64 6564 2041 7564 6965 6e63 6520 3a3a  nded Audience ::
-00000310: 2044 6576 656c 6f70 6572 730d 0a09 496e   Developers...In
-00000320: 7465 6e64 6564 2041 7564 6965 6e63 6520  tended Audience 
-00000330: 3a3a 2053 6369 656e 6365 2f52 6573 6561  :: Science/Resea
-00000340: 7263 680d 0a09 4c69 6365 6e73 6520 3a3a  rch...License ::
-00000350: 204f 5349 2041 7070 726f 7665 6420 3a3a   OSI Approved ::
-00000360: 204d 4954 204c 6963 656e 7365 0d0a 094f   MIT License...O
-00000370: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
-00000380: 3a3a 204d 6963 726f 736f 6674 203a 3a20  :: Microsoft :: 
-00000390: 5769 6e64 6f77 730d 0a09 5072 6f67 7261  Windows...Progra
-000003a0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-000003b0: 3a20 5079 7468 6f6e 203a 3a20 330d 0a09  : Python :: 3...
-000003c0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-000003d0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-000003e0: 3a20 332e 380d 0a09 546f 7069 6320 3a3a  : 3.8...Topic ::
-000003f0: 2053 6369 656e 7469 6669 632f 456e 6769   Scientific/Engi
-00000400: 6e65 6572 696e 670d 0a0d 0a5b 6f70 7469  neering....[opti
-00000410: 6f6e 735d 0d0a 7061 636b 6167 655f 6469  ons]..package_di
-00000420: 7220 3d20 0d0a 093d 2073 7263 0d0a 7061  r = ...= src..pa
-00000430: 636b 6167 6573 203d 2066 696e 643a 0d0a  ckages = find:..
-00000440: 696e 636c 7564 655f 7061 636b 6167 655f  include_package_
-00000450: 6461 7461 203d 2054 7275 650d 0a70 7974  data = True..pyt
-00000460: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
-00000470: 3d33 2e38 0d0a 696e 7374 616c 6c5f 7265  =3.8..install_re
-00000480: 7175 6972 6573 203d 200d 0a09 6461 7368  quires = ...dash
-00000490: 3e3d 322e 370d 0a09 696d 7065 6461 6e63  >=2.7...impedanc
-000004a0: 653e 3d31 2e34 0d0a 0969 6d75 7469 6c73  e>=1.4...imutils
-000004b0: 3e3d 302e 350d 0a09 6d61 7470 6c6f 746c  >=0.5...matplotl
-000004c0: 6962 3e3d 332e 330d 0a09 6e65 7374 5f61  ib>=3.3...nest_a
-000004d0: 7379 6e63 696f 3e3d 312e 350d 0a09 6e75  syncio>=1.5...nu
-000004e0: 6d70 793e 3d31 2e31 390d 0a09 6f70 656e  mpy>=1.19...open
-000004f0: 6376 5f70 7974 686f 6e3e 3d34 2e35 2e30  cv_python>=4.5.0
-00000500: 0d0a 0970 616e 6461 733e 3d31 2e32 0d0a  ...pandas>=1.2..
-00000510: 0970 6c6f 746c 793e 3d35 2e33 0d0a 0970  .plotly>=5.3...p
-00000520: 794d 6f64 6275 7354 4350 3e3d 302e 320d  yModbusTCP>=0.2.
-00000530: 0a09 7079 7365 7269 616c 3e3d 332e 350d  ..pyserial>=3.5.
-00000540: 0a09 5079 5369 6d70 6c65 4755 493e 3d34  ..PySimpleGUI>=4
-00000550: 2e36 300d 0a09 5079 5649 5341 3e3d 312e  .60...PyVISA>=1.
-00000560: 3132 0d0a 0950 7959 414d 4c3e 3d36 2e30  12...PyYAML>=6.0
-00000570: 0d0a 0973 6369 7079 3e3d 312e 360d 0a0d  ...scipy>=1.6...
-00000580: 0a5b 6f70 7469 6f6e 732e 7061 636b 6167  .[options.packag
-00000590: 6573 2e66 696e 645d 0d0a 7768 6572 6520  es.find]..where 
-000005a0: 3d20 7372 630d 0a65 7863 6c75 6465 203d  = src..exclude =
-000005b0: 2074 6573 7473 0d0a 0d0a 5b6f 7074 696f   tests....[optio
-000005c0: 6e73 2e70 6163 6b61 6765 5f64 6174 615d  ns.package_data]
-000005d0: 0d0a 2a20 3d20 2a2e 6a73 6f6e 2c20 2a2e  ..* = *.json, *.
-000005e0: 7961 6d6c 2c20 2a2e 706e 670d 0a0d 0a5b  yaml, *.png....[
-000005f0: 6567 675f 696e 666f 5d0d 0a74 6167 5f62  egg_info]..tag_b
-00000600: 7569 6c64 203d 200d 0a74 6167 5f64 6174  uild = ..tag_dat
-00000610: 6520 3d20 300d 0a0d 0a                   e = 0....
+00000030: 2e31 2d61 0d0a 6465 7363 7269 7074 696f  .1-a..descriptio
+00000040: 6e20 3d20 4c61 6220 4571 7569 706d 656e  n = Lab Equipmen
+00000050: 7420 4175 746f 6d61 7469 6f6e 2050 6163  t Automation Pac
+00000060: 6b61 6765 0d0a 6c6f 6e67 5f64 6573 6372  kage..long_descr
+00000070: 6970 7469 6f6e 203d 2066 696c 653a 2064  iption = file: d
+00000080: 6f63 732f 5245 4144 4d45 2e6d 642c 2064  ocs/README.md, d
+00000090: 6f63 732f 4348 414e 4745 4c4f 472e 6d64  ocs/CHANGELOG.md
+000000a0: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
+000000b0: 6f6e 5f63 6f6e 7465 6e74 5f74 7970 6520  on_content_type 
+000000c0: 3d20 7465 7874 2f6d 6172 6b64 6f77 6e0d  = text/markdown.
+000000d0: 0a61 7574 686f 7220 3d20 4368 616e 6720  .author = Chang 
+000000e0: 4a69 6520 4c65 6f6e 670d 0a61 7574 686f  Jie Leong..autho
+000000f0: 725f 656d 6169 6c20 3d20 6368 616e 676a  r_email = changj
+00000100: 6965 2e6c 656f 6e67 406f 7574 6c6f 6f6b  ie.leong@outlook
+00000110: 2e63 6f6d 0d0a 7572 6c20 3d20 6874 7470  .com..url = http
+00000120: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6b  s://github.com/k
+00000130: 796c 656a 6561 6e6c 6577 6973 2f63 6f6e  ylejeanlewis/con
+00000140: 7472 6f6c 2d6c 6162 2d6c 650d 0a70 726f  trol-lab-le..pro
+00000150: 6a65 6374 5f75 726c 7320 3d20 0d0a 0947  ject_urls = ...G
+00000160: 6974 4875 6220 3d20 6874 7470 733a 2f2f  itHub = https://
+00000170: 6769 7468 7562 2e63 6f6d 2f6b 796c 656a  github.com/kylej
+00000180: 6561 6e6c 6577 6973 2f63 6f6e 7472 6f6c  eanlewis/control
+00000190: 2d6c 6162 2d6c 650d 0a09 446f 6375 6d65  -lab-le...Docume
+000001a0: 6e74 6174 696f 6e20 3d20 6874 7470 733a  ntation = https:
+000001b0: 2f2f 6769 7468 7562 2e63 6f6d 2f6b 796c  //github.com/kyl
+000001c0: 656a 6561 6e6c 6577 6973 2f63 6f6e 7472  ejeanlewis/contr
+000001d0: 6f6c 2d6c 6162 2d6c 652f 626c 6f62 2f6d  ol-lab-le/blob/m
+000001e0: 6169 6e2f 646f 6373 2f52 4541 444d 452e  ain/docs/README.
+000001f0: 6d64 0d0a 0943 6861 6e67 656c 6f67 203d  md...Changelog =
+00000200: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+00000210: 636f 6d2f 6b79 6c65 6a65 616e 6c65 7769  com/kylejeanlewi
+00000220: 732f 636f 6e74 726f 6c2d 6c61 622d 6c65  s/control-lab-le
+00000230: 2f62 6c6f 622f 6d61 696e 2f64 6f63 732f  /blob/main/docs/
+00000240: 4348 414e 4745 4c4f 472e 6d64 0d0a 0954  CHANGELOG.md...T
+00000250: 7261 636b 6572 203d 2068 7474 7073 3a2f  racker = https:/
+00000260: 2f67 6974 6875 622e 636f 6d2f 6b79 6c65  /github.com/kyle
+00000270: 6a65 616e 6c65 7769 732f 636f 6e74 726f  jeanlewis/contro
+00000280: 6c2d 6c61 622d 6c65 2f69 7373 7565 730d  l-lab-le/issues.
+00000290: 0a6c 6963 656e 7365 203d 204d 4954 0d0a  .license = MIT..
+000002a0: 6b65 7977 6f72 6473 203d 200d 0a09 7079  keywords = ...py
+000002b0: 7468 6f6e 0d0a 096c 6162 2061 7574 6f6d  thon...lab autom
+000002c0: 6174 696f 6e0d 0a63 6c61 7373 6966 6965  ation..classifie
+000002d0: 7273 203d 200d 0a09 4465 7665 6c6f 706d  rs = ...Developm
+000002e0: 656e 7420 5374 6174 7573 203a 3a20 3320  ent Status :: 3 
+000002f0: 2d20 416c 7068 610d 0a09 496e 7465 6e64  - Alpha...Intend
+00000300: 6564 2041 7564 6965 6e63 6520 3a3a 2044  ed Audience :: D
+00000310: 6576 656c 6f70 6572 730d 0a09 496e 7465  evelopers...Inte
+00000320: 6e64 6564 2041 7564 6965 6e63 6520 3a3a  nded Audience ::
+00000330: 2053 6369 656e 6365 2f52 6573 6561 7263   Science/Researc
+00000340: 680d 0a09 4c69 6365 6e73 6520 3a3a 204f  h...License :: O
+00000350: 5349 2041 7070 726f 7665 6420 3a3a 204d  SI Approved :: M
+00000360: 4954 204c 6963 656e 7365 0d0a 094f 7065  IT License...Ope
+00000370: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
+00000380: 204d 6963 726f 736f 6674 203a 3a20 5769   Microsoft :: Wi
+00000390: 6e64 6f77 730d 0a09 5072 6f67 7261 6d6d  ndows...Programm
+000003a0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+000003b0: 5079 7468 6f6e 203a 3a20 330d 0a09 5072  Python :: 3...Pr
+000003c0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+000003d0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+000003e0: 332e 380d 0a09 546f 7069 6320 3a3a 2053  3.8...Topic :: S
+000003f0: 6369 656e 7469 6669 632f 456e 6769 6e65  cientific/Engine
+00000400: 6572 696e 670d 0a0d 0a5b 6f70 7469 6f6e  ering....[option
+00000410: 735d 0d0a 7061 636b 6167 655f 6469 7220  s]..package_dir 
+00000420: 3d20 0d0a 093d 2073 7263 0d0a 7061 636b  = ...= src..pack
+00000430: 6167 6573 203d 2066 696e 643a 0d0a 696e  ages = find:..in
+00000440: 636c 7564 655f 7061 636b 6167 655f 6461  clude_package_da
+00000450: 7461 203d 2054 7275 650d 0a70 7974 686f  ta = True..pytho
+00000460: 6e5f 7265 7175 6972 6573 203d 203e 3d33  n_requires = >=3
+00000470: 2e38 0d0a 696e 7374 616c 6c5f 7265 7175  .8..install_requ
+00000480: 6972 6573 203d 200d 0a09 6461 7368 3e3d  ires = ...dash>=
+00000490: 322e 370d 0a09 696d 7065 6461 6e63 653e  2.7...impedance>
+000004a0: 3d31 2e34 0d0a 0969 6d75 7469 6c73 3e3d  =1.4...imutils>=
+000004b0: 302e 350d 0a09 6d61 7470 6c6f 746c 6962  0.5...matplotlib
+000004c0: 3e3d 332e 330d 0a09 6e65 7374 5f61 7379  >=3.3...nest_asy
+000004d0: 6e63 696f 3e3d 312e 350d 0a09 6e75 6d70  ncio>=1.5...nump
+000004e0: 793e 3d31 2e31 390d 0a09 6f70 656e 6376  y>=1.19...opencv
+000004f0: 5f70 7974 686f 6e3e 3d34 2e35 2e30 0d0a  _python>=4.5.0..
+00000500: 0970 616e 6461 733e 3d31 2e32 0d0a 0970  .pandas>=1.2...p
+00000510: 6c6f 746c 793e 3d35 2e33 0d0a 0970 794d  lotly>=5.3...pyM
+00000520: 6f64 6275 7354 4350 3e3d 302e 320d 0a09  odbusTCP>=0.2...
+00000530: 7079 7365 7269 616c 3e3d 332e 350d 0a09  pyserial>=3.5...
+00000540: 5079 5369 6d70 6c65 4755 493e 3d34 2e36  PySimpleGUI>=4.6
+00000550: 300d 0a09 5079 5649 5341 3e3d 312e 3132  0...PyVISA>=1.12
+00000560: 0d0a 0950 7959 414d 4c3e 3d36 2e30 0d0a  ...PyYAML>=6.0..
+00000570: 0973 6369 7079 3e3d 312e 360d 0a0d 0a5b  .scipy>=1.6....[
+00000580: 6f70 7469 6f6e 732e 7061 636b 6167 6573  options.packages
+00000590: 2e66 696e 645d 0d0a 7768 6572 6520 3d20  .find]..where = 
+000005a0: 7372 630d 0a65 7863 6c75 6465 203d 2074  src..exclude = t
+000005b0: 6573 7473 0d0a 0d0a 5b6f 7074 696f 6e73  ests....[options
+000005c0: 2e70 6163 6b61 6765 5f64 6174 615d 0d0a  .package_data]..
+000005d0: 2a20 3d20 2a2e 6a73 6f6e 2c20 2a2e 7961  * = *.json, *.ya
+000005e0: 6d6c 2c20 2a2e 706e 670d 0a0d 0a5b 6567  ml, *.png....[eg
+000005f0: 675f 696e 666f 5d0d 0a74 6167 5f62 7569  g_info]..tag_bui
+00000600: 6c64 203d 200d 0a74 6167 5f64 6174 6520  ld = ..tag_date 
+00000610: 3d20 300d 0a0d 0a                        = 0....
```

### Comparing `control-lab-ly-1.0.0b1/src/control_lab_ly.egg-info/PKG-INFO` & `control-lab-ly-1.0.1a0/src/control_lab_ly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: control-lab-ly
-Version: 1.0.0b1
+Version: 1.0.1a0
 Summary: Lab Equipment Automation Package
 Home-page: https://github.com/kylejeanlewis/control-lab-le
 Author: Chang Jie Leong
 Author-email: changjie.leong@outlook.com
 License: MIT
 Project-URL: GitHub, https://github.com/kylejeanlewis/control-lab-le
 Project-URL: Documentation, https://github.com/kylejeanlewis/control-lab-le/blob/main/docs/README.md
@@ -292,20 +292,22 @@
 lab.Factory.register(myClass, "Make.Something.Good")
 ```
 
 #### 5.2 Registering a Python module
 Alternatively, you can automatically register all Classes and Functions in a Python module just by importing it.\
 Declare a `__where__` global variable to indicate where to register the module.
 ```python
-### my_module.py
+### my_module.py ###
 __where__ = "Make.Something.Good"                 # Where to register this module to
+# ==========
 def myClass:                                      # Main body of code goes here
   ...
-from controllably import include_this_module
-include_this_module()                             # Registers only the Classes and Functions defined above in this .py file
+# ==========
+from controllably import include_this_module      # Registers only the Classes and Functions
+include_this_module()                             # defined above in this .py file
 ```
 At the end of the .py file, import and call  the `include_this_module()` function.
 
 ---
 
 ## Dependencies
 - Dash (>=2.7.1)
```

### Comparing `control-lab-ly-1.0.0b1/src/control_lab_ly.egg-info/SOURCES.txt` & `control-lab-ly-1.0.1a0/src/control_lab_ly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/Analyse/Data/Database/database_utils.py` & `control-lab-ly-1.0.1a0/src/controllably/Analyse/Data/Database/database_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/Analyse/Data/Types/circuit_datatype.py` & `control-lab-ly-1.0.1a0/src/controllably/Analyse/Data/Types/circuit_datatype.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/Analyse/Data/Types/eis_datatype.py` & `control-lab-ly-1.0.1a0/src/controllably/Analyse/Data/Types/eis_datatype.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/Analyse/Data/Types/eis_test_circuits.yaml` & `control-lab-ly-1.0.1a0/src/controllably/Analyse/Data/Types/eis_test_circuits.yaml`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/Analyse/Data/Types/eis_tests.json` & `control-lab-ly-1.0.1a0/src/controllably/Analyse/Data/Types/eis_tests.json`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/Analyse/Visualisation/visualisation_utils.py` & `control-lab-ly-1.0.1a0/src/controllably/Analyse/Visualisation/visualisation_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/Compound/LiquidMover/liquidmover_utils.py` & `control-lab-ly-1.0.1a0/src/controllably/Compound/LiquidMover/liquidmover_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 # Standard library imports
 from __future__ import annotations
 import numpy as np
 import time
 from typing import Optional, Protocol
 
 # Local application imports
+from ...misc.layout import Well
 from ..compound_utils import CompoundSetup
 print(f"Import: OK <{__name__}>")
 
 class Liquid(Protocol):
     def aspirate(self, *args, **kwargs):
         ...
     def dispense(self, *args, **kwargs):
@@ -26,25 +27,30 @@
         ... 
     def setFlag(self, *args, **kwargs):
         ...
 
 class Mover(Protocol):
     home_coordinates: np.ndarray
     implement_offset: np.ndarray
+    speed: float
     _speed_max: float
     def home(self, *args, **kwargs):
         ...
     def isFeasible(self, *args, **kwargs):
         ...
     def loadDeck(self, *args, **kwargs):
         ...
     def move(self, *args, **kwargs):
         ...
+    def moveTo(self, *args, **kwargs):
+        ...
     def safeMoveTo(self, *args, **kwargs):
         ...
+    def setSpeed(self, *args, **kwargs):
+        ...
     
 class LiquidMoverSetup(CompoundSetup):
     """
     Liquid Mover Setup routines
 
     ### Constructor
     Args:
@@ -70,14 +76,16 @@
     - `dispenseAt`: dispense specified volume at target location, at desired speed
     - `ejectTip`: eject the pipette tip
     - `ejectTipAt`: eject the pipette tip at the specified location
     - `loadDeck`: load Labware objects onto the deck from file or dictionary
     - `reset`: alias for `rest()`
     - `rest`: go back to the rest position or home
     - `returnTip`: return current tip to its original rack position
+    - `touchTip`: touch the tip against the inner walls of the well
+    - `updateStartTip`: set the position of the first available pipette tip
     """
     
     _default_flags: dict[str, bool] = {'at_rest': False}
     def __init__(self, 
         config: Optional[str] = None, 
         layout: Optional[str] = None, 
         component_config: Optional[dict] = None, 
@@ -160,28 +168,32 @@
                 offset = self.liquid.channels[chn].offset
                 self.align(coordinates=coordinates, offset=offset)
                 self.liquid.aspirate(volume=volume, speed=speed, channel=chn)
         return
     
     def attachTip(self, 
         slot: str = 'tip_rack', 
+        start_tip: Optional[str] = None,
         tip_length: float = 80, 
         channel: Optional[int] = None
     ) -> tuple[float]:
         """
         Attach new pipette tip
 
         Args:
             slot (str, optional): name of slot with pipette tips. Defaults to 'tip_rack'.
+            start_tip (Optional[str], optional): channel to use. Defaults to None.
             tip_length (float, optional): length of pipette tip. Defaults to 80.
             channel (Optional[int], optional): channel to use. Defaults to None.
         
         Returns:
             tuple[float]: coordinates of top of tip rack well
         """
+        if start_tip is not None:
+            self.updateStartTip(start_tip=start_tip, slot=slot)
         next_tip_location, tip_length = self.positions[slot].pop(0)
         return self.attachTipAt(next_tip_location, tip_length=tip_length, channel=channel)
     
     def attachTipAt(self, 
         coordinates: tuple[float], 
         tip_length: float = 80, 
         channel: Optional[int] = None
@@ -202,15 +214,15 @@
             tuple[float]: coordinates of attach tip location
         """
         if 'eject' not in dir(self.liquid):
             raise AttributeError("`attachTip` and `attachTipAt` methods not available.")
         if self.liquid.isTipOn():
             raise RuntimeError("Please eject current tip before attaching new tip.")
         
-        tip_offset = np.array((0,0,-tip_length))
+        tip_offset = np.array((0,0,-tip_length + self.liquid.tip_inset_mm))
         self.align(coordinates)
         self.mover.move('z', -self.tip_approach_height, speed=0.01*self.mover._speed_max)
         time.sleep(3)
         
         self.liquid.tip_length = tip_length
         self.mover.implement_offset = self.mover.implement_offset + tip_offset
         self.mover.move('z', self.tip_approach_height+tip_length, speed=0.2*self.mover._speed_max)
@@ -285,15 +297,15 @@
         Returns:
             tuple[float]: coordinates of eject tip location
         """
         if 'eject' not in dir(self.liquid):
             raise AttributeError("`ejectTip` and `ejectTipAt` methods not available.")
         if not self.liquid.isTipOn():
             tip_length = self.liquid.tip_length
-            tip_offset = np.array((0,0,-tip_length))
+            tip_offset = np.array((0,0,-tip_length + self.liquid.tip_inset_mm))
             self.mover.implement_offset = self.mover.implement_offset - tip_offset
             self.liquid.tip_length = 0
             self.liquid.setFlag(tip_on=False)
             raise RuntimeError("There is currently no tip to eject.")
 
         self.align(coordinates)
         time.sleep(1)
@@ -340,8 +352,55 @@
         Return current tip to its original rack position
 
         Returns:
             tuple[float]: coordinates of eject tip location
         """
         coordinates = self.__dict__.pop('_temp_tip_home')
         return self.ejectTipAt(coordinates=(*coordinates[:2],coordinates[2]-18))
+    
+    def touchTip(self, well:Well, safe_move:bool = False) -> tuple[float]:
+        """
+        Touch the tip against the inner walls of the well
+        
+        Args:
+            well (Well): Well object
+            safe_move (bool, optional): whether to move safely (i.e. go back to safe height first). Defaults to False.
+
+        Returns:
+            tuple[float]: coordinates of well center
+        """
+        diameter = well.diameter
+        if safe_move:
+            self.align(coordinates=well.from_top((0,0,-10)))
+        else:
+            speed = self.mover.speed
+            self.mover.setSpeed(speed=0.2*self.mover._speed_max)
+            self.mover.moveTo(coordinates=well.from_top((0,0,-10)))
+            self.mover.setSpeed(speed=speed)
+        for axis in ('x','y'):
+            self.mover.move(axis, diameter/2, speed=0.2*self.mover._speed_max)
+            self.mover.move(axis, -diameter, speed=0.2*self.mover._speed_max)
+            self.mover.move(axis, diameter/2, speed=0.2*self.mover._speed_max)
+        self.mover.moveTo(coordinates=well.top)
+        return well.top
+    
+    def updateStartTip(self, start_tip:str, slot:str = 'tip_rack'):
+        """
+        Set the position of the first available pipette tip
+
+        Args:
+            start_tip (str): well name of the first available pipette tip
+            slot (str, optional): name of slot with pipette tips. Defaults to 'tip_rack'.
+        """
+        wells_list = self.deck.at(slot).wells_list.copy()
+        well_names = [well.name for well in wells_list]
+        if start_tip not in well_names:
+            print(f"Received: start_tip={start_tip}; slot={slot}")
+            print("Please enter a compatible set of inputs.")
+            return
+        self.positions[slot] = wells_list
+        for name in well_names:
+            if name == start_tip:
+                break
+            self.positions[slot].pop(0)
+        return
```

### Comparing `control-lab-ly-1.0.0b1/src/controllably/Compound/compound_utils.py` & `control-lab-ly-1.0.1a0/src/controllably/Compound/compound_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -165,27 +165,14 @@
                 print(f"Previously saved height '{key}': {self.positions[key]}\n")
                 print(f"New height received: {value}")
                 if input('Overwrite? [y/n]').lower() == 'n':
                     continue
                 self.positions[key] = value
         return
     
-    # def loadDeck(self, layout:str = None, layout_dict:dict = None):
-    #     """
-    #     Load the deck layout from JSON file
-        
-    #     Args:
-    #         layout (str, optional): filename of layout .json file. Defaults to None.
-    #         layout_dict (dict, optional): dictionary of layout. Defaults to None.
-    #     """
-    #     self.deck.load_layout(layout, layout_dict)
-    #     for name in self.deck.names:
-    #         self.positions[name] = [(well.top, well.depth) for well in self.deck.get_slot(name=name).wells_list]
-    #     return
-    
     # Protected method(s)
     def _connect(self, diagnostic:bool = False):
         """
         Make connections to the respective components
 
         Args:
             diagnostic (bool, optional): whether to run diagnostic tests to check equipment. Defaults to False.
```

### Comparing `control-lab-ly-1.0.0b1/src/controllably/Control/GUI/__init__.py` & `control-lab-ly-1.0.1a0/src/controllably/Control/GUI/__init__.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/Control/GUI/_guibuilder.py` & `control-lab-ly-1.0.1a0/src/controllably/Control/GUI/_guibuilder.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/Control/GUI/gui_utils.py` & `control-lab-ly-1.0.1a0/src/controllably/Control/GUI/gui_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/Control/GUI/loader_panel.py` & `control-lab-ly-1.0.1a0/src/controllably/Control/GUI/loader_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/Control/GUI/measurer_panel.py` & `control-lab-ly-1.0.1a0/src/controllably/Control/GUI/measurer_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/Control/GUI/mover_panel.py` & `control-lab-ly-1.0.1a0/src/controllably/Control/GUI/mover_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/Control/GUI/viewer_panel.py` & `control-lab-ly-1.0.1a0/src/controllably/Control/GUI/viewer_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/Control/Schedule/schedule_utils.py` & `control-lab-ly-1.0.1a0/src/controllably/Control/Schedule/schedule_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/Make/Heat/peltier_utils.py` & `control-lab-ly-1.0.1a0/src/controllably/Make/Heat/peltier_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,17 @@
             elif (self._power <= self.power_threshold) or (time.time()-self._stabilize_time >= self.stabilize_buffer_time):
                 print(response)
                 self.setFlag(temperature_reached=True)
                 print(f"Temperature of {self.set_point}°C reached!")
             if self.flags['record']:
                 values = [now] + values
                 row = {k:v for k,v in zip(self._columns, values)}
-                self.buffer_df = self.buffer_df.append(row, ignore_index=True)
+                # self.buffer_df = self.buffer_df.append(row, ignore_index=True)
+                new_row_df = pd.DataFrame(row)
+                self.buffer_df = pd.concat([self.buffer_df, new_row_df])
         return response
     
     def holdTemperature(self, temperature:float, time_s:float):
         """
         Hold target temperature for desired duration
 
         Args:
```

### Comparing `control-lab-ly-1.0.0b1/src/controllably/Make/Light/led_utils.py` & `control-lab-ly-1.0.1a0/src/controllably/Make/Light/led_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/Make/ThinFilm/spinner_utils.py` & `control-lab-ly-1.0.1a0/src/controllably/Make/ThinFilm/spinner_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/Make/make_utils.py` & `control-lab-ly-1.0.1a0/src/controllably/Make/make_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/Measure/Electrical/Keithley/keithley_device.py` & `control-lab-ly-1.0.1a0/src/controllably/Measure/Electrical/Keithley/keithley_device.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/Measure/Electrical/Keithley/keithley_lib.py` & `control-lab-ly-1.0.1a0/src/controllably/Measure/Electrical/Keithley/keithley_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/Measure/Electrical/Keithley/keithley_utils.py` & `control-lab-ly-1.0.1a0/src/controllably/Measure/Electrical/Keithley/keithley_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/Measure/Electrical/Keithley/programs/base_programs.py` & `control-lab-ly-1.0.1a0/src/controllably/Measure/Electrical/Keithley/programs/base_programs.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_device.py` & `control-lab-ly-1.0.1a0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_device.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_lib.py` & `control-lab-ly-1.0.1a0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_utils.py` & `control-lab-ly-1.0.1a0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/Measure/Mechanical/PiezoRobotics/programs/base_programs.py` & `control-lab-ly-1.0.1a0/src/controllably/Measure/Mechanical/PiezoRobotics/programs/base_programs.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/Measure/Physical/balance_utils.py` & `control-lab-ly-1.0.1a0/src/controllably/Measure/Physical/balance_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,15 +125,17 @@
                     now, 
                     value, 
                     self.calibration_factor, 
                     self.baseline, 
                     self._mass
                 ]
                 row = {k:v for k,v in zip(COLUMNS, values)}
-                self.buffer_df = self.buffer_df.append(row, ignore_index=True)
+                # self.buffer_df = self.buffer_df.append(row, ignore_index=True)
+                new_row_df = pd.DataFrame(row)
+                self.buffer_df = pd.concat([self.buffer_df, new_row_df])
         return response
   
     def reset(self):
         """Reset the device"""
         super().reset()
         self.baseline = 0
         return
@@ -179,14 +181,18 @@
     def zero(self, wait:int = 5):
         """
         Set current reading as baseline (i.e. zero mass)
         
         Args:
             wait (int, optional): duration to wait while zeroing, in seconds. Defaults to 5.
         """
+        if self.flags['record']:
+            print("Unable to zero while recording.")
+            print("Use `toggleRecord(False)` to stop recording.")
+            return
         temp_record_state = self.flags['record']
         temp_buffer_df = self.buffer_df.copy()
         self.reset()
         self.toggleRecord(True)
         print(f"Zeroing... ({wait}s)")
         time.sleep(wait)
         self.toggleRecord(False)
```

### Comparing `control-lab-ly-1.0.0b1/src/controllably/Measure/__init__.py` & `control-lab-ly-1.0.1a0/src/controllably/Measure/__init__.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/Measure/instrument_utils.py` & `control-lab-ly-1.0.1a0/src/controllably/Measure/instrument_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/Measure/measure_utils.py` & `control-lab-ly-1.0.1a0/src/controllably/Measure/measure_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/Measure/program_utils.py` & `control-lab-ly-1.0.1a0/src/controllably/Measure/program_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/Move/Cartesian/cartesian_utils.py` & `control-lab-ly-1.0.1a0/src/controllably/Move/Cartesian/cartesian_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/Move/Cartesian/ender_utils.py` & `control-lab-ly-1.0.1a0/src/controllably/Move/Cartesian/ender_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/Move/Cartesian/primitiv_utils.py` & `control-lab-ly-1.0.1a0/src/controllably/Move/Cartesian/primitiv_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/Move/Jointed/Dobot/dobot_api/dobot_api.py` & `control-lab-ly-1.0.1a0/src/controllably/Move/Jointed/Dobot/dobot_api/dobot_api.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/Move/Jointed/Dobot/dobot_utils.py` & `control-lab-ly-1.0.1a0/src/controllably/Move/Jointed/Dobot/dobot_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/Move/Jointed/Dobot/m1pro_utils.py` & `control-lab-ly-1.0.1a0/src/controllably/Move/Jointed/Dobot/m1pro_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/Move/Jointed/Dobot/mg400_utils.py` & `control-lab-ly-1.0.1a0/src/controllably/Move/Jointed/Dobot/mg400_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/Move/Jointed/jointed_utils.py` & `control-lab-ly-1.0.1a0/src/controllably/Move/Jointed/jointed_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/Move/move_utils.py` & `control-lab-ly-1.0.1a0/src/controllably/Move/move_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_lib.py` & `control-lab-ly-1.0.1a0/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_utils.py` & `control-lab-ly-1.0.1a0/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/Transfer/Liquid/Pumps/peristaltic_utils.py` & `control-lab-ly-1.0.1a0/src/controllably/Transfer/Liquid/Pumps/peristaltic_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/Transfer/Liquid/Pumps/pump_utils.py` & `control-lab-ly-1.0.1a0/src/controllably/Transfer/Liquid/Pumps/pump_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/Transfer/Liquid/Sartorius/sartorius_lib.py` & `control-lab-ly-1.0.1a0/src/controllably/Transfer/Liquid/Sartorius/sartorius_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/Transfer/Liquid/Sartorius/sartorius_utils.py` & `control-lab-ly-1.0.1a0/src/controllably/Transfer/Liquid/Sartorius/sartorius_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -238,1675 +238,1676 @@
 00000ed0: 2027 6f63 6375 7069 6564 273a 2046 616c   'occupied': Fal
 00000ee0: 7365 2c0d 0a20 2020 2020 2020 2027 7061  se,..        'pa
 00000ef0: 7573 655f 6665 6564 6261 636b 273a 4661  use_feedback':Fa
 00000f00: 6c73 652c 0d0a 2020 2020 2020 2020 2774  lse,..        't
 00000f10: 6970 5f6f 6e27 3a20 4661 6c73 650d 0a20  ip_on': False.. 
 00000f20: 2020 207d 0d0a 2020 2020 696d 706c 656d     }..    implem
 00000f30: 656e 745f 6f66 6673 6574 203d 2028 302c  ent_offset = (0,
-00000f40: 302c 2d32 3530 290d 0a20 2020 2064 6566  0,-250)..    def
-00000f50: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
-00000f60: 0d0a 2020 2020 2020 2020 706f 7274 3a73  ..        port:s
-00000f70: 7472 2c20 0d0a 2020 2020 2020 2020 6368  tr, ..        ch
-00000f80: 616e 6e65 6c3a 2069 6e74 203d 2031 2c20  annel: int = 1, 
-00000f90: 0d0a 2020 2020 2020 2020 6f66 6673 6574  ..        offset
-00000fa0: 3a20 7475 706c 655b 666c 6f61 745d 203d  : tuple[float] =
-00000fb0: 2028 302c 302c 3029 2c0d 0a20 2020 2020   (0,0,0),..     
-00000fc0: 2020 2072 6573 706f 6e73 655f 7469 6d65     response_time
-00000fd0: 3a20 666c 6f61 7420 3d20 312e 3033 2c0d  : float = 1.03,.
-00000fe0: 0a20 2020 2020 2020 2074 6970 5f74 6872  .        tip_thr
-00000ff0: 6573 686f 6c64 3a20 696e 7420 3d20 3237  eshold: int = 27
-00001000: 362c 0d0a 2020 2020 2020 2020 2a2a 6b77  6,..        **kw
-00001010: 6172 6773 0d0a 2020 2020 293a 0d0a 2020  args..    ):..  
-00001020: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-00001030: 2020 2049 6e73 7461 6e74 6961 7465 2074     Instantiate t
-00001040: 6865 2063 6c61 7373 0d0a 0d0a 2020 2020  he class....    
-00001050: 2020 2020 4172 6773 3a0d 0a20 2020 2020      Args:..     
-00001060: 2020 2020 2020 2070 6f72 7420 2873 7472         port (str
-00001070: 293a 2043 4f4d 2070 6f72 7420 6164 6472  ): COM port addr
-00001080: 6573 730d 0a20 2020 2020 2020 2020 2020  ess..           
-00001090: 2063 6861 6e6e 656c 2028 696e 742c 206f   channel (int, o
-000010a0: 7074 696f 6e61 6c29 3a20 6368 616e 6e65  ptional): channe
-000010b0: 6c20 6964 2e20 4465 6661 756c 7473 2074  l id. Defaults t
-000010c0: 6f20 312e 0d0a 2020 2020 2020 2020 2020  o 1...          
-000010d0: 2020 6f66 6673 6574 2028 7475 706c 655b    offset (tuple[
-000010e0: 666c 6f61 745d 2c20 6f70 7469 6f6e 616c  float], optional
-000010f0: 293a 2078 2c79 2c7a 206f 6666 7365 7420  ): x,y,z offset 
-00001100: 6f66 2074 6970 2e20 4465 6661 756c 7473  of tip. Defaults
-00001110: 2074 6f20 2830 2c30 2c30 292e 0d0a 2020   to (0,0,0)...  
-00001120: 2020 2020 2020 2020 2020 7265 7370 6f6e            respon
-00001130: 7365 5f74 696d 6520 2866 6c6f 6174 2c20  se_time (float, 
-00001140: 6f70 7469 6f6e 616c 293a 2064 656c 6179  optional): delay
-00001150: 2062 6574 7765 656e 2073 656e 6469 6e67   between sending
-00001160: 2061 2063 6f6d 6d61 6e64 2061 6e64 2072   a command and r
-00001170: 6563 6569 7669 6e67 2061 2072 6573 706f  eceiving a respo
-00001180: 6e73 652c 2069 6e20 7365 636f 6e64 732e  nse, in seconds.
-00001190: 2044 6566 6175 6c74 7320 746f 2031 2e30   Defaults to 1.0
-000011a0: 332e 0d0a 2020 2020 2020 2020 2020 2020  3...            
-000011b0: 7469 705f 7468 7265 7368 6f6c 6420 2869  tip_threshold (i
-000011c0: 6e74 2c20 6f70 7469 6f6e 616c 293a 2074  nt, optional): t
-000011d0: 6872 6573 686f 6c64 2061 626f 7665 2077  hreshold above w
-000011e0: 6869 6368 2061 2063 6f6e 6475 6374 6976  hich a conductiv
-000011f0: 6520 7069 7065 7474 6520 7469 7020 6973  e pipette tip is
-00001200: 2063 6f6e 7369 6465 7265 6420 746f 2062   considered to b
-00001210: 6520 6174 7461 6368 6564 2e20 4465 6661  e attached. Defa
-00001220: 756c 7473 2074 6f20 3237 362e 0d0a 2020  ults to 276...  
-00001230: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-00001240: 2020 2073 7570 6572 2829 2e5f 5f69 6e69     super().__ini
-00001250: 745f 5f28 2a2a 6b77 6172 6773 290d 0a20  t__(**kwargs).. 
-00001260: 2020 2020 2020 2073 656c 662e 6368 616e         self.chan
-00001270: 6e65 6c20 3d20 6368 616e 6e65 6c0d 0a20  nel = channel.. 
-00001280: 2020 2020 2020 2073 656c 662e 6f66 6673         self.offs
-00001290: 6574 203d 206f 6666 7365 740d 0a20 2020  et = offset..   
-000012a0: 2020 2020 2073 656c 662e 7265 7370 6f6e       self.respon
-000012b0: 7365 5f74 696d 6520 3d20 7265 7370 6f6e  se_time = respon
-000012c0: 7365 5f74 696d 650d 0a20 2020 2020 2020  se_time..       
-000012d0: 2073 656c 662e 7469 705f 7468 7265 7368   self.tip_thresh
-000012e0: 6f6c 6420 3d20 7469 705f 7468 7265 7368  old = tip_thresh
-000012f0: 6f6c 640d 0a20 2020 2020 2020 200d 0a20  old..        .. 
-00001300: 2020 2020 2020 2073 656c 662e 6d6f 6465         self.mode
-00001310: 6c5f 696e 666f 3a20 4d6f 6465 6c20 3d20  l_info: Model = 
-00001320: 4e6f 6e65 0d0a 2020 2020 2020 2020 7365  None..        se
-00001330: 6c66 2e6c 696d 6974 7320 3d20 2830 2c30  lf.limits = (0,0
-00001340: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00001350: 706f 7369 7469 6f6e 203d 2030 0d0a 2020  position = 0..  
-00001360: 2020 2020 2020 7365 6c66 2e73 7065 6564        self.speed
-00001370: 5f63 6f64 6520 3d20 5370 6565 6428 332c  _code = Speed(3,
-00001380: 3329 0d0a 2020 2020 2020 2020 7365 6c66  3)..        self
-00001390: 2e73 7065 6564 5f70 7265 7365 7473 203d  .speed_presets =
-000013a0: 204e 6f6e 650d 0a20 2020 2020 2020 2073   None..        s
-000013b0: 656c 662e 7469 705f 6c65 6e67 7468 203d  elf.tip_length =
-000013c0: 2030 0d0a 2020 2020 2020 2020 0d0a 2020   0..        ..  
-000013d0: 2020 2020 2020 7365 6c66 2e5f 6361 7061        self._capa
-000013e0: 6369 7461 6e63 6520 3d20 300d 0a20 2020  citance = 0..   
-000013f0: 2020 2020 2073 656c 662e 5f73 7461 7475       self._statu
-00001400: 735f 636f 6465 203d 2027 270d 0a20 2020  s_code = ''..   
-00001410: 2020 2020 2073 656c 662e 5f74 6872 6561       self._threa
-00001420: 6473 203d 207b 7d0d 0a20 2020 2020 2020  ds = {}..       
-00001430: 200d 0a20 2020 2020 2020 2070 7269 6e74   ..        print
-00001440: 2822 416e 7920 6174 7461 6368 6564 2070  ("Any attached p
-00001450: 6970 6574 7465 2074 6970 206d 6179 2064  ipette tip may d
-00001460: 726f 7020 6475 7269 6e67 2069 6e69 7469  rop during initi
-00001470: 616c 6973 6174 696f 6e2e 2229 0d0a 2020  alisation.")..  
-00001480: 2020 2020 2020 7365 6c66 2e5f 636f 6e6e        self._conn
-00001490: 6563 7428 706f 7274 290d 0a20 2020 2020  ect(port)..     
-000014a0: 2020 2072 6574 7572 6e0d 0a20 2020 200d     return..    .
-000014b0: 0a20 2020 2023 2050 726f 7065 7274 6965  .    # Propertie
-000014c0: 730d 0a20 2020 2040 7072 6f70 6572 7479  s..    @property
-000014d0: 0d0a 2020 2020 6465 6620 6361 7061 6369  ..    def capaci
-000014e0: 7461 6e63 6528 7365 6c66 2920 2d3e 2069  tance(self) -> i
-000014f0: 6e74 3a0d 0a20 2020 2020 2020 2072 6574  nt:..        ret
-00001500: 7572 6e20 7365 6c66 2e5f 6361 7061 6369  urn self._capaci
-00001510: 7461 6e63 650d 0a20 2020 2020 2020 200d  tance..        .
-00001520: 0a20 2020 2040 7072 6f70 6572 7479 0d0a  .    @property..
-00001530: 2020 2020 6465 6620 686f 6d65 5f70 6f73      def home_pos
-00001540: 6974 696f 6e28 7365 6c66 2920 2d3e 2069  ition(self) -> i
-00001550: 6e74 3a0d 0a20 2020 2020 2020 2072 6574  nt:..        ret
-00001560: 7572 6e20 7365 6c66 2e6d 6f64 656c 5f69  urn self.model_i
-00001570: 6e66 6f2e 686f 6d65 5f70 6f73 6974 696f  nfo.home_positio
-00001580: 6e0d 0a20 2020 200d 0a20 2020 2040 7072  n..    ..    @pr
-00001590: 6f70 6572 7479 0d0a 2020 2020 6465 6620  operty..    def 
-000015a0: 706f 7274 2873 656c 6629 202d 3e20 7374  port(self) -> st
-000015b0: 723a 0d0a 2020 2020 2020 2020 7265 7475  r:..        retu
-000015c0: 726e 2073 656c 662e 636f 6e6e 6563 7469  rn self.connecti
-000015d0: 6f6e 5f64 6574 6169 6c73 2e67 6574 2827  on_details.get('
-000015e0: 706f 7274 272c 2027 2729 0d0a 2020 2020  port', '')..    
-000015f0: 0d0a 2020 2020 4070 726f 7065 7274 790d  ..    @property.
-00001600: 0a20 2020 2064 6566 2072 6573 6f6c 7574  .    def resolut
-00001610: 696f 6e28 7365 6c66 2920 2d3e 2066 6c6f  ion(self) -> flo
-00001620: 6174 3a0d 0a20 2020 2020 2020 2072 6574  at:..        ret
-00001630: 7572 6e20 7365 6c66 2e6d 6f64 656c 5f69  urn self.model_i
-00001640: 6e66 6f2e 7265 736f 6c75 7469 6f6e 0d0a  nfo.resolution..
-00001650: 2020 2020 0d0a 2020 2020 4070 726f 7065      ..    @prope
-00001660: 7274 790d 0a20 2020 2064 6566 2073 7461  rty..    def sta
-00001670: 7475 7328 7365 6c66 2920 2d3e 2073 7472  tus(self) -> str
-00001680: 3a0d 0a20 2020 2020 2020 2072 6574 7572  :..        retur
-00001690: 6e20 7365 6c66 2e67 6574 5374 6174 7573  n self.getStatus
-000016a0: 2829 0d0a 2020 2020 0d0a 2020 2020 6465  ()..    ..    de
-000016b0: 6620 5f5f 6379 636c 6573 5f5f 2873 656c  f __cycles__(sel
-000016c0: 6629 202d 3e20 556e 696f 6e5b 696e 742c  f) -> Union[int,
-000016d0: 2073 7472 5d3a 0d0a 2020 2020 2020 2020   str]:..        
-000016e0: 2222 220d 0a20 2020 2020 2020 2052 6574  """..        Ret
-000016f0: 7269 6576 6520 746f 7461 6c20 6379 636c  rieve total cycl
-00001700: 6520 6c69 6665 7469 6d65 0d0a 0d0a 2020  e lifetime....  
-00001710: 2020 2020 2020 5265 7475 726e 733a 0d0a        Returns:..
-00001720: 2020 2020 2020 2020 2020 2020 556e 696f              Unio
-00001730: 6e5b 696e 742c 2073 7472 5d3a 206e 756d  n[int, str]: num
-00001740: 6265 7220 6f66 206c 6966 6574 696d 6520  ber of lifetime 
-00001750: 6379 636c 6573 2c20 6f72 2072 6573 706f  cycles, or respo
-00001760: 6e73 6520 7374 7269 6e67 0d0a 2020 2020  nse string..    
-00001770: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-00001780: 2072 6573 706f 6e73 6520 3d20 7365 6c66   response = self
-00001790: 2e5f 7175 6572 7928 2744 5827 290d 0a20  ._query('DX').. 
-000017a0: 2020 2020 2020 2074 7279 3a0d 0a20 2020         try:..   
-000017b0: 2020 2020 2020 2020 2063 7963 6c65 7320           cycles 
-000017c0: 3d20 696e 7428 7265 7370 6f6e 7365 290d  = int(response).
-000017d0: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
-000017e0: 5661 6c75 6545 7272 6f72 3a0d 0a20 2020  ValueError:..   
-000017f0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00001800: 7265 7370 6f6e 7365 0d0a 2020 2020 2020  response..      
-00001810: 2020 7072 696e 7428 6627 546f 7461 6c20    print(f'Total 
-00001820: 6379 636c 6573 3a20 7b63 7963 6c65 737d  cycles: {cycles}
-00001830: 2729 0d0a 2020 2020 2020 2020 7265 7475  ')..        retu
-00001840: 726e 2063 7963 6c65 730d 0a20 2020 200d  rn cycles..    .
-00001850: 0a20 2020 2064 6566 205f 5f6d 6f64 656c  .    def __model
-00001860: 5f5f 2873 656c 6629 202d 3e20 7374 723a  __(self) -> str:
-00001870: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-00001880: 2020 2020 2020 2052 6574 7269 6576 6520         Retrieve 
-00001890: 7468 6520 6d6f 6465 6c20 6f66 2074 6865  the model of the
-000018a0: 2064 6576 6963 650d 0a0d 0a20 2020 2020   device....     
-000018b0: 2020 2052 6574 7572 6e73 3a0d 0a20 2020     Returns:..   
-000018c0: 2020 2020 2020 2020 2073 7472 3a20 6d6f           str: mo
-000018d0: 6465 6c20 6e61 6d65 0d0a 2020 2020 2020  del name..      
-000018e0: 2020 2222 220d 0a20 2020 2020 2020 2072    """..        r
-000018f0: 6573 706f 6e73 6520 3d20 7365 6c66 2e5f  esponse = self._
-00001900: 7175 6572 7928 2744 4d27 290d 0a20 2020  query('DM')..   
-00001910: 2020 2020 2070 7269 6e74 2866 274d 6f64       print(f'Mod
-00001920: 656c 3a20 7b72 6573 706f 6e73 657d 2729  el: {response}')
-00001930: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00001940: 2072 6573 706f 6e73 650d 0a20 2020 200d   response..    .
-00001950: 0a20 2020 2064 6566 205f 5f72 6573 6f6c  .    def __resol
-00001960: 7574 696f 6e5f 5f28 7365 6c66 2920 2d3e  ution__(self) ->
-00001970: 2055 6e69 6f6e 5b69 6e74 2c20 7374 725d   Union[int, str]
-00001980: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
-00001990: 2020 2020 2020 2020 5265 7472 6965 7665          Retrieve
-000019a0: 2074 6865 2072 6573 6f6c 7574 696f 6e20   the resolution 
-000019b0: 6f66 2074 6865 2064 6576 6963 650d 0a0d  of the device...
-000019c0: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-000019d0: 3a0d 0a20 2020 2020 2020 2020 2020 2055  :..            U
-000019e0: 6e69 6f6e 5b69 6e74 2c20 7374 725d 3a20  nion[int, str]: 
-000019f0: 766f 6c75 6d65 2072 6573 6f6c 7574 696f  volume resolutio
-00001a00: 6e20 6f66 2064 6576 6963 6520 696e 206e  n of device in n
-00001a10: 4c2c 206f 7220 7265 7370 6f6e 7365 2073  L, or response s
-00001a20: 7472 696e 670d 0a20 2020 2020 2020 2022  tring..        "
-00001a30: 2222 0d0a 2020 2020 2020 2020 7265 7370  ""..        resp
-00001a40: 6f6e 7365 203d 2073 656c 662e 5f71 7565  onse = self._que
-00001a50: 7279 2827 4452 2729 0d0a 2020 2020 2020  ry('DR')..      
-00001a60: 2020 7472 793a 0d0a 2020 2020 2020 2020    try:..        
-00001a70: 2020 2020 7265 736f 6c75 7469 6f6e 203d      resolution =
-00001a80: 2069 6e74 2872 6573 706f 6e73 6529 0d0a   int(response)..
-00001a90: 2020 2020 2020 2020 6578 6365 7074 2056          except V
-00001aa0: 616c 7565 4572 726f 723a 0d0a 2020 2020  alueError:..    
-00001ab0: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-00001ac0: 6573 706f 6e73 650d 0a20 2020 2020 2020  esponse..       
-00001ad0: 2070 7269 6e74 2866 277b 7265 736f 6c75   print(f'{resolu
-00001ae0: 7469 6f6e 2f31 3030 307d 2075 4c20 2f20  tion/1000} uL / 
-00001af0: 7374 6570 2729 0d0a 2020 2020 2020 2020  step')..        
-00001b00: 7265 7475 726e 2072 6573 6f6c 7574 696f  return resolutio
-00001b10: 6e0d 0a20 2020 200d 0a20 2020 2064 6566  n..    ..    def
-00001b20: 205f 5f76 6572 7369 6f6e 5f5f 2873 656c   __version__(sel
-00001b30: 6629 202d 3e20 7374 723a 0d0a 2020 2020  f) -> str:..    
-00001b40: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-00001b50: 2052 6574 7269 6576 6520 7468 6520 736f   Retrieve the so
-00001b60: 6674 7761 7265 2076 6572 7369 6f6e 206f  ftware version o
-00001b70: 6e20 7468 6520 6465 7669 6365 0d0a 0d0a  n the device....
-00001b80: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
-00001b90: 0d0a 2020 2020 2020 2020 2020 2020 7374  ..            st
-00001ba0: 723a 2064 6576 6963 6520 7665 7273 696f  r: device versio
-00001bb0: 6e0d 0a20 2020 2020 2020 2022 2222 0d0a  n..        """..
-00001bc0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00001bd0: 656c 662e 5f71 7565 7279 2827 4456 2729  elf._query('DV')
-00001be0: 0d0a 0d0a 2020 2020 6465 6620 6164 6441  ....    def addA
-00001bf0: 6972 4761 7028 7365 6c66 2c20 7374 6570  irGap(self, step
-00001c00: 733a 696e 7420 3d20 3130 2920 2d3e 2073  s:int = 10) -> s
-00001c10: 7472 3a0d 0a20 2020 2020 2020 2022 2222  tr:..        """
-00001c20: 0d0a 2020 2020 2020 2020 4372 6561 7465  ..        Create
-00001c30: 2061 6e20 6169 7220 6761 7020 6265 7477   an air gap betw
-00001c40: 6565 6e20 7477 6f20 766f 6c75 6d65 7320  een two volumes 
-00001c50: 6f66 206c 6971 7569 6420 696e 2070 6970  of liquid in pip
-00001c60: 6574 7465 0d0a 2020 2020 2020 2020 0d0a  ette..        ..
-00001c70: 2020 2020 2020 2020 4172 6773 3a0d 0a20          Args:.. 
-00001c80: 2020 2020 2020 2020 2020 2073 7465 7073             steps
-00001c90: 2028 696e 742c 206f 7074 696f 6e61 6c29   (int, optional)
-00001ca0: 3a20 6e75 6d62 6572 206f 6620 7374 6570  : number of step
-00001cb0: 7320 666f 7220 6169 7220 6761 702e 2044  s for air gap. D
-00001cc0: 6566 6175 6c74 7320 746f 2044 4546 4155  efaults to DEFAU
-00001cd0: 4c54 5f41 4952 4741 502e 0d0a 2020 2020  LT_AIRGAP...    
-00001ce0: 2020 2020 2020 2020 6368 616e 6e65 6c20          channel 
-00001cf0: 2869 6e74 2c20 6f70 7469 6f6e 616c 293a  (int, optional):
-00001d00: 2063 6861 6e6e 656c 2074 6f20 6164 6420   channel to add 
-00001d10: 6169 7220 6761 702e 2044 6566 6175 6c74  air gap. Default
-00001d20: 7320 746f 204e 6f6e 652e 0d0a 0d0a 2020  s to None.....  
-00001d30: 2020 2020 2020 5265 7475 726e 733a 0d0a        Returns:..
-00001d40: 2020 2020 2020 2020 2020 2020 7374 723a              str:
-00001d50: 2064 6576 6963 6520 7265 7370 6f6e 7365   device response
-00001d60: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-00001d70: 2020 2020 2020 2072 6573 706f 6e73 6520         response 
-00001d80: 3d20 7365 6c66 2e5f 7175 6572 7928 6627  = self._query(f'
-00001d90: 5249 7b73 7465 7073 7d27 290d 0a20 2020  RI{steps}')..   
-00001da0: 2020 2020 2074 696d 652e 736c 6565 7028       time.sleep(
-00001db0: 3129 0d0a 2020 2020 2020 2020 7265 7475  1)..        retu
-00001dc0: 726e 2072 6573 706f 6e73 650d 0a20 2020  rn response..   
-00001dd0: 2020 2020 200d 0a20 2020 2064 6566 2061       ..    def a
-00001de0: 7370 6972 6174 6528 7365 6c66 2c20 0d0a  spirate(self, ..
-00001df0: 2020 2020 2020 2020 766f 6c75 6d65 3a20          volume: 
-00001e00: 666c 6f61 742c 200d 0a20 2020 2020 2020  float, ..       
-00001e10: 2073 7065 6564 3a20 4f70 7469 6f6e 616c   speed: Optional
-00001e20: 5b66 6c6f 6174 5d20 3d20 4e6f 6e65 2c20  [float] = None, 
-00001e30: 0d0a 2020 2020 2020 2020 7761 6974 3a20  ..        wait: 
-00001e40: 696e 7420 3d20 302c 200d 0a20 2020 2020  int = 0, ..     
-00001e50: 2020 2070 6175 7365 3a20 626f 6f6c 203d     pause: bool =
-00001e60: 2046 616c 7365 2c20 0d0a 2020 2020 2020   False, ..      
-00001e70: 2020 7265 6167 656e 743a 204f 7074 696f    reagent: Optio
-00001e80: 6e61 6c5b 7374 725d 203d 204e 6f6e 652c  nal[str] = None,
-00001e90: 0d0a 2020 2020 2020 2020 2a2a 6b77 6172  ..        **kwar
-00001ea0: 6773 0d0a 2020 2020 2920 2d3e 2073 7472  gs..    ) -> str
-00001eb0: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
-00001ec0: 2020 2020 2020 2020 4173 7069 7261 7465          Aspirate
-00001ed0: 2064 6573 6972 6564 2076 6f6c 756d 6520   desired volume 
-00001ee0: 6f66 2072 6561 6765 6e74 0d0a 0d0a 2020  of reagent....  
-00001ef0: 2020 2020 2020 4172 6773 3a0d 0a20 2020        Args:..   
-00001f00: 2020 2020 2020 2020 2076 6f6c 756d 6520           volume 
-00001f10: 2866 6c6f 6174 293a 2074 6172 6765 7420  (float): target 
-00001f20: 766f 6c75 6d65 0d0a 2020 2020 2020 2020  volume..        
-00001f30: 2020 2020 7370 6565 6420 284f 7074 696f      speed (Optio
-00001f40: 6e61 6c5b 666c 6f61 745d 2c20 6f70 7469  nal[float], opti
-00001f50: 6f6e 616c 293a 2073 7065 6564 2074 6f20  onal): speed to 
-00001f60: 6173 7069 7261 7465 2061 742e 2044 6566  aspirate at. Def
-00001f70: 6175 6c74 7320 746f 204e 6f6e 652e 0d0a  aults to None...
-00001f80: 2020 2020 2020 2020 2020 2020 7761 6974              wait
-00001f90: 2028 696e 742c 206f 7074 696f 6e61 6c29   (int, optional)
-00001fa0: 3a20 7469 6d65 2064 656c 6179 2061 6674  : time delay aft
-00001fb0: 6572 2061 7370 6972 6174 652e 2044 6566  er aspirate. Def
-00001fc0: 6175 6c74 7320 746f 2030 2e0d 0a20 2020  aults to 0...   
-00001fd0: 2020 2020 2020 2020 2070 6175 7365 2028           pause (
-00001fe0: 626f 6f6c 2c20 6f70 7469 6f6e 616c 293a  bool, optional):
-00001ff0: 2077 6865 7468 6572 2074 6f20 7061 7573   whether to paus
-00002000: 6520 666f 7220 7573 6572 2069 6e74 6572  e for user inter
-00002010: 7665 6e74 696f 6e2e 2044 6566 6175 6c74  vention. Default
-00002020: 7320 746f 2046 616c 7365 2e0d 0a20 2020  s to False...   
-00002030: 2020 2020 2020 2020 2072 6561 6765 6e74           reagent
-00002040: 2028 4f70 7469 6f6e 616c 5b73 7472 5d2c   (Optional[str],
-00002050: 206f 7074 696f 6e61 6c29 3a20 6e61 6d65   optional): name
-00002060: 206f 6620 7265 6167 656e 742e 2044 6566   of reagent. Def
-00002070: 6175 6c74 7320 746f 204e 6f6e 652e 0d0a  aults to None...
-00002080: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-00002090: 2020 2020 2020 5265 7475 726e 733a 0d0a        Returns:..
-000020a0: 2020 2020 2020 2020 2020 2020 7374 723a              str:
-000020b0: 2064 6576 6963 6520 7265 7370 6f6e 7365   device response
-000020c0: 0d0a 2020 2020 2020 2020 2222 2220 0d0a  ..        """ ..
-000020d0: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-000020e0: 466c 6167 2870 6175 7365 5f66 6565 6462  Flag(pause_feedb
-000020f0: 6163 6b3d 5472 7565 2c20 6f63 6375 7069  ack=True, occupi
-00002100: 6564 3d54 7275 6529 0d0a 2020 2020 2020  ed=True)..      
-00002110: 2020 766f 6c75 6d65 203d 206d 696e 2876    volume = min(v
-00002120: 6f6c 756d 652c 2073 656c 662e 6361 7061  olume, self.capa
-00002130: 6369 7479 202d 2073 656c 662e 766f 6c75  city - self.volu
-00002140: 6d65 290d 0a20 2020 2020 2020 2073 7465  me)..        ste
-00002150: 7073 203d 2069 6e74 2876 6f6c 756d 6520  ps = int(volume 
-00002160: 2f20 7365 6c66 2e72 6573 6f6c 7574 696f  / self.resolutio
-00002170: 6e29 0d0a 2020 2020 2020 2020 766f 6c75  n)..        volu
-00002180: 6d65 203d 2073 7465 7073 202a 2073 656c  me = steps * sel
-00002190: 662e 7265 736f 6c75 7469 6f6e 0d0a 2020  f.resolution..  
-000021a0: 2020 2020 2020 6966 2076 6f6c 756d 6520        if volume 
-000021b0: 3d3d 2030 3a0d 0a20 2020 2020 2020 2020  == 0:..         
-000021c0: 2020 2072 6574 7572 6e20 2727 0d0a 2020     return ''..  
-000021d0: 2020 2020 2020 7072 696e 7428 6627 4173        print(f'As
-000021e0: 7069 7261 7469 6e67 207b 766f 6c75 6d65  pirating {volume
-000021f0: 7d20 754c 2e2e 2e27 290d 0a20 2020 2020  } uL...')..     
-00002200: 2020 2073 7461 7274 5f61 7370 6972 6174     start_aspirat
-00002210: 6520 3d20 7469 6d65 2e74 696d 6528 290d  e = time.time().
-00002220: 0a20 2020 2020 2020 2073 7065 6564 203d  .        speed =
-00002230: 2073 656c 662e 7370 6565 642e 7570 2069   self.speed.up i
-00002240: 6620 7370 6565 6420 6973 204e 6f6e 6520  f speed is None 
-00002250: 656c 7365 2073 7065 6564 0d0a 2020 2020  else speed..    
-00002260: 2020 2020 0d0a 2020 2020 2020 2020 6966      ..        if
-00002270: 2073 7065 6564 2069 6e20 7365 6c66 2e73   speed in self.s
-00002280: 7065 6564 5f70 7265 7365 7473 3a0d 0a20  peed_presets:.. 
-00002290: 2020 2020 2020 2020 2020 2069 6620 7370             if sp
-000022a0: 6565 6420 213d 2073 656c 662e 7370 6565  eed != self.spee
-000022b0: 642e 7570 3a0d 0a20 2020 2020 2020 2020  d.up:..         
-000022c0: 2020 2020 2020 2073 656c 662e 7365 7453         self.setS
-000022d0: 7065 6564 2873 7065 6564 3d73 7065 6564  peed(speed=speed
-000022e0: 2c20 7570 3d54 7275 6529 0d0a 2020 2020  , up=True)..    
-000022f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00002300: 2e73 7065 6564 2e75 7020 3d20 7370 6565  .speed.up = spee
-00002310: 640d 0a20 2020 2020 2020 2020 2020 2073  d..            s
-00002320: 7461 7274 5f61 7370 6972 6174 6520 3d20  tart_aspirate = 
-00002330: 7469 6d65 2e74 696d 6528 290d 0a20 2020  time.time()..   
-00002340: 2020 2020 2020 2020 2072 6573 706f 6e73           respons
-00002350: 6520 3d20 7365 6c66 2e5f 7175 6572 7928  e = self._query(
-00002360: 6627 5249 7b73 7465 7073 7d27 290d 0a20  f'RI{steps}').. 
-00002370: 2020 2020 2020 2020 2020 206d 6f76 655f             move_
-00002380: 7469 6d65 203d 2073 7465 7073 2a73 656c  time = steps*sel
-00002390: 662e 7265 736f 6c75 7469 6f6e 202f 2073  f.resolution / s
-000023a0: 7065 6564 0d0a 2020 2020 2020 2020 2020  peed..          
-000023b0: 2020 7469 6d65 2e73 6c65 6570 286d 6f76    time.sleep(mov
-000023c0: 655f 7469 6d65 290d 0a20 2020 2020 2020  e_time)..       
-000023d0: 2020 2020 2023 2069 6620 7265 7370 6f6e       # if respon
-000023e0: 7365 2021 3d20 276f 6b27 3a0d 0a20 2020  se != 'ok':..   
-000023f0: 2020 2020 2020 2020 2023 2020 2020 2072           #     r
-00002400: 6574 7572 6e20 7265 7370 6f6e 7365 0d0a  eturn response..
-00002410: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-00002420: 2020 2020 2020 656c 6966 2073 7065 6564        elif speed
-00002430: 206e 6f74 2069 6e20 7365 6c66 2e73 7065   not in self.spe
-00002440: 6564 5f70 7265 7365 7473 3a0d 0a20 2020  ed_presets:..   
-00002450: 2020 2020 2020 2020 2070 7269 6e74 2866           print(f
-00002460: 2254 6172 6765 743a 207b 766f 6c75 6d65  "Target: {volume
-00002470: 7d20 754c 2061 7420 7b73 7065 6564 7d20  } uL at {speed} 
-00002480: 754c 2f73 2e2e 2e22 290d 0a20 2020 2020  uL/s...")..     
-00002490: 2020 2020 2020 2073 7065 6564 5f70 6172         speed_par
-000024a0: 616d 6574 6572 7320 3d20 7365 6c66 2e5f  ameters = self._
-000024b0: 6361 6c63 756c 6174 655f 7370 6565 645f  calculate_speed_
-000024c0: 7061 7261 6d65 7465 7273 2876 6f6c 756d  parameters(volum
-000024d0: 653d 766f 6c75 6d65 2c20 7370 6565 643d  e=volume, speed=
-000024e0: 7370 6565 6429 0d0a 2020 2020 2020 2020  speed)..        
-000024f0: 2020 2020 7072 696e 7428 7370 6565 645f      print(speed_
-00002500: 7061 7261 6d65 7465 7273 290d 0a20 2020  parameters)..   
-00002510: 2020 2020 2020 2020 2070 7265 7365 7420           preset 
-00002520: 3d20 7370 6565 645f 7061 7261 6d65 7465  = speed_paramete
-00002530: 7273 2e70 7265 7365 740d 0a20 2020 2020  rs.preset..     
-00002540: 2020 2020 2020 2069 6620 7072 6573 6574         if preset
-00002550: 2069 7320 4e6f 6e65 3a0d 0a20 2020 2020   is None:..     
-00002560: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00002570: 2052 756e 7469 6d65 4572 726f 7228 2754   RuntimeError('T
-00002580: 6172 6765 7420 7370 6565 6420 6e6f 7420  arget speed not 
-00002590: 706f 7373 6962 6c65 2e27 290d 0a20 2020  possible.')..   
-000025a0: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
-000025b0: 7453 7065 6564 2873 7065 6564 3d70 7265  tSpeed(speed=pre
-000025c0: 7365 742c 2075 703d 5472 7565 290d 0a20  set, up=True).. 
-000025d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000025e0: 7370 6565 642e 7570 203d 2073 7065 6564  speed.up = speed
-000025f0: 0d0a 2020 2020 2020 2020 2020 2020 7374  ..            st
-00002600: 6172 745f 6173 7069 7261 7465 203d 2074  art_aspirate = t
-00002610: 696d 652e 7469 6d65 2829 0d0a 2020 2020  ime.time()..    
-00002620: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00002630: 2020 2020 2020 7374 6570 735f 6c65 6674        steps_left
-00002640: 203d 2073 7465 7073 0d0a 2020 2020 2020   = steps..      
-00002650: 2020 2020 2020 6465 6c61 7920 3d20 7370        delay = sp
-00002660: 6565 645f 7061 7261 6d65 7465 7273 2e64  eed_parameters.d
-00002670: 656c 6179 0d0a 2020 2020 2020 2020 2020  elay..          
-00002680: 2020 7374 6570 5f73 697a 6520 3d20 7370    step_size = sp
-00002690: 6565 645f 7061 7261 6d65 7465 7273 2e73  eed_parameters.s
-000026a0: 7465 705f 7369 7a65 0d0a 2020 2020 2020  tep_size..      
-000026b0: 2020 2020 2020 696e 7465 7276 616c 7320        intervals 
-000026c0: 3d20 7370 6565 645f 7061 7261 6d65 7465  = speed_paramete
-000026d0: 7273 2e69 6e74 6572 7661 6c73 0d0a 2020  rs.intervals..  
-000026e0: 2020 2020 2020 2020 2020 666f 7220 6920            for i 
-000026f0: 696e 2072 616e 6765 2869 6e74 6572 7661  in range(interva
-00002700: 6c73 293a 0d0a 2020 2020 2020 2020 2020  ls):..          
-00002710: 2020 2020 2020 7374 6172 745f 7469 6d65        start_time
-00002720: 203d 2074 696d 652e 7469 6d65 2829 0d0a   = time.time()..
-00002730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002740: 7374 6570 203d 2073 7465 705f 7369 7a65  step = step_size
-00002750: 2069 6620 2869 2b31 2021 3d20 696e 7465   if (i+1 != inte
-00002760: 7276 616c 7329 2065 6c73 6520 7374 6570  rvals) else step
-00002770: 735f 6c65 6674 0d0a 2020 2020 2020 2020  s_left..        
-00002780: 2020 2020 2020 2020 6d6f 7665 5f74 696d          move_tim
-00002790: 6520 3d20 7374 6570 2a73 656c 662e 7265  e = step*self.re
-000027a0: 736f 6c75 7469 6f6e 202f 2070 7265 7365  solution / prese
-000027b0: 740d 0a20 2020 2020 2020 2020 2020 2020  t..             
-000027c0: 2020 2072 6573 706f 6e73 6520 3d20 7365     response = se
-000027d0: 6c66 2e5f 7175 6572 7928 6627 5249 7b73  lf._query(f'RI{s
-000027e0: 7465 707d 272c 2072 6573 756d 655f 6665  tep}', resume_fe
-000027f0: 6564 6261 636b 3d46 616c 7365 290d 0a20  edback=False).. 
-00002800: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00002810: 2069 6620 7265 7370 6f6e 7365 2021 3d20   if response != 
-00002820: 276f 6b27 3a0d 0a20 2020 2020 2020 2020  'ok':..         
-00002830: 2020 2020 2020 2023 2020 2020 2070 7269         #     pri
-00002840: 6e74 2822 4173 7069 7261 7469 6f6e 2066  nt("Aspiration f
-00002850: 6169 6c65 6422 290d 0a20 2020 2020 2020  ailed")..       
-00002860: 2020 2020 2020 2020 2023 2020 2020 2072           #     r
-00002870: 6574 7572 6e20 7265 7370 6f6e 7365 0d0a  eturn response..
-00002880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002890: 7374 6570 735f 6c65 6674 202d 3d20 7374  steps_left -= st
-000028a0: 6570 0d0a 2020 2020 2020 2020 2020 2020  ep..            
-000028b0: 2020 2020 6475 7261 7469 6f6e 203d 2074      duration = t
-000028c0: 696d 652e 7469 6d65 2829 202d 2073 7461  ime.time() - sta
-000028d0: 7274 5f74 696d 650d 0a20 2020 2020 2020  rt_time..       
-000028e0: 2020 2020 2020 2020 2069 6620 6475 7261           if dura
-000028f0: 7469 6f6e 203c 2028 6465 6c61 792b 6d6f  tion < (delay+mo
-00002900: 7665 5f74 696d 6529 3a0d 0a20 2020 2020  ve_time):..     
-00002910: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00002920: 696d 652e 736c 6565 7028 6465 6c61 792b  ime.sleep(delay+
-00002930: 6d6f 7665 5f74 696d 652d 6475 7261 7469  move_time-durati
-00002940: 6f6e 290d 0a20 2020 2020 2020 200d 0a20  on)..        .. 
-00002950: 2020 2020 2020 2023 2055 7064 6174 6520         # Update 
-00002960: 7661 6c75 6573 0d0a 2020 2020 2020 2020  values..        
-00002970: 7072 696e 7428 6627 4173 7069 7261 7469  print(f'Aspirati
-00002980: 6f6e 2074 696d 653a 207b 7469 6d65 2e74  on time: {time.t
-00002990: 696d 6528 292d 7374 6172 745f 6173 7069  ime()-start_aspi
-000029a0: 7261 7465 7d73 2729 0d0a 2020 2020 2020  rate}s')..      
-000029b0: 2020 7469 6d65 2e73 6c65 6570 2877 6169    time.sleep(wai
-000029c0: 7429 0d0a 2020 2020 2020 2020 7365 6c66  t)..        self
-000029d0: 2e73 6574 466c 6167 286f 6363 7570 6965  .setFlag(occupie
-000029e0: 643d 4661 6c73 652c 2070 6175 7365 5f66  d=False, pause_f
-000029f0: 6565 6462 6163 6b3d 4661 6c73 6529 0d0a  eedback=False)..
-00002a00: 2020 2020 2020 2020 7365 6c66 2e76 6f6c          self.vol
-00002a10: 756d 6520 2b3d 2076 6f6c 756d 650d 0a20  ume += volume.. 
-00002a20: 2020 2020 2020 2073 656c 662e 706f 7369         self.posi
-00002a30: 7469 6f6e 202b 3d20 7374 6570 730d 0a20  tion += steps.. 
-00002a40: 2020 2020 2020 2069 6620 7265 6167 656e         if reagen
-00002a50: 7420 6973 206e 6f74 204e 6f6e 653a 0d0a  t is not None:..
-00002a60: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00002a70: 2e72 6561 6765 6e74 203d 2072 6561 6765  .reagent = reage
-00002a80: 6e74 0d0a 2020 2020 2020 2020 6966 2070  nt..        if p
-00002a90: 6175 7365 3a0d 0a20 2020 2020 2020 2020  ause:..         
-00002aa0: 2020 2069 6e70 7574 2822 5072 6573 7320     input("Press 
-00002ab0: 2745 6e74 6572 2720 746f 2070 726f 6365  'Enter' to proce
-00002ac0: 6564 2e22 290d 0a20 2020 2020 2020 2072  ed.")..        r
-00002ad0: 6574 7572 6e20 7265 7370 6f6e 7365 0d0a  eturn response..
-00002ae0: 2020 2020 0d0a 2020 2020 6465 6620 626c      ..    def bl
-00002af0: 6f77 6f75 7428 7365 6c66 2c20 686f 6d65  owout(self, home
-00002b00: 3a62 6f6f 6c20 3d20 5472 7565 2c20 2a2a  :bool = True, **
-00002b10: 6b77 6172 6773 2920 2d3e 2073 7472 3a0d  kwargs) -> str:.
-00002b20: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-00002b30: 2020 2020 2020 426c 6f77 6f75 7420 6c69        Blowout li
-00002b40: 7175 6964 2066 726f 6d20 7469 700d 0a0d  quid from tip...
-00002b50: 0a20 2020 2020 2020 2041 7267 733a 0d0a  .        Args:..
-00002b60: 2020 2020 2020 2020 2020 2020 686f 6d65              home
-00002b70: 2028 626f 6f6c 2c20 6f70 7469 6f6e 616c   (bool, optional
-00002b80: 293a 2077 6865 7468 6572 2074 6f20 7265  ): whether to re
-00002b90: 7475 726e 2070 6c75 6e67 6572 2074 6f20  turn plunger to 
-00002ba0: 686f 6d65 2070 6f73 6974 696f 6e2e 2044  home position. D
-00002bb0: 6566 6175 6c74 7320 746f 2054 7275 652e  efaults to True.
-00002bc0: 0d0a 0d0a 2020 2020 2020 2020 5265 7475  ....        Retu
-00002bd0: 726e 733a 0d0a 2020 2020 2020 2020 2020  rns:..          
-00002be0: 2020 7374 723a 2064 6576 6963 6520 7265    str: device re
-00002bf0: 7370 6f6e 7365 0d0a 2020 2020 2020 2020  sponse..        
-00002c00: 2222 220d 0a20 2020 2020 2020 2063 6f6d  """..        com
-00002c10: 6d61 6e64 203d 2066 2752 427b 7365 6c66  mand = f'RB{self
-00002c20: 2e68 6f6d 655f 706f 7369 7469 6f6e 7d27  .home_position}'
-00002c30: 2069 6620 686f 6d65 2065 6c73 6520 2752   if home else 'R
-00002c40: 4227 0d0a 2020 2020 2020 2020 7265 7370  B'..        resp
-00002c50: 6f6e 7365 203d 2073 656c 662e 5f71 7565  onse = self._que
-00002c60: 7279 2863 6f6d 6d61 6e64 290d 0a20 2020  ry(command)..   
-00002c70: 2020 2020 2073 656c 662e 706f 7369 7469       self.positi
-00002c80: 6f6e 203d 2073 656c 662e 686f 6d65 5f70  on = self.home_p
-00002c90: 6f73 6974 696f 6e0d 0a20 2020 2020 2020  osition..       
-00002ca0: 2074 696d 652e 736c 6565 7028 3129 0d0a   time.sleep(1)..
-00002cb0: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-00002cc0: 6573 706f 6e73 650d 0a20 2020 200d 0a20  esponse..    .. 
-00002cd0: 2020 2064 6566 2064 6973 7065 6e73 6528     def dispense(
-00002ce0: 7365 6c66 2c20 0d0a 2020 2020 2020 2020  self, ..        
-00002cf0: 766f 6c75 6d65 3a20 666c 6f61 742c 200d  volume: float, .
-00002d00: 0a20 2020 2020 2020 2073 7065 6564 3a20  .        speed: 
-00002d10: 4f70 7469 6f6e 616c 5b66 6c6f 6174 5d20  Optional[float] 
-00002d20: 3d20 4e6f 6e65 2c20 0d0a 2020 2020 2020  = None, ..      
-00002d30: 2020 7761 6974 3a20 696e 7420 3d20 302c    wait: int = 0,
-00002d40: 200d 0a20 2020 2020 2020 2070 6175 7365   ..        pause
-00002d50: 3a20 626f 6f6c 203d 2046 616c 7365 2c20  : bool = False, 
-00002d60: 0d0a 2020 2020 2020 2020 626c 6f77 6f75  ..        blowou
-00002d70: 743a 2062 6f6f 6c20 3d20 4661 6c73 652c  t: bool = False,
-00002d80: 0d0a 2020 2020 2020 2020 626c 6f77 6f75  ..        blowou
-00002d90: 745f 686f 6d65 3a20 626f 6f6c 203d 2054  t_home: bool = T
-00002da0: 7275 652c 0d0a 2020 2020 2020 2020 666f  rue,..        fo
-00002db0: 7263 655f 6469 7370 656e 7365 3a20 626f  rce_dispense: bo
-00002dc0: 6f6c 203d 2046 616c 7365 2c20 0d0a 2020  ol = False, ..  
-00002dd0: 2020 2020 2020 2a2a 6b77 6172 6773 0d0a        **kwargs..
-00002de0: 2020 2020 2920 2d3e 2073 7472 3a0d 0a20      ) -> str:.. 
-00002df0: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-00002e00: 2020 2020 4469 7370 656e 7365 2064 6573      Dispense des
-00002e10: 6972 6564 2076 6f6c 756d 6520 6f66 2072  ired volume of r
-00002e20: 6561 6765 6e74 0d0a 0d0a 2020 2020 2020  eagent....      
-00002e30: 2020 4172 6773 3a0d 0a20 2020 2020 2020    Args:..       
-00002e40: 2020 2020 2076 6f6c 756d 6520 2866 6c6f       volume (flo
-00002e50: 6174 293a 2074 6172 6765 7420 766f 6c75  at): target volu
-00002e60: 6d65 0d0a 2020 2020 2020 2020 2020 2020  me..            
-00002e70: 7370 6565 6420 284f 7074 696f 6e61 6c5b  speed (Optional[
-00002e80: 666c 6f61 745d 2c20 6f70 7469 6f6e 616c  float], optional
-00002e90: 293a 2073 7065 6564 2074 6f20 6469 7370  ): speed to disp
-00002ea0: 656e 7365 2061 742e 2044 6566 6175 6c74  ense at. Default
-00002eb0: 7320 746f 204e 6f6e 652e 0d0a 2020 2020  s to None...    
-00002ec0: 2020 2020 2020 2020 7761 6974 2028 696e          wait (in
-00002ed0: 742c 206f 7074 696f 6e61 6c29 3a20 7469  t, optional): ti
-00002ee0: 6d65 2064 656c 6179 2061 6674 6572 2064  me delay after d
-00002ef0: 6973 7065 6e73 652e 2044 6566 6175 6c74  ispense. Default
-00002f00: 7320 746f 2030 2e0d 0a20 2020 2020 2020  s to 0...       
-00002f10: 2020 2020 2070 6175 7365 2028 626f 6f6c       pause (bool
-00002f20: 2c20 6f70 7469 6f6e 616c 293a 2077 6865  , optional): whe
-00002f30: 7468 6572 2074 6f20 7061 7573 6520 666f  ther to pause fo
-00002f40: 7220 7573 6572 2069 6e74 6572 7665 6e74  r user intervent
-00002f50: 696f 6e2e 2044 6566 6175 6c74 7320 746f  ion. Defaults to
-00002f60: 2046 616c 7365 2e0d 0a20 2020 2020 2020   False...       
-00002f70: 2020 2020 2062 6c6f 776f 7574 2028 626f       blowout (bo
-00002f80: 6f6c 2c20 6f70 7469 6f6e 616c 293a 2077  ol, optional): w
-00002f90: 6865 7468 6572 2070 6572 666f 726d 2062  hether perform b
-00002fa0: 6c6f 776f 7574 2e20 4465 6661 756c 7473  lowout. Defaults
-00002fb0: 2074 6f20 4661 6c73 652e 0d0a 2020 2020   to False...    
-00002fc0: 2020 2020 2020 2020 626c 6f77 6f75 745f          blowout_
-00002fd0: 686f 6d65 2028 626f 6f6c 2c20 6f70 7469  home (bool, opti
-00002fe0: 6f6e 616c 293a 2077 6865 7468 6572 2074  onal): whether t
-00002ff0: 6f20 7265 7475 726e 2074 6865 2070 6c75  o return the plu
-00003000: 6e67 6572 2068 6f6d 6520 6166 7465 7220  nger home after 
-00003010: 626c 6f77 6f75 742e 2044 6566 6175 6c74  blowout. Default
-00003020: 7320 746f 2054 7275 652e 0d0a 2020 2020  s to True...    
-00003030: 2020 2020 2020 2020 666f 7263 655f 6469          force_di
-00003040: 7370 656e 7365 2028 626f 6f6c 2c20 6f70  spense (bool, op
-00003050: 7469 6f6e 616c 293a 2077 6865 7468 6572  tional): whether
-00003060: 2074 6f20 6469 7370 656e 7365 2072 6561   to dispense rea
-00003070: 6765 6e74 2072 6567 6172 646c 6573 732e  gent regardless.
-00003080: 2044 6566 6175 6c74 7320 746f 2046 616c   Defaults to Fal
-00003090: 7365 2e0d 0a0d 0a20 2020 2020 2020 2052  se.....        R
-000030a0: 6169 7365 733a 0d0a 2020 2020 2020 2020  aises:..        
-000030b0: 2020 2020 5661 6c75 6545 7272 6f72 3a20      ValueError: 
-000030c0: 5265 7175 6972 6564 2064 6973 7065 6e73  Required dispens
-000030d0: 6520 766f 6c75 6d65 2069 7320 6772 6561  e volume is grea
-000030e0: 7465 7220 7468 616e 2076 6f6c 756d 6520  ter than volume 
-000030f0: 696e 2074 6970 0d0a 0d0a 2020 2020 2020  in tip....      
-00003100: 2020 5265 7475 726e 733a 0d0a 2020 2020    Returns:..    
-00003110: 2020 2020 2020 2020 7374 723a 2064 6576          str: dev
-00003120: 6963 6520 7265 7370 6f6e 7365 0d0a 2020  ice response..  
-00003130: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-00003140: 2020 2073 656c 662e 7365 7446 6c61 6728     self.setFlag(
-00003150: 7061 7573 655f 6665 6564 6261 636b 3d54  pause_feedback=T
-00003160: 7275 652c 206f 6363 7570 6965 643d 5472  rue, occupied=Tr
-00003170: 7565 290d 0a20 2020 2020 2020 2069 6620  ue)..        if 
-00003180: 666f 7263 655f 6469 7370 656e 7365 3a0d  force_dispense:.
-00003190: 0a20 2020 2020 2020 2020 2020 2076 6f6c  .            vol
-000031a0: 756d 6520 3d20 6d69 6e28 766f 6c75 6d65  ume = min(volume
-000031b0: 2c20 7365 6c66 2e76 6f6c 756d 6529 0d0a  , self.volume)..
-000031c0: 2020 2020 2020 2020 656c 6966 2076 6f6c          elif vol
-000031d0: 756d 6520 3e20 7365 6c66 2e76 6f6c 756d  ume > self.volum
-000031e0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-000031f0: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
-00003200: 2827 5265 7175 6972 6564 2064 6973 7065  ('Required dispe
-00003210: 6e73 6520 766f 6c75 6d65 2069 7320 6772  nse volume is gr
-00003220: 6561 7465 7220 7468 616e 2076 6f6c 756d  eater than volum
-00003230: 6520 696e 2074 6970 2e27 290d 0a20 2020  e in tip.')..   
-00003240: 2020 2020 2073 7465 7073 203d 2069 6e74       steps = int
-00003250: 2876 6f6c 756d 6520 2f20 7365 6c66 2e72  (volume / self.r
-00003260: 6573 6f6c 7574 696f 6e29 0d0a 2020 2020  esolution)..    
-00003270: 2020 2020 766f 6c75 6d65 203d 2073 7465      volume = ste
-00003280: 7073 202a 2073 656c 662e 7265 736f 6c75  ps * self.resolu
-00003290: 7469 6f6e 0d0a 2020 2020 2020 2020 6966  tion..        if
-000032a0: 2076 6f6c 756d 6520 3d3d 2030 3a0d 0a20   volume == 0:.. 
-000032b0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000032c0: 6e20 2727 0d0a 2020 2020 2020 2020 7072  n ''..        pr
-000032d0: 696e 7428 6627 4469 7370 656e 7369 6e67  int(f'Dispensing
-000032e0: 207b 766f 6c75 6d65 7d20 754c 2e2e 2e27   {volume} uL...'
-000032f0: 290d 0a20 2020 2020 2020 2073 7461 7274  )..        start
-00003300: 5f64 6973 7065 6e73 6520 3d20 7469 6d65  _dispense = time
-00003310: 2e74 696d 6528 290d 0a20 2020 2020 2020  .time()..       
-00003320: 2073 7065 6564 203d 2073 656c 662e 7370   speed = self.sp
-00003330: 6565 642e 646f 776e 2069 6620 7370 6565  eed.down if spee
-00003340: 6420 6973 204e 6f6e 6520 656c 7365 2073  d is None else s
-00003350: 7065 6564 0d0a 0d0a 2020 2020 2020 2020  peed....        
-00003360: 6966 2073 7065 6564 2069 6e20 7365 6c66  if speed in self
-00003370: 2e73 7065 6564 5f70 7265 7365 7473 3a0d  .speed_presets:.
-00003380: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00003390: 7370 6565 6420 213d 2073 656c 662e 7370  speed != self.sp
-000033a0: 6565 642e 646f 776e 3a0d 0a20 2020 2020  eed.down:..     
-000033b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000033c0: 7365 7453 7065 6564 2873 7065 6564 3d73  setSpeed(speed=s
-000033d0: 7065 6564 2c20 7570 3d46 616c 7365 290d  peed, up=False).
-000033e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000033f0: 2073 656c 662e 7370 6565 642e 646f 776e   self.speed.down
-00003400: 203d 2073 7065 6564 0d0a 2020 2020 2020   = speed..      
-00003410: 2020 2020 2020 7374 6172 745f 6469 7370        start_disp
-00003420: 656e 7365 203d 2074 696d 652e 7469 6d65  ense = time.time
-00003430: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-00003440: 7265 7370 6f6e 7365 203d 2073 656c 662e  response = self.
-00003450: 5f71 7565 7279 2866 2752 4f7b 7374 6570  _query(f'RO{step
-00003460: 737d 2729 0d0a 2020 2020 2020 2020 2020  s}')..          
-00003470: 2020 6d6f 7665 5f74 696d 6520 3d20 7374    move_time = st
-00003480: 6570 732a 7365 6c66 2e72 6573 6f6c 7574  eps*self.resolut
-00003490: 696f 6e20 2f20 7370 6565 640d 0a20 2020  ion / speed..   
-000034a0: 2020 2020 2020 2020 2074 696d 652e 736c           time.sl
-000034b0: 6565 7028 6d6f 7665 5f74 696d 6529 0d0a  eep(move_time)..
-000034c0: 2020 2020 2020 2020 2020 2020 2320 6966              # if
-000034d0: 2072 6573 706f 6e73 6520 213d 2027 6f6b   response != 'ok
-000034e0: 273a 0d0a 2020 2020 2020 2020 2020 2020  ':..            
-000034f0: 2320 2020 2020 7265 7475 726e 2072 6573  #     return res
-00003500: 706f 6e73 650d 0a20 2020 2020 2020 2020  ponse..         
-00003510: 2020 200d 0a20 2020 2020 2020 2065 6c69     ..        eli
-00003520: 6620 7370 6565 6420 6e6f 7420 696e 2073  f speed not in s
-00003530: 656c 662e 7370 6565 645f 7072 6573 6574  elf.speed_preset
-00003540: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-00003550: 7072 696e 7428 6622 5461 7267 6574 3a20  print(f"Target: 
-00003560: 7b76 6f6c 756d 657d 2075 4c20 6174 207b  {volume} uL at {
-00003570: 7370 6565 647d 2075 4c2f 732e 2e2e 2229  speed} uL/s...")
-00003580: 0d0a 2020 2020 2020 2020 2020 2020 7370  ..            sp
-00003590: 6565 645f 7061 7261 6d65 7465 7273 203d  eed_parameters =
-000035a0: 2073 656c 662e 5f63 616c 6375 6c61 7465   self._calculate
-000035b0: 5f73 7065 6564 5f70 6172 616d 6574 6572  _speed_parameter
-000035c0: 7328 766f 6c75 6d65 3d76 6f6c 756d 652c  s(volume=volume,
-000035d0: 2073 7065 6564 3d73 7065 6564 290d 0a20   speed=speed).. 
-000035e0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-000035f0: 2873 7065 6564 5f70 6172 616d 6574 6572  (speed_parameter
-00003600: 7329 0d0a 2020 2020 2020 2020 2020 2020  s)..            
-00003610: 7072 6573 6574 203d 2073 7065 6564 5f70  preset = speed_p
-00003620: 6172 616d 6574 6572 732e 7072 6573 6574  arameters.preset
-00003630: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00003640: 2070 7265 7365 7420 6973 204e 6f6e 653a   preset is None:
-00003650: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00003660: 2020 7261 6973 6520 5275 6e74 696d 6545    raise RuntimeE
-00003670: 7272 6f72 2827 5461 7267 6574 2073 7065  rror('Target spe
-00003680: 6564 206e 6f74 2070 6f73 7369 626c 652e  ed not possible.
-00003690: 2729 0d0a 2020 2020 2020 2020 2020 2020  ')..            
-000036a0: 7365 6c66 2e73 6574 5370 6565 6428 7370  self.setSpeed(sp
-000036b0: 6565 643d 7072 6573 6574 2c20 7570 3d46  eed=preset, up=F
-000036c0: 616c 7365 290d 0a20 2020 2020 2020 2020  alse)..         
-000036d0: 2020 2073 656c 662e 7370 6565 642e 646f     self.speed.do
-000036e0: 776e 203d 2073 7065 6564 0d0a 2020 2020  wn = speed..    
-000036f0: 2020 2020 2020 2020 7374 6172 745f 6469          start_di
-00003700: 7370 656e 7365 203d 2074 696d 652e 7469  spense = time.ti
-00003710: 6d65 2829 0d0a 2020 2020 2020 2020 0d0a  me()..        ..
-00003720: 2020 2020 2020 2020 2020 2020 7374 6570              step
-00003730: 735f 6c65 6674 203d 2073 7465 7073 0d0a  s_left = steps..
-00003740: 2020 2020 2020 2020 2020 2020 6465 6c61              dela
-00003750: 7920 3d20 7370 6565 645f 7061 7261 6d65  y = speed_parame
-00003760: 7465 7273 2e64 656c 6179 0d0a 2020 2020  ters.delay..    
-00003770: 2020 2020 2020 2020 7374 6570 5f73 697a          step_siz
-00003780: 6520 3d20 7370 6565 645f 7061 7261 6d65  e = speed_parame
-00003790: 7465 7273 2e73 7465 705f 7369 7a65 0d0a  ters.step_size..
-000037a0: 2020 2020 2020 2020 2020 2020 696e 7465              inte
-000037b0: 7276 616c 7320 3d20 7370 6565 645f 7061  rvals = speed_pa
-000037c0: 7261 6d65 7465 7273 2e69 6e74 6572 7661  rameters.interva
-000037d0: 6c73 0d0a 2020 2020 2020 2020 2020 2020  ls..            
-000037e0: 666f 7220 6920 696e 2072 616e 6765 2869  for i in range(i
-000037f0: 6e74 6572 7661 6c73 293a 0d0a 2020 2020  ntervals):..    
-00003800: 2020 2020 2020 2020 2020 2020 7374 6172              star
-00003810: 745f 7469 6d65 203d 2074 696d 652e 7469  t_time = time.ti
-00003820: 6d65 2829 0d0a 2020 2020 2020 2020 2020  me()..          
-00003830: 2020 2020 2020 7374 6570 203d 2073 7465        step = ste
-00003840: 705f 7369 7a65 2069 6620 2869 2b31 2021  p_size if (i+1 !
-00003850: 3d20 696e 7465 7276 616c 7329 2065 6c73  = intervals) els
-00003860: 6520 7374 6570 735f 6c65 6674 0d0a 2020  e steps_left..  
-00003870: 2020 2020 2020 2020 2020 2020 2020 6d6f                mo
-00003880: 7665 5f74 696d 6520 3d20 7374 6570 2a73  ve_time = step*s
-00003890: 656c 662e 7265 736f 6c75 7469 6f6e 202f  elf.resolution /
-000038a0: 2070 7265 7365 740d 0a20 2020 2020 2020   preset..       
-000038b0: 2020 2020 2020 2020 2072 6573 706f 6e73           respons
-000038c0: 6520 3d20 7365 6c66 2e5f 7175 6572 7928  e = self._query(
-000038d0: 6627 524f 7b73 7465 707d 272c 2072 6573  f'RO{step}', res
-000038e0: 756d 655f 6665 6564 6261 636b 3d46 616c  ume_feedback=Fal
-000038f0: 7365 290d 0a20 2020 2020 2020 2020 2020  se)..           
-00003900: 2020 2020 2023 2069 6620 7265 7370 6f6e       # if respon
-00003910: 7365 2021 3d20 276f 6b27 3a0d 0a20 2020  se != 'ok':..   
-00003920: 2020 2020 2020 2020 2020 2020 2023 2020               #  
-00003930: 2020 2070 7269 6e74 2822 4469 7370 656e     print("Dispen
-00003940: 7365 2066 6169 6c65 6422 290d 0a20 2020  se failed")..   
-00003950: 2020 2020 2020 2020 2020 2020 2023 2020               #  
-00003960: 2020 2072 6574 7572 6e20 7265 7370 6f6e     return respon
-00003970: 7365 0d0a 2020 2020 2020 2020 2020 2020  se..            
-00003980: 2020 2020 7374 6570 735f 6c65 6674 202d      steps_left -
-00003990: 3d20 7374 6570 0d0a 2020 2020 2020 2020  = step..        
-000039a0: 2020 2020 2020 2020 6475 7261 7469 6f6e          duration
-000039b0: 203d 2074 696d 652e 7469 6d65 2829 202d   = time.time() -
-000039c0: 2073 7461 7274 5f74 696d 650d 0a20 2020   start_time..   
-000039d0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-000039e0: 6475 7261 7469 6f6e 203c 2028 6465 6c61  duration < (dela
-000039f0: 792b 6d6f 7665 5f74 696d 6529 3a0d 0a20  y+move_time):.. 
-00003a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a10: 2020 2074 696d 652e 736c 6565 7028 6465     time.sleep(de
-00003a20: 6c61 792b 6d6f 7665 5f74 696d 652d 6475  lay+move_time-du
-00003a30: 7261 7469 6f6e 290d 0a0d 0a20 2020 2020  ration)....     
-00003a40: 2020 2023 2055 7064 6174 6520 7661 6c75     # Update valu
-00003a50: 6573 0d0a 2020 2020 2020 2020 7072 696e  es..        prin
-00003a60: 7428 6627 4469 7370 656e 7365 2074 696d  t(f'Dispense tim
-00003a70: 653a 207b 7469 6d65 2e74 696d 6528 292d  e: {time.time()-
-00003a80: 7374 6172 745f 6469 7370 656e 7365 7d73  start_dispense}s
-00003a90: 2729 0d0a 2020 2020 2020 2020 7469 6d65  ')..        time
-00003aa0: 2e73 6c65 6570 2877 6169 7429 0d0a 2020  .sleep(wait)..  
-00003ab0: 2020 2020 2020 7365 6c66 2e73 6574 466c        self.setFl
-00003ac0: 6167 286f 6363 7570 6965 643d 4661 6c73  ag(occupied=Fals
-00003ad0: 652c 2070 6175 7365 5f66 6565 6462 6163  e, pause_feedbac
-00003ae0: 6b3d 4661 6c73 6529 0d0a 2020 2020 2020  k=False)..      
-00003af0: 2020 7365 6c66 2e76 6f6c 756d 6520 3d20    self.volume = 
-00003b00: 6d61 7828 7365 6c66 2e76 6f6c 756d 6520  max(self.volume 
-00003b10: 2d20 766f 6c75 6d65 2c20 3029 0d0a 2020  - volume, 0)..  
-00003b20: 2020 2020 2020 7365 6c66 2e70 6f73 6974        self.posit
-00003b30: 696f 6e20 2d3d 2073 7465 7073 0d0a 2020  ion -= steps..  
-00003b40: 2020 2020 2020 6966 2073 656c 662e 766f        if self.vo
-00003b50: 6c75 6d65 203d 3d20 3020 616e 6420 626c  lume == 0 and bl
-00003b60: 6f77 6f75 743a 0d0a 2020 2020 2020 2020  owout:..        
-00003b70: 2020 2020 7365 6c66 2e62 6c6f 776f 7574      self.blowout
-00003b80: 2868 6f6d 653d 626c 6f77 6f75 745f 686f  (home=blowout_ho
-00003b90: 6d65 290d 0a20 2020 2020 2020 2069 6620  me)..        if 
-00003ba0: 7061 7573 653a 0d0a 2020 2020 2020 2020  pause:..        
-00003bb0: 2020 2020 696e 7075 7428 2250 7265 7373      input("Press
-00003bc0: 2027 456e 7465 7227 2074 6f20 7072 6f63   'Enter' to proc
-00003bd0: 6565 642e 2229 0d0a 2020 2020 2020 2020  eed.")..        
-00003be0: 7265 7475 726e 2072 6573 706f 6e73 650d  return response.
-00003bf0: 0a20 2020 200d 0a20 2020 2064 6566 2065  .    ..    def e
-00003c00: 6a65 6374 2873 656c 662c 2068 6f6d 653a  ject(self, home:
-00003c10: 626f 6f6c 203d 2054 7275 6529 202d 3e20  bool = True) -> 
-00003c20: 7374 723a 0d0a 2020 2020 2020 2020 2222  str:..        ""
-00003c30: 220d 0a20 2020 2020 2020 2045 6a65 6374  "..        Eject
-00003c40: 2074 6865 2070 6970 6574 7465 2074 6970   the pipette tip
-00003c50: 0d0a 0d0a 2020 2020 2020 2020 4172 6773  ....        Args
-00003c60: 3a0d 0a20 2020 2020 2020 2020 2020 2068  :..            h
-00003c70: 6f6d 6520 2862 6f6f 6c2c 206f 7074 696f  ome (bool, optio
-00003c80: 6e61 6c29 3a20 7768 6574 6865 7220 746f  nal): whether to
-00003c90: 2072 6574 7572 6e20 706c 756e 6765 7220   return plunger 
-00003ca0: 746f 2068 6f6d 6520 706f 7369 7469 6f6e  to home position
-00003cb0: 2e20 4465 6661 756c 7473 2074 6f20 5472  . Defaults to Tr
-00003cc0: 7565 2e0d 0a0d 0a20 2020 2020 2020 2052  ue.....        R
-00003cd0: 6574 7572 6e73 3a0d 0a20 2020 2020 2020  eturns:..       
-00003ce0: 2020 2020 2073 7472 3a20 6465 7669 6365       str: device
-00003cf0: 2072 6573 706f 6e73 650d 0a20 2020 2020   response..     
-00003d00: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-00003d10: 7365 6c66 2e72 6561 6765 6e74 203d 2027  self.reagent = '
-00003d20: 270d 0a20 2020 2020 2020 2063 6f6d 6d61  '..        comma
-00003d30: 6e64 203d 2066 2752 457b 7365 6c66 2e68  nd = f'RE{self.h
-00003d40: 6f6d 655f 706f 7369 7469 6f6e 7d27 2069  ome_position}' i
-00003d50: 6620 686f 6d65 2065 6c73 6520 2752 4527  f home else 'RE'
-00003d60: 0d0a 2020 2020 2020 2020 7265 7370 6f6e  ..        respon
-00003d70: 7365 203d 2073 656c 662e 5f71 7565 7279  se = self._query
-00003d80: 2863 6f6d 6d61 6e64 290d 0a20 2020 2020  (command)..     
-00003d90: 2020 2073 656c 662e 706f 7369 7469 6f6e     self.position
-00003da0: 203d 2073 656c 662e 686f 6d65 5f70 6f73   = self.home_pos
-00003db0: 6974 696f 6e20 6966 2068 6f6d 6520 656c  ition if home el
-00003dc0: 7365 2030 0d0a 2020 2020 2020 2020 7469  se 0..        ti
-00003dd0: 6d65 2e73 6c65 6570 2831 290d 0a20 2020  me.sleep(1)..   
-00003de0: 2020 2020 2072 6574 7572 6e20 7265 7370       return resp
-00003df0: 6f6e 7365 0d0a 2020 2020 0d0a 2020 2020  onse..    ..    
-00003e00: 6465 6620 656d 7074 7928 7365 6c66 2c20  def empty(self, 
-00003e10: 2a2a 6b77 6172 6773 293a 0d0a 2020 2020  **kwargs):..    
-00003e20: 2020 2020 2222 2245 6d70 7479 2074 6865      """Empty the
-00003e30: 2070 6970 6574 7465 2222 220d 0a20 2020   pipette"""..   
-00003e40: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00003e50: 2e68 6f6d 6528 290d 0a20 2020 200d 0a20  .home()..    .. 
-00003e60: 2020 2064 6566 2067 6574 4361 7061 6369     def getCapaci
-00003e70: 7461 6e63 6528 7365 6c66 2920 2d3e 2055  tance(self) -> U
-00003e80: 6e69 6f6e 5b69 6e74 2c20 7374 725d 3a0d  nion[int, str]:.
-00003e90: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-00003ea0: 2020 2020 2020 4765 7420 7468 6520 6361        Get the ca
-00003eb0: 7061 6369 7461 6e63 6520 6173 206d 6561  pacitance as mea
-00003ec0: 7375 7265 6420 6174 2074 6865 2065 6e64  sured at the end
-00003ed0: 206f 6620 7468 6520 7069 7065 7474 650d   of the pipette.
-00003ee0: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
-00003ef0: 2020 2052 6574 7572 6e73 3a0d 0a20 2020     Returns:..   
-00003f00: 2020 2020 2020 2020 2055 6e69 6f6e 5b69           Union[i
-00003f10: 6e74 2c20 7374 725d 3a20 6361 7061 6369  nt, str]: capaci
-00003f20: 7461 6e63 6520 7661 6c75 652c 206f 7220  tance value, or 
-00003f30: 6465 7669 6365 2072 6573 706f 6e73 650d  device response.
-00003f40: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-00003f50: 2020 2020 2020 7265 7370 6f6e 7365 203d        response =
-00003f60: 2073 656c 662e 5f71 7565 7279 2827 444e   self._query('DN
-00003f70: 2729 0d0a 2020 2020 2020 2020 7472 793a  ')..        try:
-00003f80: 0d0a 2020 2020 2020 2020 2020 2020 6361  ..            ca
-00003f90: 7061 6369 7461 6e63 6520 3d20 696e 7428  pacitance = int(
-00003fa0: 7265 7370 6f6e 7365 290d 0a20 2020 2020  response)..     
-00003fb0: 2020 2065 7863 6570 7420 5661 6c75 6545     except ValueE
-00003fc0: 7272 6f72 3a0d 0a20 2020 2020 2020 2020  rror:..         
-00003fd0: 2020 2072 6574 7572 6e20 7265 7370 6f6e     return respon
-00003fe0: 7365 0d0a 2020 2020 2020 2020 7365 6c66  se..        self
-00003ff0: 2e5f 6361 7061 6369 7461 6e63 6520 3d20  ._capacitance = 
-00004000: 6361 7061 6369 7461 6e63 650d 0a20 2020  capacitance..   
-00004010: 2020 2020 2072 6574 7572 6e20 6361 7061       return capa
-00004020: 6369 7461 6e63 650d 0a20 0d0a 2020 2020  citance.. ..    
-00004030: 6465 6620 6765 7445 7272 6f72 7328 7365  def getErrors(se
-00004040: 6c66 2920 2d3e 2073 7472 3a0d 0a20 2020  lf) -> str:..   
-00004050: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-00004060: 2020 4765 7420 6572 726f 7273 2066 726f    Get errors fro
-00004070: 6d20 7468 6520 6465 7669 6365 0d0a 0d0a  m the device....
-00004080: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
-00004090: 0d0a 2020 2020 2020 2020 2020 2020 7374  ..            st
-000040a0: 723a 2064 6576 6963 6520 7265 7370 6f6e  r: device respon
-000040b0: 7365 0d0a 2020 2020 2020 2020 2222 220d  se..        """.
-000040c0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000040d0: 7365 6c66 2e5f 7175 6572 7928 2744 4527  self._query('DE'
-000040e0: 290d 0a20 2020 200d 0a20 2020 2064 6566  )..    ..    def
-000040f0: 2067 6574 496e 666f 2873 656c 662c 206d   getInfo(self, m
-00004100: 6f64 656c 3a20 4f70 7469 6f6e 616c 5b73  odel: Optional[s
-00004110: 7472 5d20 3d20 4e6f 6e65 293a 0d0a 2020  tr] = None):..  
-00004120: 2020 2020 2020 2222 2247 6574 2064 6574        """Get det
-00004130: 6169 6c73 206f 6620 7468 6520 5361 7274  ails of the Sart
-00004140: 6f72 6975 7320 7069 7065 7474 6520 6d6f  orius pipette mo
-00004150: 6465 6c22 2222 0d0a 2020 2020 2020 2020  del"""..        
-00004160: 6d6f 6465 6c20 3d20 7365 6c66 2e5f 5f6d  model = self.__m
-00004170: 6f64 656c 5f5f 2829 2e73 706c 6974 2827  odel__().split('
-00004180: 2d27 295b 305d 2069 6620 6d6f 6465 6c20  -')[0] if model 
-00004190: 6973 204e 6f6e 6520 656c 7365 206d 6f64  is None else mod
-000041a0: 656c 0d0a 2020 2020 2020 2020 6966 206d  el..        if m
-000041b0: 6f64 656c 206e 6f74 2069 6e20 4d6f 6465  odel not in Mode
-000041c0: 6c49 6e66 6f2e 5f6d 656d 6265 725f 6e61  lInfo._member_na
-000041d0: 6d65 735f 3a0d 0a20 2020 2020 2020 2020  mes_:..         
-000041e0: 2020 2070 7269 6e74 2866 2752 6563 6569     print(f'Recei
-000041f0: 7665 643a 207b 6d6f 6465 6c7d 2729 0d0a  ved: {model}')..
-00004200: 2020 2020 2020 2020 2020 2020 6d6f 6465              mode
-00004210: 6c20 3d20 2742 524c 3027 0d0a 2020 2020  l = 'BRL0'..    
-00004220: 2020 2020 2020 2020 7072 696e 7428 6622          print(f"
-00004230: 4465 6661 756c 7469 6e67 2074 6f3a 207b  Defaulting to: {
-00004240: 2742 524c 3027 7d22 290d 0a20 2020 2020  'BRL0'}")..     
-00004250: 2020 2020 2020 2070 7269 6e74 2866 2256         print(f"V
-00004260: 616c 6964 206d 6f64 656c 7320 6172 653a  alid models are:
-00004270: 207b 272c 2027 2e6a 6f69 6e28 4d6f 6465   {', '.join(Mode
-00004280: 6c49 6e66 6f2e 5f6d 656d 6265 725f 6e61  lInfo._member_na
-00004290: 6d65 735f 297d 2229 0d0a 2020 2020 2020  mes_)}")..      
-000042a0: 2020 696e 666f 3a20 4d6f 6465 6c20 3d20    info: Model = 
-000042b0: 4d6f 6465 6c49 6e66 6f5b 6d6f 6465 6c5d  ModelInfo[model]
-000042c0: 2e76 616c 7565 0d0a 2020 2020 2020 2020  .value..        
-000042d0: 7072 696e 7428 696e 666f 290d 0a20 2020  print(info)..   
-000042e0: 2020 2020 2073 656c 662e 6d6f 6465 6c5f       self.model_
-000042f0: 696e 666f 203d 2069 6e66 6f0d 0a20 2020  info = info..   
-00004300: 2020 2020 2073 656c 662e 6361 7061 6369       self.capaci
-00004310: 7479 203d 2069 6e66 6f2e 6361 7061 6369  ty = info.capaci
-00004320: 7479 0d0a 2020 2020 2020 2020 7365 6c66  ty..        self
-00004330: 2e6c 696d 6974 7320 3d20 2869 6e66 6f2e  .limits = (info.
-00004340: 7469 705f 656a 6563 745f 706f 7369 7469  tip_eject_positi
-00004350: 6f6e 2c20 696e 666f 2e6d 6178 5f70 6f73  on, info.max_pos
-00004360: 6974 696f 6e29 0d0a 2020 2020 2020 2020  ition)..        
-00004370: 7365 6c66 2e73 7065 6564 5f70 7265 7365  self.speed_prese
-00004380: 7473 203d 2069 6e66 6f2e 7072 6573 6574  ts = info.preset
-00004390: 5f73 7065 6564 730d 0a20 2020 2020 2020  _speeds..       
-000043a0: 2073 656c 662e 7370 6565 642e 7570 203d   self.speed.up =
-000043b0: 2073 656c 662e 7370 6565 645f 7072 6573   self.speed_pres
-000043c0: 6574 735b 7365 6c66 2e73 7065 6564 5f63  ets[self.speed_c
-000043d0: 6f64 652e 7570 5d0d 0a20 2020 2020 2020  ode.up]..       
-000043e0: 2073 656c 662e 7370 6565 642e 646f 776e   self.speed.down
-000043f0: 203d 2073 656c 662e 7370 6565 645f 7072   = self.speed_pr
-00004400: 6573 6574 735b 7365 6c66 2e73 7065 6564  esets[self.speed
-00004410: 5f63 6f64 652e 646f 776e 5d0d 0a20 2020  _code.down]..   
-00004420: 2020 2020 2072 6574 7572 6e0d 0a20 2020       return..   
-00004430: 200d 0a20 2020 2064 6566 2067 6574 506f   ..    def getPo
-00004440: 7369 7469 6f6e 2873 656c 662c 202a 2a6b  sition(self, **k
-00004450: 7761 7267 7329 202d 3e20 696e 743a 0d0a  wargs) -> int:..
-00004460: 2020 2020 2020 2020 2222 2247 6574 2074          """Get t
-00004470: 6865 2063 7572 7265 6e74 2070 6f73 6974  he current posit
-00004480: 696f 6e20 6f66 2074 6865 2070 6970 6574  ion of the pipet
-00004490: 7465 2222 220d 0a20 2020 2020 2020 2072  te"""..        r
-000044a0: 6573 706f 6e73 6520 3d20 7365 6c66 2e5f  esponse = self._
-000044b0: 7175 6572 7928 2744 5027 290d 0a20 2020  query('DP')..   
-000044c0: 2020 2020 2074 7279 3a0d 0a20 2020 2020       try:..     
-000044d0: 2020 2020 2020 2070 6f73 6974 696f 6e20         position 
-000044e0: 3d20 696e 7428 7265 7370 6f6e 7365 290d  = int(response).
-000044f0: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
-00004500: 5661 6c75 6545 7272 6f72 3a0d 0a20 2020  ValueError:..   
-00004510: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00004520: 7265 7370 6f6e 7365 0d0a 2020 2020 2020  response..      
-00004530: 2020 7365 6c66 2e70 6f73 6974 696f 6e20    self.position 
-00004540: 3d20 706f 7369 7469 6f6e 0d0a 2020 2020  = position..    
-00004550: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00004560: 706f 7369 7469 6f6e 0d0a 2020 2020 2020  position..      
-00004570: 0d0a 2020 2020 6465 6620 6765 7453 7461  ..    def getSta
-00004580: 7475 7328 7365 6c66 2c20 2a2a 6b77 6172  tus(self, **kwar
-00004590: 6773 2920 2d3e 2073 7472 3a0d 0a20 2020  gs) -> str:..   
-000045a0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-000045b0: 2020 4765 7420 7468 6520 7374 6174 7573    Get the status
-000045c0: 206f 6620 7468 6520 7069 7065 7474 650d   of the pipette.
-000045d0: 0a0d 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-000045e0: 6e73 3a0d 0a20 2020 2020 2020 2020 2020  ns:..           
-000045f0: 2073 7472 3a20 6465 7669 6365 2072 6573   str: device res
-00004600: 706f 6e73 650d 0a20 2020 2020 2020 2022  ponse..        "
-00004610: 2222 0d0a 2020 2020 2020 2020 7265 7370  ""..        resp
-00004620: 6f6e 7365 203d 2073 656c 662e 5f71 7565  onse = self._que
-00004630: 7279 2827 4453 2729 0d0a 2020 2020 2020  ry('DS')..      
-00004640: 2020 7472 793a 0d0a 2020 2020 2020 2020    try:..        
-00004650: 2020 2020 7374 6174 7573 203d 2069 6e74      status = int
-00004660: 2872 6573 706f 6e73 6529 0d0a 2020 2020  (response)..    
-00004670: 2020 2020 6578 6365 7074 2056 616c 7565      except Value
-00004680: 4572 726f 723a 0d0a 2020 2020 2020 2020  Error:..        
-00004690: 2020 2020 7265 7475 726e 2072 6573 706f      return respo
-000046a0: 6e73 650d 0a20 2020 2020 2020 2069 6620  nse..        if 
-000046b0: 7265 7370 6f6e 7365 206e 6f74 2069 6e20  response not in 
-000046c0: 5b5f 7374 6174 7573 2e76 616c 7565 2066  [_status.value f
-000046d0: 6f72 205f 7374 6174 7573 2069 6e20 5374  or _status in St
-000046e0: 6174 7573 436f 6465 5d3a 0d0a 2020 2020  atusCode]:..    
-000046f0: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-00004700: 6573 706f 6e73 650d 0a20 2020 2020 2020  esponse..       
-00004710: 200d 0a20 2020 2020 2020 2073 656c 662e   ..        self.
-00004720: 5f73 7461 7475 735f 636f 6465 203d 2073  _status_code = s
-00004730: 7461 7475 730d 0a20 2020 2020 2020 2069  tatus..        i
-00004740: 6620 7374 6174 7573 2069 6e20 5b34 2c36  f status in [4,6
-00004750: 2c38 5d3a 0d0a 2020 2020 2020 2020 2020  ,8]:..          
-00004760: 2020 7365 6c66 2e73 6574 466c 6167 2862    self.setFlag(b
-00004770: 7573 793d 5472 7565 290d 0a20 2020 2020  usy=True)..     
-00004780: 2020 2020 2020 2069 6620 7365 6c66 2e76         if self.v
-00004790: 6572 626f 7365 3a0d 0a20 2020 2020 2020  erbose:..       
-000047a0: 2020 2020 2020 2020 2070 7269 6e74 2853           print(S
-000047b0: 7461 7475 7343 6f64 6528 7374 6174 7573  tatusCode(status
-000047c0: 292e 6e61 6d65 290d 0a20 2020 2020 2020  ).name)..       
-000047d0: 2065 6c69 6620 7374 6174 7573 203d 3d20   elif status == 
-000047e0: 303a 0d0a 2020 2020 2020 2020 2020 2020  0:..            
-000047f0: 7365 6c66 2e73 6574 466c 6167 2862 7573  self.setFlag(bus
-00004800: 793d 4661 6c73 6529 0d0a 2020 2020 2020  y=False)..      
-00004810: 2020 7265 7475 726e 2053 7461 7475 7343    return StatusC
-00004820: 6f64 6528 7365 6c66 2e5f 7374 6174 7573  ode(self._status
-00004830: 5f63 6f64 6529 2e6e 616d 650d 0a20 2020  _code).name..   
-00004840: 200d 0a20 2020 2064 6566 2068 6f6d 6528   ..    def home(
-00004850: 7365 6c66 2920 2d3e 2073 7472 3a0d 0a20  self) -> str:.. 
-00004860: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-00004870: 2020 2020 5265 7475 726e 2070 6c75 6e67      Return plung
-00004880: 6572 2074 6f20 686f 6d65 2070 6f73 6974  er to home posit
-00004890: 696f 6e0d 0a20 2020 2020 2020 200d 0a20  ion..        .. 
-000048a0: 2020 2020 2020 2052 6574 7572 6e73 3a0d         Returns:.
-000048b0: 0a20 2020 2020 2020 2020 2020 2073 7472  .            str
-000048c0: 3a20 6465 7669 6365 2072 6573 706f 6e73  : device respons
-000048d0: 650d 0a20 2020 2020 2020 2022 2222 0d0a  e..        """..
-000048e0: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
-000048f0: 203d 2073 656c 662e 5f71 7565 7279 2866   = self._query(f
-00004900: 2752 507b 7365 6c66 2e68 6f6d 655f 706f  'RP{self.home_po
-00004910: 7369 7469 6f6e 7d27 290d 0a20 2020 2020  sition}')..     
-00004920: 2020 2073 656c 662e 766f 6c75 6d65 203d     self.volume =
-00004930: 2030 0d0a 2020 2020 2020 2020 7365 6c66   0..        self
-00004940: 2e70 6f73 6974 696f 6e20 3d20 7365 6c66  .position = self
-00004950: 2e68 6f6d 655f 706f 7369 7469 6f6e 0d0a  .home_position..
-00004960: 2020 2020 2020 2020 7469 6d65 2e73 6c65          time.sle
-00004970: 6570 2831 290d 0a20 2020 2020 2020 2072  ep(1)..        r
-00004980: 6574 7572 6e20 7265 7370 6f6e 7365 0d0a  eturn response..
-00004990: 2020 2020 0d0a 2020 2020 6465 6620 6973      ..    def is
-000049a0: 4665 6173 6962 6c65 2873 656c 662c 2070  Feasible(self, p
-000049b0: 6f73 6974 696f 6e3a 696e 7429 202d 3e20  osition:int) -> 
-000049c0: 626f 6f6c 3a0d 0a20 2020 2020 2020 2022  bool:..        "
-000049d0: 2222 0d0a 2020 2020 2020 2020 4368 6563  ""..        Chec
-000049e0: 6b73 2061 6e64 2072 6574 7572 6e73 2077  ks and returns w
-000049f0: 6865 7468 6572 2074 6865 2070 6c75 6e67  hether the plung
-00004a00: 6572 2070 6f73 6974 696f 6e20 6973 2066  er position is f
-00004a10: 6561 7369 626c 650d 0a0d 0a20 2020 2020  easible....     
-00004a20: 2020 2041 7267 733a 0d0a 2020 2020 2020     Args:..      
-00004a30: 2020 2020 2020 706f 7369 7469 6f6e 2028        position (
-00004a40: 696e 7429 3a20 706c 756e 6765 7220 706f  int): plunger po
-00004a50: 7369 7469 6f6e 0d0a 0d0a 2020 2020 2020  sition....      
-00004a60: 2020 5265 7475 726e 733a 0d0a 2020 2020    Returns:..    
-00004a70: 2020 2020 2020 2020 626f 6f6c 3a20 7768          bool: wh
-00004a80: 6574 6865 7220 706c 756e 6765 7220 706f  ether plunger po
-00004a90: 7369 7469 6f6e 2069 7320 6665 6173 6962  sition is feasib
-00004aa0: 6c65 0d0a 2020 2020 2020 2020 2222 220d  le..        """.
-00004ab0: 0a20 2020 2020 2020 2069 6620 2873 656c  .        if (sel
-00004ac0: 662e 6c69 6d69 7473 5b30 5d20 3c3d 2070  f.limits[0] <= p
-00004ad0: 6f73 6974 696f 6e20 3c3d 2073 656c 662e  osition <= self.
-00004ae0: 6c69 6d69 7473 5b31 5d29 3a0d 0a20 2020  limits[1]):..   
-00004af0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00004b00: 5472 7565 0d0a 2020 2020 2020 2020 7072  True..        pr
-00004b10: 696e 7428 6622 5261 6e67 6520 6c69 6d69  int(f"Range limi
-00004b20: 7473 2072 6561 6368 6564 2120 7b73 656c  ts reached! {sel
-00004b30: 662e 6c69 6d69 7473 7d22 290d 0a20 2020  f.limits}")..   
-00004b40: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
-00004b50: 650d 0a20 2020 200d 0a20 2020 2064 6566  e..    ..    def
-00004b60: 2069 7354 6970 4f6e 2873 656c 6629 202d   isTipOn(self) -
-00004b70: 3e20 626f 6f6c 3a0d 0a20 2020 2020 2020  > bool:..       
-00004b80: 2022 2222 0d0a 2020 2020 2020 2020 4368   """..        Ch
-00004b90: 6563 6b73 2061 6e64 2072 6574 7572 6e73  ecks and returns
-00004ba0: 2077 6865 7468 6572 2061 2070 6970 6574   whether a pipet
-00004bb0: 7465 2074 6970 2069 7320 6174 7461 6368  te tip is attach
-00004bc0: 6564 0d0a 2020 2020 2020 2020 0d0a 2020  ed..        ..  
-00004bd0: 2020 2020 2020 5265 7475 726e 733a 0d0a        Returns:..
-00004be0: 2020 2020 2020 2020 2020 2020 626f 6f6c              bool
-00004bf0: 3a20 7768 6574 6865 7220 6120 7069 7065  : whether a pipe
-00004c00: 7474 6520 7469 7020 696e 2061 7474 6163  tte tip in attac
-00004c10: 6865 640d 0a20 2020 2020 2020 2022 2222  hed..        """
-00004c20: 0d0a 2020 2020 2020 2020 7365 6c66 2e67  ..        self.g
-00004c30: 6574 4361 7061 6369 7461 6e63 6528 290d  etCapacitance().
-00004c40: 0a20 2020 2020 2020 2070 7269 6e74 2866  .        print(f
-00004c50: 2754 6970 2063 6170 6163 6974 616e 6365  'Tip capacitance
-00004c60: 3a20 7b73 656c 662e 6361 7061 6369 7461  : {self.capacita
-00004c70: 6e63 657d 2729 0d0a 2020 2020 2020 2020  nce}')..        
-00004c80: 6966 2073 656c 662e 666c 6167 735b 2763  if self.flags['c
-00004c90: 6f6e 6475 6374 6976 655f 7469 7073 275d  onductive_tips']
-00004ca0: 3a0d 0a20 2020 2020 2020 2020 2020 2074  :..            t
-00004cb0: 6970 5f6f 6e20 3d20 2873 656c 662e 6361  ip_on = (self.ca
-00004cc0: 7061 6369 7461 6e63 6520 3e20 7365 6c66  pacitance > self
-00004cd0: 2e74 6970 5f74 6872 6573 686f 6c64 290d  .tip_threshold).
-00004ce0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00004cf0: 662e 7365 7446 6c61 6728 7469 705f 6f6e  f.setFlag(tip_on
-00004d00: 3d74 6970 5f6f 6e29 0d0a 2020 2020 2020  =tip_on)..      
-00004d10: 2020 7469 705f 6f6e 203d 2073 656c 662e    tip_on = self.
-00004d20: 666c 6167 735b 2774 6970 5f6f 6e27 5d0d  flags['tip_on'].
-00004d30: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00004d40: 7469 705f 6f6e 0d0a 2020 2020 0d0a 2020  tip_on..    ..  
-00004d50: 2020 6465 6620 6d6f 7665 2873 656c 662c    def move(self,
-00004d60: 2073 7465 7073 3a69 6e74 2c20 7570 3a62   steps:int, up:b
-00004d70: 6f6f 6c2c 202a 2a6b 7761 7267 7329 202d  ool, **kwargs) -
-00004d80: 3e20 7374 723a 0d0a 2020 2020 2020 2020  > str:..        
-00004d90: 2222 220d 0a20 2020 2020 2020 204d 6f76  """..        Mov
-00004da0: 6520 7468 6520 706c 756e 6765 7220 6569  e the plunger ei
-00004db0: 7468 6572 2075 7020 6f72 2064 6f77 6e20  ther up or down 
-00004dc0: 6279 2061 2073 7065 6369 6669 6564 206e  by a specified n
-00004dd0: 756d 6265 7220 6f66 2073 7465 7073 0d0a  umber of steps..
-00004de0: 0d0a 2020 2020 2020 2020 4172 6773 3a0d  ..        Args:.
-00004df0: 0a20 2020 2020 2020 2020 2020 2073 7465  .            ste
-00004e00: 7073 2028 696e 7429 3a20 6e75 6d62 6572  ps (int): number
-00004e10: 206f 6620 7374 6570 7320 746f 206d 6f76   of steps to mov
-00004e20: 6520 706c 756e 6765 7220 6279 0d0a 2020  e plunger by..  
-00004e30: 2020 2020 2020 2020 2020 7570 2028 626f            up (bo
-00004e40: 6f6c 293a 2077 6865 7468 6572 2074 6f20  ol): whether to 
-00004e50: 6d6f 7665 2074 6865 2070 6c75 6e67 6572  move the plunger
-00004e60: 2075 700d 0a0d 0a20 2020 2020 2020 2052   up....        R
-00004e70: 6574 7572 6e73 3a0d 0a20 2020 2020 2020  eturns:..       
-00004e80: 2020 2020 2073 7472 3a20 6465 7669 6365       str: device
-00004e90: 2072 6573 706f 6e73 650d 0a20 2020 2020   response..     
-00004ea0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-00004eb0: 7374 6570 7320 3d20 6162 7328 7374 6570  steps = abs(step
-00004ec0: 7329 2069 6620 7570 2065 6c73 6520 2d61  s) if up else -a
-00004ed0: 6273 2873 7465 7073 290d 0a20 2020 2020  bs(steps)..     
-00004ee0: 2020 2072 6574 7572 6e20 7365 6c66 2e6d     return self.m
-00004ef0: 6f76 6542 7928 7374 6570 7329 0d0a 2020  oveBy(steps)..  
-00004f00: 2020 0d0a 2020 2020 6465 6620 6d6f 7665    ..    def move
-00004f10: 4279 2873 656c 662c 2073 7465 7073 3a69  By(self, steps:i
-00004f20: 6e74 2c20 2a2a 6b77 6172 6773 2920 2d3e  nt, **kwargs) ->
-00004f30: 2073 7472 3a0d 0a20 2020 2020 2020 2022   str:..        "
-00004f40: 2222 0d0a 2020 2020 2020 2020 4d6f 7665  ""..        Move
-00004f50: 2074 6865 2070 6c75 6e67 6572 2062 7920   the plunger by 
-00004f60: 7370 6563 6966 6965 6420 6e75 6d62 6572  specified number
-00004f70: 206f 6620 7374 6570 730d 0a0d 0a20 2020   of steps....   
-00004f80: 2020 2020 2041 7267 733a 0d0a 2020 2020       Args:..    
-00004f90: 2020 2020 2020 2020 7374 6570 7320 2869          steps (i
-00004fa0: 6e74 293a 206e 756d 6265 7220 6f66 2073  nt): number of s
-00004fb0: 7465 7073 2074 6f20 6d6f 7665 2070 6c75  teps to move plu
-00004fc0: 6e67 6572 2062 7920 283c 303a 206d 6f76  nger by (<0: mov
-00004fd0: 6520 646f 776e 2f64 6973 7065 6e73 653b  e down/dispense;
-00004fe0: 203e 3020 6d6f 7665 2075 702f 6173 7069   >0 move up/aspi
-00004ff0: 7261 7465 290d 0a0d 0a20 2020 2020 2020  rate)....       
-00005000: 2052 6574 7572 6e73 3a0d 0a20 2020 2020   Returns:..     
-00005010: 2020 2020 2020 2073 7472 3a20 6465 7669         str: devi
-00005020: 6365 2072 6573 706f 6e73 650d 0a20 2020  ce response..   
-00005030: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-00005040: 2020 636f 6d6d 616e 6420 3d20 6627 5249    command = f'RI
-00005050: 7b73 7465 7073 7d27 2069 6620 7374 6570  {steps}' if step
-00005060: 7320 3e20 3020 656c 7365 2066 2752 4f7b  s > 0 else f'RO{
-00005070: 2d73 7465 7073 7d27 0d0a 2020 2020 2020  -steps}'..      
-00005080: 2020 7365 6c66 2e70 6f73 6974 696f 6e20    self.position 
-00005090: 2b3d 2073 7465 7073 0d0a 2020 2020 2020  += steps..      
-000050a0: 2020 7265 7475 726e 2073 656c 662e 5f71    return self._q
-000050b0: 7565 7279 2863 6f6d 6d61 6e64 290d 0a20  uery(command).. 
-000050c0: 2020 200d 0a20 2020 2064 6566 206d 6f76     ..    def mov
-000050d0: 6554 6f28 7365 6c66 2c20 706f 7369 7469  eTo(self, positi
-000050e0: 6f6e 3a69 6e74 2c20 2a2a 6b77 6172 6773  on:int, **kwargs
-000050f0: 2920 2d3e 2073 7472 3a0d 0a20 2020 2020  ) -> str:..     
-00005100: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-00005110: 4d6f 7665 2074 6865 2070 6c75 6e67 6572  Move the plunger
-00005120: 2074 6f20 6120 7370 6563 6966 6965 6420   to a specified 
-00005130: 706f 7369 7469 6f6e 0d0a 0d0a 2020 2020  position....    
-00005140: 2020 2020 4172 6773 3a0d 0a20 2020 2020      Args:..     
-00005150: 2020 2020 2020 2070 6f73 6974 696f 6e20         position 
-00005160: 2869 6e74 293a 2074 6172 6765 7420 706c  (int): target pl
-00005170: 756e 6765 7220 706f 7369 7469 6f6e 0d0a  unger position..
-00005180: 0d0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-00005190: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-000051a0: 7374 723a 2064 6576 6963 6520 7265 7370  str: device resp
-000051b0: 6f6e 7365 0d0a 2020 2020 2020 2020 2222  onse..        ""
-000051c0: 220d 0a20 2020 2020 2020 2073 656c 662e  "..        self.
-000051d0: 706f 7369 7469 6f6e 203d 2070 6f73 6974  position = posit
-000051e0: 696f 6e0d 0a20 2020 2020 2020 2072 6574  ion..        ret
-000051f0: 7572 6e20 7365 6c66 2e5f 7175 6572 7928  urn self._query(
-00005200: 6627 5250 7b70 6f73 6974 696f 6e7d 2729  f'RP{position}')
-00005210: 0d0a 2020 2020 0d0a 2020 2020 6465 6620  ..    ..    def 
-00005220: 7075 6c6c 6261 636b 2873 656c 662c 2073  pullback(self, s
-00005230: 7465 7073 3a69 6e74 203d 2035 2c20 2a2a  teps:int = 5, **
-00005240: 6b77 6172 6773 2920 2d3e 2073 7472 3a0d  kwargs) -> str:.
-00005250: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-00005260: 2020 2020 2020 5075 6c6c 6261 636b 206c        Pullback l
-00005270: 6971 7569 6420 6672 6f6d 2074 6970 0d0a  iquid from tip..
-00005280: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00005290: 2020 4172 6773 3a0d 0a20 2020 2020 2020    Args:..       
-000052a0: 2020 2020 2073 7465 7073 2028 696e 742c       steps (int,
-000052b0: 206f 7074 696f 6e61 6c29 3a20 6e75 6d62   optional): numb
-000052c0: 6572 206f 6620 7374 6570 7320 746f 2070  er of steps to p
-000052d0: 756c 6c62 6163 6b2e 2044 6566 6175 6c74  ullback. Default
-000052e0: 7320 746f 2035 2e0d 0a0d 0a20 2020 2020  s to 5.....     
-000052f0: 2020 2052 6574 7572 6e73 3a0d 0a20 2020     Returns:..   
-00005300: 2020 2020 2020 2020 2073 7472 3a20 6465           str: de
-00005310: 7669 6365 2072 6573 706f 6e73 650d 0a20  vice response.. 
-00005320: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-00005330: 2020 2020 7265 7370 6f6e 7365 203d 2073      response = s
-00005340: 656c 662e 5f71 7565 7279 2866 2752 497b  elf._query(f'RI{
-00005350: 7374 6570 737d 2729 0d0a 2020 2020 2020  steps}')..      
-00005360: 2020 7365 6c66 2e70 6f73 6974 696f 6e20    self.position 
-00005370: 2b3d 2073 7465 7073 0d0a 2020 2020 2020  += steps..      
-00005380: 2020 7469 6d65 2e73 6c65 6570 2831 290d    time.sleep(1).
-00005390: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000053a0: 7265 7370 6f6e 7365 0d0a 2020 2020 0d0a  response..    ..
-000053b0: 2020 2020 6465 6620 7265 7365 7428 7365      def reset(se
-000053c0: 6c66 2920 2d3e 2073 7472 3a0d 0a20 2020  lf) -> str:..   
-000053d0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-000053e0: 2020 5265 7365 7420 7468 6520 7069 7065    Reset the pipe
-000053f0: 7474 650d 0a0d 0a20 2020 2020 2020 2052  tte....        R
-00005400: 6574 7572 6e73 3a0d 0a20 2020 2020 2020  eturns:..       
-00005410: 2020 2020 2073 7472 3a20 6465 7669 6365       str: device
-00005420: 2072 6573 706f 6e73 650d 0a20 2020 2020   response..     
-00005430: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-00005440: 7365 6c66 2e7a 6572 6f28 290d 0a20 2020  self.zero()..   
-00005450: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00005460: 2e68 6f6d 6528 290d 0a20 2020 200d 0a20  .home()..    .. 
-00005470: 2020 2064 6566 2073 6574 5370 6565 6428     def setSpeed(
-00005480: 7365 6c66 2c20 7370 6565 643a 696e 742c  self, speed:int,
-00005490: 2075 703a 626f 6f6c 2c20 2a2a 6b77 6172   up:bool, **kwar
-000054a0: 6773 2920 2d3e 2073 7472 3a0d 0a20 2020  gs) -> str:..   
-000054b0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-000054c0: 2020 5365 7420 7468 6520 7370 6565 6420    Set the speed 
-000054d0: 6f66 2074 6865 2070 6c75 6e67 6572 0d0a  of the plunger..
-000054e0: 0d0a 2020 2020 2020 2020 4172 6773 3a0d  ..        Args:.
-000054f0: 0a20 2020 2020 2020 2020 2020 2073 7065  .            spe
-00005500: 6564 2028 696e 7429 3a20 7370 6565 6420  ed (int): speed 
-00005510: 6f66 2070 6c75 6e67 6572 0d0a 2020 2020  of plunger..    
-00005520: 2020 2020 2020 2020 7570 2028 626f 6f6c          up (bool
-00005530: 293a 2064 6972 6563 7469 6f6e 206f 6620  ): direction of 
-00005540: 7472 6176 656c 0d0a 0d0a 2020 2020 2020  travel....      
-00005550: 2020 5265 7475 726e 733a 0d0a 2020 2020    Returns:..    
-00005560: 2020 2020 2020 2020 7374 723a 2064 6576          str: dev
-00005570: 6963 6520 7265 7370 6f6e 7365 0d0a 2020  ice response..  
-00005580: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-00005590: 2020 2073 7065 6564 5f63 6f64 6520 3d20     speed_code = 
-000055a0: 3120 2b20 5b78 2066 6f72 2078 2c76 616c  1 + [x for x,val
-000055b0: 2069 6e20 656e 756d 6572 6174 6528 6e70   in enumerate(np
-000055c0: 2e61 7272 6179 2873 656c 662e 7370 6565  .array(self.spee
-000055d0: 645f 7072 6573 6574 7329 2d73 7065 6564  d_presets)-speed
-000055e0: 2920 6966 2076 616c 203e 3d20 305d 5b30  ) if val >= 0][0
-000055f0: 5d0d 0a20 2020 2020 2020 2070 7269 6e74  ]..        print
-00005600: 2866 2753 7065 6564 207b 7370 6565 645f  (f'Speed {speed_
-00005610: 636f 6465 7d3a 207b 7365 6c66 2e73 7065  code}: {self.spe
-00005620: 6564 5f70 7265 7365 7473 5b73 7065 6564  ed_presets[speed
-00005630: 5f63 6f64 652d 315d 7d20 754c 2f73 2729  _code-1]} uL/s')
-00005640: 0d0a 2020 2020 2020 2020 6469 7265 6374  ..        direct
-00005650: 696f 6e20 3d20 2749 2720 6966 2075 7020  ion = 'I' if up 
-00005660: 656c 7365 2027 4f27 0d0a 2020 2020 2020  else 'O'..      
-00005670: 2020 7365 6c66 2e5f 7175 6572 7928 6627    self._query(f'
-00005680: 537b 6469 7265 6374 696f 6e7d 7b73 7065  S{direction}{spe
-00005690: 6564 5f63 6f64 657d 2729 0d0a 2020 2020  ed_code}')..    
-000056a0: 2020 2020 6966 2075 703a 0d0a 2020 2020      if up:..    
-000056b0: 2020 2020 2020 2020 7365 6c66 2e73 7065          self.spe
-000056c0: 6564 5f63 6f64 652e 7570 203d 2073 7065  ed_code.up = spe
-000056d0: 6564 5f63 6f64 650d 0a20 2020 2020 2020  ed_code..       
-000056e0: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-000056f0: 2020 2020 7365 6c66 2e73 7065 6564 5f63      self.speed_c
-00005700: 6f64 652e 646f 776e 203d 2073 7065 6564  ode.down = speed
-00005710: 5f63 6f64 650d 0a20 2020 2020 2020 2072  _code..        r
-00005720: 6574 7572 6e20 7365 6c66 2e5f 7175 6572  eturn self._quer
-00005730: 7928 6627 447b 6469 7265 6374 696f 6e7d  y(f'D{direction}
-00005740: 2729 0d0a 2020 2020 0d0a 2020 2020 6465  ')..    ..    de
-00005750: 6620 7368 7574 646f 776e 2873 656c 6629  f shutdown(self)
-00005760: 3a0d 0a20 2020 2020 2020 2022 2222 5368  :..        """Sh
-00005770: 7574 646f 776e 2070 726f 6365 6475 7265  utdown procedure
-00005780: 2066 6f72 2074 6f6f 6c22 2222 0d0a 2020   for tool"""..  
-00005790: 2020 2020 2020 7365 6c66 2e74 6f67 676c        self.toggl
-000057a0: 6546 6565 6462 6163 6b4c 6f6f 7028 6f6e  eFeedbackLoop(on
-000057b0: 3d46 616c 7365 290d 0a20 2020 2020 2020  =False)..       
-000057c0: 2072 6574 7572 6e20 7375 7065 7228 292e   return super().
-000057d0: 7368 7574 646f 776e 2829 0d0a 2020 2020  shutdown()..    
-000057e0: 0d0a 2020 2020 6465 6620 746f 6767 6c65  ..    def toggle
-000057f0: 4665 6564 6261 636b 4c6f 6f70 2873 656c  FeedbackLoop(sel
-00005800: 662c 206f 6e3a 626f 6f6c 293a 0d0a 2020  f, on:bool):..  
-00005810: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-00005820: 2020 2053 7461 7274 206f 7220 7374 6f70     Start or stop
-00005830: 2066 6565 6462 6163 6b20 6c6f 6f70 0d0a   feedback loop..
-00005840: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00005850: 2020 4172 6773 3a0d 0a20 2020 2020 2020    Args:..       
-00005860: 2020 2020 206f 6e20 2862 6f6f 6c29 3a20       on (bool): 
-00005870: 7768 6574 6865 7220 746f 2073 7461 7274  whether to start
-00005880: 2066 6565 6462 6163 6b20 6c6f 6f70 0d0a   feedback loop..
-00005890: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
-000058a0: 2020 2020 2073 656c 662e 7365 7446 6c61       self.setFla
-000058b0: 6728 6765 745f 6665 6564 6261 636b 3d6f  g(get_feedback=o
-000058c0: 6e29 0d0a 2020 2020 2020 2020 6966 206f  n)..        if o
-000058d0: 6e3a 0d0a 2020 2020 2020 2020 2020 2020  n:..            
-000058e0: 6966 2027 6665 6564 6261 636b 5f6c 6f6f  if 'feedback_loo
-000058f0: 7027 2069 6e20 7365 6c66 2e5f 7468 7265  p' in self._thre
-00005900: 6164 733a 0d0a 2020 2020 2020 2020 2020  ads:..          
-00005910: 2020 2020 2020 7365 6c66 2e5f 7468 7265        self._thre
-00005920: 6164 735b 2766 6565 6462 6163 6b5f 6c6f  ads['feedback_lo
-00005930: 6f70 275d 2e6a 6f69 6e28 290d 0a20 2020  op'].join()..   
-00005940: 2020 2020 2020 2020 2074 6872 6561 6420           thread 
-00005950: 3d20 5468 7265 6164 2874 6172 6765 743d  = Thread(target=
-00005960: 7365 6c66 2e5f 6c6f 6f70 5f66 6565 6462  self._loop_feedb
-00005970: 6163 6b29 0d0a 2020 2020 2020 2020 2020  ack)..          
-00005980: 2020 7468 7265 6164 2e73 7461 7274 2829    thread.start()
-00005990: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-000059a0: 6c66 2e5f 7468 7265 6164 735b 2766 6565  lf._threads['fee
-000059b0: 6462 6163 6b5f 6c6f 6f70 275d 203d 2074  dback_loop'] = t
-000059c0: 6872 6561 640d 0a20 2020 2020 2020 2065  hread..        e
-000059d0: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-000059e0: 2020 6966 2027 6665 6564 6261 636b 5f6c    if 'feedback_l
-000059f0: 6f6f 7027 2069 6e20 7365 6c66 2e5f 7468  oop' in self._th
-00005a00: 7265 6164 733a 0d0a 2020 2020 2020 2020  reads:..        
-00005a10: 2020 2020 2020 2020 7365 6c66 2e5f 7468          self._th
-00005a20: 7265 6164 735b 2766 6565 6462 6163 6b5f  reads['feedback_
-00005a30: 6c6f 6f70 275d 2e6a 6f69 6e28 290d 0a20  loop'].join().. 
-00005a40: 2020 2020 2020 2072 6574 7572 6e0d 0a0d         return...
-00005a50: 0a20 2020 2064 6566 207a 6572 6f28 7365  .    def zero(se
-00005a60: 6c66 2920 2d3e 2073 7472 3a0d 0a20 2020  lf) -> str:..   
-00005a70: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-00005a80: 2020 5a65 726f 2074 6865 2070 6c75 6e67    Zero the plung
-00005a90: 6572 2070 6f73 6974 696f 6e0d 0a20 2020  er position..   
-00005aa0: 2020 2020 200d 0a20 2020 2020 2020 2052       ..        R
-00005ab0: 6574 7572 6e73 3a0d 0a20 2020 2020 2020  eturns:..       
-00005ac0: 2020 2020 2073 7472 3a20 6465 7669 6365       str: device
-00005ad0: 2072 6573 706f 6e73 650d 0a20 2020 2020   response..     
-00005ae0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-00005af0: 7365 6c66 2e65 6a65 6374 2829 0d0a 2020  self.eject()..  
-00005b00: 2020 2020 2020 7265 7370 6f6e 7365 203d        response =
-00005b10: 2073 656c 662e 5f71 7565 7279 2827 525a   self._query('RZ
-00005b20: 2729 0d0a 2020 2020 2020 2020 7365 6c66  ')..        self
-00005b30: 2e70 6f73 6974 696f 6e20 3d20 300d 0a20  .position = 0.. 
-00005b40: 2020 2020 2020 2074 696d 652e 736c 6565         time.slee
-00005b50: 7028 3229 0d0a 2020 2020 2020 2020 7265  p(2)..        re
-00005b60: 7475 726e 2072 6573 706f 6e73 650d 0a0d  turn response...
-00005b70: 0a20 2020 2023 2050 726f 7465 6374 6564  .    # Protected
-00005b80: 206d 6574 686f 6428 7329 0d0a 2020 2020   method(s)..    
-00005b90: 6465 6620 5f63 616c 6375 6c61 7465 5f73  def _calculate_s
-00005ba0: 7065 6564 5f70 6172 616d 6574 6572 7328  peed_parameters(
-00005bb0: 7365 6c66 2c20 766f 6c75 6d65 3a69 6e74  self, volume:int
-00005bc0: 2c20 7370 6565 643a 696e 7429 202d 3e20  , speed:int) -> 
-00005bd0: 5370 6565 6450 6172 616d 6574 6572 733a  SpeedParameters:
-00005be0: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-00005bf0: 2020 2020 2020 2043 616c 6375 6c61 7465         Calculate
-00005c00: 7320 7468 6520 6265 7374 2070 6172 616d  s the best param
-00005c10: 6574 6572 7320 666f 7220 766f 6c75 6d65  eters for volume
-00005c20: 2061 6e64 2073 7065 6564 0d0a 0d0a 2020   and speed....  
-00005c30: 2020 2020 2020 4172 6773 3a0d 0a20 2020        Args:..   
-00005c40: 2020 2020 2020 2020 2076 6f6c 756d 6520           volume 
-00005c50: 2869 6e74 293a 2076 6f6c 756d 6520 746f  (int): volume to
-00005c60: 2062 6520 7472 616e 7366 6572 7265 640d   be transferred.
-00005c70: 0a20 2020 2020 2020 2020 2020 2073 7065  .            spe
-00005c80: 6564 2028 696e 7429 3a20 7370 6565 6420  ed (int): speed 
-00005c90: 6174 2077 6869 6368 206c 6971 7569 6420  at which liquid 
-00005ca0: 6973 2074 7261 6e73 6665 7272 6564 0d0a  is transferred..
-00005cb0: 0d0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-00005cc0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-00005cd0: 6469 6374 3a20 6469 6374 696f 6e61 7279  dict: dictionary
-00005ce0: 206f 6620 6265 7374 2070 6172 616d 6574   of best paramet
-00005cf0: 6572 730d 0a20 2020 2020 2020 2022 2222  ers..        """
-00005d00: 0d0a 2020 2020 2020 2020 6f75 7463 6f6d  ..        outcom
-00005d10: 6573 203d 207b 7d0d 0a20 2020 2020 2020  es = {}..       
-00005d20: 2073 7465 705f 696e 7465 7276 616c 5f6c   step_interval_l
-00005d30: 696d 6974 203d 2069 6e74 2876 6f6c 756d  imit = int(volum
-00005d40: 652f 7365 6c66 2e72 6573 6f6c 7574 696f  e/self.resolutio
-00005d50: 6e2f 5354 4550 5f52 4553 4f4c 5554 494f  n/STEP_RESOLUTIO
-00005d60: 4e29 0d0a 2020 2020 2020 2020 666f 7220  N)..        for 
-00005d70: 7072 6573 6574 2069 6e20 7365 6c66 2e73  preset in self.s
-00005d80: 7065 6564 5f70 7265 7365 7473 3a0d 0a20  peed_presets:.. 
-00005d90: 2020 2020 2020 2020 2020 2069 6620 7072             if pr
-00005da0: 6573 6574 203c 2073 7065 6564 3a0d 0a20  eset < speed:.. 
-00005db0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00005dc0: 2070 7265 7365 7420 6973 2073 6c6f 7765   preset is slowe
-00005dd0: 7220 7468 616e 2074 6172 6765 7420 7370  r than target sp
-00005de0: 6565 642c 2069 7420 7769 6c6c 206e 6576  eed, it will nev
-00005df0: 6572 2068 6974 2074 6172 6765 7420 7370  er hit target sp
-00005e00: 6565 640d 0a20 2020 2020 2020 2020 2020  eed..           
-00005e10: 2020 2020 2063 6f6e 7469 6e75 650d 0a20       continue.. 
-00005e20: 2020 2020 2020 2020 2020 2074 696d 655f             time_
-00005e30: 696e 7465 7276 616c 5f6c 696d 6974 203d  interval_limit =
-00005e40: 2069 6e74 2876 6f6c 756d 652a 2831 2f73   int(volume*(1/s
-00005e50: 7065 6564 202d 2031 2f70 7265 7365 7429  peed - 1/preset)
-00005e60: 2f73 656c 662e 7265 7370 6f6e 7365 5f74  /self.response_t
-00005e70: 696d 6529 0d0a 2020 2020 2020 2020 2020  ime)..          
-00005e80: 2020 6966 206e 6f74 2073 7465 705f 696e    if not step_in
-00005e90: 7465 7276 616c 5f6c 696d 6974 206f 7220  terval_limit or 
-00005ea0: 6e6f 7420 7469 6d65 5f69 6e74 6572 7661  not time_interva
-00005eb0: 6c5f 6c69 6d69 743a 0d0a 2020 2020 2020  l_limit:..      
-00005ec0: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
-00005ed0: 7565 0d0a 2020 2020 2020 2020 2020 2020  ue..            
-00005ee0: 696e 7465 7276 616c 7320 3d20 6d61 7828  intervals = max(
-00005ef0: 6d69 6e28 7374 6570 5f69 6e74 6572 7661  min(step_interva
-00005f00: 6c5f 6c69 6d69 742c 2074 696d 655f 696e  l_limit, time_in
-00005f10: 7465 7276 616c 5f6c 696d 6974 292c 2031  terval_limit), 1
-00005f20: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
-00005f30: 6163 685f 7374 6570 7320 3d20 766f 6c75  ach_steps = volu
-00005f40: 6d65 2f73 656c 662e 7265 736f 6c75 7469  me/self.resoluti
-00005f50: 6f6e 2f69 6e74 6572 7661 6c73 0d0a 2020  on/intervals..  
-00005f60: 2020 2020 2020 2020 2020 6561 6368 5f64            each_d
-00005f70: 656c 6179 203d 2076 6f6c 756d 652a 2831  elay = volume*(1
-00005f80: 2f73 7065 6564 202d 2031 2f70 7265 7365  /speed - 1/prese
-00005f90: 7429 2f69 6e74 6572 7661 6c73 0d0a 2020  t)/intervals..  
-00005fa0: 2020 2020 2020 2020 2020 6172 6561 203d            area =
-00005fb0: 2030 2e35 202a 2028 766f 6c75 6d65 2a2a   0.5 * (volume**
-00005fc0: 3229 202a 2028 312f 7365 6c66 2e72 6573  2) * (1/self.res
-00005fd0: 6f6c 7574 696f 6e29 202a 2028 312f 696e  olution) * (1/in
-00005fe0: 7465 7276 616c 7329 202a 2028 312f 7370  tervals) * (1/sp
-00005ff0: 6565 6420 2d20 312f 7072 6573 6574 290d  eed - 1/preset).
-00006000: 0a20 2020 2020 2020 2020 2020 206f 7574  .            out
-00006010: 636f 6d65 735b 6172 6561 5d20 3d20 5370  comes[area] = Sp
-00006020: 6565 6450 6172 616d 6574 6572 7328 7072  eedParameters(pr
-00006030: 6573 6574 2c20 696e 7465 7276 616c 732c  eset, intervals,
-00006040: 2069 6e74 2865 6163 685f 7374 6570 7329   int(each_steps)
-00006050: 2c20 6561 6368 5f64 656c 6179 290d 0a20  , each_delay).. 
-00006060: 2020 2020 2020 2069 6620 6c65 6e28 6f75         if len(ou
-00006070: 7463 6f6d 6573 2920 3d3d 2030 3a0d 0a20  tcomes) == 0:.. 
-00006080: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-00006090: 2822 4e6f 2066 6561 7369 626c 6520 7370  ("No feasible sp
-000060a0: 6565 6420 7061 7261 6d65 7465 7273 2e22  eed parameters."
-000060b0: 290d 0a20 2020 2020 2020 2020 2020 2072  )..            r
-000060c0: 6574 7572 6e20 5370 6565 6450 6172 616d  eturn SpeedParam
-000060d0: 6574 6572 7328 4e6f 6e65 2c20 5354 4550  eters(None, STEP
-000060e0: 5f52 4553 4f4c 5554 494f 4e2c 2053 5445  _RESOLUTION, STE
-000060f0: 505f 5245 534f 4c55 5449 4f4e 2c20 7365  P_RESOLUTION, se
-00006100: 6c66 2e72 6573 706f 6e73 655f 7469 6d65  lf.response_time
-00006110: 290d 0a20 2020 2020 2020 2070 7269 6e74  )..        print
-00006120: 2866 2742 6573 7420 7061 7261 6d65 7465  (f'Best paramete
-00006130: 7273 3a20 7b6f 7574 636f 6d65 735b 6d69  rs: {outcomes[mi
-00006140: 6e28 6f75 7463 6f6d 6573 295d 7d27 290d  n(outcomes)]}').
-00006150: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00006160: 6f75 7463 6f6d 6573 5b6d 696e 286f 7574  outcomes[min(out
-00006170: 636f 6d65 7329 5d0d 0a20 2020 200d 0a20  comes)]..    .. 
-00006180: 2020 2064 6566 205f 636f 6e6e 6563 7428     def _connect(
-00006190: 7365 6c66 2c20 706f 7274 3a73 7472 2c20  self, port:str, 
-000061a0: 6261 7564 7261 7465 3a69 6e74 203d 2039  baudrate:int = 9
-000061b0: 3630 302c 2074 696d 656f 7574 3a69 6e74  600, timeout:int
-000061c0: 203d 2031 293a 0d0a 2020 2020 2020 2020   = 1):..        
-000061d0: 2222 220d 0a20 2020 2020 2020 2043 6f6e  """..        Con
-000061e0: 6e65 6374 696f 6e20 7072 6f63 6564 7572  nection procedur
-000061f0: 6520 666f 7220 746f 6f6c 0d0a 0d0a 2020  e for tool....  
-00006200: 2020 2020 2020 4172 6773 3a0d 0a20 2020        Args:..   
-00006210: 2020 2020 2020 2020 2070 6f72 7420 2873           port (s
-00006220: 7472 293a 2043 4f4d 2070 6f72 7420 6164  tr): COM port ad
-00006230: 6472 6573 730d 0a20 2020 2020 2020 2020  dress..         
-00006240: 2020 2062 6175 6472 6174 6520 2869 6e74     baudrate (int
-00006250: 2c20 6f70 7469 6f6e 616c 293a 2062 6175  , optional): bau
-00006260: 6472 6174 652e 2044 6566 6175 6c74 7320  drate. Defaults 
-00006270: 746f 2039 3630 302e 0d0a 2020 2020 2020  to 9600...      
-00006280: 2020 2020 2020 7469 6d65 6f75 7420 2869        timeout (i
-00006290: 6e74 2c20 6f70 7469 6f6e 616c 293a 2074  nt, optional): t
-000062a0: 696d 656f 7574 2069 6e20 7365 636f 6e64  imeout in second
-000062b0: 732e 2044 6566 6175 6c74 7320 746f 2031  s. Defaults to 1
-000062c0: 2e0d 0a20 2020 2020 2020 2022 2222 0d0a  ...        """..
-000062d0: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
-000062e0: 6e65 6374 696f 6e5f 6465 7461 696c 7320  nection_details 
-000062f0: 3d20 7b0d 0a20 2020 2020 2020 2020 2020  = {..           
-00006300: 2027 706f 7274 273a 2070 6f72 742c 0d0a   'port': port,..
-00006310: 2020 2020 2020 2020 2020 2020 2762 6175              'bau
-00006320: 6472 6174 6527 3a20 6261 7564 7261 7465  drate': baudrate
-00006330: 2c0d 0a20 2020 2020 2020 2020 2020 2027  ,..            '
-00006340: 7469 6d65 6f75 7427 3a20 7469 6d65 6f75  timeout': timeou
-00006350: 740d 0a20 2020 2020 2020 207d 0d0a 2020  t..        }..  
-00006360: 2020 2020 2020 6465 7669 6365 203d 204e        device = N
-00006370: 6f6e 650d 0a20 2020 2020 2020 2074 7279  one..        try
-00006380: 3a0d 0a20 2020 2020 2020 2020 2020 2064  :..            d
-00006390: 6576 6963 6520 3d20 7365 7269 616c 2e53  evice = serial.S
-000063a0: 6572 6961 6c28 706f 7274 2c20 6261 7564  erial(port, baud
-000063b0: 7261 7465 2c20 7469 6d65 6f75 743d 7469  rate, timeout=ti
-000063c0: 6d65 6f75 7429 0d0a 2020 2020 2020 2020  meout)..        
-000063d0: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
-000063e0: 2061 7320 653a 0d0a 2020 2020 2020 2020   as e:..        
-000063f0: 2020 2020 7072 696e 7428 6622 436f 756c      print(f"Coul
-00006400: 6420 6e6f 7420 636f 6e6e 6563 7420 746f  d not connect to
-00006410: 207b 706f 7274 7d22 290d 0a20 2020 2020   {port}")..     
-00006420: 2020 2020 2020 2069 6620 7365 6c66 2e76         if self.v
-00006430: 6572 626f 7365 3a0d 0a20 2020 2020 2020  erbose:..       
-00006440: 2020 2020 2020 2020 2070 7269 6e74 2865           print(e
-00006450: 290d 0a20 2020 2020 2020 2065 6c73 653a  )..        else:
-00006460: 0d0a 2020 2020 2020 2020 2020 2020 7469  ..            ti
-00006470: 6d65 2e73 6c65 6570 2832 2920 2020 2320  me.sleep(2)   # 
-00006480: 5761 6974 2066 6f72 2067 7262 6c20 746f  Wait for grbl to
-00006490: 2069 6e69 7469 616c 697a 650d 0a20 2020   initialize..   
-000064a0: 2020 2020 2020 2020 2064 6576 6963 652e           device.
-000064b0: 666c 7573 6849 6e70 7574 2829 0d0a 2020  flushInput()..  
-000064c0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-000064d0: 6622 436f 6e6e 6563 7469 6f6e 206f 7065  f"Connection ope
-000064e0: 6e65 6420 746f 207b 706f 7274 7d22 290d  ned to {port}").
-000064f0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00006500: 662e 7365 7446 6c61 6728 636f 6e6e 6563  f.setFlag(connec
-00006510: 7465 643d 5472 7565 290d 0a20 2020 2020  ted=True)..     
-00006520: 2020 2073 656c 662e 6465 7669 6365 203d     self.device =
-00006530: 2064 6576 6963 650d 0a20 2020 2020 2020   device..       
-00006540: 2073 656c 662e 6765 7449 6e66 6f28 290d   self.getInfo().
-00006550: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
-00006560: 7365 7428 290d 0a20 2020 2020 2020 2072  set()..        r
-00006570: 6574 7572 6e0d 0a20 2020 200d 0a20 2020  eturn..    ..   
-00006580: 2064 6566 205f 6973 5f65 7870 6563 7465   def _is_expecte
-00006590: 645f 7265 706c 7928 7365 6c66 2c20 7265  d_reply(self, re
-000065a0: 7370 6f6e 7365 3a73 7472 2c20 636f 6d6d  sponse:str, comm
-000065b0: 616e 645f 636f 6465 3a73 7472 2c20 2a2a  and_code:str, **
-000065c0: 6b77 6172 6773 2920 2d3e 2062 6f6f 6c3a  kwargs) -> bool:
-000065d0: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-000065e0: 2020 2020 2020 2043 6865 636b 7320 616e         Checks an
-000065f0: 6420 7265 7475 726e 7320 7768 6574 6865  d returns whethe
-00006600: 7220 7468 6520 7265 7370 6f6e 7365 2069  r the response i
-00006610: 7320 616e 2065 7870 6563 7465 6420 7265  s an expected re
-00006620: 706c 790d 0a0d 0a20 2020 2020 2020 2041  ply....        A
-00006630: 7267 733a 0d0a 2020 2020 2020 2020 2020  rgs:..          
-00006640: 2020 7265 7370 6f6e 7365 2028 7374 7229    response (str)
-00006650: 3a20 7265 7370 6f6e 7365 2073 7472 696e  : response strin
-00006660: 6720 6672 6f6d 2064 6576 6963 650d 0a20  g from device.. 
-00006670: 2020 2020 2020 2020 2020 2063 6f6d 6d61             comma
-00006680: 6e64 5f63 6f64 6520 2873 7472 293a 2074  nd_code (str): t
-00006690: 776f 2d63 6861 7261 6374 6572 2063 6f6d  wo-character com
-000066a0: 6d61 6e64 2063 6f64 650d 0a0d 0a20 2020  mand code....   
-000066b0: 2020 2020 2052 6574 7572 6e73 3a0d 0a20       Returns:.. 
-000066c0: 2020 2020 2020 2020 2020 2062 6f6f 6c3a             bool:
-000066d0: 2077 6865 7468 6572 2074 6865 2072 6573   whether the res
-000066e0: 706f 6e73 6520 6973 2061 6e20 6578 7065  ponse is an expe
-000066f0: 6374 6564 2072 6570 6c79 0d0a 2020 2020  cted reply..    
-00006700: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-00006710: 2069 6620 7265 7370 6f6e 7365 2069 6e20   if response in 
-00006720: 4572 726f 7243 6f64 652e 5f6d 656d 6265  ErrorCode._membe
-00006730: 725f 6e61 6d65 735f 3a0d 0a20 2020 2020  r_names_:..     
-00006740: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
-00006750: 7565 0d0a 2020 2020 2020 2020 6966 2063  ue..        if c
-00006760: 6f6d 6d61 6e64 5f63 6f64 6520 6e6f 7420  ommand_code not 
-00006770: 696e 2051 5545 5249 4553 2061 6e64 2072  in QUERIES and r
-00006780: 6573 706f 6e73 6520 3d3d 2027 6f6b 273a  esponse == 'ok':
-00006790: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-000067a0: 7475 726e 2054 7275 650d 0a20 2020 2020  turn True..     
-000067b0: 2020 2069 6620 636f 6d6d 616e 645f 636f     if command_co
-000067c0: 6465 2069 6e20 5155 4552 4945 5320 616e  de in QUERIES an
-000067d0: 6420 7265 7370 6f6e 7365 5b3a 325d 203d  d response[:2] =
-000067e0: 3d20 636f 6d6d 616e 645f 636f 6465 2e6c  = command_code.l
-000067f0: 6f77 6572 2829 3a0d 0a20 2020 2020 2020  ower():..       
-00006800: 2020 2020 2072 6570 6c79 5f63 6f64 652c       reply_code,
-00006810: 2064 6174 6120 3d20 7265 7370 6f6e 7365   data = response
-00006820: 5b3a 325d 2c20 7265 7370 6f6e 7365 5b32  [:2], response[2
-00006830: 3a5d 0d0a 2020 2020 2020 2020 2020 2020  :]..            
-00006840: 6966 2073 656c 662e 7665 7262 6f73 653a  if self.verbose:
-00006850: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006860: 2020 7072 696e 7428 6627 5b7b 7265 706c    print(f'[{repl
-00006870: 795f 636f 6465 7d5d 207b 6461 7461 7d27  y_code}] {data}'
-00006880: 290d 0a20 2020 2020 2020 2020 2020 2072  )..            r
-00006890: 6574 7572 6e20 5472 7565 0d0a 2020 2020  eturn True..    
-000068a0: 2020 2020 7265 7475 726e 2046 616c 7365      return False
-000068b0: 0d0a 0d0a 2020 2020 6465 6620 5f6c 6f6f  ....    def _loo
-000068c0: 705f 6665 6564 6261 636b 2873 656c 6629  p_feedback(self)
-000068d0: 3a0d 0a20 2020 2020 2020 2022 2222 4c6f  :..        """Lo
-000068e0: 6f70 2074 6f20 636f 6e73 7461 6e74 6c79  op to constantly
-000068f0: 2072 6561 6420 6672 6f6d 2064 6576 6963   read from devic
-00006900: 6522 2222 0d0a 2020 2020 2020 2020 7072  e"""..        pr
-00006910: 696e 7428 274c 6973 7465 6e69 6e67 2e2e  int('Listening..
-00006920: 2e27 290d 0a20 2020 2020 2020 2077 6869  .')..        whi
-00006930: 6c65 2073 656c 662e 666c 6167 735b 2767  le self.flags['g
-00006940: 6574 5f66 6565 6462 6163 6b27 5d3a 0d0a  et_feedback']:..
-00006950: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00006960: 656c 662e 666c 6167 735b 2770 6175 7365  elf.flags['pause
-00006970: 5f66 6565 6462 6163 6b27 5d3a 0d0a 2020  _feedback']:..  
-00006980: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00006990: 6e74 696e 7565 0d0a 2020 2020 2020 2020  ntinue..        
-000069a0: 2020 2020 7365 6c66 2e67 6574 5374 6174      self.getStat
-000069b0: 7573 2829 0d0a 2020 2020 2020 2020 2020  us()..          
-000069c0: 2020 7365 6c66 2e67 6574 4361 7061 6369    self.getCapaci
-000069d0: 7461 6e63 6528 290d 0a20 2020 2020 2020  tance()..       
-000069e0: 2070 7269 6e74 2827 5374 6f70 206c 6973   print('Stop lis
-000069f0: 7465 6e69 6e67 2e2e 2e27 290d 0a20 2020  tening...')..   
-00006a00: 2020 2020 2072 6574 7572 6e0d 0a20 2020       return..   
-00006a10: 200d 0a20 2020 2064 6566 205f 7175 6572   ..    def _quer
-00006a20: 7928 7365 6c66 2c20 0d0a 2020 2020 2020  y(self, ..      
-00006a30: 2020 636f 6d6d 616e 643a 2073 7472 2c20    command: str, 
-00006a40: 0d0a 2020 2020 2020 2020 7469 6d65 6f75  ..        timeou
-00006a50: 745f 733a 2066 6c6f 6174 203d 2030 2e33  t_s: float = 0.3
-00006a60: 2c20 0d0a 2020 2020 2020 2020 7265 7375  , ..        resu
-00006a70: 6d65 5f66 6565 6462 6163 6b3a 2062 6f6f  me_feedback: boo
-00006a80: 6c20 3d20 4661 6c73 650d 0a20 2020 2029  l = False..    )
-00006a90: 202d 3e20 7374 723a 0d0a 2020 2020 2020   -> str:..      
-00006aa0: 2020 2222 220d 0a20 2020 2020 2020 2057    """..        W
-00006ab0: 7269 7465 2063 6f6d 6d61 6e64 2074 6f20  rite command to 
-00006ac0: 616e 6420 7265 6164 2072 6573 706f 6e73  and read respons
-00006ad0: 6520 6672 6f6d 2064 6576 6963 650d 0a0d  e from device...
-00006ae0: 0a20 2020 2020 2020 2041 7267 733a 0d0a  .        Args:..
-00006af0: 2020 2020 2020 2020 2020 2020 636f 6d6d              comm
-00006b00: 616e 6420 2873 7472 293a 2063 6f6d 6d61  and (str): comma
-00006b10: 6e64 2073 7472 696e 670d 0a20 2020 2020  nd string..     
-00006b20: 2020 2020 2020 2074 696d 656f 7574 5f73         timeout_s
-00006b30: 2028 666c 6f61 742c 206f 7074 696f 6e61   (float, optiona
-00006b40: 6c29 3a20 6475 7261 7469 6f6e 2074 6f20  l): duration to 
-00006b50: 7761 6974 2062 6566 6f72 6520 7469 6d65  wait before time
-00006b60: 6f75 742e 2044 6566 6175 6c74 7320 746f  out. Defaults to
-00006b70: 2030 2e33 2e0d 0a20 2020 2020 2020 2020   0.3...         
-00006b80: 2020 2072 6573 756d 655f 6665 6564 6261     resume_feedba
-00006b90: 636b 2028 626f 6f6c 2c20 6f70 7469 6f6e  ck (bool, option
-00006ba0: 616c 293a 2077 6865 7468 6572 2074 6f20  al): whether to 
-00006bb0: 7265 7375 6d65 2072 6561 6469 6e67 2066  resume reading f
-00006bc0: 726f 6d20 6465 7669 6365 2e20 4465 6661  rom device. Defa
-00006bd0: 756c 7473 2074 6f20 4661 6c73 652e 0d0a  ults to False...
-00006be0: 0d0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-00006bf0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-00006c00: 7374 723a 2072 6573 706f 6e73 6520 7374  str: response st
-00006c10: 7269 6e67 0d0a 2020 2020 2020 2020 2222  ring..        ""
-00006c20: 220d 0a20 2020 2020 2020 2063 6f6d 6d61  "..        comma
-00006c30: 6e64 5f63 6f64 6520 3d20 636f 6d6d 616e  nd_code = comman
-00006c40: 645b 3a32 5d0d 0a20 2020 2020 2020 2069  d[:2]..        i
-00006c50: 6620 636f 6d6d 616e 645f 636f 6465 206e  f command_code n
-00006c60: 6f74 2069 6e20 5354 4154 5553 5f51 5545  ot in STATUS_QUE
-00006c70: 5249 4553 3a0d 0a20 2020 2020 2020 2020  RIES:..         
-00006c80: 2020 2069 6620 7365 6c66 2e66 6c61 6773     if self.flags
-00006c90: 5b27 6765 745f 6665 6564 6261 636b 275d  ['get_feedback']
-00006ca0: 2061 6e64 206e 6f74 2073 656c 662e 666c   and not self.fl
-00006cb0: 6167 735b 2770 6175 7365 5f66 6565 6462  ags['pause_feedb
-00006cc0: 6163 6b27 5d3a 0d0a 2020 2020 2020 2020  ack']:..        
-00006cd0: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-00006ce0: 466c 6167 2870 6175 7365 5f66 6565 6462  Flag(pause_feedb
-00006cf0: 6163 6b3d 5472 7565 290d 0a20 2020 2020  ack=True)..     
-00006d00: 2020 2020 2020 2020 2020 2074 696d 652e             time.
-00006d10: 736c 6565 7028 7469 6d65 6f75 745f 7329  sleep(timeout_s)
-00006d20: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-00006d30: 6c66 2e67 6574 5374 6174 7573 2829 0d0a  lf.getStatus()..
-00006d40: 2020 2020 2020 2020 2020 2020 7768 696c              whil
-00006d50: 6520 7365 6c66 2e69 7342 7573 7928 293a  e self.isBusy():
-00006d60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006d70: 2020 7365 6c66 2e67 6574 5374 6174 7573    self.getStatus
-00006d80: 2829 0d0a 2020 2020 2020 2020 0d0a 2020  ()..        ..  
-00006d90: 2020 2020 2020 7374 6172 745f 7469 6d65        start_time
-00006da0: 203d 2074 696d 652e 7469 6d65 2829 0d0a   = time.time()..
-00006db0: 2020 2020 2020 2020 7365 6c66 2e5f 7772          self._wr
-00006dc0: 6974 6528 636f 6d6d 616e 6429 0d0a 2020  ite(command)..  
-00006dd0: 2020 2020 2020 7265 7370 6f6e 7365 203d        response =
-00006de0: 2027 270d 0a20 2020 2020 2020 2077 6869   ''..        whi
-00006df0: 6c65 206e 6f74 2073 656c 662e 5f69 735f  le not self._is_
-00006e00: 6578 7065 6374 6564 5f72 6570 6c79 2872  expected_reply(r
-00006e10: 6573 706f 6e73 652c 2063 6f6d 6d61 6e64  esponse, command
-00006e20: 5f63 6f64 6529 3a0d 0a20 2020 2020 2020  _code):..       
-00006e30: 2020 2020 2069 6620 7469 6d65 2e74 696d       if time.tim
-00006e40: 6528 2920 2d20 7374 6172 745f 7469 6d65  e() - start_time
-00006e50: 203e 2074 696d 656f 7574 5f73 3a0d 0a20   > timeout_s:.. 
-00006e60: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-00006e70: 7265 616b 0d0a 2020 2020 2020 2020 2020  reak..          
-00006e80: 2020 7265 7370 6f6e 7365 203d 2073 656c    response = sel
-00006e90: 662e 5f72 6561 6428 290d 0a20 2020 2020  f._read()..     
-00006ea0: 2020 2023 2070 7269 6e74 2874 696d 652e     # print(time.
-00006eb0: 7469 6d65 2829 202d 2073 7461 7274 5f74  time() - start_t
-00006ec0: 696d 6529 0d0a 2020 2020 2020 2020 6966  ime)..        if
-00006ed0: 2063 6f6d 6d61 6e64 5f63 6f64 6520 696e   command_code in
-00006ee0: 2051 5545 5249 4553 3a0d 0a20 2020 2020   QUERIES:..     
-00006ef0: 2020 2020 2020 2072 6573 706f 6e73 6520         response 
-00006f00: 3d20 7265 7370 6f6e 7365 5b32 3a5d 0d0a  = response[2:]..
-00006f10: 2020 2020 2020 2020 6966 2063 6f6d 6d61          if comma
-00006f20: 6e64 5f63 6f64 6520 6e6f 7420 696e 2053  nd_code not in S
-00006f30: 5441 5455 535f 5155 4552 4945 533a 0d0a  TATUS_QUERIES:..
-00006f40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00006f50: 2e67 6574 506f 7369 7469 6f6e 2829 0d0a  .getPosition()..
-00006f60: 2020 2020 2020 2020 2020 2020 6966 2072              if r
-00006f70: 6573 756d 655f 6665 6564 6261 636b 3a0d  esume_feedback:.
-00006f80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006f90: 2073 656c 662e 7365 7446 6c61 6728 7061   self.setFlag(pa
-00006fa0: 7573 655f 6665 6564 6261 636b 3d46 616c  use_feedback=Fal
-00006fb0: 7365 290d 0a20 2020 2020 2020 2072 6574  se)..        ret
-00006fc0: 7572 6e20 7265 7370 6f6e 7365 0d0a 0d0a  urn response....
-00006fd0: 2020 2020 6465 6620 5f72 6561 6428 7365      def _read(se
-00006fe0: 6c66 2920 2d3e 2073 7472 3a0d 0a20 2020  lf) -> str:..   
-00006ff0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-00007000: 2020 5265 6164 2072 6573 706f 6e73 6520    Read response 
-00007010: 6672 6f6d 2064 6576 6963 650d 0a0d 0a20  from device.... 
-00007020: 2020 2020 2020 2052 6574 7572 6e73 3a0d         Returns:.
-00007030: 0a20 2020 2020 2020 2020 2020 2073 7472  .            str
-00007040: 3a20 7265 7370 6f6e 7365 2073 7472 696e  : response strin
-00007050: 670d 0a20 2020 2020 2020 2022 2222 0d0a  g..        """..
-00007060: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
-00007070: 203d 2027 270d 0a20 2020 2020 2020 2074   = ''..        t
-00007080: 7279 3a0d 0a20 2020 2020 2020 2020 2020  ry:..           
-00007090: 2072 6573 706f 6e73 6520 3d20 7365 6c66   response = self
-000070a0: 2e64 6576 6963 652e 7265 6164 6c69 6e65  .device.readline
-000070b0: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-000070c0: 6966 206c 656e 2872 6573 706f 6e73 6529  if len(response)
-000070d0: 203d 3d20 303a 0d0a 2020 2020 2020 2020   == 0:..        
-000070e0: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
-000070f0: 203d 2073 656c 662e 6465 7669 6365 2e72   = self.device.r
-00007100: 6561 646c 696e 6528 290d 0a20 2020 2020  eadline()..     
-00007110: 2020 2020 2020 2072 6573 706f 6e73 6520         response 
-00007120: 3d20 7265 7370 6f6e 7365 5b32 3a2d 325d  = response[2:-2]
-00007130: 2e64 6563 6f64 6528 2775 7466 2d38 2729  .decode('utf-8')
-00007140: 0d0a 2020 2020 2020 2020 6578 6365 7074  ..        except
-00007150: 2041 7474 7269 6275 7465 4572 726f 723a   AttributeError:
-00007160: 0d0a 2020 2020 2020 2020 2020 2020 7061  ..            pa
-00007170: 7373 0d0a 2020 2020 2020 2020 6578 6365  ss..        exce
-00007180: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
-00007190: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-000071a0: 6966 2073 656c 662e 7665 7262 6f73 653a  if self.verbose:
-000071b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000071c0: 2020 7072 696e 7428 6529 0d0a 2020 2020    print(e)..    
-000071d0: 2020 2020 6966 2072 6573 706f 6e73 6520      if response 
-000071e0: 696e 2045 7272 6f72 436f 6465 2e5f 6d65  in ErrorCode._me
-000071f0: 6d62 6572 5f6e 616d 6573 5f3a 0d0a 2020  mber_names_:..  
-00007200: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-00007210: 4572 726f 7243 6f64 655b 7265 7370 6f6e  ErrorCode[respon
-00007220: 7365 5d2e 7661 6c75 6529 0d0a 2020 2020  se].value)..    
-00007230: 2020 2020 7265 7475 726e 2072 6573 706f      return respo
-00007240: 6e73 650d 0a20 2020 200d 0a20 2020 2064  nse..    ..    d
-00007250: 6566 205f 7365 745f 6368 616e 6e65 6c5f  ef _set_channel_
-00007260: 6964 2873 656c 662c 206e 6577 5f63 6861  id(self, new_cha
-00007270: 6e6e 656c 5f69 643a 696e 7429 3a0d 0a20  nnel_id:int):.. 
-00007280: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-00007290: 2020 2020 5365 7420 6368 616e 6e65 6c20      Set channel 
-000072a0: 6964 206f 6620 6465 7669 6365 0d0a 0d0a  id of device....
-000072b0: 2020 2020 2020 2020 4172 6773 3a0d 0a20          Args:.. 
-000072c0: 2020 2020 2020 2020 2020 206e 6577 5f63             new_c
-000072d0: 6861 6e6e 656c 2028 696e 7429 3a20 6e65  hannel (int): ne
-000072e0: 7720 6368 616e 6e65 6c20 6964 0d0a 0d0a  w channel id....
-000072f0: 2020 2020 2020 2020 5261 6973 6573 3a0d          Raises:.
-00007300: 0a20 2020 2020 2020 2020 2020 2056 616c  .            Val
-00007310: 7565 4572 726f 723a 2050 6c65 6173 6520  ueError: Please 
-00007320: 7365 6c65 6374 2061 2076 616c 6964 2072  select a valid r
-00007330: 4c69 6e65 2061 6464 7265 7373 2066 726f  Line address fro
-00007340: 6d20 3120 746f 2039 0d0a 2020 2020 2020  m 1 to 9..      
-00007350: 2020 2222 220d 0a20 2020 2020 2020 2069    """..        i
-00007360: 6620 6e6f 7420 2830 203c 206e 6577 5f63  f not (0 < new_c
-00007370: 6861 6e6e 656c 5f69 6420 3c20 3130 293a  hannel_id < 10):
-00007380: 0d0a 2020 2020 2020 2020 2020 2020 7261  ..            ra
-00007390: 6973 6520 5661 6c75 6545 7272 6f72 2827  ise ValueError('
-000073a0: 506c 6561 7365 2073 656c 6563 7420 6120  Please select a 
-000073b0: 7661 6c69 6420 724c 696e 6520 6164 6472  valid rLine addr
-000073c0: 6573 7320 6672 6f6d 2031 2074 6f20 392e  ess from 1 to 9.
-000073d0: 2729 0d0a 2020 2020 2020 2020 7265 7370  ')..        resp
-000073e0: 6f6e 7365 203d 2073 656c 662e 5f71 7565  onse = self._que
-000073f0: 7279 2866 272a 417b 6e65 775f 6368 616e  ry(f'*A{new_chan
-00007400: 6e65 6c5f 6964 7d27 290d 0a20 2020 2020  nel_id}')..     
-00007410: 2020 2069 6620 7265 7370 6f6e 7365 203d     if response =
-00007420: 3d20 276f 6b27 3a0d 0a20 2020 2020 2020  = 'ok':..       
-00007430: 2020 2020 2073 656c 662e 6368 616e 6e65       self.channe
-00007440: 6c20 3d20 6e65 775f 6368 616e 6e65 6c5f  l = new_channel_
-00007450: 6964 0d0a 2020 2020 2020 2020 7265 7475  id..        retu
-00007460: 726e 0d0a 2020 2020 0d0a 2020 2020 6465  rn..    ..    de
-00007470: 6620 5f77 7269 7465 2873 656c 662c 2063  f _write(self, c
-00007480: 6f6d 6d61 6e64 3a73 7472 2920 2d3e 2062  ommand:str) -> b
-00007490: 6f6f 6c3a 0d0a 2020 2020 2020 2020 2222  ool:..        ""
-000074a0: 220d 0a20 2020 2020 2020 2057 7269 7465  "..        Write
-000074b0: 2063 6f6d 6d61 6e64 2074 6f20 6465 7669   command to devi
-000074c0: 6365 0d0a 0d0a 2020 2020 2020 2020 4172  ce....        Ar
-000074d0: 6773 3a0d 0a20 2020 2020 2020 2020 2020  gs:..           
-000074e0: 2063 6f6d 6d61 6e64 2028 7374 7229 3a20   command (str): 
-000074f0: 3c63 6f6d 6d61 6e64 2063 6f64 653e 3c76  <command code><v
-00007500: 616c 7565 3e0d 0a0d 0a20 2020 2020 2020  alue>....       
-00007510: 2052 6574 7572 6e73 3a0d 0a20 2020 2020   Returns:..     
-00007520: 2020 2020 2020 2062 6f6f 6c3a 2077 6865         bool: whe
-00007530: 7468 6572 2063 6f6d 6d61 6e64 2077 6173  ther command was
-00007540: 2073 656e 7420 7375 6363 6573 7366 756c   sent successful
-00007550: 6c79 0d0a 2020 2020 2020 2020 2222 220d  ly..        """.
-00007560: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00007570: 2e76 6572 626f 7365 3a0d 0a20 2020 2020  .verbose:..     
-00007580: 2020 2020 2020 2070 7269 6e74 2863 6f6d         print(com
-00007590: 6d61 6e64 290d 0a20 2020 2020 2020 2066  mand)..        f
-000075a0: 7374 7269 6e67 203d 2066 2701 7b73 656c  string = f'.{sel
-000075b0: 662e 6368 616e 6e65 6c7d 7b63 6f6d 6d61  f.channel}{comma
-000075c0: 6e64 7dc2 ba5c 7227 2023 2063 6f6d 6d61  nd}..\r' # comma
-000075d0: 6e64 2074 656d 706c 6174 653a 203c 5052  nd template: <PR
-000075e0: 453e 3c41 4452 3e3c 434f 4445 3e3c 4441  E><ADR><CODE><DA
-000075f0: 5441 3e3c 4c52 433e 3c50 4f53 543e 0d0a  TA><LRC><POST>..
-00007600: 2020 2020 2020 2020 2320 6273 7472 696e          # bstrin
-00007610: 6720 3d20 6279 7465 6172 7261 792e 6672  g = bytearray.fr
-00007620: 6f6d 6865 7828 6673 7472 696e 672e 656e  omhex(fstring.en
-00007630: 636f 6465 2827 7574 662d 3827 292e 6865  code('utf-8').he
-00007640: 7828 2929 0d0a 2020 2020 2020 2020 7472  x())..        tr
-00007650: 793a 0d0a 2020 2020 2020 2020 2020 2020  y:..            
-00007660: 2320 5479 7069 6361 6c20 7469 6d65 6f75  # Typical timeou
-00007670: 7420 7761 6974 2069 7320 3430 306d 730d  t wait is 400ms.
-00007680: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00007690: 662e 6465 7669 6365 2e77 7269 7465 2866  f.device.write(f
-000076a0: 7374 7269 6e67 2e65 6e63 6f64 6528 2775  string.encode('u
-000076b0: 7466 2d38 2729 290d 0a20 2020 2020 2020  tf-8'))..       
-000076c0: 2065 7863 6570 7420 4174 7472 6962 7574   except Attribut
-000076d0: 6545 7272 6f72 3a0d 0a20 2020 2020 2020  eError:..       
-000076e0: 2020 2020 2070 6173 730d 0a20 2020 2020       pass..     
-000076f0: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
-00007700: 696f 6e20 6173 2065 3a0d 0a20 2020 2020  ion as e:..     
-00007710: 2020 2020 2020 2069 6620 7365 6c66 2e76         if self.v
-00007720: 6572 626f 7365 3a0d 0a20 2020 2020 2020  erbose:..       
-00007730: 2020 2020 2020 2020 2070 7269 6e74 2865           print(e
-00007740: 290d 0a20 2020 2020 2020 2020 2020 2072  )..            r
-00007750: 6574 7572 6e20 4661 6c73 650d 0a20 2020  eturn False..   
-00007760: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
-00007770: 0d0a 2020 2020                           ..    
+00000f40: 302c 2d32 3530 290d 0a20 2020 2074 6970  0,-250)..    tip
+00000f50: 5f69 6e73 6574 5f6d 6d20 3d20 3132 0d0a  _inset_mm = 12..
+00000f60: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+00000f70: 2873 656c 662c 200d 0a20 2020 2020 2020  (self, ..       
+00000f80: 2070 6f72 743a 7374 722c 200d 0a20 2020   port:str, ..   
+00000f90: 2020 2020 2063 6861 6e6e 656c 3a20 696e       channel: in
+00000fa0: 7420 3d20 312c 200d 0a20 2020 2020 2020  t = 1, ..       
+00000fb0: 206f 6666 7365 743a 2074 7570 6c65 5b66   offset: tuple[f
+00000fc0: 6c6f 6174 5d20 3d20 2830 2c30 2c30 292c  loat] = (0,0,0),
+00000fd0: 0d0a 2020 2020 2020 2020 7265 7370 6f6e  ..        respon
+00000fe0: 7365 5f74 696d 653a 2066 6c6f 6174 203d  se_time: float =
+00000ff0: 2031 2e30 332c 0d0a 2020 2020 2020 2020   1.03,..        
+00001000: 7469 705f 7468 7265 7368 6f6c 643a 2069  tip_threshold: i
+00001010: 6e74 203d 2032 3736 2c0d 0a20 2020 2020  nt = 276,..     
+00001020: 2020 202a 2a6b 7761 7267 730d 0a20 2020     **kwargs..   
+00001030: 2029 3a0d 0a20 2020 2020 2020 2022 2222   ):..        """
+00001040: 0d0a 2020 2020 2020 2020 496e 7374 616e  ..        Instan
+00001050: 7469 6174 6520 7468 6520 636c 6173 730d  tiate the class.
+00001060: 0a0d 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
+00001070: 0d0a 2020 2020 2020 2020 2020 2020 706f  ..            po
+00001080: 7274 2028 7374 7229 3a20 434f 4d20 706f  rt (str): COM po
+00001090: 7274 2061 6464 7265 7373 0d0a 2020 2020  rt address..    
+000010a0: 2020 2020 2020 2020 6368 616e 6e65 6c20          channel 
+000010b0: 2869 6e74 2c20 6f70 7469 6f6e 616c 293a  (int, optional):
+000010c0: 2063 6861 6e6e 656c 2069 642e 2044 6566   channel id. Def
+000010d0: 6175 6c74 7320 746f 2031 2e0d 0a20 2020  aults to 1...   
+000010e0: 2020 2020 2020 2020 206f 6666 7365 7420           offset 
+000010f0: 2874 7570 6c65 5b66 6c6f 6174 5d2c 206f  (tuple[float], o
+00001100: 7074 696f 6e61 6c29 3a20 782c 792c 7a20  ptional): x,y,z 
+00001110: 6f66 6673 6574 206f 6620 7469 702e 2044  offset of tip. D
+00001120: 6566 6175 6c74 7320 746f 2028 302c 302c  efaults to (0,0,
+00001130: 3029 2e0d 0a20 2020 2020 2020 2020 2020  0)...           
+00001140: 2072 6573 706f 6e73 655f 7469 6d65 2028   response_time (
+00001150: 666c 6f61 742c 206f 7074 696f 6e61 6c29  float, optional)
+00001160: 3a20 6465 6c61 7920 6265 7477 6565 6e20  : delay between 
+00001170: 7365 6e64 696e 6720 6120 636f 6d6d 616e  sending a comman
+00001180: 6420 616e 6420 7265 6365 6976 696e 6720  d and receiving 
+00001190: 6120 7265 7370 6f6e 7365 2c20 696e 2073  a response, in s
+000011a0: 6563 6f6e 6473 2e20 4465 6661 756c 7473  econds. Defaults
+000011b0: 2074 6f20 312e 3033 2e0d 0a20 2020 2020   to 1.03...     
+000011c0: 2020 2020 2020 2074 6970 5f74 6872 6573         tip_thres
+000011d0: 686f 6c64 2028 696e 742c 206f 7074 696f  hold (int, optio
+000011e0: 6e61 6c29 3a20 7468 7265 7368 6f6c 6420  nal): threshold 
+000011f0: 6162 6f76 6520 7768 6963 6820 6120 636f  above which a co
+00001200: 6e64 7563 7469 7665 2070 6970 6574 7465  nductive pipette
+00001210: 2074 6970 2069 7320 636f 6e73 6964 6572   tip is consider
+00001220: 6564 2074 6f20 6265 2061 7474 6163 6865  ed to be attache
+00001230: 642e 2044 6566 6175 6c74 7320 746f 2032  d. Defaults to 2
+00001240: 3736 2e0d 0a20 2020 2020 2020 2022 2222  76...        """
+00001250: 0d0a 2020 2020 2020 2020 7375 7065 7228  ..        super(
+00001260: 292e 5f5f 696e 6974 5f5f 282a 2a6b 7761  ).__init__(**kwa
+00001270: 7267 7329 0d0a 2020 2020 2020 2020 7365  rgs)..        se
+00001280: 6c66 2e63 6861 6e6e 656c 203d 2063 6861  lf.channel = cha
+00001290: 6e6e 656c 0d0a 2020 2020 2020 2020 7365  nnel..        se
+000012a0: 6c66 2e6f 6666 7365 7420 3d20 6f66 6673  lf.offset = offs
+000012b0: 6574 0d0a 2020 2020 2020 2020 7365 6c66  et..        self
+000012c0: 2e72 6573 706f 6e73 655f 7469 6d65 203d  .response_time =
+000012d0: 2072 6573 706f 6e73 655f 7469 6d65 0d0a   response_time..
+000012e0: 2020 2020 2020 2020 7365 6c66 2e74 6970          self.tip
+000012f0: 5f74 6872 6573 686f 6c64 203d 2074 6970  _threshold = tip
+00001300: 5f74 6872 6573 686f 6c64 0d0a 2020 2020  _threshold..    
+00001310: 2020 2020 0d0a 2020 2020 2020 2020 7365      ..        se
+00001320: 6c66 2e6d 6f64 656c 5f69 6e66 6f3a 204d  lf.model_info: M
+00001330: 6f64 656c 203d 204e 6f6e 650d 0a20 2020  odel = None..   
+00001340: 2020 2020 2073 656c 662e 6c69 6d69 7473       self.limits
+00001350: 203d 2028 302c 3029 0d0a 2020 2020 2020   = (0,0)..      
+00001360: 2020 7365 6c66 2e70 6f73 6974 696f 6e20    self.position 
+00001370: 3d20 300d 0a20 2020 2020 2020 2073 656c  = 0..        sel
+00001380: 662e 7370 6565 645f 636f 6465 203d 2053  f.speed_code = S
+00001390: 7065 6564 2833 2c33 290d 0a20 2020 2020  peed(3,3)..     
+000013a0: 2020 2073 656c 662e 7370 6565 645f 7072     self.speed_pr
+000013b0: 6573 6574 7320 3d20 4e6f 6e65 0d0a 2020  esets = None..  
+000013c0: 2020 2020 2020 7365 6c66 2e74 6970 5f6c        self.tip_l
+000013d0: 656e 6774 6820 3d20 300d 0a20 2020 2020  ength = 0..     
+000013e0: 2020 200d 0a20 2020 2020 2020 2073 656c     ..        sel
+000013f0: 662e 5f63 6170 6163 6974 616e 6365 203d  f._capacitance =
+00001400: 2030 0d0a 2020 2020 2020 2020 7365 6c66   0..        self
+00001410: 2e5f 7374 6174 7573 5f63 6f64 6520 3d20  ._status_code = 
+00001420: 2727 0d0a 2020 2020 2020 2020 7365 6c66  ''..        self
+00001430: 2e5f 7468 7265 6164 7320 3d20 7b7d 0d0a  ._threads = {}..
+00001440: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00001450: 2020 7072 696e 7428 2241 6e79 2061 7474    print("Any att
+00001460: 6163 6865 6420 7069 7065 7474 6520 7469  ached pipette ti
+00001470: 7020 6d61 7920 6472 6f70 2064 7572 696e  p may drop durin
+00001480: 6720 696e 6974 6961 6c69 7361 7469 6f6e  g initialisation
+00001490: 2e22 290d 0a20 2020 2020 2020 2073 656c  .")..        sel
+000014a0: 662e 5f63 6f6e 6e65 6374 2870 6f72 7429  f._connect(port)
+000014b0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+000014c0: 0d0a 2020 2020 0d0a 2020 2020 2320 5072  ..    ..    # Pr
+000014d0: 6f70 6572 7469 6573 0d0a 2020 2020 4070  operties..    @p
+000014e0: 726f 7065 7274 790d 0a20 2020 2064 6566  roperty..    def
+000014f0: 2063 6170 6163 6974 616e 6365 2873 656c   capacitance(sel
+00001500: 6629 202d 3e20 696e 743a 0d0a 2020 2020  f) -> int:..    
+00001510: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00001520: 5f63 6170 6163 6974 616e 6365 0d0a 2020  _capacitance..  
+00001530: 2020 2020 2020 0d0a 2020 2020 4070 726f        ..    @pro
+00001540: 7065 7274 790d 0a20 2020 2064 6566 2068  perty..    def h
+00001550: 6f6d 655f 706f 7369 7469 6f6e 2873 656c  ome_position(sel
+00001560: 6629 202d 3e20 696e 743a 0d0a 2020 2020  f) -> int:..    
+00001570: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00001580: 6d6f 6465 6c5f 696e 666f 2e68 6f6d 655f  model_info.home_
+00001590: 706f 7369 7469 6f6e 0d0a 2020 2020 0d0a  position..    ..
+000015a0: 2020 2020 4070 726f 7065 7274 790d 0a20      @property.. 
+000015b0: 2020 2064 6566 2070 6f72 7428 7365 6c66     def port(self
+000015c0: 2920 2d3e 2073 7472 3a0d 0a20 2020 2020  ) -> str:..     
+000015d0: 2020 2072 6574 7572 6e20 7365 6c66 2e63     return self.c
+000015e0: 6f6e 6e65 6374 696f 6e5f 6465 7461 696c  onnection_detail
+000015f0: 732e 6765 7428 2770 6f72 7427 2c20 2727  s.get('port', ''
+00001600: 290d 0a20 2020 200d 0a20 2020 2040 7072  )..    ..    @pr
+00001610: 6f70 6572 7479 0d0a 2020 2020 6465 6620  operty..    def 
+00001620: 7265 736f 6c75 7469 6f6e 2873 656c 6629  resolution(self)
+00001630: 202d 3e20 666c 6f61 743a 0d0a 2020 2020   -> float:..    
+00001640: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00001650: 6d6f 6465 6c5f 696e 666f 2e72 6573 6f6c  model_info.resol
+00001660: 7574 696f 6e0d 0a20 2020 200d 0a20 2020  ution..    ..   
+00001670: 2040 7072 6f70 6572 7479 0d0a 2020 2020   @property..    
+00001680: 6465 6620 7374 6174 7573 2873 656c 6629  def status(self)
+00001690: 202d 3e20 7374 723a 0d0a 2020 2020 2020   -> str:..      
+000016a0: 2020 7265 7475 726e 2073 656c 662e 6765    return self.ge
+000016b0: 7453 7461 7475 7328 290d 0a20 2020 200d  tStatus()..    .
+000016c0: 0a20 2020 2064 6566 205f 5f63 7963 6c65  .    def __cycle
+000016d0: 735f 5f28 7365 6c66 2920 2d3e 2055 6e69  s__(self) -> Uni
+000016e0: 6f6e 5b69 6e74 2c20 7374 725d 3a0d 0a20  on[int, str]:.. 
+000016f0: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+00001700: 2020 2020 5265 7472 6965 7665 2074 6f74      Retrieve tot
+00001710: 616c 2063 7963 6c65 206c 6966 6574 696d  al cycle lifetim
+00001720: 650d 0a0d 0a20 2020 2020 2020 2052 6574  e....        Ret
+00001730: 7572 6e73 3a0d 0a20 2020 2020 2020 2020  urns:..         
+00001740: 2020 2055 6e69 6f6e 5b69 6e74 2c20 7374     Union[int, st
+00001750: 725d 3a20 6e75 6d62 6572 206f 6620 6c69  r]: number of li
+00001760: 6665 7469 6d65 2063 7963 6c65 732c 206f  fetime cycles, o
+00001770: 7220 7265 7370 6f6e 7365 2073 7472 696e  r response strin
+00001780: 670d 0a20 2020 2020 2020 2022 2222 0d0a  g..        """..
+00001790: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
+000017a0: 203d 2073 656c 662e 5f71 7565 7279 2827   = self._query('
+000017b0: 4458 2729 0d0a 2020 2020 2020 2020 7472  DX')..        tr
+000017c0: 793a 0d0a 2020 2020 2020 2020 2020 2020  y:..            
+000017d0: 6379 636c 6573 203d 2069 6e74 2872 6573  cycles = int(res
+000017e0: 706f 6e73 6529 0d0a 2020 2020 2020 2020  ponse)..        
+000017f0: 6578 6365 7074 2056 616c 7565 4572 726f  except ValueErro
+00001800: 723a 0d0a 2020 2020 2020 2020 2020 2020  r:..            
+00001810: 7265 7475 726e 2072 6573 706f 6e73 650d  return response.
+00001820: 0a20 2020 2020 2020 2070 7269 6e74 2866  .        print(f
+00001830: 2754 6f74 616c 2063 7963 6c65 733a 207b  'Total cycles: {
+00001840: 6379 636c 6573 7d27 290d 0a20 2020 2020  cycles}')..     
+00001850: 2020 2072 6574 7572 6e20 6379 636c 6573     return cycles
+00001860: 0d0a 2020 2020 0d0a 2020 2020 6465 6620  ..    ..    def 
+00001870: 5f5f 6d6f 6465 6c5f 5f28 7365 6c66 2920  __model__(self) 
+00001880: 2d3e 2073 7472 3a0d 0a20 2020 2020 2020  -> str:..       
+00001890: 2022 2222 0d0a 2020 2020 2020 2020 5265   """..        Re
+000018a0: 7472 6965 7665 2074 6865 206d 6f64 656c  trieve the model
+000018b0: 206f 6620 7468 6520 6465 7669 6365 0d0a   of the device..
+000018c0: 0d0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+000018d0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+000018e0: 7374 723a 206d 6f64 656c 206e 616d 650d  str: model name.
+000018f0: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+00001900: 2020 2020 2020 7265 7370 6f6e 7365 203d        response =
+00001910: 2073 656c 662e 5f71 7565 7279 2827 444d   self._query('DM
+00001920: 2729 0d0a 2020 2020 2020 2020 7072 696e  ')..        prin
+00001930: 7428 6627 4d6f 6465 6c3a 207b 7265 7370  t(f'Model: {resp
+00001940: 6f6e 7365 7d27 290d 0a20 2020 2020 2020  onse}')..       
+00001950: 2072 6574 7572 6e20 7265 7370 6f6e 7365   return response
+00001960: 0d0a 2020 2020 0d0a 2020 2020 6465 6620  ..    ..    def 
+00001970: 5f5f 7265 736f 6c75 7469 6f6e 5f5f 2873  __resolution__(s
+00001980: 656c 6629 202d 3e20 556e 696f 6e5b 696e  elf) -> Union[in
+00001990: 742c 2073 7472 5d3a 0d0a 2020 2020 2020  t, str]:..      
+000019a0: 2020 2222 220d 0a20 2020 2020 2020 2052    """..        R
+000019b0: 6574 7269 6576 6520 7468 6520 7265 736f  etrieve the reso
+000019c0: 6c75 7469 6f6e 206f 6620 7468 6520 6465  lution of the de
+000019d0: 7669 6365 0d0a 0d0a 2020 2020 2020 2020  vice....        
+000019e0: 5265 7475 726e 733a 0d0a 2020 2020 2020  Returns:..      
+000019f0: 2020 2020 2020 556e 696f 6e5b 696e 742c        Union[int,
+00001a00: 2073 7472 5d3a 2076 6f6c 756d 6520 7265   str]: volume re
+00001a10: 736f 6c75 7469 6f6e 206f 6620 6465 7669  solution of devi
+00001a20: 6365 2069 6e20 6e4c 2c20 6f72 2072 6573  ce in nL, or res
+00001a30: 706f 6e73 6520 7374 7269 6e67 0d0a 2020  ponse string..  
+00001a40: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+00001a50: 2020 2072 6573 706f 6e73 6520 3d20 7365     response = se
+00001a60: 6c66 2e5f 7175 6572 7928 2744 5227 290d  lf._query('DR').
+00001a70: 0a20 2020 2020 2020 2074 7279 3a0d 0a20  .        try:.. 
+00001a80: 2020 2020 2020 2020 2020 2072 6573 6f6c             resol
+00001a90: 7574 696f 6e20 3d20 696e 7428 7265 7370  ution = int(resp
+00001aa0: 6f6e 7365 290d 0a20 2020 2020 2020 2065  onse)..        e
+00001ab0: 7863 6570 7420 5661 6c75 6545 7272 6f72  xcept ValueError
+00001ac0: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
+00001ad0: 6574 7572 6e20 7265 7370 6f6e 7365 0d0a  eturn response..
+00001ae0: 2020 2020 2020 2020 7072 696e 7428 6627          print(f'
+00001af0: 7b72 6573 6f6c 7574 696f 6e2f 3130 3030  {resolution/1000
+00001b00: 7d20 754c 202f 2073 7465 7027 290d 0a20  } uL / step').. 
+00001b10: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+00001b20: 736f 6c75 7469 6f6e 0d0a 2020 2020 0d0a  solution..    ..
+00001b30: 2020 2020 6465 6620 5f5f 7665 7273 696f      def __versio
+00001b40: 6e5f 5f28 7365 6c66 2920 2d3e 2073 7472  n__(self) -> str
+00001b50: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
+00001b60: 2020 2020 2020 2020 5265 7472 6965 7665          Retrieve
+00001b70: 2074 6865 2073 6f66 7477 6172 6520 7665   the software ve
+00001b80: 7273 696f 6e20 6f6e 2074 6865 2064 6576  rsion on the dev
+00001b90: 6963 650d 0a0d 0a20 2020 2020 2020 2052  ice....        R
+00001ba0: 6574 7572 6e73 3a0d 0a20 2020 2020 2020  eturns:..       
+00001bb0: 2020 2020 2073 7472 3a20 6465 7669 6365       str: device
+00001bc0: 2076 6572 7369 6f6e 0d0a 2020 2020 2020   version..      
+00001bd0: 2020 2222 220d 0a20 2020 2020 2020 2072    """..        r
+00001be0: 6574 7572 6e20 7365 6c66 2e5f 7175 6572  eturn self._quer
+00001bf0: 7928 2744 5627 290d 0a0d 0a20 2020 2064  y('DV')....    d
+00001c00: 6566 2061 6464 4169 7247 6170 2873 656c  ef addAirGap(sel
+00001c10: 662c 2073 7465 7073 3a69 6e74 203d 2031  f, steps:int = 1
+00001c20: 3029 202d 3e20 7374 723a 0d0a 2020 2020  0) -> str:..    
+00001c30: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+00001c40: 2043 7265 6174 6520 616e 2061 6972 2067   Create an air g
+00001c50: 6170 2062 6574 7765 656e 2074 776f 2076  ap between two v
+00001c60: 6f6c 756d 6573 206f 6620 6c69 7175 6964  olumes of liquid
+00001c70: 2069 6e20 7069 7065 7474 650d 0a20 2020   in pipette..   
+00001c80: 2020 2020 200d 0a20 2020 2020 2020 2041       ..        A
+00001c90: 7267 733a 0d0a 2020 2020 2020 2020 2020  rgs:..          
+00001ca0: 2020 7374 6570 7320 2869 6e74 2c20 6f70    steps (int, op
+00001cb0: 7469 6f6e 616c 293a 206e 756d 6265 7220  tional): number 
+00001cc0: 6f66 2073 7465 7073 2066 6f72 2061 6972  of steps for air
+00001cd0: 2067 6170 2e20 4465 6661 756c 7473 2074   gap. Defaults t
+00001ce0: 6f20 4445 4641 554c 545f 4149 5247 4150  o DEFAULT_AIRGAP
+00001cf0: 2e0d 0a20 2020 2020 2020 2020 2020 2063  ...            c
+00001d00: 6861 6e6e 656c 2028 696e 742c 206f 7074  hannel (int, opt
+00001d10: 696f 6e61 6c29 3a20 6368 616e 6e65 6c20  ional): channel 
+00001d20: 746f 2061 6464 2061 6972 2067 6170 2e20  to add air gap. 
+00001d30: 4465 6661 756c 7473 2074 6f20 4e6f 6e65  Defaults to None
+00001d40: 2e0d 0a0d 0a20 2020 2020 2020 2052 6574  .....        Ret
+00001d50: 7572 6e73 3a0d 0a20 2020 2020 2020 2020  urns:..         
+00001d60: 2020 2073 7472 3a20 6465 7669 6365 2072     str: device r
+00001d70: 6573 706f 6e73 650d 0a20 2020 2020 2020  esponse..       
+00001d80: 2022 2222 0d0a 2020 2020 2020 2020 7265   """..        re
+00001d90: 7370 6f6e 7365 203d 2073 656c 662e 5f71  sponse = self._q
+00001da0: 7565 7279 2866 2752 497b 7374 6570 737d  uery(f'RI{steps}
+00001db0: 2729 0d0a 2020 2020 2020 2020 7469 6d65  ')..        time
+00001dc0: 2e73 6c65 6570 2831 290d 0a20 2020 2020  .sleep(1)..     
+00001dd0: 2020 2072 6574 7572 6e20 7265 7370 6f6e     return respon
+00001de0: 7365 0d0a 2020 2020 2020 2020 0d0a 2020  se..        ..  
+00001df0: 2020 6465 6620 6173 7069 7261 7465 2873    def aspirate(s
+00001e00: 656c 662c 200d 0a20 2020 2020 2020 2076  elf, ..        v
+00001e10: 6f6c 756d 653a 2066 6c6f 6174 2c20 0d0a  olume: float, ..
+00001e20: 2020 2020 2020 2020 7370 6565 643a 204f          speed: O
+00001e30: 7074 696f 6e61 6c5b 666c 6f61 745d 203d  ptional[float] =
+00001e40: 204e 6f6e 652c 200d 0a20 2020 2020 2020   None, ..       
+00001e50: 2077 6169 743a 2069 6e74 203d 2030 2c20   wait: int = 0, 
+00001e60: 0d0a 2020 2020 2020 2020 7061 7573 653a  ..        pause:
+00001e70: 2062 6f6f 6c20 3d20 4661 6c73 652c 200d   bool = False, .
+00001e80: 0a20 2020 2020 2020 2072 6561 6765 6e74  .        reagent
+00001e90: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
+00001ea0: 3d20 4e6f 6e65 2c0d 0a20 2020 2020 2020  = None,..       
+00001eb0: 202a 2a6b 7761 7267 730d 0a20 2020 2029   **kwargs..    )
+00001ec0: 202d 3e20 7374 723a 0d0a 2020 2020 2020   -> str:..      
+00001ed0: 2020 2222 220d 0a20 2020 2020 2020 2041    """..        A
+00001ee0: 7370 6972 6174 6520 6465 7369 7265 6420  spirate desired 
+00001ef0: 766f 6c75 6d65 206f 6620 7265 6167 656e  volume of reagen
+00001f00: 740d 0a0d 0a20 2020 2020 2020 2041 7267  t....        Arg
+00001f10: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00001f20: 766f 6c75 6d65 2028 666c 6f61 7429 3a20  volume (float): 
+00001f30: 7461 7267 6574 2076 6f6c 756d 650d 0a20  target volume.. 
+00001f40: 2020 2020 2020 2020 2020 2073 7065 6564             speed
+00001f50: 2028 4f70 7469 6f6e 616c 5b66 6c6f 6174   (Optional[float
+00001f60: 5d2c 206f 7074 696f 6e61 6c29 3a20 7370  ], optional): sp
+00001f70: 6565 6420 746f 2061 7370 6972 6174 6520  eed to aspirate 
+00001f80: 6174 2e20 4465 6661 756c 7473 2074 6f20  at. Defaults to 
+00001f90: 4e6f 6e65 2e0d 0a20 2020 2020 2020 2020  None...         
+00001fa0: 2020 2077 6169 7420 2869 6e74 2c20 6f70     wait (int, op
+00001fb0: 7469 6f6e 616c 293a 2074 696d 6520 6465  tional): time de
+00001fc0: 6c61 7920 6166 7465 7220 6173 7069 7261  lay after aspira
+00001fd0: 7465 2e20 4465 6661 756c 7473 2074 6f20  te. Defaults to 
+00001fe0: 302e 0d0a 2020 2020 2020 2020 2020 2020  0...            
+00001ff0: 7061 7573 6520 2862 6f6f 6c2c 206f 7074  pause (bool, opt
+00002000: 696f 6e61 6c29 3a20 7768 6574 6865 7220  ional): whether 
+00002010: 746f 2070 6175 7365 2066 6f72 2075 7365  to pause for use
+00002020: 7220 696e 7465 7276 656e 7469 6f6e 2e20  r intervention. 
+00002030: 4465 6661 756c 7473 2074 6f20 4661 6c73  Defaults to Fals
+00002040: 652e 0d0a 2020 2020 2020 2020 2020 2020  e...            
+00002050: 7265 6167 656e 7420 284f 7074 696f 6e61  reagent (Optiona
+00002060: 6c5b 7374 725d 2c20 6f70 7469 6f6e 616c  l[str], optional
+00002070: 293a 206e 616d 6520 6f66 2072 6561 6765  ): name of reage
+00002080: 6e74 2e20 4465 6661 756c 7473 2074 6f20  nt. Defaults to 
+00002090: 4e6f 6e65 2e0d 0a20 2020 2020 2020 2020  None...         
+000020a0: 2020 200d 0a20 2020 2020 2020 2052 6574     ..        Ret
+000020b0: 7572 6e73 3a0d 0a20 2020 2020 2020 2020  urns:..         
+000020c0: 2020 2073 7472 3a20 6465 7669 6365 2072     str: device r
+000020d0: 6573 706f 6e73 650d 0a20 2020 2020 2020  esponse..       
+000020e0: 2022 2222 200d 0a20 2020 2020 2020 2073   """ ..        s
+000020f0: 656c 662e 7365 7446 6c61 6728 7061 7573  elf.setFlag(paus
+00002100: 655f 6665 6564 6261 636b 3d54 7275 652c  e_feedback=True,
+00002110: 206f 6363 7570 6965 643d 5472 7565 290d   occupied=True).
+00002120: 0a20 2020 2020 2020 2076 6f6c 756d 6520  .        volume 
+00002130: 3d20 6d69 6e28 766f 6c75 6d65 2c20 7365  = min(volume, se
+00002140: 6c66 2e63 6170 6163 6974 7920 2d20 7365  lf.capacity - se
+00002150: 6c66 2e76 6f6c 756d 6529 0d0a 2020 2020  lf.volume)..    
+00002160: 2020 2020 7374 6570 7320 3d20 696e 7428      steps = int(
+00002170: 766f 6c75 6d65 202f 2073 656c 662e 7265  volume / self.re
+00002180: 736f 6c75 7469 6f6e 290d 0a20 2020 2020  solution)..     
+00002190: 2020 2076 6f6c 756d 6520 3d20 7374 6570     volume = step
+000021a0: 7320 2a20 7365 6c66 2e72 6573 6f6c 7574  s * self.resolut
+000021b0: 696f 6e0d 0a20 2020 2020 2020 2069 6620  ion..        if 
+000021c0: 766f 6c75 6d65 203d 3d20 303a 0d0a 2020  volume == 0:..  
+000021d0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+000021e0: 2027 270d 0a20 2020 2020 2020 2070 7269   ''..        pri
+000021f0: 6e74 2866 2741 7370 6972 6174 696e 6720  nt(f'Aspirating 
+00002200: 7b76 6f6c 756d 657d 2075 4c2e 2e2e 2729  {volume} uL...')
+00002210: 0d0a 2020 2020 2020 2020 7374 6172 745f  ..        start_
+00002220: 6173 7069 7261 7465 203d 2074 696d 652e  aspirate = time.
+00002230: 7469 6d65 2829 0d0a 2020 2020 2020 2020  time()..        
+00002240: 7370 6565 6420 3d20 7365 6c66 2e73 7065  speed = self.spe
+00002250: 6564 2e75 7020 6966 2073 7065 6564 2069  ed.up if speed i
+00002260: 7320 4e6f 6e65 2065 6c73 6520 7370 6565  s None else spee
+00002270: 640d 0a20 2020 2020 2020 200d 0a20 2020  d..        ..   
+00002280: 2020 2020 2069 6620 7370 6565 6420 696e       if speed in
+00002290: 2073 656c 662e 7370 6565 645f 7072 6573   self.speed_pres
+000022a0: 6574 733a 0d0a 2020 2020 2020 2020 2020  ets:..          
+000022b0: 2020 6966 2073 7065 6564 2021 3d20 7365    if speed != se
+000022c0: 6c66 2e73 7065 6564 2e75 703a 0d0a 2020  lf.speed.up:..  
+000022d0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000022e0: 6c66 2e73 6574 5370 6565 6428 7370 6565  lf.setSpeed(spee
+000022f0: 643d 7370 6565 642c 2075 703d 5472 7565  d=speed, up=True
+00002300: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00002310: 2020 2073 656c 662e 7370 6565 642e 7570     self.speed.up
+00002320: 203d 2073 7065 6564 0d0a 2020 2020 2020   = speed..      
+00002330: 2020 2020 2020 7374 6172 745f 6173 7069        start_aspi
+00002340: 7261 7465 203d 2074 696d 652e 7469 6d65  rate = time.time
+00002350: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
+00002360: 7265 7370 6f6e 7365 203d 2073 656c 662e  response = self.
+00002370: 5f71 7565 7279 2866 2752 497b 7374 6570  _query(f'RI{step
+00002380: 737d 2729 0d0a 2020 2020 2020 2020 2020  s}')..          
+00002390: 2020 6d6f 7665 5f74 696d 6520 3d20 7374    move_time = st
+000023a0: 6570 732a 7365 6c66 2e72 6573 6f6c 7574  eps*self.resolut
+000023b0: 696f 6e20 2f20 7370 6565 640d 0a20 2020  ion / speed..   
+000023c0: 2020 2020 2020 2020 2074 696d 652e 736c           time.sl
+000023d0: 6565 7028 6d6f 7665 5f74 696d 6529 0d0a  eep(move_time)..
+000023e0: 2020 2020 2020 2020 2020 2020 2320 6966              # if
+000023f0: 2072 6573 706f 6e73 6520 213d 2027 6f6b   response != 'ok
+00002400: 273a 0d0a 2020 2020 2020 2020 2020 2020  ':..            
+00002410: 2320 2020 2020 7265 7475 726e 2072 6573  #     return res
+00002420: 706f 6e73 650d 0a20 2020 2020 2020 2020  ponse..         
+00002430: 2020 200d 0a20 2020 2020 2020 2065 6c69     ..        eli
+00002440: 6620 7370 6565 6420 6e6f 7420 696e 2073  f speed not in s
+00002450: 656c 662e 7370 6565 645f 7072 6573 6574  elf.speed_preset
+00002460: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00002470: 7072 696e 7428 6622 5461 7267 6574 3a20  print(f"Target: 
+00002480: 7b76 6f6c 756d 657d 2075 4c20 6174 207b  {volume} uL at {
+00002490: 7370 6565 647d 2075 4c2f 732e 2e2e 2229  speed} uL/s...")
+000024a0: 0d0a 2020 2020 2020 2020 2020 2020 7370  ..            sp
+000024b0: 6565 645f 7061 7261 6d65 7465 7273 203d  eed_parameters =
+000024c0: 2073 656c 662e 5f63 616c 6375 6c61 7465   self._calculate
+000024d0: 5f73 7065 6564 5f70 6172 616d 6574 6572  _speed_parameter
+000024e0: 7328 766f 6c75 6d65 3d76 6f6c 756d 652c  s(volume=volume,
+000024f0: 2073 7065 6564 3d73 7065 6564 290d 0a20   speed=speed).. 
+00002500: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+00002510: 2873 7065 6564 5f70 6172 616d 6574 6572  (speed_parameter
+00002520: 7329 0d0a 2020 2020 2020 2020 2020 2020  s)..            
+00002530: 7072 6573 6574 203d 2073 7065 6564 5f70  preset = speed_p
+00002540: 6172 616d 6574 6572 732e 7072 6573 6574  arameters.preset
+00002550: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00002560: 2070 7265 7365 7420 6973 204e 6f6e 653a   preset is None:
+00002570: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002580: 2020 7261 6973 6520 5275 6e74 696d 6545    raise RuntimeE
+00002590: 7272 6f72 2827 5461 7267 6574 2073 7065  rror('Target spe
+000025a0: 6564 206e 6f74 2070 6f73 7369 626c 652e  ed not possible.
+000025b0: 2729 0d0a 2020 2020 2020 2020 2020 2020  ')..            
+000025c0: 7365 6c66 2e73 6574 5370 6565 6428 7370  self.setSpeed(sp
+000025d0: 6565 643d 7072 6573 6574 2c20 7570 3d54  eed=preset, up=T
+000025e0: 7275 6529 0d0a 2020 2020 2020 2020 2020  rue)..          
+000025f0: 2020 7365 6c66 2e73 7065 6564 2e75 7020    self.speed.up 
+00002600: 3d20 7370 6565 640d 0a20 2020 2020 2020  = speed..       
+00002610: 2020 2020 2073 7461 7274 5f61 7370 6972       start_aspir
+00002620: 6174 6520 3d20 7469 6d65 2e74 696d 6528  ate = time.time(
+00002630: 290d 0a20 2020 2020 2020 2020 2020 200d  )..            .
+00002640: 0a20 2020 2020 2020 2020 2020 2073 7465  .            ste
+00002650: 7073 5f6c 6566 7420 3d20 7374 6570 730d  ps_left = steps.
+00002660: 0a20 2020 2020 2020 2020 2020 2064 656c  .            del
+00002670: 6179 203d 2073 7065 6564 5f70 6172 616d  ay = speed_param
+00002680: 6574 6572 732e 6465 6c61 790d 0a20 2020  eters.delay..   
+00002690: 2020 2020 2020 2020 2073 7465 705f 7369           step_si
+000026a0: 7a65 203d 2073 7065 6564 5f70 6172 616d  ze = speed_param
+000026b0: 6574 6572 732e 7374 6570 5f73 697a 650d  eters.step_size.
+000026c0: 0a20 2020 2020 2020 2020 2020 2069 6e74  .            int
+000026d0: 6572 7661 6c73 203d 2073 7065 6564 5f70  ervals = speed_p
+000026e0: 6172 616d 6574 6572 732e 696e 7465 7276  arameters.interv
+000026f0: 616c 730d 0a20 2020 2020 2020 2020 2020  als..           
+00002700: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
+00002710: 696e 7465 7276 616c 7329 3a0d 0a20 2020  intervals):..   
+00002720: 2020 2020 2020 2020 2020 2020 2073 7461               sta
+00002730: 7274 5f74 696d 6520 3d20 7469 6d65 2e74  rt_time = time.t
+00002740: 696d 6528 290d 0a20 2020 2020 2020 2020  ime()..         
+00002750: 2020 2020 2020 2073 7465 7020 3d20 7374         step = st
+00002760: 6570 5f73 697a 6520 6966 2028 692b 3120  ep_size if (i+1 
+00002770: 213d 2069 6e74 6572 7661 6c73 2920 656c  != intervals) el
+00002780: 7365 2073 7465 7073 5f6c 6566 740d 0a20  se steps_left.. 
+00002790: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+000027a0: 6f76 655f 7469 6d65 203d 2073 7465 702a  ove_time = step*
+000027b0: 7365 6c66 2e72 6573 6f6c 7574 696f 6e20  self.resolution 
+000027c0: 2f20 7072 6573 6574 0d0a 2020 2020 2020  / preset..      
+000027d0: 2020 2020 2020 2020 2020 7265 7370 6f6e            respon
+000027e0: 7365 203d 2073 656c 662e 5f71 7565 7279  se = self._query
+000027f0: 2866 2752 497b 7374 6570 7d27 2c20 7265  (f'RI{step}', re
+00002800: 7375 6d65 5f66 6565 6462 6163 6b3d 4661  sume_feedback=Fa
+00002810: 6c73 6529 0d0a 2020 2020 2020 2020 2020  lse)..          
+00002820: 2020 2020 2020 2320 6966 2072 6573 706f        # if respo
+00002830: 6e73 6520 213d 2027 6f6b 273a 0d0a 2020  nse != 'ok':..  
+00002840: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00002850: 2020 2020 7072 696e 7428 2241 7370 6972      print("Aspir
+00002860: 6174 696f 6e20 6661 696c 6564 2229 0d0a  ation failed")..
+00002870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002880: 2320 2020 2020 7265 7475 726e 2072 6573  #     return res
+00002890: 706f 6e73 650d 0a20 2020 2020 2020 2020  ponse..         
+000028a0: 2020 2020 2020 2073 7465 7073 5f6c 6566         steps_lef
+000028b0: 7420 2d3d 2073 7465 700d 0a20 2020 2020  t -= step..     
+000028c0: 2020 2020 2020 2020 2020 2064 7572 6174             durat
+000028d0: 696f 6e20 3d20 7469 6d65 2e74 696d 6528  ion = time.time(
+000028e0: 2920 2d20 7374 6172 745f 7469 6d65 0d0a  ) - start_time..
+000028f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002900: 6966 2064 7572 6174 696f 6e20 3c20 2864  if duration < (d
+00002910: 656c 6179 2b6d 6f76 655f 7469 6d65 293a  elay+move_time):
+00002920: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002930: 2020 2020 2020 7469 6d65 2e73 6c65 6570        time.sleep
+00002940: 2864 656c 6179 2b6d 6f76 655f 7469 6d65  (delay+move_time
+00002950: 2d64 7572 6174 696f 6e29 0d0a 2020 2020  -duration)..    
+00002960: 2020 2020 0d0a 2020 2020 2020 2020 2320      ..        # 
+00002970: 5570 6461 7465 2076 616c 7565 730d 0a20  Update values.. 
+00002980: 2020 2020 2020 2070 7269 6e74 2866 2741         print(f'A
+00002990: 7370 6972 6174 696f 6e20 7469 6d65 3a20  spiration time: 
+000029a0: 7b74 696d 652e 7469 6d65 2829 2d73 7461  {time.time()-sta
+000029b0: 7274 5f61 7370 6972 6174 657d 7327 290d  rt_aspirate}s').
+000029c0: 0a20 2020 2020 2020 2074 696d 652e 736c  .        time.sl
+000029d0: 6565 7028 7761 6974 290d 0a20 2020 2020  eep(wait)..     
+000029e0: 2020 2073 656c 662e 7365 7446 6c61 6728     self.setFlag(
+000029f0: 6f63 6375 7069 6564 3d46 616c 7365 2c20  occupied=False, 
+00002a00: 7061 7573 655f 6665 6564 6261 636b 3d46  pause_feedback=F
+00002a10: 616c 7365 290d 0a20 2020 2020 2020 2073  alse)..        s
+00002a20: 656c 662e 766f 6c75 6d65 202b 3d20 766f  elf.volume += vo
+00002a30: 6c75 6d65 0d0a 2020 2020 2020 2020 7365  lume..        se
+00002a40: 6c66 2e70 6f73 6974 696f 6e20 2b3d 2073  lf.position += s
+00002a50: 7465 7073 0d0a 2020 2020 2020 2020 6966  teps..        if
+00002a60: 2072 6561 6765 6e74 2069 7320 6e6f 7420   reagent is not 
+00002a70: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
+00002a80: 2020 2073 656c 662e 7265 6167 656e 7420     self.reagent 
+00002a90: 3d20 7265 6167 656e 740d 0a20 2020 2020  = reagent..     
+00002aa0: 2020 2069 6620 7061 7573 653a 0d0a 2020     if pause:..  
+00002ab0: 2020 2020 2020 2020 2020 696e 7075 7428            input(
+00002ac0: 2250 7265 7373 2027 456e 7465 7227 2074  "Press 'Enter' t
+00002ad0: 6f20 7072 6f63 6565 642e 2229 0d0a 2020  o proceed.")..  
+00002ae0: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+00002af0: 706f 6e73 650d 0a20 2020 200d 0a20 2020  ponse..    ..   
+00002b00: 2064 6566 2062 6c6f 776f 7574 2873 656c   def blowout(sel
+00002b10: 662c 2068 6f6d 653a 626f 6f6c 203d 2054  f, home:bool = T
+00002b20: 7275 652c 202a 2a6b 7761 7267 7329 202d  rue, **kwargs) -
+00002b30: 3e20 7374 723a 0d0a 2020 2020 2020 2020  > str:..        
+00002b40: 2222 220d 0a20 2020 2020 2020 2042 6c6f  """..        Blo
+00002b50: 776f 7574 206c 6971 7569 6420 6672 6f6d  wout liquid from
+00002b60: 2074 6970 0d0a 0d0a 2020 2020 2020 2020   tip....        
+00002b70: 4172 6773 3a0d 0a20 2020 2020 2020 2020  Args:..         
+00002b80: 2020 2068 6f6d 6520 2862 6f6f 6c2c 206f     home (bool, o
+00002b90: 7074 696f 6e61 6c29 3a20 7768 6574 6865  ptional): whethe
+00002ba0: 7220 746f 2072 6574 7572 6e20 706c 756e  r to return plun
+00002bb0: 6765 7220 746f 2068 6f6d 6520 706f 7369  ger to home posi
+00002bc0: 7469 6f6e 2e20 4465 6661 756c 7473 2074  tion. Defaults t
+00002bd0: 6f20 5472 7565 2e0d 0a0d 0a20 2020 2020  o True.....     
+00002be0: 2020 2052 6574 7572 6e73 3a0d 0a20 2020     Returns:..   
+00002bf0: 2020 2020 2020 2020 2073 7472 3a20 6465           str: de
+00002c00: 7669 6365 2072 6573 706f 6e73 650d 0a20  vice response.. 
+00002c10: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+00002c20: 2020 2020 636f 6d6d 616e 6420 3d20 6627      command = f'
+00002c30: 5242 7b73 656c 662e 686f 6d65 5f70 6f73  RB{self.home_pos
+00002c40: 6974 696f 6e7d 2720 6966 2068 6f6d 6520  ition}' if home 
+00002c50: 656c 7365 2027 5242 270d 0a20 2020 2020  else 'RB'..     
+00002c60: 2020 2072 6573 706f 6e73 6520 3d20 7365     response = se
+00002c70: 6c66 2e5f 7175 6572 7928 636f 6d6d 616e  lf._query(comman
+00002c80: 6429 0d0a 2020 2020 2020 2020 7365 6c66  d)..        self
+00002c90: 2e70 6f73 6974 696f 6e20 3d20 7365 6c66  .position = self
+00002ca0: 2e68 6f6d 655f 706f 7369 7469 6f6e 0d0a  .home_position..
+00002cb0: 2020 2020 2020 2020 7469 6d65 2e73 6c65          time.sle
+00002cc0: 6570 2831 290d 0a20 2020 2020 2020 2072  ep(1)..        r
+00002cd0: 6574 7572 6e20 7265 7370 6f6e 7365 0d0a  eturn response..
+00002ce0: 2020 2020 0d0a 2020 2020 6465 6620 6469      ..    def di
+00002cf0: 7370 656e 7365 2873 656c 662c 200d 0a20  spense(self, .. 
+00002d00: 2020 2020 2020 2076 6f6c 756d 653a 2066         volume: f
+00002d10: 6c6f 6174 2c20 0d0a 2020 2020 2020 2020  loat, ..        
+00002d20: 7370 6565 643a 204f 7074 696f 6e61 6c5b  speed: Optional[
+00002d30: 666c 6f61 745d 203d 204e 6f6e 652c 200d  float] = None, .
+00002d40: 0a20 2020 2020 2020 2077 6169 743a 2069  .        wait: i
+00002d50: 6e74 203d 2030 2c20 0d0a 2020 2020 2020  nt = 0, ..      
+00002d60: 2020 7061 7573 653a 2062 6f6f 6c20 3d20    pause: bool = 
+00002d70: 4661 6c73 652c 200d 0a20 2020 2020 2020  False, ..       
+00002d80: 2062 6c6f 776f 7574 3a20 626f 6f6c 203d   blowout: bool =
+00002d90: 2046 616c 7365 2c0d 0a20 2020 2020 2020   False,..       
+00002da0: 2062 6c6f 776f 7574 5f68 6f6d 653a 2062   blowout_home: b
+00002db0: 6f6f 6c20 3d20 5472 7565 2c0d 0a20 2020  ool = True,..   
+00002dc0: 2020 2020 2066 6f72 6365 5f64 6973 7065       force_dispe
+00002dd0: 6e73 653a 2062 6f6f 6c20 3d20 4661 6c73  nse: bool = Fals
+00002de0: 652c 200d 0a20 2020 2020 2020 202a 2a6b  e, ..        **k
+00002df0: 7761 7267 730d 0a20 2020 2029 202d 3e20  wargs..    ) -> 
+00002e00: 7374 723a 0d0a 2020 2020 2020 2020 2222  str:..        ""
+00002e10: 220d 0a20 2020 2020 2020 2044 6973 7065  "..        Dispe
+00002e20: 6e73 6520 6465 7369 7265 6420 766f 6c75  nse desired volu
+00002e30: 6d65 206f 6620 7265 6167 656e 740d 0a0d  me of reagent...
+00002e40: 0a20 2020 2020 2020 2041 7267 733a 0d0a  .        Args:..
+00002e50: 2020 2020 2020 2020 2020 2020 766f 6c75              volu
+00002e60: 6d65 2028 666c 6f61 7429 3a20 7461 7267  me (float): targ
+00002e70: 6574 2076 6f6c 756d 650d 0a20 2020 2020  et volume..     
+00002e80: 2020 2020 2020 2073 7065 6564 2028 4f70         speed (Op
+00002e90: 7469 6f6e 616c 5b66 6c6f 6174 5d2c 206f  tional[float], o
+00002ea0: 7074 696f 6e61 6c29 3a20 7370 6565 6420  ptional): speed 
+00002eb0: 746f 2064 6973 7065 6e73 6520 6174 2e20  to dispense at. 
+00002ec0: 4465 6661 756c 7473 2074 6f20 4e6f 6e65  Defaults to None
+00002ed0: 2e0d 0a20 2020 2020 2020 2020 2020 2077  ...            w
+00002ee0: 6169 7420 2869 6e74 2c20 6f70 7469 6f6e  ait (int, option
+00002ef0: 616c 293a 2074 696d 6520 6465 6c61 7920  al): time delay 
+00002f00: 6166 7465 7220 6469 7370 656e 7365 2e20  after dispense. 
+00002f10: 4465 6661 756c 7473 2074 6f20 302e 0d0a  Defaults to 0...
+00002f20: 2020 2020 2020 2020 2020 2020 7061 7573              paus
+00002f30: 6520 2862 6f6f 6c2c 206f 7074 696f 6e61  e (bool, optiona
+00002f40: 6c29 3a20 7768 6574 6865 7220 746f 2070  l): whether to p
+00002f50: 6175 7365 2066 6f72 2075 7365 7220 696e  ause for user in
+00002f60: 7465 7276 656e 7469 6f6e 2e20 4465 6661  tervention. Defa
+00002f70: 756c 7473 2074 6f20 4661 6c73 652e 0d0a  ults to False...
+00002f80: 2020 2020 2020 2020 2020 2020 626c 6f77              blow
+00002f90: 6f75 7420 2862 6f6f 6c2c 206f 7074 696f  out (bool, optio
+00002fa0: 6e61 6c29 3a20 7768 6574 6865 7220 7065  nal): whether pe
+00002fb0: 7266 6f72 6d20 626c 6f77 6f75 742e 2044  rform blowout. D
+00002fc0: 6566 6175 6c74 7320 746f 2046 616c 7365  efaults to False
+00002fd0: 2e0d 0a20 2020 2020 2020 2020 2020 2062  ...            b
+00002fe0: 6c6f 776f 7574 5f68 6f6d 6520 2862 6f6f  lowout_home (boo
+00002ff0: 6c2c 206f 7074 696f 6e61 6c29 3a20 7768  l, optional): wh
+00003000: 6574 6865 7220 746f 2072 6574 7572 6e20  ether to return 
+00003010: 7468 6520 706c 756e 6765 7220 686f 6d65  the plunger home
+00003020: 2061 6674 6572 2062 6c6f 776f 7574 2e20   after blowout. 
+00003030: 4465 6661 756c 7473 2074 6f20 5472 7565  Defaults to True
+00003040: 2e0d 0a20 2020 2020 2020 2020 2020 2066  ...            f
+00003050: 6f72 6365 5f64 6973 7065 6e73 6520 2862  orce_dispense (b
+00003060: 6f6f 6c2c 206f 7074 696f 6e61 6c29 3a20  ool, optional): 
+00003070: 7768 6574 6865 7220 746f 2064 6973 7065  whether to dispe
+00003080: 6e73 6520 7265 6167 656e 7420 7265 6761  nse reagent rega
+00003090: 7264 6c65 7373 2e20 4465 6661 756c 7473  rdless. Defaults
+000030a0: 2074 6f20 4661 6c73 652e 0d0a 0d0a 2020   to False.....  
+000030b0: 2020 2020 2020 5261 6973 6573 3a0d 0a20        Raises:.. 
+000030c0: 2020 2020 2020 2020 2020 2056 616c 7565             Value
+000030d0: 4572 726f 723a 2052 6571 7569 7265 6420  Error: Required 
+000030e0: 6469 7370 656e 7365 2076 6f6c 756d 6520  dispense volume 
+000030f0: 6973 2067 7265 6174 6572 2074 6861 6e20  is greater than 
+00003100: 766f 6c75 6d65 2069 6e20 7469 700d 0a0d  volume in tip...
+00003110: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+00003120: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
+00003130: 7472 3a20 6465 7669 6365 2072 6573 706f  tr: device respo
+00003140: 6e73 650d 0a20 2020 2020 2020 2022 2222  nse..        """
+00003150: 0d0a 2020 2020 2020 2020 7365 6c66 2e73  ..        self.s
+00003160: 6574 466c 6167 2870 6175 7365 5f66 6565  etFlag(pause_fee
+00003170: 6462 6163 6b3d 5472 7565 2c20 6f63 6375  dback=True, occu
+00003180: 7069 6564 3d54 7275 6529 0d0a 2020 2020  pied=True)..    
+00003190: 2020 2020 6966 2066 6f72 6365 5f64 6973      if force_dis
+000031a0: 7065 6e73 653a 0d0a 2020 2020 2020 2020  pense:..        
+000031b0: 2020 2020 766f 6c75 6d65 203d 206d 696e      volume = min
+000031c0: 2876 6f6c 756d 652c 2073 656c 662e 766f  (volume, self.vo
+000031d0: 6c75 6d65 290d 0a20 2020 2020 2020 2065  lume)..        e
+000031e0: 6c69 6620 766f 6c75 6d65 203e 2073 656c  lif volume > sel
+000031f0: 662e 766f 6c75 6d65 3a0d 0a20 2020 2020  f.volume:..     
+00003200: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+00003210: 7565 4572 726f 7228 2752 6571 7569 7265  ueError('Require
+00003220: 6420 6469 7370 656e 7365 2076 6f6c 756d  d dispense volum
+00003230: 6520 6973 2067 7265 6174 6572 2074 6861  e is greater tha
+00003240: 6e20 766f 6c75 6d65 2069 6e20 7469 702e  n volume in tip.
+00003250: 2729 0d0a 2020 2020 2020 2020 7374 6570  ')..        step
+00003260: 7320 3d20 696e 7428 766f 6c75 6d65 202f  s = int(volume /
+00003270: 2073 656c 662e 7265 736f 6c75 7469 6f6e   self.resolution
+00003280: 290d 0a20 2020 2020 2020 2076 6f6c 756d  )..        volum
+00003290: 6520 3d20 7374 6570 7320 2a20 7365 6c66  e = steps * self
+000032a0: 2e72 6573 6f6c 7574 696f 6e0d 0a20 2020  .resolution..   
+000032b0: 2020 2020 2069 6620 766f 6c75 6d65 203d       if volume =
+000032c0: 3d20 303a 0d0a 2020 2020 2020 2020 2020  = 0:..          
+000032d0: 2020 7265 7475 726e 2027 270d 0a20 2020    return ''..   
+000032e0: 2020 2020 2070 7269 6e74 2866 2744 6973       print(f'Dis
+000032f0: 7065 6e73 696e 6720 7b76 6f6c 756d 657d  pensing {volume}
+00003300: 2075 4c2e 2e2e 2729 0d0a 2020 2020 2020   uL...')..      
+00003310: 2020 7374 6172 745f 6469 7370 656e 7365    start_dispense
+00003320: 203d 2074 696d 652e 7469 6d65 2829 0d0a   = time.time()..
+00003330: 2020 2020 2020 2020 7370 6565 6420 3d20          speed = 
+00003340: 7365 6c66 2e73 7065 6564 2e64 6f77 6e20  self.speed.down 
+00003350: 6966 2073 7065 6564 2069 7320 4e6f 6e65  if speed is None
+00003360: 2065 6c73 6520 7370 6565 640d 0a0d 0a20   else speed.... 
+00003370: 2020 2020 2020 2069 6620 7370 6565 6420         if speed 
+00003380: 696e 2073 656c 662e 7370 6565 645f 7072  in self.speed_pr
+00003390: 6573 6574 733a 0d0a 2020 2020 2020 2020  esets:..        
+000033a0: 2020 2020 6966 2073 7065 6564 2021 3d20      if speed != 
+000033b0: 7365 6c66 2e73 7065 6564 2e64 6f77 6e3a  self.speed.down:
+000033c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000033d0: 2020 7365 6c66 2e73 6574 5370 6565 6428    self.setSpeed(
+000033e0: 7370 6565 643d 7370 6565 642c 2075 703d  speed=speed, up=
+000033f0: 4661 6c73 6529 0d0a 2020 2020 2020 2020  False)..        
+00003400: 2020 2020 2020 2020 7365 6c66 2e73 7065          self.spe
+00003410: 6564 2e64 6f77 6e20 3d20 7370 6565 640d  ed.down = speed.
+00003420: 0a20 2020 2020 2020 2020 2020 2073 7461  .            sta
+00003430: 7274 5f64 6973 7065 6e73 6520 3d20 7469  rt_dispense = ti
+00003440: 6d65 2e74 696d 6528 290d 0a20 2020 2020  me.time()..     
+00003450: 2020 2020 2020 2072 6573 706f 6e73 6520         response 
+00003460: 3d20 7365 6c66 2e5f 7175 6572 7928 6627  = self._query(f'
+00003470: 524f 7b73 7465 7073 7d27 290d 0a20 2020  RO{steps}')..   
+00003480: 2020 2020 2020 2020 206d 6f76 655f 7469           move_ti
+00003490: 6d65 203d 2073 7465 7073 2a73 656c 662e  me = steps*self.
+000034a0: 7265 736f 6c75 7469 6f6e 202f 2073 7065  resolution / spe
+000034b0: 6564 0d0a 2020 2020 2020 2020 2020 2020  ed..            
+000034c0: 7469 6d65 2e73 6c65 6570 286d 6f76 655f  time.sleep(move_
+000034d0: 7469 6d65 290d 0a20 2020 2020 2020 2020  time)..         
+000034e0: 2020 2023 2069 6620 7265 7370 6f6e 7365     # if response
+000034f0: 2021 3d20 276f 6b27 3a0d 0a20 2020 2020   != 'ok':..     
+00003500: 2020 2020 2020 2023 2020 2020 2072 6574         #     ret
+00003510: 7572 6e20 7265 7370 6f6e 7365 0d0a 2020  urn response..  
+00003520: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00003530: 2020 2020 656c 6966 2073 7065 6564 206e      elif speed n
+00003540: 6f74 2069 6e20 7365 6c66 2e73 7065 6564  ot in self.speed
+00003550: 5f70 7265 7365 7473 3a0d 0a20 2020 2020  _presets:..     
+00003560: 2020 2020 2020 2070 7269 6e74 2866 2254         print(f"T
+00003570: 6172 6765 743a 207b 766f 6c75 6d65 7d20  arget: {volume} 
+00003580: 754c 2061 7420 7b73 7065 6564 7d20 754c  uL at {speed} uL
+00003590: 2f73 2e2e 2e22 290d 0a20 2020 2020 2020  /s...")..       
+000035a0: 2020 2020 2073 7065 6564 5f70 6172 616d       speed_param
+000035b0: 6574 6572 7320 3d20 7365 6c66 2e5f 6361  eters = self._ca
+000035c0: 6c63 756c 6174 655f 7370 6565 645f 7061  lculate_speed_pa
+000035d0: 7261 6d65 7465 7273 2876 6f6c 756d 653d  rameters(volume=
+000035e0: 766f 6c75 6d65 2c20 7370 6565 643d 7370  volume, speed=sp
+000035f0: 6565 6429 0d0a 2020 2020 2020 2020 2020  eed)..          
+00003600: 2020 7072 696e 7428 7370 6565 645f 7061    print(speed_pa
+00003610: 7261 6d65 7465 7273 290d 0a20 2020 2020  rameters)..     
+00003620: 2020 2020 2020 2070 7265 7365 7420 3d20         preset = 
+00003630: 7370 6565 645f 7061 7261 6d65 7465 7273  speed_parameters
+00003640: 2e70 7265 7365 740d 0a20 2020 2020 2020  .preset..       
+00003650: 2020 2020 2069 6620 7072 6573 6574 2069       if preset i
+00003660: 7320 4e6f 6e65 3a0d 0a20 2020 2020 2020  s None:..       
+00003670: 2020 2020 2020 2020 2072 6169 7365 2052           raise R
+00003680: 756e 7469 6d65 4572 726f 7228 2754 6172  untimeError('Tar
+00003690: 6765 7420 7370 6565 6420 6e6f 7420 706f  get speed not po
+000036a0: 7373 6962 6c65 2e27 290d 0a20 2020 2020  ssible.')..     
+000036b0: 2020 2020 2020 2073 656c 662e 7365 7453         self.setS
+000036c0: 7065 6564 2873 7065 6564 3d70 7265 7365  peed(speed=prese
+000036d0: 742c 2075 703d 4661 6c73 6529 0d0a 2020  t, up=False)..  
+000036e0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+000036f0: 7065 6564 2e64 6f77 6e20 3d20 7370 6565  peed.down = spee
+00003700: 640d 0a20 2020 2020 2020 2020 2020 2073  d..            s
+00003710: 7461 7274 5f64 6973 7065 6e73 6520 3d20  tart_dispense = 
+00003720: 7469 6d65 2e74 696d 6528 290d 0a20 2020  time.time()..   
+00003730: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00003740: 2020 2073 7465 7073 5f6c 6566 7420 3d20     steps_left = 
+00003750: 7374 6570 730d 0a20 2020 2020 2020 2020  steps..         
+00003760: 2020 2064 656c 6179 203d 2073 7065 6564     delay = speed
+00003770: 5f70 6172 616d 6574 6572 732e 6465 6c61  _parameters.dela
+00003780: 790d 0a20 2020 2020 2020 2020 2020 2073  y..            s
+00003790: 7465 705f 7369 7a65 203d 2073 7065 6564  tep_size = speed
+000037a0: 5f70 6172 616d 6574 6572 732e 7374 6570  _parameters.step
+000037b0: 5f73 697a 650d 0a20 2020 2020 2020 2020  _size..         
+000037c0: 2020 2069 6e74 6572 7661 6c73 203d 2073     intervals = s
+000037d0: 7065 6564 5f70 6172 616d 6574 6572 732e  peed_parameters.
+000037e0: 696e 7465 7276 616c 730d 0a20 2020 2020  intervals..     
+000037f0: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
+00003800: 7261 6e67 6528 696e 7465 7276 616c 7329  range(intervals)
+00003810: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00003820: 2020 2073 7461 7274 5f74 696d 6520 3d20     start_time = 
+00003830: 7469 6d65 2e74 696d 6528 290d 0a20 2020  time.time()..   
+00003840: 2020 2020 2020 2020 2020 2020 2073 7465               ste
+00003850: 7020 3d20 7374 6570 5f73 697a 6520 6966  p = step_size if
+00003860: 2028 692b 3120 213d 2069 6e74 6572 7661   (i+1 != interva
+00003870: 6c73 2920 656c 7365 2073 7465 7073 5f6c  ls) else steps_l
+00003880: 6566 740d 0a20 2020 2020 2020 2020 2020  eft..           
+00003890: 2020 2020 206d 6f76 655f 7469 6d65 203d       move_time =
+000038a0: 2073 7465 702a 7365 6c66 2e72 6573 6f6c   step*self.resol
+000038b0: 7574 696f 6e20 2f20 7072 6573 6574 0d0a  ution / preset..
+000038c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000038d0: 7265 7370 6f6e 7365 203d 2073 656c 662e  response = self.
+000038e0: 5f71 7565 7279 2866 2752 4f7b 7374 6570  _query(f'RO{step
+000038f0: 7d27 2c20 7265 7375 6d65 5f66 6565 6462  }', resume_feedb
+00003900: 6163 6b3d 4661 6c73 6529 0d0a 2020 2020  ack=False)..    
+00003910: 2020 2020 2020 2020 2020 2020 2320 6966              # if
+00003920: 2072 6573 706f 6e73 6520 213d 2027 6f6b   response != 'ok
+00003930: 273a 0d0a 2020 2020 2020 2020 2020 2020  ':..            
+00003940: 2020 2020 2320 2020 2020 7072 696e 7428      #     print(
+00003950: 2244 6973 7065 6e73 6520 6661 696c 6564  "Dispense failed
+00003960: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
+00003970: 2020 2020 2320 2020 2020 7265 7475 726e      #     return
+00003980: 2072 6573 706f 6e73 650d 0a20 2020 2020   response..     
+00003990: 2020 2020 2020 2020 2020 2073 7465 7073             steps
+000039a0: 5f6c 6566 7420 2d3d 2073 7465 700d 0a20  _left -= step.. 
+000039b0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+000039c0: 7572 6174 696f 6e20 3d20 7469 6d65 2e74  uration = time.t
+000039d0: 696d 6528 2920 2d20 7374 6172 745f 7469  ime() - start_ti
+000039e0: 6d65 0d0a 2020 2020 2020 2020 2020 2020  me..            
+000039f0: 2020 2020 6966 2064 7572 6174 696f 6e20      if duration 
+00003a00: 3c20 2864 656c 6179 2b6d 6f76 655f 7469  < (delay+move_ti
+00003a10: 6d65 293a 0d0a 2020 2020 2020 2020 2020  me):..          
+00003a20: 2020 2020 2020 2020 2020 7469 6d65 2e73            time.s
+00003a30: 6c65 6570 2864 656c 6179 2b6d 6f76 655f  leep(delay+move_
+00003a40: 7469 6d65 2d64 7572 6174 696f 6e29 0d0a  time-duration)..
+00003a50: 0d0a 2020 2020 2020 2020 2320 5570 6461  ..        # Upda
+00003a60: 7465 2076 616c 7565 730d 0a20 2020 2020  te values..     
+00003a70: 2020 2070 7269 6e74 2866 2744 6973 7065     print(f'Dispe
+00003a80: 6e73 6520 7469 6d65 3a20 7b74 696d 652e  nse time: {time.
+00003a90: 7469 6d65 2829 2d73 7461 7274 5f64 6973  time()-start_dis
+00003aa0: 7065 6e73 657d 7327 290d 0a20 2020 2020  pense}s')..     
+00003ab0: 2020 2074 696d 652e 736c 6565 7028 7761     time.sleep(wa
+00003ac0: 6974 290d 0a20 2020 2020 2020 2073 656c  it)..        sel
+00003ad0: 662e 7365 7446 6c61 6728 6f63 6375 7069  f.setFlag(occupi
+00003ae0: 6564 3d46 616c 7365 2c20 7061 7573 655f  ed=False, pause_
+00003af0: 6665 6564 6261 636b 3d46 616c 7365 290d  feedback=False).
+00003b00: 0a20 2020 2020 2020 2073 656c 662e 766f  .        self.vo
+00003b10: 6c75 6d65 203d 206d 6178 2873 656c 662e  lume = max(self.
+00003b20: 766f 6c75 6d65 202d 2076 6f6c 756d 652c  volume - volume,
+00003b30: 2030 290d 0a20 2020 2020 2020 2073 656c   0)..        sel
+00003b40: 662e 706f 7369 7469 6f6e 202d 3d20 7374  f.position -= st
+00003b50: 6570 730d 0a20 2020 2020 2020 2069 6620  eps..        if 
+00003b60: 7365 6c66 2e76 6f6c 756d 6520 3d3d 2030  self.volume == 0
+00003b70: 2061 6e64 2062 6c6f 776f 7574 3a0d 0a20   and blowout:.. 
+00003b80: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00003b90: 626c 6f77 6f75 7428 686f 6d65 3d62 6c6f  blowout(home=blo
+00003ba0: 776f 7574 5f68 6f6d 6529 0d0a 2020 2020  wout_home)..    
+00003bb0: 2020 2020 6966 2070 6175 7365 3a0d 0a20      if pause:.. 
+00003bc0: 2020 2020 2020 2020 2020 2069 6e70 7574             input
+00003bd0: 2822 5072 6573 7320 2745 6e74 6572 2720  ("Press 'Enter' 
+00003be0: 746f 2070 726f 6365 6564 2e22 290d 0a20  to proceed.").. 
+00003bf0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+00003c00: 7370 6f6e 7365 0d0a 2020 2020 0d0a 2020  sponse..    ..  
+00003c10: 2020 6465 6620 656a 6563 7428 7365 6c66    def eject(self
+00003c20: 2c20 686f 6d65 3a62 6f6f 6c20 3d20 5472  , home:bool = Tr
+00003c30: 7565 2920 2d3e 2073 7472 3a0d 0a20 2020  ue) -> str:..   
+00003c40: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+00003c50: 2020 456a 6563 7420 7468 6520 7069 7065    Eject the pipe
+00003c60: 7474 6520 7469 700d 0a0d 0a20 2020 2020  tte tip....     
+00003c70: 2020 2041 7267 733a 0d0a 2020 2020 2020     Args:..      
+00003c80: 2020 2020 2020 686f 6d65 2028 626f 6f6c        home (bool
+00003c90: 2c20 6f70 7469 6f6e 616c 293a 2077 6865  , optional): whe
+00003ca0: 7468 6572 2074 6f20 7265 7475 726e 2070  ther to return p
+00003cb0: 6c75 6e67 6572 2074 6f20 686f 6d65 2070  lunger to home p
+00003cc0: 6f73 6974 696f 6e2e 2044 6566 6175 6c74  osition. Default
+00003cd0: 7320 746f 2054 7275 652e 0d0a 0d0a 2020  s to True.....  
+00003ce0: 2020 2020 2020 5265 7475 726e 733a 0d0a        Returns:..
+00003cf0: 2020 2020 2020 2020 2020 2020 7374 723a              str:
+00003d00: 2064 6576 6963 6520 7265 7370 6f6e 7365   device response
+00003d10: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+00003d20: 2020 2020 2020 2073 656c 662e 7265 6167         self.reag
+00003d30: 656e 7420 3d20 2727 0d0a 2020 2020 2020  ent = ''..      
+00003d40: 2020 636f 6d6d 616e 6420 3d20 6627 5245    command = f'RE
+00003d50: 7b73 656c 662e 686f 6d65 5f70 6f73 6974  {self.home_posit
+00003d60: 696f 6e7d 2720 6966 2068 6f6d 6520 656c  ion}' if home el
+00003d70: 7365 2027 5245 270d 0a20 2020 2020 2020  se 'RE'..       
+00003d80: 2072 6573 706f 6e73 6520 3d20 7365 6c66   response = self
+00003d90: 2e5f 7175 6572 7928 636f 6d6d 616e 6429  ._query(command)
+00003da0: 0d0a 2020 2020 2020 2020 7365 6c66 2e70  ..        self.p
+00003db0: 6f73 6974 696f 6e20 3d20 7365 6c66 2e68  osition = self.h
+00003dc0: 6f6d 655f 706f 7369 7469 6f6e 2069 6620  ome_position if 
+00003dd0: 686f 6d65 2065 6c73 6520 300d 0a20 2020  home else 0..   
+00003de0: 2020 2020 2074 696d 652e 736c 6565 7028       time.sleep(
+00003df0: 3129 0d0a 2020 2020 2020 2020 7265 7475  1)..        retu
+00003e00: 726e 2072 6573 706f 6e73 650d 0a20 2020  rn response..   
+00003e10: 200d 0a20 2020 2064 6566 2065 6d70 7479   ..    def empty
+00003e20: 2873 656c 662c 202a 2a6b 7761 7267 7329  (self, **kwargs)
+00003e30: 3a0d 0a20 2020 2020 2020 2022 2222 456d  :..        """Em
+00003e40: 7074 7920 7468 6520 7069 7065 7474 6522  pty the pipette"
+00003e50: 2222 0d0a 2020 2020 2020 2020 7265 7475  ""..        retu
+00003e60: 726e 2073 656c 662e 686f 6d65 2829 0d0a  rn self.home()..
+00003e70: 2020 2020 0d0a 2020 2020 6465 6620 6765      ..    def ge
+00003e80: 7443 6170 6163 6974 616e 6365 2873 656c  tCapacitance(sel
+00003e90: 6629 202d 3e20 556e 696f 6e5b 696e 742c  f) -> Union[int,
+00003ea0: 2073 7472 5d3a 0d0a 2020 2020 2020 2020   str]:..        
+00003eb0: 2222 220d 0a20 2020 2020 2020 2047 6574  """..        Get
+00003ec0: 2074 6865 2063 6170 6163 6974 616e 6365   the capacitance
+00003ed0: 2061 7320 6d65 6173 7572 6564 2061 7420   as measured at 
+00003ee0: 7468 6520 656e 6420 6f66 2074 6865 2070  the end of the p
+00003ef0: 6970 6574 7465 0d0a 2020 2020 2020 2020  ipette..        
+00003f00: 0d0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+00003f10: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00003f20: 556e 696f 6e5b 696e 742c 2073 7472 5d3a  Union[int, str]:
+00003f30: 2063 6170 6163 6974 616e 6365 2076 616c   capacitance val
+00003f40: 7565 2c20 6f72 2064 6576 6963 6520 7265  ue, or device re
+00003f50: 7370 6f6e 7365 0d0a 2020 2020 2020 2020  sponse..        
+00003f60: 2222 220d 0a20 2020 2020 2020 2072 6573  """..        res
+00003f70: 706f 6e73 6520 3d20 7365 6c66 2e5f 7175  ponse = self._qu
+00003f80: 6572 7928 2744 4e27 290d 0a20 2020 2020  ery('DN')..     
+00003f90: 2020 2074 7279 3a0d 0a20 2020 2020 2020     try:..       
+00003fa0: 2020 2020 2063 6170 6163 6974 616e 6365       capacitance
+00003fb0: 203d 2069 6e74 2872 6573 706f 6e73 6529   = int(response)
+00003fc0: 0d0a 2020 2020 2020 2020 6578 6365 7074  ..        except
+00003fd0: 2056 616c 7565 4572 726f 723a 0d0a 2020   ValueError:..  
+00003fe0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00003ff0: 2072 6573 706f 6e73 650d 0a20 2020 2020   response..     
+00004000: 2020 2073 656c 662e 5f63 6170 6163 6974     self._capacit
+00004010: 616e 6365 203d 2063 6170 6163 6974 616e  ance = capacitan
+00004020: 6365 0d0a 2020 2020 2020 2020 7265 7475  ce..        retu
+00004030: 726e 2063 6170 6163 6974 616e 6365 0d0a  rn capacitance..
+00004040: 200d 0a20 2020 2064 6566 2067 6574 4572   ..    def getEr
+00004050: 726f 7273 2873 656c 6629 202d 3e20 7374  rors(self) -> st
+00004060: 723a 0d0a 2020 2020 2020 2020 2222 220d  r:..        """.
+00004070: 0a20 2020 2020 2020 2047 6574 2065 7272  .        Get err
+00004080: 6f72 7320 6672 6f6d 2074 6865 2064 6576  ors from the dev
+00004090: 6963 650d 0a0d 0a20 2020 2020 2020 2052  ice....        R
+000040a0: 6574 7572 6e73 3a0d 0a20 2020 2020 2020  eturns:..       
+000040b0: 2020 2020 2073 7472 3a20 6465 7669 6365       str: device
+000040c0: 2072 6573 706f 6e73 650d 0a20 2020 2020   response..     
+000040d0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+000040e0: 7265 7475 726e 2073 656c 662e 5f71 7565  return self._que
+000040f0: 7279 2827 4445 2729 0d0a 2020 2020 0d0a  ry('DE')..    ..
+00004100: 2020 2020 6465 6620 6765 7449 6e66 6f28      def getInfo(
+00004110: 7365 6c66 2c20 6d6f 6465 6c3a 204f 7074  self, model: Opt
+00004120: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+00004130: 6529 3a0d 0a20 2020 2020 2020 2022 2222  e):..        """
+00004140: 4765 7420 6465 7461 696c 7320 6f66 2074  Get details of t
+00004150: 6865 2053 6172 746f 7269 7573 2070 6970  he Sartorius pip
+00004160: 6574 7465 206d 6f64 656c 2222 220d 0a20  ette model""".. 
+00004170: 2020 2020 2020 206d 6f64 656c 203d 2073         model = s
+00004180: 656c 662e 5f5f 6d6f 6465 6c5f 5f28 292e  elf.__model__().
+00004190: 7370 6c69 7428 272d 2729 5b30 5d20 6966  split('-')[0] if
+000041a0: 206d 6f64 656c 2069 7320 4e6f 6e65 2065   model is None e
+000041b0: 6c73 6520 6d6f 6465 6c0d 0a20 2020 2020  lse model..     
+000041c0: 2020 2069 6620 6d6f 6465 6c20 6e6f 7420     if model not 
+000041d0: 696e 204d 6f64 656c 496e 666f 2e5f 6d65  in ModelInfo._me
+000041e0: 6d62 6572 5f6e 616d 6573 5f3a 0d0a 2020  mber_names_:..  
+000041f0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+00004200: 6627 5265 6365 6976 6564 3a20 7b6d 6f64  f'Received: {mod
+00004210: 656c 7d27 290d 0a20 2020 2020 2020 2020  el}')..         
+00004220: 2020 206d 6f64 656c 203d 2027 4252 4c30     model = 'BRL0
+00004230: 270d 0a20 2020 2020 2020 2020 2020 2070  '..            p
+00004240: 7269 6e74 2866 2244 6566 6175 6c74 696e  rint(f"Defaultin
+00004250: 6720 746f 3a20 7b27 4252 4c30 277d 2229  g to: {'BRL0'}")
+00004260: 0d0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
+00004270: 696e 7428 6622 5661 6c69 6420 6d6f 6465  int(f"Valid mode
+00004280: 6c73 2061 7265 3a20 7b27 2c20 272e 6a6f  ls are: {', '.jo
+00004290: 696e 284d 6f64 656c 496e 666f 2e5f 6d65  in(ModelInfo._me
+000042a0: 6d62 6572 5f6e 616d 6573 5f29 7d22 290d  mber_names_)}").
+000042b0: 0a20 2020 2020 2020 2069 6e66 6f3a 204d  .        info: M
+000042c0: 6f64 656c 203d 204d 6f64 656c 496e 666f  odel = ModelInfo
+000042d0: 5b6d 6f64 656c 5d2e 7661 6c75 650d 0a20  [model].value.. 
+000042e0: 2020 2020 2020 2070 7269 6e74 2869 6e66         print(inf
+000042f0: 6f29 0d0a 2020 2020 2020 2020 7365 6c66  o)..        self
+00004300: 2e6d 6f64 656c 5f69 6e66 6f20 3d20 696e  .model_info = in
+00004310: 666f 0d0a 2020 2020 2020 2020 7365 6c66  fo..        self
+00004320: 2e63 6170 6163 6974 7920 3d20 696e 666f  .capacity = info
+00004330: 2e63 6170 6163 6974 790d 0a20 2020 2020  .capacity..     
+00004340: 2020 2073 656c 662e 6c69 6d69 7473 203d     self.limits =
+00004350: 2028 696e 666f 2e74 6970 5f65 6a65 6374   (info.tip_eject
+00004360: 5f70 6f73 6974 696f 6e2c 2069 6e66 6f2e  _position, info.
+00004370: 6d61 785f 706f 7369 7469 6f6e 290d 0a20  max_position).. 
+00004380: 2020 2020 2020 2073 656c 662e 7370 6565         self.spee
+00004390: 645f 7072 6573 6574 7320 3d20 696e 666f  d_presets = info
+000043a0: 2e70 7265 7365 745f 7370 6565 6473 0d0a  .preset_speeds..
+000043b0: 2020 2020 2020 2020 7365 6c66 2e73 7065          self.spe
+000043c0: 6564 2e75 7020 3d20 7365 6c66 2e73 7065  ed.up = self.spe
+000043d0: 6564 5f70 7265 7365 7473 5b73 656c 662e  ed_presets[self.
+000043e0: 7370 6565 645f 636f 6465 2e75 705d 0d0a  speed_code.up]..
+000043f0: 2020 2020 2020 2020 7365 6c66 2e73 7065          self.spe
+00004400: 6564 2e64 6f77 6e20 3d20 7365 6c66 2e73  ed.down = self.s
+00004410: 7065 6564 5f70 7265 7365 7473 5b73 656c  peed_presets[sel
+00004420: 662e 7370 6565 645f 636f 6465 2e64 6f77  f.speed_code.dow
+00004430: 6e5d 0d0a 2020 2020 2020 2020 7265 7475  n]..        retu
+00004440: 726e 0d0a 2020 2020 0d0a 2020 2020 6465  rn..    ..    de
+00004450: 6620 6765 7450 6f73 6974 696f 6e28 7365  f getPosition(se
+00004460: 6c66 2c20 2a2a 6b77 6172 6773 2920 2d3e  lf, **kwargs) ->
+00004470: 2069 6e74 3a0d 0a20 2020 2020 2020 2022   int:..        "
+00004480: 2222 4765 7420 7468 6520 6375 7272 656e  ""Get the curren
+00004490: 7420 706f 7369 7469 6f6e 206f 6620 7468  t position of th
+000044a0: 6520 7069 7065 7474 6522 2222 0d0a 2020  e pipette"""..  
+000044b0: 2020 2020 2020 7265 7370 6f6e 7365 203d        response =
+000044c0: 2073 656c 662e 5f71 7565 7279 2827 4450   self._query('DP
+000044d0: 2729 0d0a 2020 2020 2020 2020 7472 793a  ')..        try:
+000044e0: 0d0a 2020 2020 2020 2020 2020 2020 706f  ..            po
+000044f0: 7369 7469 6f6e 203d 2069 6e74 2872 6573  sition = int(res
+00004500: 706f 6e73 6529 0d0a 2020 2020 2020 2020  ponse)..        
+00004510: 6578 6365 7074 2056 616c 7565 4572 726f  except ValueErro
+00004520: 723a 0d0a 2020 2020 2020 2020 2020 2020  r:..            
+00004530: 7265 7475 726e 2072 6573 706f 6e73 650d  return response.
+00004540: 0a20 2020 2020 2020 2073 656c 662e 706f  .        self.po
+00004550: 7369 7469 6f6e 203d 2070 6f73 6974 696f  sition = positio
+00004560: 6e0d 0a20 2020 2020 2020 2072 6574 7572  n..        retur
+00004570: 6e20 7365 6c66 2e70 6f73 6974 696f 6e0d  n self.position.
+00004580: 0a20 2020 2020 200d 0a20 2020 2064 6566  .      ..    def
+00004590: 2067 6574 5374 6174 7573 2873 656c 662c   getStatus(self,
+000045a0: 202a 2a6b 7761 7267 7329 202d 3e20 7374   **kwargs) -> st
+000045b0: 723a 0d0a 2020 2020 2020 2020 2222 220d  r:..        """.
+000045c0: 0a20 2020 2020 2020 2047 6574 2074 6865  .        Get the
+000045d0: 2073 7461 7475 7320 6f66 2074 6865 2070   status of the p
+000045e0: 6970 6574 7465 0d0a 0d0a 2020 2020 2020  ipette....      
+000045f0: 2020 5265 7475 726e 733a 0d0a 2020 2020    Returns:..    
+00004600: 2020 2020 2020 2020 7374 723a 2064 6576          str: dev
+00004610: 6963 6520 7265 7370 6f6e 7365 0d0a 2020  ice response..  
+00004620: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+00004630: 2020 2072 6573 706f 6e73 6520 3d20 7365     response = se
+00004640: 6c66 2e5f 7175 6572 7928 2744 5327 290d  lf._query('DS').
+00004650: 0a20 2020 2020 2020 2074 7279 3a0d 0a20  .        try:.. 
+00004660: 2020 2020 2020 2020 2020 2073 7461 7475             statu
+00004670: 7320 3d20 696e 7428 7265 7370 6f6e 7365  s = int(response
+00004680: 290d 0a20 2020 2020 2020 2065 7863 6570  )..        excep
+00004690: 7420 5661 6c75 6545 7272 6f72 3a0d 0a20  t ValueError:.. 
+000046a0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000046b0: 6e20 7265 7370 6f6e 7365 0d0a 2020 2020  n response..    
+000046c0: 2020 2020 6966 2072 6573 706f 6e73 6520      if response 
+000046d0: 6e6f 7420 696e 205b 5f73 7461 7475 732e  not in [_status.
+000046e0: 7661 6c75 6520 666f 7220 5f73 7461 7475  value for _statu
+000046f0: 7320 696e 2053 7461 7475 7343 6f64 655d  s in StatusCode]
+00004700: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
+00004710: 6574 7572 6e20 7265 7370 6f6e 7365 0d0a  eturn response..
+00004720: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00004730: 2020 7365 6c66 2e5f 7374 6174 7573 5f63    self._status_c
+00004740: 6f64 6520 3d20 7374 6174 7573 0d0a 2020  ode = status..  
+00004750: 2020 2020 2020 6966 2073 7461 7475 7320        if status 
+00004760: 696e 205b 342c 362c 385d 3a0d 0a20 2020  in [4,6,8]:..   
+00004770: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
+00004780: 7446 6c61 6728 6275 7379 3d54 7275 6529  tFlag(busy=True)
+00004790: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+000047a0: 2073 656c 662e 7665 7262 6f73 653a 0d0a   self.verbose:..
+000047b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000047c0: 7072 696e 7428 5374 6174 7573 436f 6465  print(StatusCode
+000047d0: 2873 7461 7475 7329 2e6e 616d 6529 0d0a  (status).name)..
+000047e0: 2020 2020 2020 2020 656c 6966 2073 7461          elif sta
+000047f0: 7475 7320 3d3d 2030 3a0d 0a20 2020 2020  tus == 0:..     
+00004800: 2020 2020 2020 2073 656c 662e 7365 7446         self.setF
+00004810: 6c61 6728 6275 7379 3d46 616c 7365 290d  lag(busy=False).
+00004820: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00004830: 5374 6174 7573 436f 6465 2873 656c 662e  StatusCode(self.
+00004840: 5f73 7461 7475 735f 636f 6465 292e 6e61  _status_code).na
+00004850: 6d65 0d0a 2020 2020 0d0a 2020 2020 6465  me..    ..    de
+00004860: 6620 686f 6d65 2873 656c 6629 202d 3e20  f home(self) -> 
+00004870: 7374 723a 0d0a 2020 2020 2020 2020 2222  str:..        ""
+00004880: 220d 0a20 2020 2020 2020 2052 6574 7572  "..        Retur
+00004890: 6e20 706c 756e 6765 7220 746f 2068 6f6d  n plunger to hom
+000048a0: 6520 706f 7369 7469 6f6e 0d0a 2020 2020  e position..    
+000048b0: 2020 2020 0d0a 2020 2020 2020 2020 5265      ..        Re
+000048c0: 7475 726e 733a 0d0a 2020 2020 2020 2020  turns:..        
+000048d0: 2020 2020 7374 723a 2064 6576 6963 6520      str: device 
+000048e0: 7265 7370 6f6e 7365 0d0a 2020 2020 2020  response..      
+000048f0: 2020 2222 220d 0a20 2020 2020 2020 2072    """..        r
+00004900: 6573 706f 6e73 6520 3d20 7365 6c66 2e5f  esponse = self._
+00004910: 7175 6572 7928 6627 5250 7b73 656c 662e  query(f'RP{self.
+00004920: 686f 6d65 5f70 6f73 6974 696f 6e7d 2729  home_position}')
+00004930: 0d0a 2020 2020 2020 2020 7365 6c66 2e76  ..        self.v
+00004940: 6f6c 756d 6520 3d20 300d 0a20 2020 2020  olume = 0..     
+00004950: 2020 2073 656c 662e 706f 7369 7469 6f6e     self.position
+00004960: 203d 2073 656c 662e 686f 6d65 5f70 6f73   = self.home_pos
+00004970: 6974 696f 6e0d 0a20 2020 2020 2020 2074  ition..        t
+00004980: 696d 652e 736c 6565 7028 3129 0d0a 2020  ime.sleep(1)..  
+00004990: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+000049a0: 706f 6e73 650d 0a20 2020 200d 0a20 2020  ponse..    ..   
+000049b0: 2064 6566 2069 7346 6561 7369 626c 6528   def isFeasible(
+000049c0: 7365 6c66 2c20 706f 7369 7469 6f6e 3a69  self, position:i
+000049d0: 6e74 2920 2d3e 2062 6f6f 6c3a 0d0a 2020  nt) -> bool:..  
+000049e0: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+000049f0: 2020 2043 6865 636b 7320 616e 6420 7265     Checks and re
+00004a00: 7475 726e 7320 7768 6574 6865 7220 7468  turns whether th
+00004a10: 6520 706c 756e 6765 7220 706f 7369 7469  e plunger positi
+00004a20: 6f6e 2069 7320 6665 6173 6962 6c65 0d0a  on is feasible..
+00004a30: 0d0a 2020 2020 2020 2020 4172 6773 3a0d  ..        Args:.
+00004a40: 0a20 2020 2020 2020 2020 2020 2070 6f73  .            pos
+00004a50: 6974 696f 6e20 2869 6e74 293a 2070 6c75  ition (int): plu
+00004a60: 6e67 6572 2070 6f73 6974 696f 6e0d 0a0d  nger position...
+00004a70: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+00004a80: 3a0d 0a20 2020 2020 2020 2020 2020 2062  :..            b
+00004a90: 6f6f 6c3a 2077 6865 7468 6572 2070 6c75  ool: whether plu
+00004aa0: 6e67 6572 2070 6f73 6974 696f 6e20 6973  nger position is
+00004ab0: 2066 6561 7369 626c 650d 0a20 2020 2020   feasible..     
+00004ac0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+00004ad0: 6966 2028 7365 6c66 2e6c 696d 6974 735b  if (self.limits[
+00004ae0: 305d 203c 3d20 706f 7369 7469 6f6e 203c  0] <= position <
+00004af0: 3d20 7365 6c66 2e6c 696d 6974 735b 315d  = self.limits[1]
+00004b00: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00004b10: 7265 7475 726e 2054 7275 650d 0a20 2020  return True..   
+00004b20: 2020 2020 2070 7269 6e74 2866 2252 616e       print(f"Ran
+00004b30: 6765 206c 696d 6974 7320 7265 6163 6865  ge limits reache
+00004b40: 6421 207b 7365 6c66 2e6c 696d 6974 737d  d! {self.limits}
+00004b50: 2229 0d0a 2020 2020 2020 2020 7265 7475  ")..        retu
+00004b60: 726e 2046 616c 7365 0d0a 2020 2020 0d0a  rn False..    ..
+00004b70: 2020 2020 6465 6620 6973 5469 704f 6e28      def isTipOn(
+00004b80: 7365 6c66 2920 2d3e 2062 6f6f 6c3a 0d0a  self) -> bool:..
+00004b90: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+00004ba0: 2020 2020 2043 6865 636b 7320 616e 6420       Checks and 
+00004bb0: 7265 7475 726e 7320 7768 6574 6865 7220  returns whether 
+00004bc0: 6120 7069 7065 7474 6520 7469 7020 6973  a pipette tip is
+00004bd0: 2061 7474 6163 6865 640d 0a20 2020 2020   attached..     
+00004be0: 2020 200d 0a20 2020 2020 2020 2052 6574     ..        Ret
+00004bf0: 7572 6e73 3a0d 0a20 2020 2020 2020 2020  urns:..         
+00004c00: 2020 2062 6f6f 6c3a 2077 6865 7468 6572     bool: whether
+00004c10: 2061 2070 6970 6574 7465 2074 6970 2069   a pipette tip i
+00004c20: 6e20 6174 7461 6368 6564 0d0a 2020 2020  n attached..    
+00004c30: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+00004c40: 2073 656c 662e 6765 7443 6170 6163 6974   self.getCapacit
+00004c50: 616e 6365 2829 0d0a 2020 2020 2020 2020  ance()..        
+00004c60: 7072 696e 7428 6627 5469 7020 6361 7061  print(f'Tip capa
+00004c70: 6369 7461 6e63 653a 207b 7365 6c66 2e63  citance: {self.c
+00004c80: 6170 6163 6974 616e 6365 7d27 290d 0a20  apacitance}').. 
+00004c90: 2020 2020 2020 2069 6620 7365 6c66 2e66         if self.f
+00004ca0: 6c61 6773 5b27 636f 6e64 7563 7469 7665  lags['conductive
+00004cb0: 5f74 6970 7327 5d3a 0d0a 2020 2020 2020  _tips']:..      
+00004cc0: 2020 2020 2020 7469 705f 6f6e 203d 2028        tip_on = (
+00004cd0: 7365 6c66 2e63 6170 6163 6974 616e 6365  self.capacitance
+00004ce0: 203e 2073 656c 662e 7469 705f 7468 7265   > self.tip_thre
+00004cf0: 7368 6f6c 6429 0d0a 2020 2020 2020 2020  shold)..        
+00004d00: 2020 2020 7365 6c66 2e73 6574 466c 6167      self.setFlag
+00004d10: 2874 6970 5f6f 6e3d 7469 705f 6f6e 290d  (tip_on=tip_on).
+00004d20: 0a20 2020 2020 2020 2074 6970 5f6f 6e20  .        tip_on 
+00004d30: 3d20 7365 6c66 2e66 6c61 6773 5b27 7469  = self.flags['ti
+00004d40: 705f 6f6e 275d 0d0a 2020 2020 2020 2020  p_on']..        
+00004d50: 7265 7475 726e 2074 6970 5f6f 6e0d 0a20  return tip_on.. 
+00004d60: 2020 200d 0a20 2020 2064 6566 206d 6f76     ..    def mov
+00004d70: 6528 7365 6c66 2c20 7374 6570 733a 696e  e(self, steps:in
+00004d80: 742c 2075 703a 626f 6f6c 2c20 2a2a 6b77  t, up:bool, **kw
+00004d90: 6172 6773 2920 2d3e 2073 7472 3a0d 0a20  args) -> str:.. 
+00004da0: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+00004db0: 2020 2020 4d6f 7665 2074 6865 2070 6c75      Move the plu
+00004dc0: 6e67 6572 2065 6974 6865 7220 7570 206f  nger either up o
+00004dd0: 7220 646f 776e 2062 7920 6120 7370 6563  r down by a spec
+00004de0: 6966 6965 6420 6e75 6d62 6572 206f 6620  ified number of 
+00004df0: 7374 6570 730d 0a0d 0a20 2020 2020 2020  steps....       
+00004e00: 2041 7267 733a 0d0a 2020 2020 2020 2020   Args:..        
+00004e10: 2020 2020 7374 6570 7320 2869 6e74 293a      steps (int):
+00004e20: 206e 756d 6265 7220 6f66 2073 7465 7073   number of steps
+00004e30: 2074 6f20 6d6f 7665 2070 6c75 6e67 6572   to move plunger
+00004e40: 2062 790d 0a20 2020 2020 2020 2020 2020   by..           
+00004e50: 2075 7020 2862 6f6f 6c29 3a20 7768 6574   up (bool): whet
+00004e60: 6865 7220 746f 206d 6f76 6520 7468 6520  her to move the 
+00004e70: 706c 756e 6765 7220 7570 0d0a 0d0a 2020  plunger up....  
+00004e80: 2020 2020 2020 5265 7475 726e 733a 0d0a        Returns:..
+00004e90: 2020 2020 2020 2020 2020 2020 7374 723a              str:
+00004ea0: 2064 6576 6963 6520 7265 7370 6f6e 7365   device response
+00004eb0: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+00004ec0: 2020 2020 2020 2073 7465 7073 203d 2061         steps = a
+00004ed0: 6273 2873 7465 7073 2920 6966 2075 7020  bs(steps) if up 
+00004ee0: 656c 7365 202d 6162 7328 7374 6570 7329  else -abs(steps)
+00004ef0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00004f00: 2073 656c 662e 6d6f 7665 4279 2873 7465   self.moveBy(ste
+00004f10: 7073 290d 0a20 2020 200d 0a20 2020 2064  ps)..    ..    d
+00004f20: 6566 206d 6f76 6542 7928 7365 6c66 2c20  ef moveBy(self, 
+00004f30: 7374 6570 733a 696e 742c 202a 2a6b 7761  steps:int, **kwa
+00004f40: 7267 7329 202d 3e20 7374 723a 0d0a 2020  rgs) -> str:..  
+00004f50: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+00004f60: 2020 204d 6f76 6520 7468 6520 706c 756e     Move the plun
+00004f70: 6765 7220 6279 2073 7065 6369 6669 6564  ger by specified
+00004f80: 206e 756d 6265 7220 6f66 2073 7465 7073   number of steps
+00004f90: 0d0a 0d0a 2020 2020 2020 2020 4172 6773  ....        Args
+00004fa0: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
+00004fb0: 7465 7073 2028 696e 7429 3a20 6e75 6d62  teps (int): numb
+00004fc0: 6572 206f 6620 7374 6570 7320 746f 206d  er of steps to m
+00004fd0: 6f76 6520 706c 756e 6765 7220 6279 2028  ove plunger by (
+00004fe0: 3c30 3a20 6d6f 7665 2064 6f77 6e2f 6469  <0: move down/di
+00004ff0: 7370 656e 7365 3b20 3e30 206d 6f76 6520  spense; >0 move 
+00005000: 7570 2f61 7370 6972 6174 6529 0d0a 0d0a  up/aspirate)....
+00005010: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
+00005020: 0d0a 2020 2020 2020 2020 2020 2020 7374  ..            st
+00005030: 723a 2064 6576 6963 6520 7265 7370 6f6e  r: device respon
+00005040: 7365 0d0a 2020 2020 2020 2020 2222 220d  se..        """.
+00005050: 0a20 2020 2020 2020 2063 6f6d 6d61 6e64  .        command
+00005060: 203d 2066 2752 497b 7374 6570 737d 2720   = f'RI{steps}' 
+00005070: 6966 2073 7465 7073 203e 2030 2065 6c73  if steps > 0 els
+00005080: 6520 6627 524f 7b2d 7374 6570 737d 270d  e f'RO{-steps}'.
+00005090: 0a20 2020 2020 2020 2073 656c 662e 706f  .        self.po
+000050a0: 7369 7469 6f6e 202b 3d20 7374 6570 730d  sition += steps.
+000050b0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000050c0: 7365 6c66 2e5f 7175 6572 7928 636f 6d6d  self._query(comm
+000050d0: 616e 6429 0d0a 2020 2020 0d0a 2020 2020  and)..    ..    
+000050e0: 6465 6620 6d6f 7665 546f 2873 656c 662c  def moveTo(self,
+000050f0: 2070 6f73 6974 696f 6e3a 696e 742c 202a   position:int, *
+00005100: 2a6b 7761 7267 7329 202d 3e20 7374 723a  *kwargs) -> str:
+00005110: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+00005120: 2020 2020 2020 204d 6f76 6520 7468 6520         Move the 
+00005130: 706c 756e 6765 7220 746f 2061 2073 7065  plunger to a spe
+00005140: 6369 6669 6564 2070 6f73 6974 696f 6e0d  cified position.
+00005150: 0a0d 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
+00005160: 0d0a 2020 2020 2020 2020 2020 2020 706f  ..            po
+00005170: 7369 7469 6f6e 2028 696e 7429 3a20 7461  sition (int): ta
+00005180: 7267 6574 2070 6c75 6e67 6572 2070 6f73  rget plunger pos
+00005190: 6974 696f 6e0d 0a0d 0a20 2020 2020 2020  ition....       
+000051a0: 2052 6574 7572 6e73 3a0d 0a20 2020 2020   Returns:..     
+000051b0: 2020 2020 2020 2073 7472 3a20 6465 7669         str: devi
+000051c0: 6365 2072 6573 706f 6e73 650d 0a20 2020  ce response..   
+000051d0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+000051e0: 2020 7365 6c66 2e70 6f73 6974 696f 6e20    self.position 
+000051f0: 3d20 706f 7369 7469 6f6e 0d0a 2020 2020  = position..    
+00005200: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00005210: 5f71 7565 7279 2866 2752 507b 706f 7369  _query(f'RP{posi
+00005220: 7469 6f6e 7d27 290d 0a20 2020 200d 0a20  tion}')..    .. 
+00005230: 2020 2064 6566 2070 756c 6c62 6163 6b28     def pullback(
+00005240: 7365 6c66 2c20 7374 6570 733a 696e 7420  self, steps:int 
+00005250: 3d20 352c 202a 2a6b 7761 7267 7329 202d  = 5, **kwargs) -
+00005260: 3e20 7374 723a 0d0a 2020 2020 2020 2020  > str:..        
+00005270: 2222 220d 0a20 2020 2020 2020 2050 756c  """..        Pul
+00005280: 6c62 6163 6b20 6c69 7175 6964 2066 726f  lback liquid fro
+00005290: 6d20 7469 700d 0a20 2020 2020 2020 200d  m tip..        .
+000052a0: 0a20 2020 2020 2020 2041 7267 733a 0d0a  .        Args:..
+000052b0: 2020 2020 2020 2020 2020 2020 7374 6570              step
+000052c0: 7320 2869 6e74 2c20 6f70 7469 6f6e 616c  s (int, optional
+000052d0: 293a 206e 756d 6265 7220 6f66 2073 7465  ): number of ste
+000052e0: 7073 2074 6f20 7075 6c6c 6261 636b 2e20  ps to pullback. 
+000052f0: 4465 6661 756c 7473 2074 6f20 352e 0d0a  Defaults to 5...
+00005300: 0d0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+00005310: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00005320: 7374 723a 2064 6576 6963 6520 7265 7370  str: device resp
+00005330: 6f6e 7365 0d0a 2020 2020 2020 2020 2222  onse..        ""
+00005340: 220d 0a20 2020 2020 2020 2072 6573 706f  "..        respo
+00005350: 6e73 6520 3d20 7365 6c66 2e5f 7175 6572  nse = self._quer
+00005360: 7928 6627 5249 7b73 7465 7073 7d27 290d  y(f'RI{steps}').
+00005370: 0a20 2020 2020 2020 2073 656c 662e 706f  .        self.po
+00005380: 7369 7469 6f6e 202b 3d20 7374 6570 730d  sition += steps.
+00005390: 0a20 2020 2020 2020 2074 696d 652e 736c  .        time.sl
+000053a0: 6565 7028 3129 0d0a 2020 2020 2020 2020  eep(1)..        
+000053b0: 7265 7475 726e 2072 6573 706f 6e73 650d  return response.
+000053c0: 0a20 2020 200d 0a20 2020 2064 6566 2072  .    ..    def r
+000053d0: 6573 6574 2873 656c 6629 202d 3e20 7374  eset(self) -> st
+000053e0: 723a 0d0a 2020 2020 2020 2020 2222 220d  r:..        """.
+000053f0: 0a20 2020 2020 2020 2052 6573 6574 2074  .        Reset t
+00005400: 6865 2070 6970 6574 7465 0d0a 0d0a 2020  he pipette....  
+00005410: 2020 2020 2020 5265 7475 726e 733a 0d0a        Returns:..
+00005420: 2020 2020 2020 2020 2020 2020 7374 723a              str:
+00005430: 2064 6576 6963 6520 7265 7370 6f6e 7365   device response
+00005440: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+00005450: 2020 2020 2020 2073 656c 662e 7a65 726f         self.zero
+00005460: 2829 0d0a 2020 2020 2020 2020 7265 7475  ()..        retu
+00005470: 726e 2073 656c 662e 686f 6d65 2829 0d0a  rn self.home()..
+00005480: 2020 2020 0d0a 2020 2020 6465 6620 7365      ..    def se
+00005490: 7453 7065 6564 2873 656c 662c 2073 7065  tSpeed(self, spe
+000054a0: 6564 3a69 6e74 2c20 7570 3a62 6f6f 6c2c  ed:int, up:bool,
+000054b0: 202a 2a6b 7761 7267 7329 202d 3e20 7374   **kwargs) -> st
+000054c0: 723a 0d0a 2020 2020 2020 2020 2222 220d  r:..        """.
+000054d0: 0a20 2020 2020 2020 2053 6574 2074 6865  .        Set the
+000054e0: 2073 7065 6564 206f 6620 7468 6520 706c   speed of the pl
+000054f0: 756e 6765 720d 0a0d 0a20 2020 2020 2020  unger....       
+00005500: 2041 7267 733a 0d0a 2020 2020 2020 2020   Args:..        
+00005510: 2020 2020 7370 6565 6420 2869 6e74 293a      speed (int):
+00005520: 2073 7065 6564 206f 6620 706c 756e 6765   speed of plunge
+00005530: 720d 0a20 2020 2020 2020 2020 2020 2075  r..            u
+00005540: 7020 2862 6f6f 6c29 3a20 6469 7265 6374  p (bool): direct
+00005550: 696f 6e20 6f66 2074 7261 7665 6c0d 0a0d  ion of travel...
+00005560: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+00005570: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
+00005580: 7472 3a20 6465 7669 6365 2072 6573 706f  tr: device respo
+00005590: 6e73 650d 0a20 2020 2020 2020 2022 2222  nse..        """
+000055a0: 0d0a 2020 2020 2020 2020 7370 6565 645f  ..        speed_
+000055b0: 636f 6465 203d 2031 202b 205b 7820 666f  code = 1 + [x fo
+000055c0: 7220 782c 7661 6c20 696e 2065 6e75 6d65  r x,val in enume
+000055d0: 7261 7465 286e 702e 6172 7261 7928 7365  rate(np.array(se
+000055e0: 6c66 2e73 7065 6564 5f70 7265 7365 7473  lf.speed_presets
+000055f0: 292d 7370 6565 6429 2069 6620 7661 6c20  )-speed) if val 
+00005600: 3e3d 2030 5d5b 305d 0d0a 2020 2020 2020  >= 0][0]..      
+00005610: 2020 7072 696e 7428 6627 5370 6565 6420    print(f'Speed 
+00005620: 7b73 7065 6564 5f63 6f64 657d 3a20 7b73  {speed_code}: {s
+00005630: 656c 662e 7370 6565 645f 7072 6573 6574  elf.speed_preset
+00005640: 735b 7370 6565 645f 636f 6465 2d31 5d7d  s[speed_code-1]}
+00005650: 2075 4c2f 7327 290d 0a20 2020 2020 2020   uL/s')..       
+00005660: 2064 6972 6563 7469 6f6e 203d 2027 4927   direction = 'I'
+00005670: 2069 6620 7570 2065 6c73 6520 274f 270d   if up else 'O'.
+00005680: 0a20 2020 2020 2020 2073 656c 662e 5f71  .        self._q
+00005690: 7565 7279 2866 2753 7b64 6972 6563 7469  uery(f'S{directi
+000056a0: 6f6e 7d7b 7370 6565 645f 636f 6465 7d27  on}{speed_code}'
+000056b0: 290d 0a20 2020 2020 2020 2069 6620 7570  )..        if up
+000056c0: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
+000056d0: 656c 662e 7370 6565 645f 636f 6465 2e75  elf.speed_code.u
+000056e0: 7020 3d20 7370 6565 645f 636f 6465 0d0a  p = speed_code..
+000056f0: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+00005700: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00005710: 7370 6565 645f 636f 6465 2e64 6f77 6e20  speed_code.down 
+00005720: 3d20 7370 6565 645f 636f 6465 0d0a 2020  = speed_code..  
+00005730: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00005740: 662e 5f71 7565 7279 2866 2744 7b64 6972  f._query(f'D{dir
+00005750: 6563 7469 6f6e 7d27 290d 0a20 2020 200d  ection}')..    .
+00005760: 0a20 2020 2064 6566 2073 6875 7464 6f77  .    def shutdow
+00005770: 6e28 7365 6c66 293a 0d0a 2020 2020 2020  n(self):..      
+00005780: 2020 2222 2253 6875 7464 6f77 6e20 7072    """Shutdown pr
+00005790: 6f63 6564 7572 6520 666f 7220 746f 6f6c  ocedure for tool
+000057a0: 2222 220d 0a20 2020 2020 2020 2073 656c  """..        sel
+000057b0: 662e 746f 6767 6c65 4665 6564 6261 636b  f.toggleFeedback
+000057c0: 4c6f 6f70 286f 6e3d 4661 6c73 6529 0d0a  Loop(on=False)..
+000057d0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+000057e0: 7570 6572 2829 2e73 6875 7464 6f77 6e28  uper().shutdown(
+000057f0: 290d 0a20 2020 200d 0a20 2020 2064 6566  )..    ..    def
+00005800: 2074 6f67 676c 6546 6565 6462 6163 6b4c   toggleFeedbackL
+00005810: 6f6f 7028 7365 6c66 2c20 6f6e 3a62 6f6f  oop(self, on:boo
+00005820: 6c29 3a0d 0a20 2020 2020 2020 2022 2222  l):..        """
+00005830: 0d0a 2020 2020 2020 2020 5374 6172 7420  ..        Start 
+00005840: 6f72 2073 746f 7020 6665 6564 6261 636b  or stop feedback
+00005850: 206c 6f6f 700d 0a20 2020 2020 2020 200d   loop..        .
+00005860: 0a20 2020 2020 2020 2041 7267 733a 0d0a  .        Args:..
+00005870: 2020 2020 2020 2020 2020 2020 6f6e 2028              on (
+00005880: 626f 6f6c 293a 2077 6865 7468 6572 2074  bool): whether t
+00005890: 6f20 7374 6172 7420 6665 6564 6261 636b  o start feedback
+000058a0: 206c 6f6f 700d 0a20 2020 2020 2020 2022   loop..        "
+000058b0: 2222 0d0a 2020 2020 2020 2020 7365 6c66  ""..        self
+000058c0: 2e73 6574 466c 6167 2867 6574 5f66 6565  .setFlag(get_fee
+000058d0: 6462 6163 6b3d 6f6e 290d 0a20 2020 2020  dback=on)..     
+000058e0: 2020 2069 6620 6f6e 3a0d 0a20 2020 2020     if on:..     
+000058f0: 2020 2020 2020 2069 6620 2766 6565 6462         if 'feedb
+00005900: 6163 6b5f 6c6f 6f70 2720 696e 2073 656c  ack_loop' in sel
+00005910: 662e 5f74 6872 6561 6473 3a0d 0a20 2020  f._threads:..   
+00005920: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00005930: 662e 5f74 6872 6561 6473 5b27 6665 6564  f._threads['feed
+00005940: 6261 636b 5f6c 6f6f 7027 5d2e 6a6f 696e  back_loop'].join
+00005950: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
+00005960: 7468 7265 6164 203d 2054 6872 6561 6428  thread = Thread(
+00005970: 7461 7267 6574 3d73 656c 662e 5f6c 6f6f  target=self._loo
+00005980: 705f 6665 6564 6261 636b 290d 0a20 2020  p_feedback)..   
+00005990: 2020 2020 2020 2020 2074 6872 6561 642e           thread.
+000059a0: 7374 6172 7428 290d 0a20 2020 2020 2020  start()..       
+000059b0: 2020 2020 2073 656c 662e 5f74 6872 6561       self._threa
+000059c0: 6473 5b27 6665 6564 6261 636b 5f6c 6f6f  ds['feedback_loo
+000059d0: 7027 5d20 3d20 7468 7265 6164 0d0a 2020  p'] = thread..  
+000059e0: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+000059f0: 2020 2020 2020 2020 2069 6620 2766 6565           if 'fee
+00005a00: 6462 6163 6b5f 6c6f 6f70 2720 696e 2073  dback_loop' in s
+00005a10: 656c 662e 5f74 6872 6561 6473 3a0d 0a20  elf._threads:.. 
+00005a20: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00005a30: 656c 662e 5f74 6872 6561 6473 5b27 6665  elf._threads['fe
+00005a40: 6564 6261 636b 5f6c 6f6f 7027 5d2e 6a6f  edback_loop'].jo
+00005a50: 696e 2829 0d0a 2020 2020 2020 2020 7265  in()..        re
+00005a60: 7475 726e 0d0a 0d0a 2020 2020 6465 6620  turn....    def 
+00005a70: 7a65 726f 2873 656c 6629 202d 3e20 7374  zero(self) -> st
+00005a80: 723a 0d0a 2020 2020 2020 2020 2222 220d  r:..        """.
+00005a90: 0a20 2020 2020 2020 205a 6572 6f20 7468  .        Zero th
+00005aa0: 6520 706c 756e 6765 7220 706f 7369 7469  e plunger positi
+00005ab0: 6f6e 0d0a 2020 2020 2020 2020 0d0a 2020  on..        ..  
+00005ac0: 2020 2020 2020 5265 7475 726e 733a 0d0a        Returns:..
+00005ad0: 2020 2020 2020 2020 2020 2020 7374 723a              str:
+00005ae0: 2064 6576 6963 6520 7265 7370 6f6e 7365   device response
+00005af0: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+00005b00: 2020 2020 2020 2073 656c 662e 656a 6563         self.ejec
+00005b10: 7428 290d 0a20 2020 2020 2020 2072 6573  t()..        res
+00005b20: 706f 6e73 6520 3d20 7365 6c66 2e5f 7175  ponse = self._qu
+00005b30: 6572 7928 2752 5a27 290d 0a20 2020 2020  ery('RZ')..     
+00005b40: 2020 2073 656c 662e 706f 7369 7469 6f6e     self.position
+00005b50: 203d 2030 0d0a 2020 2020 2020 2020 7469   = 0..        ti
+00005b60: 6d65 2e73 6c65 6570 2832 290d 0a20 2020  me.sleep(2)..   
+00005b70: 2020 2020 2072 6574 7572 6e20 7265 7370       return resp
+00005b80: 6f6e 7365 0d0a 0d0a 2020 2020 2320 5072  onse....    # Pr
+00005b90: 6f74 6563 7465 6420 6d65 7468 6f64 2873  otected method(s
+00005ba0: 290d 0a20 2020 2064 6566 205f 6361 6c63  )..    def _calc
+00005bb0: 756c 6174 655f 7370 6565 645f 7061 7261  ulate_speed_para
+00005bc0: 6d65 7465 7273 2873 656c 662c 2076 6f6c  meters(self, vol
+00005bd0: 756d 653a 696e 742c 2073 7065 6564 3a69  ume:int, speed:i
+00005be0: 6e74 2920 2d3e 2053 7065 6564 5061 7261  nt) -> SpeedPara
+00005bf0: 6d65 7465 7273 3a0d 0a20 2020 2020 2020  meters:..       
+00005c00: 2022 2222 0d0a 2020 2020 2020 2020 4361   """..        Ca
+00005c10: 6c63 756c 6174 6573 2074 6865 2062 6573  lculates the bes
+00005c20: 7420 7061 7261 6d65 7465 7273 2066 6f72  t parameters for
+00005c30: 2076 6f6c 756d 6520 616e 6420 7370 6565   volume and spee
+00005c40: 640d 0a0d 0a20 2020 2020 2020 2041 7267  d....        Arg
+00005c50: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00005c60: 766f 6c75 6d65 2028 696e 7429 3a20 766f  volume (int): vo
+00005c70: 6c75 6d65 2074 6f20 6265 2074 7261 6e73  lume to be trans
+00005c80: 6665 7272 6564 0d0a 2020 2020 2020 2020  ferred..        
+00005c90: 2020 2020 7370 6565 6420 2869 6e74 293a      speed (int):
+00005ca0: 2073 7065 6564 2061 7420 7768 6963 6820   speed at which 
+00005cb0: 6c69 7175 6964 2069 7320 7472 616e 7366  liquid is transf
+00005cc0: 6572 7265 640d 0a0d 0a20 2020 2020 2020  erred....       
+00005cd0: 2052 6574 7572 6e73 3a0d 0a20 2020 2020   Returns:..     
+00005ce0: 2020 2020 2020 2064 6963 743a 2064 6963         dict: dic
+00005cf0: 7469 6f6e 6172 7920 6f66 2062 6573 7420  tionary of best 
+00005d00: 7061 7261 6d65 7465 7273 0d0a 2020 2020  parameters..    
+00005d10: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+00005d20: 206f 7574 636f 6d65 7320 3d20 7b7d 0d0a   outcomes = {}..
+00005d30: 2020 2020 2020 2020 7374 6570 5f69 6e74          step_int
+00005d40: 6572 7661 6c5f 6c69 6d69 7420 3d20 696e  erval_limit = in
+00005d50: 7428 766f 6c75 6d65 2f73 656c 662e 7265  t(volume/self.re
+00005d60: 736f 6c75 7469 6f6e 2f53 5445 505f 5245  solution/STEP_RE
+00005d70: 534f 4c55 5449 4f4e 290d 0a20 2020 2020  SOLUTION)..     
+00005d80: 2020 2066 6f72 2070 7265 7365 7420 696e     for preset in
+00005d90: 2073 656c 662e 7370 6565 645f 7072 6573   self.speed_pres
+00005da0: 6574 733a 0d0a 2020 2020 2020 2020 2020  ets:..          
+00005db0: 2020 6966 2070 7265 7365 7420 3c20 7370    if preset < sp
+00005dc0: 6565 643a 0d0a 2020 2020 2020 2020 2020  eed:..          
+00005dd0: 2020 2020 2020 2320 7072 6573 6574 2069        # preset i
+00005de0: 7320 736c 6f77 6572 2074 6861 6e20 7461  s slower than ta
+00005df0: 7267 6574 2073 7065 6564 2c20 6974 2077  rget speed, it w
+00005e00: 696c 6c20 6e65 7665 7220 6869 7420 7461  ill never hit ta
+00005e10: 7267 6574 2073 7065 6564 0d0a 2020 2020  rget speed..    
+00005e20: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
+00005e30: 696e 7565 0d0a 2020 2020 2020 2020 2020  inue..          
+00005e40: 2020 7469 6d65 5f69 6e74 6572 7661 6c5f    time_interval_
+00005e50: 6c69 6d69 7420 3d20 696e 7428 766f 6c75  limit = int(volu
+00005e60: 6d65 2a28 312f 7370 6565 6420 2d20 312f  me*(1/speed - 1/
+00005e70: 7072 6573 6574 292f 7365 6c66 2e72 6573  preset)/self.res
+00005e80: 706f 6e73 655f 7469 6d65 290d 0a20 2020  ponse_time)..   
+00005e90: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+00005ea0: 7374 6570 5f69 6e74 6572 7661 6c5f 6c69  step_interval_li
+00005eb0: 6d69 7420 6f72 206e 6f74 2074 696d 655f  mit or not time_
+00005ec0: 696e 7465 7276 616c 5f6c 696d 6974 3a0d  interval_limit:.
+00005ed0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005ee0: 2063 6f6e 7469 6e75 650d 0a20 2020 2020   continue..     
+00005ef0: 2020 2020 2020 2069 6e74 6572 7661 6c73         intervals
+00005f00: 203d 206d 6178 286d 696e 2873 7465 705f   = max(min(step_
+00005f10: 696e 7465 7276 616c 5f6c 696d 6974 2c20  interval_limit, 
+00005f20: 7469 6d65 5f69 6e74 6572 7661 6c5f 6c69  time_interval_li
+00005f30: 6d69 7429 2c20 3129 0d0a 2020 2020 2020  mit), 1)..      
+00005f40: 2020 2020 2020 6561 6368 5f73 7465 7073        each_steps
+00005f50: 203d 2076 6f6c 756d 652f 7365 6c66 2e72   = volume/self.r
+00005f60: 6573 6f6c 7574 696f 6e2f 696e 7465 7276  esolution/interv
+00005f70: 616c 730d 0a20 2020 2020 2020 2020 2020  als..           
+00005f80: 2065 6163 685f 6465 6c61 7920 3d20 766f   each_delay = vo
+00005f90: 6c75 6d65 2a28 312f 7370 6565 6420 2d20  lume*(1/speed - 
+00005fa0: 312f 7072 6573 6574 292f 696e 7465 7276  1/preset)/interv
+00005fb0: 616c 730d 0a20 2020 2020 2020 2020 2020  als..           
+00005fc0: 2061 7265 6120 3d20 302e 3520 2a20 2876   area = 0.5 * (v
+00005fd0: 6f6c 756d 652a 2a32 2920 2a20 2831 2f73  olume**2) * (1/s
+00005fe0: 656c 662e 7265 736f 6c75 7469 6f6e 2920  elf.resolution) 
+00005ff0: 2a20 2831 2f69 6e74 6572 7661 6c73 2920  * (1/intervals) 
+00006000: 2a20 2831 2f73 7065 6564 202d 2031 2f70  * (1/speed - 1/p
+00006010: 7265 7365 7429 0d0a 2020 2020 2020 2020  reset)..        
+00006020: 2020 2020 6f75 7463 6f6d 6573 5b61 7265      outcomes[are
+00006030: 615d 203d 2053 7065 6564 5061 7261 6d65  a] = SpeedParame
+00006040: 7465 7273 2870 7265 7365 742c 2069 6e74  ters(preset, int
+00006050: 6572 7661 6c73 2c20 696e 7428 6561 6368  ervals, int(each
+00006060: 5f73 7465 7073 292c 2065 6163 685f 6465  _steps), each_de
+00006070: 6c61 7929 0d0a 2020 2020 2020 2020 6966  lay)..        if
+00006080: 206c 656e 286f 7574 636f 6d65 7329 203d   len(outcomes) =
+00006090: 3d20 303a 0d0a 2020 2020 2020 2020 2020  = 0:..          
+000060a0: 2020 7072 696e 7428 224e 6f20 6665 6173    print("No feas
+000060b0: 6962 6c65 2073 7065 6564 2070 6172 616d  ible speed param
+000060c0: 6574 6572 732e 2229 0d0a 2020 2020 2020  eters.")..      
+000060d0: 2020 2020 2020 7265 7475 726e 2053 7065        return Spe
+000060e0: 6564 5061 7261 6d65 7465 7273 284e 6f6e  edParameters(Non
+000060f0: 652c 2053 5445 505f 5245 534f 4c55 5449  e, STEP_RESOLUTI
+00006100: 4f4e 2c20 5354 4550 5f52 4553 4f4c 5554  ON, STEP_RESOLUT
+00006110: 494f 4e2c 2073 656c 662e 7265 7370 6f6e  ION, self.respon
+00006120: 7365 5f74 696d 6529 0d0a 2020 2020 2020  se_time)..      
+00006130: 2020 7072 696e 7428 6627 4265 7374 2070    print(f'Best p
+00006140: 6172 616d 6574 6572 733a 207b 6f75 7463  arameters: {outc
+00006150: 6f6d 6573 5b6d 696e 286f 7574 636f 6d65  omes[min(outcome
+00006160: 7329 5d7d 2729 0d0a 2020 2020 2020 2020  s)]}')..        
+00006170: 7265 7475 726e 206f 7574 636f 6d65 735b  return outcomes[
+00006180: 6d69 6e28 6f75 7463 6f6d 6573 295d 0d0a  min(outcomes)]..
+00006190: 2020 2020 0d0a 2020 2020 6465 6620 5f63      ..    def _c
+000061a0: 6f6e 6e65 6374 2873 656c 662c 2070 6f72  onnect(self, por
+000061b0: 743a 7374 722c 2062 6175 6472 6174 653a  t:str, baudrate:
+000061c0: 696e 7420 3d20 3936 3030 2c20 7469 6d65  int = 9600, time
+000061d0: 6f75 743a 696e 7420 3d20 3129 3a0d 0a20  out:int = 1):.. 
+000061e0: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+000061f0: 2020 2020 436f 6e6e 6563 7469 6f6e 2070      Connection p
+00006200: 726f 6365 6475 7265 2066 6f72 2074 6f6f  rocedure for too
+00006210: 6c0d 0a0d 0a20 2020 2020 2020 2041 7267  l....        Arg
+00006220: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00006230: 706f 7274 2028 7374 7229 3a20 434f 4d20  port (str): COM 
+00006240: 706f 7274 2061 6464 7265 7373 0d0a 2020  port address..  
+00006250: 2020 2020 2020 2020 2020 6261 7564 7261            baudra
+00006260: 7465 2028 696e 742c 206f 7074 696f 6e61  te (int, optiona
+00006270: 6c29 3a20 6261 7564 7261 7465 2e20 4465  l): baudrate. De
+00006280: 6661 756c 7473 2074 6f20 3936 3030 2e0d  faults to 9600..
+00006290: 0a20 2020 2020 2020 2020 2020 2074 696d  .            tim
+000062a0: 656f 7574 2028 696e 742c 206f 7074 696f  eout (int, optio
+000062b0: 6e61 6c29 3a20 7469 6d65 6f75 7420 696e  nal): timeout in
+000062c0: 2073 6563 6f6e 6473 2e20 4465 6661 756c   seconds. Defaul
+000062d0: 7473 2074 6f20 312e 0d0a 2020 2020 2020  ts to 1...      
+000062e0: 2020 2222 220d 0a20 2020 2020 2020 2073    """..        s
+000062f0: 656c 662e 636f 6e6e 6563 7469 6f6e 5f64  elf.connection_d
+00006300: 6574 6169 6c73 203d 207b 0d0a 2020 2020  etails = {..    
+00006310: 2020 2020 2020 2020 2770 6f72 7427 3a20          'port': 
+00006320: 706f 7274 2c0d 0a20 2020 2020 2020 2020  port,..         
+00006330: 2020 2027 6261 7564 7261 7465 273a 2062     'baudrate': b
+00006340: 6175 6472 6174 652c 0d0a 2020 2020 2020  audrate,..      
+00006350: 2020 2020 2020 2774 696d 656f 7574 273a        'timeout':
+00006360: 2074 696d 656f 7574 0d0a 2020 2020 2020   timeout..      
+00006370: 2020 7d0d 0a20 2020 2020 2020 2064 6576    }..        dev
+00006380: 6963 6520 3d20 4e6f 6e65 0d0a 2020 2020  ice = None..    
+00006390: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
+000063a0: 2020 2020 2020 6465 7669 6365 203d 2073        device = s
+000063b0: 6572 6961 6c2e 5365 7269 616c 2870 6f72  erial.Serial(por
+000063c0: 742c 2062 6175 6472 6174 652c 2074 696d  t, baudrate, tim
+000063d0: 656f 7574 3d74 696d 656f 7574 290d 0a20  eout=timeout).. 
+000063e0: 2020 2020 2020 2065 7863 6570 7420 4578         except Ex
+000063f0: 6365 7074 696f 6e20 6173 2065 3a0d 0a20  ception as e:.. 
+00006400: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+00006410: 2866 2243 6f75 6c64 206e 6f74 2063 6f6e  (f"Could not con
+00006420: 6e65 6374 2074 6f20 7b70 6f72 747d 2229  nect to {port}")
+00006430: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00006440: 2073 656c 662e 7665 7262 6f73 653a 0d0a   self.verbose:..
+00006450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006460: 7072 696e 7428 6529 0d0a 2020 2020 2020  print(e)..      
+00006470: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+00006480: 2020 2020 2074 696d 652e 736c 6565 7028       time.sleep(
+00006490: 3229 2020 2023 2057 6169 7420 666f 7220  2)   # Wait for 
+000064a0: 6772 626c 2074 6f20 696e 6974 6961 6c69  grbl to initiali
+000064b0: 7a65 0d0a 2020 2020 2020 2020 2020 2020  ze..            
+000064c0: 6465 7669 6365 2e66 6c75 7368 496e 7075  device.flushInpu
+000064d0: 7428 290d 0a20 2020 2020 2020 2020 2020  t()..           
+000064e0: 2070 7269 6e74 2866 2243 6f6e 6e65 6374   print(f"Connect
+000064f0: 696f 6e20 6f70 656e 6564 2074 6f20 7b70  ion opened to {p
+00006500: 6f72 747d 2229 0d0a 2020 2020 2020 2020  ort}")..        
+00006510: 2020 2020 7365 6c66 2e73 6574 466c 6167      self.setFlag
+00006520: 2863 6f6e 6e65 6374 6564 3d54 7275 6529  (connected=True)
+00006530: 0d0a 2020 2020 2020 2020 7365 6c66 2e64  ..        self.d
+00006540: 6576 6963 6520 3d20 6465 7669 6365 0d0a  evice = device..
+00006550: 2020 2020 2020 2020 7365 6c66 2e67 6574          self.get
+00006560: 496e 666f 2829 0d0a 2020 2020 2020 2020  Info()..        
+00006570: 7365 6c66 2e72 6573 6574 2829 0d0a 2020  self.reset()..  
+00006580: 2020 2020 2020 7265 7475 726e 0d0a 2020        return..  
+00006590: 2020 0d0a 2020 2020 6465 6620 5f69 735f    ..    def _is_
+000065a0: 6578 7065 6374 6564 5f72 6570 6c79 2873  expected_reply(s
+000065b0: 656c 662c 2072 6573 706f 6e73 653a 7374  elf, response:st
+000065c0: 722c 2063 6f6d 6d61 6e64 5f63 6f64 653a  r, command_code:
+000065d0: 7374 722c 202a 2a6b 7761 7267 7329 202d  str, **kwargs) -
+000065e0: 3e20 626f 6f6c 3a0d 0a20 2020 2020 2020  > bool:..       
+000065f0: 2022 2222 0d0a 2020 2020 2020 2020 4368   """..        Ch
+00006600: 6563 6b73 2061 6e64 2072 6574 7572 6e73  ecks and returns
+00006610: 2077 6865 7468 6572 2074 6865 2072 6573   whether the res
+00006620: 706f 6e73 6520 6973 2061 6e20 6578 7065  ponse is an expe
+00006630: 6374 6564 2072 6570 6c79 0d0a 0d0a 2020  cted reply....  
+00006640: 2020 2020 2020 4172 6773 3a0d 0a20 2020        Args:..   
+00006650: 2020 2020 2020 2020 2072 6573 706f 6e73           respons
+00006660: 6520 2873 7472 293a 2072 6573 706f 6e73  e (str): respons
+00006670: 6520 7374 7269 6e67 2066 726f 6d20 6465  e string from de
+00006680: 7669 6365 0d0a 2020 2020 2020 2020 2020  vice..          
+00006690: 2020 636f 6d6d 616e 645f 636f 6465 2028    command_code (
+000066a0: 7374 7229 3a20 7477 6f2d 6368 6172 6163  str): two-charac
+000066b0: 7465 7220 636f 6d6d 616e 6420 636f 6465  ter command code
+000066c0: 0d0a 0d0a 2020 2020 2020 2020 5265 7475  ....        Retu
+000066d0: 726e 733a 0d0a 2020 2020 2020 2020 2020  rns:..          
+000066e0: 2020 626f 6f6c 3a20 7768 6574 6865 7220    bool: whether 
+000066f0: 7468 6520 7265 7370 6f6e 7365 2069 7320  the response is 
+00006700: 616e 2065 7870 6563 7465 6420 7265 706c  an expected repl
+00006710: 790d 0a20 2020 2020 2020 2022 2222 0d0a  y..        """..
+00006720: 2020 2020 2020 2020 6966 2072 6573 706f          if respo
+00006730: 6e73 6520 696e 2045 7272 6f72 436f 6465  nse in ErrorCode
+00006740: 2e5f 6d65 6d62 6572 5f6e 616d 6573 5f3a  ._member_names_:
+00006750: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+00006760: 7475 726e 2054 7275 650d 0a20 2020 2020  turn True..     
+00006770: 2020 2069 6620 636f 6d6d 616e 645f 636f     if command_co
+00006780: 6465 206e 6f74 2069 6e20 5155 4552 4945  de not in QUERIE
+00006790: 5320 616e 6420 7265 7370 6f6e 7365 203d  S and response =
+000067a0: 3d20 276f 6b27 3a0d 0a20 2020 2020 2020  = 'ok':..       
+000067b0: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
+000067c0: 0d0a 2020 2020 2020 2020 6966 2063 6f6d  ..        if com
+000067d0: 6d61 6e64 5f63 6f64 6520 696e 2051 5545  mand_code in QUE
+000067e0: 5249 4553 2061 6e64 2072 6573 706f 6e73  RIES and respons
+000067f0: 655b 3a32 5d20 3d3d 2063 6f6d 6d61 6e64  e[:2] == command
+00006800: 5f63 6f64 652e 6c6f 7765 7228 293a 0d0a  _code.lower():..
+00006810: 2020 2020 2020 2020 2020 2020 7265 706c              repl
+00006820: 795f 636f 6465 2c20 6461 7461 203d 2072  y_code, data = r
+00006830: 6573 706f 6e73 655b 3a32 5d2c 2072 6573  esponse[:2], res
+00006840: 706f 6e73 655b 323a 5d0d 0a20 2020 2020  ponse[2:]..     
+00006850: 2020 2020 2020 2069 6620 7365 6c66 2e76         if self.v
+00006860: 6572 626f 7365 3a0d 0a20 2020 2020 2020  erbose:..       
+00006870: 2020 2020 2020 2020 2070 7269 6e74 2866           print(f
+00006880: 275b 7b72 6570 6c79 5f63 6f64 657d 5d20  '[{reply_code}] 
+00006890: 7b64 6174 617d 2729 0d0a 2020 2020 2020  {data}')..      
+000068a0: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
+000068b0: 650d 0a20 2020 2020 2020 2072 6574 7572  e..        retur
+000068c0: 6e20 4661 6c73 650d 0a0d 0a20 2020 2064  n False....    d
+000068d0: 6566 205f 6c6f 6f70 5f66 6565 6462 6163  ef _loop_feedbac
+000068e0: 6b28 7365 6c66 293a 0d0a 2020 2020 2020  k(self):..      
+000068f0: 2020 2222 224c 6f6f 7020 746f 2063 6f6e    """Loop to con
+00006900: 7374 616e 746c 7920 7265 6164 2066 726f  stantly read fro
+00006910: 6d20 6465 7669 6365 2222 220d 0a20 2020  m device"""..   
+00006920: 2020 2020 2070 7269 6e74 2827 4c69 7374       print('List
+00006930: 656e 696e 672e 2e2e 2729 0d0a 2020 2020  ening...')..    
+00006940: 2020 2020 7768 696c 6520 7365 6c66 2e66      while self.f
+00006950: 6c61 6773 5b27 6765 745f 6665 6564 6261  lags['get_feedba
+00006960: 636b 275d 3a0d 0a20 2020 2020 2020 2020  ck']:..         
+00006970: 2020 2069 6620 7365 6c66 2e66 6c61 6773     if self.flags
+00006980: 5b27 7061 7573 655f 6665 6564 6261 636b  ['pause_feedback
+00006990: 275d 3a0d 0a20 2020 2020 2020 2020 2020  ']:..           
+000069a0: 2020 2020 2063 6f6e 7469 6e75 650d 0a20       continue.. 
+000069b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000069c0: 6765 7453 7461 7475 7328 290d 0a20 2020  getStatus()..   
+000069d0: 2020 2020 2020 2020 2073 656c 662e 6765           self.ge
+000069e0: 7443 6170 6163 6974 616e 6365 2829 0d0a  tCapacitance()..
+000069f0: 2020 2020 2020 2020 7072 696e 7428 2753          print('S
+00006a00: 746f 7020 6c69 7374 656e 696e 672e 2e2e  top listening...
+00006a10: 2729 0d0a 2020 2020 2020 2020 7265 7475  ')..        retu
+00006a20: 726e 0d0a 2020 2020 0d0a 2020 2020 6465  rn..    ..    de
+00006a30: 6620 5f71 7565 7279 2873 656c 662c 200d  f _query(self, .
+00006a40: 0a20 2020 2020 2020 2063 6f6d 6d61 6e64  .        command
+00006a50: 3a20 7374 722c 200d 0a20 2020 2020 2020  : str, ..       
+00006a60: 2074 696d 656f 7574 5f73 3a20 666c 6f61   timeout_s: floa
+00006a70: 7420 3d20 302e 332c 200d 0a20 2020 2020  t = 0.3, ..     
+00006a80: 2020 2072 6573 756d 655f 6665 6564 6261     resume_feedba
+00006a90: 636b 3a20 626f 6f6c 203d 2046 616c 7365  ck: bool = False
+00006aa0: 0d0a 2020 2020 2920 2d3e 2073 7472 3a0d  ..    ) -> str:.
+00006ab0: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+00006ac0: 2020 2020 2020 5772 6974 6520 636f 6d6d        Write comm
+00006ad0: 616e 6420 746f 2061 6e64 2072 6561 6420  and to and read 
+00006ae0: 7265 7370 6f6e 7365 2066 726f 6d20 6465  response from de
+00006af0: 7669 6365 0d0a 0d0a 2020 2020 2020 2020  vice....        
+00006b00: 4172 6773 3a0d 0a20 2020 2020 2020 2020  Args:..         
+00006b10: 2020 2063 6f6d 6d61 6e64 2028 7374 7229     command (str)
+00006b20: 3a20 636f 6d6d 616e 6420 7374 7269 6e67  : command string
+00006b30: 0d0a 2020 2020 2020 2020 2020 2020 7469  ..            ti
+00006b40: 6d65 6f75 745f 7320 2866 6c6f 6174 2c20  meout_s (float, 
+00006b50: 6f70 7469 6f6e 616c 293a 2064 7572 6174  optional): durat
+00006b60: 696f 6e20 746f 2077 6169 7420 6265 666f  ion to wait befo
+00006b70: 7265 2074 696d 656f 7574 2e20 4465 6661  re timeout. Defa
+00006b80: 756c 7473 2074 6f20 302e 332e 0d0a 2020  ults to 0.3...  
+00006b90: 2020 2020 2020 2020 2020 7265 7375 6d65            resume
+00006ba0: 5f66 6565 6462 6163 6b20 2862 6f6f 6c2c  _feedback (bool,
+00006bb0: 206f 7074 696f 6e61 6c29 3a20 7768 6574   optional): whet
+00006bc0: 6865 7220 746f 2072 6573 756d 6520 7265  her to resume re
+00006bd0: 6164 696e 6720 6672 6f6d 2064 6576 6963  ading from devic
+00006be0: 652e 2044 6566 6175 6c74 7320 746f 2046  e. Defaults to F
+00006bf0: 616c 7365 2e0d 0a0d 0a20 2020 2020 2020  alse.....       
+00006c00: 2052 6574 7572 6e73 3a0d 0a20 2020 2020   Returns:..     
+00006c10: 2020 2020 2020 2073 7472 3a20 7265 7370         str: resp
+00006c20: 6f6e 7365 2073 7472 696e 670d 0a20 2020  onse string..   
+00006c30: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+00006c40: 2020 636f 6d6d 616e 645f 636f 6465 203d    command_code =
+00006c50: 2063 6f6d 6d61 6e64 5b3a 325d 0d0a 2020   command[:2]..  
+00006c60: 2020 2020 2020 6966 2063 6f6d 6d61 6e64        if command
+00006c70: 5f63 6f64 6520 6e6f 7420 696e 2053 5441  _code not in STA
+00006c80: 5455 535f 5155 4552 4945 533a 0d0a 2020  TUS_QUERIES:..  
+00006c90: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00006ca0: 662e 666c 6167 735b 2767 6574 5f66 6565  f.flags['get_fee
+00006cb0: 6462 6163 6b27 5d20 616e 6420 6e6f 7420  dback'] and not 
+00006cc0: 7365 6c66 2e66 6c61 6773 5b27 7061 7573  self.flags['paus
+00006cd0: 655f 6665 6564 6261 636b 275d 3a0d 0a20  e_feedback']:.. 
+00006ce0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00006cf0: 656c 662e 7365 7446 6c61 6728 7061 7573  elf.setFlag(paus
+00006d00: 655f 6665 6564 6261 636b 3d54 7275 6529  e_feedback=True)
+00006d10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00006d20: 2020 7469 6d65 2e73 6c65 6570 2874 696d    time.sleep(tim
+00006d30: 656f 7574 5f73 290d 0a20 2020 2020 2020  eout_s)..       
+00006d40: 2020 2020 2073 656c 662e 6765 7453 7461       self.getSta
+00006d50: 7475 7328 290d 0a20 2020 2020 2020 2020  tus()..         
+00006d60: 2020 2077 6869 6c65 2073 656c 662e 6973     while self.is
+00006d70: 4275 7379 2829 3a0d 0a20 2020 2020 2020  Busy():..       
+00006d80: 2020 2020 2020 2020 2073 656c 662e 6765           self.ge
+00006d90: 7453 7461 7475 7328 290d 0a20 2020 2020  tStatus()..     
+00006da0: 2020 200d 0a20 2020 2020 2020 2073 7461     ..        sta
+00006db0: 7274 5f74 696d 6520 3d20 7469 6d65 2e74  rt_time = time.t
+00006dc0: 696d 6528 290d 0a20 2020 2020 2020 2073  ime()..        s
+00006dd0: 656c 662e 5f77 7269 7465 2863 6f6d 6d61  elf._write(comma
+00006de0: 6e64 290d 0a20 2020 2020 2020 2072 6573  nd)..        res
+00006df0: 706f 6e73 6520 3d20 2727 0d0a 2020 2020  ponse = ''..    
+00006e00: 2020 2020 7768 696c 6520 6e6f 7420 7365      while not se
+00006e10: 6c66 2e5f 6973 5f65 7870 6563 7465 645f  lf._is_expected_
+00006e20: 7265 706c 7928 7265 7370 6f6e 7365 2c20  reply(response, 
+00006e30: 636f 6d6d 616e 645f 636f 6465 293a 0d0a  command_code):..
+00006e40: 2020 2020 2020 2020 2020 2020 6966 2074              if t
+00006e50: 696d 652e 7469 6d65 2829 202d 2073 7461  ime.time() - sta
+00006e60: 7274 5f74 696d 6520 3e20 7469 6d65 6f75  rt_time > timeou
+00006e70: 745f 733a 0d0a 2020 2020 2020 2020 2020  t_s:..          
+00006e80: 2020 2020 2020 6272 6561 6b0d 0a20 2020        break..   
+00006e90: 2020 2020 2020 2020 2072 6573 706f 6e73           respons
+00006ea0: 6520 3d20 7365 6c66 2e5f 7265 6164 2829  e = self._read()
+00006eb0: 0d0a 2020 2020 2020 2020 2320 7072 696e  ..        # prin
+00006ec0: 7428 7469 6d65 2e74 696d 6528 2920 2d20  t(time.time() - 
+00006ed0: 7374 6172 745f 7469 6d65 290d 0a20 2020  start_time)..   
+00006ee0: 2020 2020 2069 6620 636f 6d6d 616e 645f       if command_
+00006ef0: 636f 6465 2069 6e20 5155 4552 4945 533a  code in QUERIES:
+00006f00: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+00006f10: 7370 6f6e 7365 203d 2072 6573 706f 6e73  sponse = respons
+00006f20: 655b 323a 5d0d 0a20 2020 2020 2020 2069  e[2:]..        i
+00006f30: 6620 636f 6d6d 616e 645f 636f 6465 206e  f command_code n
+00006f40: 6f74 2069 6e20 5354 4154 5553 5f51 5545  ot in STATUS_QUE
+00006f50: 5249 4553 3a0d 0a20 2020 2020 2020 2020  RIES:..         
+00006f60: 2020 2073 656c 662e 6765 7450 6f73 6974     self.getPosit
+00006f70: 696f 6e28 290d 0a20 2020 2020 2020 2020  ion()..         
+00006f80: 2020 2069 6620 7265 7375 6d65 5f66 6565     if resume_fee
+00006f90: 6462 6163 6b3a 0d0a 2020 2020 2020 2020  dback:..        
+00006fa0: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
+00006fb0: 466c 6167 2870 6175 7365 5f66 6565 6462  Flag(pause_feedb
+00006fc0: 6163 6b3d 4661 6c73 6529 0d0a 2020 2020  ack=False)..    
+00006fd0: 2020 2020 7265 7475 726e 2072 6573 706f      return respo
+00006fe0: 6e73 650d 0a0d 0a20 2020 2064 6566 205f  nse....    def _
+00006ff0: 7265 6164 2873 656c 6629 202d 3e20 7374  read(self) -> st
+00007000: 723a 0d0a 2020 2020 2020 2020 2222 220d  r:..        """.
+00007010: 0a20 2020 2020 2020 2052 6561 6420 7265  .        Read re
+00007020: 7370 6f6e 7365 2066 726f 6d20 6465 7669  sponse from devi
+00007030: 6365 0d0a 0d0a 2020 2020 2020 2020 5265  ce....        Re
+00007040: 7475 726e 733a 0d0a 2020 2020 2020 2020  turns:..        
+00007050: 2020 2020 7374 723a 2072 6573 706f 6e73      str: respons
+00007060: 6520 7374 7269 6e67 0d0a 2020 2020 2020  e string..      
+00007070: 2020 2222 220d 0a20 2020 2020 2020 2072    """..        r
+00007080: 6573 706f 6e73 6520 3d20 2727 0d0a 2020  esponse = ''..  
+00007090: 2020 2020 2020 7472 793a 0d0a 2020 2020        try:..    
+000070a0: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
+000070b0: 203d 2073 656c 662e 6465 7669 6365 2e72   = self.device.r
+000070c0: 6561 646c 696e 6528 290d 0a20 2020 2020  eadline()..     
+000070d0: 2020 2020 2020 2069 6620 6c65 6e28 7265         if len(re
+000070e0: 7370 6f6e 7365 2920 3d3d 2030 3a0d 0a20  sponse) == 0:.. 
+000070f0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00007100: 6573 706f 6e73 6520 3d20 7365 6c66 2e64  esponse = self.d
+00007110: 6576 6963 652e 7265 6164 6c69 6e65 2829  evice.readline()
+00007120: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+00007130: 7370 6f6e 7365 203d 2072 6573 706f 6e73  sponse = respons
+00007140: 655b 323a 2d32 5d2e 6465 636f 6465 2827  e[2:-2].decode('
+00007150: 7574 662d 3827 290d 0a20 2020 2020 2020  utf-8')..       
+00007160: 2065 7863 6570 7420 4174 7472 6962 7574   except Attribut
+00007170: 6545 7272 6f72 3a0d 0a20 2020 2020 2020  eError:..       
+00007180: 2020 2020 2070 6173 730d 0a20 2020 2020       pass..     
+00007190: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
+000071a0: 696f 6e20 6173 2065 3a0d 0a20 2020 2020  ion as e:..     
+000071b0: 2020 2020 2020 2069 6620 7365 6c66 2e76         if self.v
+000071c0: 6572 626f 7365 3a0d 0a20 2020 2020 2020  erbose:..       
+000071d0: 2020 2020 2020 2020 2070 7269 6e74 2865           print(e
+000071e0: 290d 0a20 2020 2020 2020 2069 6620 7265  )..        if re
+000071f0: 7370 6f6e 7365 2069 6e20 4572 726f 7243  sponse in ErrorC
+00007200: 6f64 652e 5f6d 656d 6265 725f 6e61 6d65  ode._member_name
+00007210: 735f 3a0d 0a20 2020 2020 2020 2020 2020  s_:..           
+00007220: 2070 7269 6e74 2845 7272 6f72 436f 6465   print(ErrorCode
+00007230: 5b72 6573 706f 6e73 655d 2e76 616c 7565  [response].value
+00007240: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+00007250: 6e20 7265 7370 6f6e 7365 0d0a 2020 2020  n response..    
+00007260: 0d0a 2020 2020 6465 6620 5f73 6574 5f63  ..    def _set_c
+00007270: 6861 6e6e 656c 5f69 6428 7365 6c66 2c20  hannel_id(self, 
+00007280: 6e65 775f 6368 616e 6e65 6c5f 6964 3a69  new_channel_id:i
+00007290: 6e74 293a 0d0a 2020 2020 2020 2020 2222  nt):..        ""
+000072a0: 220d 0a20 2020 2020 2020 2053 6574 2063  "..        Set c
+000072b0: 6861 6e6e 656c 2069 6420 6f66 2064 6576  hannel id of dev
+000072c0: 6963 650d 0a0d 0a20 2020 2020 2020 2041  ice....        A
+000072d0: 7267 733a 0d0a 2020 2020 2020 2020 2020  rgs:..          
+000072e0: 2020 6e65 775f 6368 616e 6e65 6c20 2869    new_channel (i
+000072f0: 6e74 293a 206e 6577 2063 6861 6e6e 656c  nt): new channel
+00007300: 2069 640d 0a0d 0a20 2020 2020 2020 2052   id....        R
+00007310: 6169 7365 733a 0d0a 2020 2020 2020 2020  aises:..        
+00007320: 2020 2020 5661 6c75 6545 7272 6f72 3a20      ValueError: 
+00007330: 506c 6561 7365 2073 656c 6563 7420 6120  Please select a 
+00007340: 7661 6c69 6420 724c 696e 6520 6164 6472  valid rLine addr
+00007350: 6573 7320 6672 6f6d 2031 2074 6f20 390d  ess from 1 to 9.
+00007360: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+00007370: 2020 2020 2020 6966 206e 6f74 2028 3020        if not (0 
+00007380: 3c20 6e65 775f 6368 616e 6e65 6c5f 6964  < new_channel_id
+00007390: 203c 2031 3029 3a0d 0a20 2020 2020 2020   < 10):..       
+000073a0: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
+000073b0: 4572 726f 7228 2750 6c65 6173 6520 7365  Error('Please se
+000073c0: 6c65 6374 2061 2076 616c 6964 2072 4c69  lect a valid rLi
+000073d0: 6e65 2061 6464 7265 7373 2066 726f 6d20  ne address from 
+000073e0: 3120 746f 2039 2e27 290d 0a20 2020 2020  1 to 9.')..     
+000073f0: 2020 2072 6573 706f 6e73 6520 3d20 7365     response = se
+00007400: 6c66 2e5f 7175 6572 7928 6627 2a41 7b6e  lf._query(f'*A{n
+00007410: 6577 5f63 6861 6e6e 656c 5f69 647d 2729  ew_channel_id}')
+00007420: 0d0a 2020 2020 2020 2020 6966 2072 6573  ..        if res
+00007430: 706f 6e73 6520 3d3d 2027 6f6b 273a 0d0a  ponse == 'ok':..
+00007440: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00007450: 2e63 6861 6e6e 656c 203d 206e 6577 5f63  .channel = new_c
+00007460: 6861 6e6e 656c 5f69 640d 0a20 2020 2020  hannel_id..     
+00007470: 2020 2072 6574 7572 6e0d 0a20 2020 200d     return..    .
+00007480: 0a20 2020 2064 6566 205f 7772 6974 6528  .    def _write(
+00007490: 7365 6c66 2c20 636f 6d6d 616e 643a 7374  self, command:st
+000074a0: 7229 202d 3e20 626f 6f6c 3a0d 0a20 2020  r) -> bool:..   
+000074b0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+000074c0: 2020 5772 6974 6520 636f 6d6d 616e 6420    Write command 
+000074d0: 746f 2064 6576 6963 650d 0a0d 0a20 2020  to device....   
+000074e0: 2020 2020 2041 7267 733a 0d0a 2020 2020       Args:..    
+000074f0: 2020 2020 2020 2020 636f 6d6d 616e 6420          command 
+00007500: 2873 7472 293a 203c 636f 6d6d 616e 6420  (str): <command 
+00007510: 636f 6465 3e3c 7661 6c75 653e 0d0a 0d0a  code><value>....
+00007520: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
+00007530: 0d0a 2020 2020 2020 2020 2020 2020 626f  ..            bo
+00007540: 6f6c 3a20 7768 6574 6865 7220 636f 6d6d  ol: whether comm
+00007550: 616e 6420 7761 7320 7365 6e74 2073 7563  and was sent suc
+00007560: 6365 7373 6675 6c6c 790d 0a20 2020 2020  cessfully..     
+00007570: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+00007580: 6966 2073 656c 662e 7665 7262 6f73 653a  if self.verbose:
+00007590: 0d0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
+000075a0: 696e 7428 636f 6d6d 616e 6429 0d0a 2020  int(command)..  
+000075b0: 2020 2020 2020 6673 7472 696e 6720 3d20        fstring = 
+000075c0: 6627 017b 7365 6c66 2e63 6861 6e6e 656c  f'.{self.channel
+000075d0: 7d7b 636f 6d6d 616e 647d c2ba 5c72 2720  }{command}..\r' 
+000075e0: 2320 636f 6d6d 616e 6420 7465 6d70 6c61  # command templa
+000075f0: 7465 3a20 3c50 5245 3e3c 4144 523e 3c43  te: <PRE><ADR><C
+00007600: 4f44 453e 3c44 4154 413e 3c4c 5243 3e3c  ODE><DATA><LRC><
+00007610: 504f 5354 3e0d 0a20 2020 2020 2020 2023  POST>..        #
+00007620: 2062 7374 7269 6e67 203d 2062 7974 6561   bstring = bytea
+00007630: 7272 6179 2e66 726f 6d68 6578 2866 7374  rray.fromhex(fst
+00007640: 7269 6e67 2e65 6e63 6f64 6528 2775 7466  ring.encode('utf
+00007650: 2d38 2729 2e68 6578 2829 290d 0a20 2020  -8').hex())..   
+00007660: 2020 2020 2074 7279 3a0d 0a20 2020 2020       try:..     
+00007670: 2020 2020 2020 2023 2054 7970 6963 616c         # Typical
+00007680: 2074 696d 656f 7574 2077 6169 7420 6973   timeout wait is
+00007690: 2034 3030 6d73 0d0a 2020 2020 2020 2020   400ms..        
+000076a0: 2020 2020 7365 6c66 2e64 6576 6963 652e      self.device.
+000076b0: 7772 6974 6528 6673 7472 696e 672e 656e  write(fstring.en
+000076c0: 636f 6465 2827 7574 662d 3827 2929 0d0a  code('utf-8'))..
+000076d0: 2020 2020 2020 2020 6578 6365 7074 2041          except A
+000076e0: 7474 7269 6275 7465 4572 726f 723a 0d0a  ttributeError:..
+000076f0: 2020 2020 2020 2020 2020 2020 7061 7373              pass
+00007700: 0d0a 2020 2020 2020 2020 6578 6365 7074  ..        except
+00007710: 2045 7863 6570 7469 6f6e 2061 7320 653a   Exception as e:
+00007720: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00007730: 2073 656c 662e 7665 7262 6f73 653a 0d0a   self.verbose:..
+00007740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007750: 7072 696e 7428 6529 0d0a 2020 2020 2020  print(e)..      
+00007760: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
+00007770: 7365 0d0a 2020 2020 2020 2020 7265 7475  se..        retu
+00007780: 726e 2054 7275 650d 0a20 2020 20         rn True..
```

### Comparing `control-lab-ly-1.0.0b1/src/controllably/Transfer/Liquid/liquid_utils.py` & `control-lab-ly-1.0.1a0/src/controllably/Transfer/Liquid/liquid_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/Transfer/Liquid/syringe_lib.py` & `control-lab-ly-1.0.1a0/src/controllably/Transfer/Liquid/syringe_lib.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 Other constants and variables:
     CALIBRATION (SyringeCalibration)
 """
 # Standard library imports
 from __future__ import annotations
 from collections import namedtuple
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 import numpy as np
 print(f"Import: OK <{__name__}>")
 
 Calibration = namedtuple('Calibration', ['aspirate','dispense'])
 """Calibration is a named tuple for an aspirate-dispense pair calibration value"""
 
 @dataclass
@@ -76,15 +76,15 @@
     
     capacity: float
     channel: int
     offset: tuple[float] = (0,0,0)
     volume: float = 0
     reagent: str = ''
     pullback_time: float = 2
-    _calibration: SyringeCalibration = CALIBRATION
+    _calibration: SyringeCalibration = field(default_factory=lambda: CALIBRATION)
     
     def __post_init__(self):
         self.offset = np.array(self.offset)
         return
     
     def __repr__(self) -> str:
         return f"Syringe {self.channel} (capacity={self.capacity}, volume={self.volume}, reagent={self.reagent}, offset={self.offset})"
```

### Comparing `control-lab-ly-1.0.0b1/src/controllably/Transfer/Liquid/syringe_utils.py` & `control-lab-ly-1.0.1a0/src/controllably/Transfer/Liquid/syringe_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/Transfer/Substrate/Dobot/dobot_attachments.py` & `control-lab-ly-1.0.1a0/src/controllably/Transfer/Substrate/Dobot/dobot_attachments.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/Transfer/Substrate/substrate_utils.py` & `control-lab-ly-1.0.1a0/src/controllably/Transfer/Substrate/substrate_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/View/Classifiers/classifier_utils.py` & `control-lab-ly-1.0.1a0/src/controllably/View/Classifiers/classifier_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/View/Optical/optical_utils.py` & `control-lab-ly-1.0.1a0/src/controllably/View/Optical/optical_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/View/Optical/placeholders/optical_camera.png` & `control-lab-ly-1.0.1a0/src/controllably/View/Optical/placeholders/optical_camera.png`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/View/Thermal/Flir/ax8/ax8.py` & `control-lab-ly-1.0.1a0/src/controllably/View/Thermal/Flir/ax8/ax8.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/View/Thermal/Flir/ax8/ax8_camera_feed.py` & `control-lab-ly-1.0.1a0/src/controllably/View/Thermal/Flir/ax8/ax8_camera_feed.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_regs.py` & `control-lab-ly-1.0.1a0/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_regs.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_utils.py` & `control-lab-ly-1.0.1a0/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/View/Thermal/placeholders/infrared_camera.png` & `control-lab-ly-1.0.1a0/src/controllably/View/Thermal/placeholders/infrared_camera.png`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/View/Thermal/thermal_utils.py` & `control-lab-ly-1.0.1a0/src/controllably/View/Thermal/thermal_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/View/image_utils.py` & `control-lab-ly-1.0.1a0/src/controllably/View/image_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/View/view_utils.py` & `control-lab-ly-1.0.1a0/src/controllably/View/view_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/misc/__init__.py` & `control-lab-ly-1.0.1a0/src/controllably/misc/__init__.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/misc/decorators.py` & `control-lab-ly-1.0.1a0/src/controllably/misc/decorators.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/misc/factory.py` & `control-lab-ly-1.0.1a0/src/controllably/misc/factory.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/misc/helper.py` & `control-lab-ly-1.0.1a0/src/controllably/misc/helper.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/misc/layout.py` & `control-lab-ly-1.0.1a0/src/controllably/misc/layout.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,16 @@
     - `details` (dict): well details; dictionary of depth, total liquid volume, shape, diameter, x,y,z
     - `name` (str): name of well
     - `reference_point` (tuple[int]): bottom left reference corner of Labware
     
     ### Properties
     - `bottom` (np.ndarray): bottom of well
     - `center` (np.ndarray): center of well
-    - `depth` (np.ndarray): well depth
+    - `depth` (float): well depth
+    - `diameter` (float): well diameter
     - `middle` (np.ndarray): middle of well
     - `offset` (np.ndarray): well offset from Labware reference point
     - `top` (np.ndarray): top of well
     
     ### Methods
     - `from_bottom`: offset from bottom of well
     - `from_middle`: offset from middle of well
@@ -79,14 +80,18 @@
         return np.array(self.reference_point) + self.offset
     
     @property
     def depth(self) -> float:
         return self.details.get('depth', 0)
     
     @property
+    def diameter(self) -> float:
+        return self.details.get('diameter', 0)
+    
+    @property
     def middle(self) -> np.ndarray:
         depth = self.details.get('depth', 0)
         return self.center + np.array((0,0,depth/2))
         
     @property
     def offset(self) -> np.ndarray:
         x = self.details.get('x', 0)
@@ -273,14 +278,15 @@
             name (str): name of well
 
         Returns:
             Well: `Well` object
         """
         return self.wells.get(name)
     
+    # Protected method(s)
     def _load_wells(self):
         """Load wells into memory"""
         wells = self.details.get('wells',{})
         for well in wells:
             self._wells[well] = Well(labware_info=self.info, name=well, details=wells[well])
         return
```

### Comparing `control-lab-ly-1.0.0b1/src/controllably/misc/logger.py` & `control-lab-ly-1.0.1a0/src/controllably/misc/logger.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/misc/misc_utils.py` & `control-lab-ly-1.0.1a0/src/controllably/misc/misc_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/misc/templates/configs/plugins/plugin_template.py` & `control-lab-ly-1.0.1a0/src/controllably/misc/templates/configs/plugins/plugin_template.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/misc/templates/setup/__init__.py` & `control-lab-ly-1.0.1a0/src/controllably/misc/templates/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/misc/templates/setup/config.yaml` & `control-lab-ly-1.0.1a0/src/controllably/misc/templates/setup/config.yaml`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/src/controllably/misc/templates/setup/layout.json` & `control-lab-ly-1.0.1a0/src/controllably/misc/templates/setup/layout.json`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/tests/test_compound_liquidmover.py` & `control-lab-ly-1.0.1a0/tests/test_compound_liquidmover.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/tests/test_compound_spin_printer.py` & `control-lab-ly-1.0.1a0/tests/test_compound_spin_printer.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/tests/test_dobot_m1pro.py` & `control-lab-ly-1.0.1a0/tests/test_dobot_m1pro.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/tests/test_dobot_mg400.py` & `control-lab-ly-1.0.1a0/tests/test_dobot_mg400.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/tests/test_heat_peltier.py` & `control-lab-ly-1.0.1a0/tests/test_heat_peltier.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b1/tests/test_liquid_tricontinent.py` & `control-lab-ly-1.0.1a0/tests/test_liquid_tricontinent.py`

 * *Files identical despite different names*

