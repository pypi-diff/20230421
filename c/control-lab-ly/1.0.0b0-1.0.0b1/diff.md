# Comparing `tmp/control-lab-ly-1.0.0b0.tar.gz` & `tmp/control-lab-ly-1.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "control-lab-ly-1.0.0b0.tar", last modified: Wed Apr 12 15:59:31 2023, max compression
+gzip compressed data, was "control-lab-ly-1.0.0b1.tar", last modified: Wed Apr 12 16:17:50 2023, max compression
```

## Comparing `control-lab-ly-1.0.0b0.tar` & `control-lab-ly-1.0.0b1.tar`

### file list

```diff
@@ -1,218 +1,218 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 15:59:31.012549 control-lab-ly-1.0.0b0/
--rw-rw-rw-   0        0        0     1093 2023-02-24 13:59:16.000000 control-lab-ly-1.0.0b0/LICENSE.md
--rw-rw-rw-   0        0        0       17 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b0/MANIFEST.in
--rw-rw-rw-   0        0        0    17511 2023-04-12 15:59:31.012549 control-lab-ly-1.0.0b0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-12 15:59:29.487610 control-lab-ly-1.0.0b0/docs/
--rw-rw-rw-   0        0        0     4263 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/docs/CHANGELOG.md
--rw-rw-rw-   0        0        0     5356 2023-02-24 14:06:11.000000 control-lab-ly-1.0.0b0/docs/CODE_OF_CONDUCT.md
--rw-rw-rw-   0        0        0       33 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0b0/docs/CONTRIBUTING.md
--rw-rw-rw-   0        0        0     1093 2023-02-24 13:59:16.000000 control-lab-ly-1.0.0b0/docs/LICENSE.md
--rw-rw-rw-   0        0        0    12128 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/docs/README.md
--rw-rw-rw-   0        0        0      108 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0b0/pyproject.toml
--rw-rw-rw-   0        0        0     1559 2023-04-12 15:59:31.012549 control-lab-ly-1.0.0b0/setup.cfg
--rw-rw-rw-   0        0        0       37 2023-03-10 02:02:34.000000 control-lab-ly-1.0.0b0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-12 15:59:29.105592 control-lab-ly-1.0.0b0/src/
-drwxrwxrwx   0        0        0        0 2023-04-12 15:59:29.579377 control-lab-ly-1.0.0b0/src/control_lab_ly.egg-info/
--rw-rw-rw-   0        0        0    17511 2023-04-12 15:59:28.000000 control-lab-ly-1.0.0b0/src/control_lab_ly.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7306 2023-04-12 15:59:29.000000 control-lab-ly-1.0.0b0/src/control_lab_ly.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 15:59:28.000000 control-lab-ly-1.0.0b0/src/control_lab_ly.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      214 2023-04-12 15:59:28.000000 control-lab-ly-1.0.0b0/src/control_lab_ly.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-12 15:59:28.000000 control-lab-ly-1.0.0b0/src/control_lab_ly.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-12 15:59:29.588512 control-lab-ly-1.0.0b0/src/controllably/
-drwxrwxrwx   0        0        0        0 2023-04-12 15:59:29.596525 control-lab-ly-1.0.0b0/src/controllably/Analyse/
-drwxrwxrwx   0        0        0        0 2023-04-12 15:59:29.596525 control-lab-ly-1.0.0b0/src/controllably/Analyse/Data/
-drwxrwxrwx   0        0        0        0 2023-04-12 15:59:29.612525 control-lab-ly-1.0.0b0/src/controllably/Analyse/Data/Database/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b0/src/controllably/Analyse/Data/Database/__init__.py
--rw-rw-rw-   0        0        0     3029 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b0/src/controllably/Analyse/Data/Database/database_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-12 15:59:29.644701 control-lab-ly-1.0.0b0/src/controllably/Analyse/Data/Types/
--rw-rw-rw-   0        0        0      277 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b0/src/controllably/Analyse/Data/Types/__init__.py
--rw-rw-rw-   0        0        0     6448 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b0/src/controllably/Analyse/Data/Types/circuit_datatype.py
--rw-rw-rw-   0        0        0    26583 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b0/src/controllably/Analyse/Data/Types/eis_datatype.py
--rw-rw-rw-   0        0        0      956 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b0/src/controllably/Analyse/Data/Types/eis_test_circuits.yaml
--rw-rw-rw-   0        0        0     1585 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b0/src/controllably/Analyse/Data/Types/eis_tests.json
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b0/src/controllably/Analyse/Data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 15:59:29.661282 control-lab-ly-1.0.0b0/src/controllably/Analyse/Visualisation/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b0/src/controllably/Analyse/Visualisation/__init__.py
--rw-rw-rw-   0        0        0      830 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b0/src/controllably/Analyse/Visualisation/visualisation_utils.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b0/src/controllably/Analyse/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 15:59:29.677673 control-lab-ly-1.0.0b0/src/controllably/Compound/
-drwxrwxrwx   0        0        0        0 2023-04-12 15:59:29.693863 control-lab-ly-1.0.0b0/src/controllably/Compound/LiquidMover/
-drwxrwxrwx   0        0        0        0 2023-04-12 15:59:29.721655 control-lab-ly-1.0.0b0/src/controllably/Compound/LiquidMover/Opentrons/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b0/src/controllably/Compound/LiquidMover/Opentrons/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b0/src/controllably/Compound/LiquidMover/Opentrons/opentrons_utils.py
--rw-rw-rw-   0        0        0      259 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Compound/LiquidMover/__init__.py
--rw-rw-rw-   0        0        0    14057 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Compound/LiquidMover/liquidmover_utils.py
--rw-rw-rw-   0        0        0      241 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Compound/__init__.py
--rw-rw-rw-   0        0        0     8733 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Compound/compound_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-12 15:59:29.734897 control-lab-ly-1.0.0b0/src/controllably/Control/
-drwxrwxrwx   0        0        0        0 2023-04-12 15:59:29.810279 control-lab-ly-1.0.0b0/src/controllably/Control/GUI/
--rw-rw-rw-   0        0        0      516 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Control/GUI/__init__.py
--rw-rw-rw-   0        0        0    30932 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b0/src/controllably/Control/GUI/_guibuilder.py
--rw-rw-rw-   0        0        0    17704 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Control/GUI/gui_utils.py
--rw-rw-rw-   0        0        0      886 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Control/GUI/loader_panel.py
--rw-rw-rw-   0        0        0     8608 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Control/GUI/measurer_panel.py
--rw-rw-rw-   0        0        0    15405 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Control/GUI/mover_panel.py
--rw-rw-rw-   0        0        0     3624 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Control/GUI/viewer_panel.py
-drwxrwxrwx   0        0        0        0 2023-04-12 15:59:29.835322 control-lab-ly-1.0.0b0/src/controllably/Control/Schedule/
--rw-rw-rw-   0        0        0      147 2023-04-11 14:01:57.000000 control-lab-ly-1.0.0b0/src/controllably/Control/Schedule/__init__.py
--rw-rw-rw-   0        0        0     1868 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Control/Schedule/schedule_utils.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b0/src/controllably/Control/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 15:59:29.857550 control-lab-ly-1.0.0b0/src/controllably/Make/
-drwxrwxrwx   0        0        0        0 2023-04-12 15:59:29.894688 control-lab-ly-1.0.0b0/src/controllably/Make/Heat/
--rw-rw-rw-   0        0        0      225 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Make/Heat/__init__.py
--rw-rw-rw-   0        0        0    10393 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Make/Heat/peltier_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-12 15:59:29.920275 control-lab-ly-1.0.0b0/src/controllably/Make/Light/
--rw-rw-rw-   0        0        0      218 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Make/Light/__init__.py
--rw-rw-rw-   0        0        0     9094 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Make/Light/led_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-12 15:59:29.935354 control-lab-ly-1.0.0b0/src/controllably/Make/Mixture/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b0/src/controllably/Make/Mixture/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 15:59:29.950711 control-lab-ly-1.0.0b0/src/controllably/Make/ThinFilm/
--rw-rw-rw-   0        0        0      268 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Make/ThinFilm/__init__.py
--rw-rw-rw-   0        0        0     9660 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Make/ThinFilm/spinner_utils.py
--rw-rw-rw-   0        0        0      217 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Make/__init__.py
--rw-rw-rw-   0        0        0     3956 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Make/make_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.007123 control-lab-ly-1.0.0b0/src/controllably/Measure/
-drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.025165 control-lab-ly-1.0.0b0/src/controllably/Measure/Electrical/
-drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.079009 control-lab-ly-1.0.0b0/src/controllably/Measure/Electrical/Keithley/
--rw-rw-rw-   0        0        0      314 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Measure/Electrical/Keithley/__init__.py
--rw-rw-rw-   0        0        0    18015 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Measure/Electrical/Keithley/keithley_device.py
--rw-rw-rw-   0        0        0     7492 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Measure/Electrical/Keithley/keithley_lib.py
--rw-rw-rw-   0        0        0     2102 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Measure/Electrical/Keithley/keithley_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.099136 control-lab-ly-1.0.0b0/src/controllably/Measure/Electrical/Keithley/programs/
--rw-rw-rw-   0        0        0      401 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Measure/Electrical/Keithley/programs/__init__.py
--rw-rw-rw-   0        0        0    10256 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Measure/Electrical/Keithley/programs/base_programs.py
--rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b0/src/controllably/Measure/Electrical/__init__.py
--rw-rw-rw-   0        0        0      298 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Measure/Electrical/electrical_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.112969 control-lab-ly-1.0.0b0/src/controllably/Measure/Mechanical/
-drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.140213 control-lab-ly-1.0.0b0/src/controllably/Measure/Mechanical/PiezoRobotics/
--rw-rw-rw-   0        0        0      334 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Measure/Mechanical/PiezoRobotics/__init__.py
--rw-rw-rw-   0        0        0    10329 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_device.py
--rw-rw-rw-   0        0        0     3163 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_lib.py
--rw-rw-rw-   0        0        0     2093 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.160646 control-lab-ly-1.0.0b0/src/controllably/Measure/Mechanical/PiezoRobotics/programs/
--rw-rw-rw-   0        0        0      350 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Measure/Mechanical/PiezoRobotics/programs/__init__.py
--rw-rw-rw-   0        0        0     3973 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Measure/Mechanical/PiezoRobotics/programs/base_programs.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b0/src/controllably/Measure/Mechanical/__init__.py
--rw-rw-rw-   0        0        0      298 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Measure/Mechanical/mechanical_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.169356 control-lab-ly-1.0.0b0/src/controllably/Measure/Physical/
--rw-rw-rw-   0        0        0      249 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Measure/Physical/__init__.py
--rw-rw-rw-   0        0        0     7972 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Measure/Physical/balance_utils.py
--rw-rw-rw-   0        0        0      535 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Measure/__init__.py
--rw-rw-rw-   0        0        0     5398 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Measure/instrument_utils.py
--rw-rw-rw-   0        0        0    13804 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Measure/measure_utils.py
--rw-rw-rw-   0        0        0     4176 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Measure/program_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.185407 control-lab-ly-1.0.0b0/src/controllably/Move/
-drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.211676 control-lab-ly-1.0.0b0/src/controllably/Move/Cartesian/
--rw-rw-rw-   0        0        0      346 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Move/Cartesian/__init__.py
--rw-rw-rw-   0        0        0     9049 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Move/Cartesian/cartesian_utils.py
--rw-rw-rw-   0        0        0     3402 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Move/Cartesian/ender_utils.py
--rw-rw-rw-   0        0        0     2853 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Move/Cartesian/primitiv_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.228095 control-lab-ly-1.0.0b0/src/controllably/Move/Jointed/
-drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.248401 control-lab-ly-1.0.0b0/src/controllably/Move/Jointed/Dobot/
--rw-rw-rw-   0        0        0      336 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Move/Jointed/Dobot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.264530 control-lab-ly-1.0.0b0/src/controllably/Move/Jointed/Dobot/dobot_api/
--rw-rw-rw-   0        0        0       62 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b0/src/controllably/Move/Jointed/Dobot/dobot_api/__init__.py
--rw-rw-rw-   0        0        0    24262 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b0/src/controllably/Move/Jointed/Dobot/dobot_api/dobot_api.py
--rw-rw-rw-   0        0        0    15851 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Move/Jointed/Dobot/dobot_utils.py
--rw-rw-rw-   0        0        0     7030 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Move/Jointed/Dobot/m1pro_utils.py
--rw-rw-rw-   0        0        0     4325 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Move/Jointed/Dobot/mg400_utils.py
--rw-rw-rw-   0        0        0      233 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Move/Jointed/__init__.py
--rw-rw-rw-   0        0        0    10507 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Move/Jointed/jointed_utils.py
--rw-rw-rw-   0        0        0      217 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Move/__init__.py
--rw-rw-rw-   0        0        0    32152 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Move/move_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.281075 control-lab-ly-1.0.0b0/src/controllably/Transfer/
-drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.313773 control-lab-ly-1.0.0b0/src/controllably/Transfer/Liquid/
-drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.336095 control-lab-ly-1.0.0b0/src/controllably/Transfer/Liquid/Pumps/
-drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.401096 control-lab-ly-1.0.0b0/src/controllably/Transfer/Liquid/Pumps/TriContinent/
--rw-rw-rw-   0        0        0      255 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Transfer/Liquid/Pumps/TriContinent/__init__.py
--rw-rw-rw-   0        0        0     3460 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_lib.py
--rw-rw-rw-   0        0        0    29831 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_utils.py
--rw-rw-rw-   0        0        0      332 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Transfer/Liquid/Pumps/__init__.py
--rw-rw-rw-   0        0        0     9064 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Transfer/Liquid/Pumps/peristaltic_utils.py
--rw-rw-rw-   0        0        0     3097 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Transfer/Liquid/Pumps/pump_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.446322 control-lab-ly-1.0.0b0/src/controllably/Transfer/Liquid/Sartorius/
--rw-rw-rw-   0        0        0      252 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Transfer/Liquid/Sartorius/__init__.py
--rw-rw-rw-   0        0        0     3210 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Transfer/Liquid/Sartorius/sartorius_lib.py
--rw-rw-rw-   0        0        0    30582 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Transfer/Liquid/Sartorius/sartorius_utils.py
--rw-rw-rw-   0        0        0      364 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Transfer/Liquid/__init__.py
--rw-rw-rw-   0        0        0    13126 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Transfer/Liquid/liquid_utils.py
--rw-rw-rw-   0        0        0     3413 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Transfer/Liquid/syringe_lib.py
--rw-rw-rw-   0        0        0    14619 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Transfer/Liquid/syringe_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.460983 control-lab-ly-1.0.0b0/src/controllably/Transfer/Powder/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b0/src/controllably/Transfer/Powder/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.513402 control-lab-ly-1.0.0b0/src/controllably/Transfer/Substrate/
-drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.529303 control-lab-ly-1.0.0b0/src/controllably/Transfer/Substrate/Dobot/
--rw-rw-rw-   0        0        0      348 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Transfer/Substrate/Dobot/__init__.py
--rw-rw-rw-   0        0        0     8255 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Transfer/Substrate/Dobot/dobot_attachments.py
--rw-rw-rw-   0        0        0      238 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Transfer/Substrate/__init__.py
--rw-rw-rw-   0        0        0     1032 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Transfer/Substrate/substrate_utils.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b0/src/controllably/Transfer/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b0/src/controllably/Transfer/transfer_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.553922 control-lab-ly-1.0.0b0/src/controllably/View/
-drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.570365 control-lab-ly-1.0.0b0/src/controllably/View/Classifiers/
--rw-rw-rw-   0        0        0      333 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/View/Classifiers/__init__.py
--rw-rw-rw-   0        0        0     2586 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/View/Classifiers/classifier_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.586360 control-lab-ly-1.0.0b0/src/controllably/View/Optical/
--rw-rw-rw-   0        0        0      219 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/View/Optical/__init__.py
--rw-rw-rw-   0        0        0     3163 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/View/Optical/optical_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.610419 control-lab-ly-1.0.0b0/src/controllably/View/Optical/placeholders/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b0/src/controllably/View/Optical/placeholders/__init__.py
--rw-rw-rw-   0        0        0    15567 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0b0/src/controllably/View/Optical/placeholders/optical_camera.png
-drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.618961 control-lab-ly-1.0.0b0/src/controllably/View/Thermal/
-drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.627009 control-lab-ly-1.0.0b0/src/controllably/View/Thermal/Flir/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0b0/src/controllably/View/Thermal/Flir/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.667104 control-lab-ly-1.0.0b0/src/controllably/View/Thermal/Flir/ax8/
--rw-rw-rw-   0        0        0       33 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0b0/src/controllably/View/Thermal/Flir/ax8/__init__.py
--rw-rw-rw-   0        0        0    10147 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0b0/src/controllably/View/Thermal/Flir/ax8/ax8.py
--rw-rw-rw-   0        0        0     3821 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0b0/src/controllably/View/Thermal/Flir/ax8/ax8_camera_feed.py
--rw-rw-rw-   0        0        0      636 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0b0/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_regs.py
--rw-rw-rw-   0        0        0      819 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0b0/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_utils.py
--rw-rw-rw-   0        0        0      219 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/View/Thermal/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.683469 control-lab-ly-1.0.0b0/src/controllably/View/Thermal/placeholders/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0b0/src/controllably/View/Thermal/placeholders/__init__.py
--rw-rw-rw-   0        0        0   148660 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0b0/src/controllably/View/Thermal/placeholders/infrared_camera.png
--rw-rw-rw-   0        0        0     2983 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/View/Thermal/thermal_utils.py
--rw-rw-rw-   0        0        0      294 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/View/__init__.py
--rw-rw-rw-   0        0        0    15729 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/View/image_utils.py
--rw-rw-rw-   0        0        0    17366 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/View/view_utils.py
--rw-rw-rw-   0        0        0       98 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.748995 control-lab-ly-1.0.0b0/src/controllably/misc/
--rw-rw-rw-   0        0        0      586 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/misc/__init__.py
--rw-rw-rw-   0        0        0     2522 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/misc/decorators.py
--rw-rw-rw-   0        0        0    10014 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/misc/factory.py
--rw-rw-rw-   0        0        0     6551 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/misc/helper.py
--rw-rw-rw-   0        0        0    17274 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/misc/layout.py
--rw-rw-rw-   0        0        0     2867 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/misc/logger.py
--rw-rw-rw-   0        0        0     4576 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/misc/misc_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.756938 control-lab-ly-1.0.0b0/src/controllably/misc/templates/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0b0/src/controllably/misc/templates/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.779479 control-lab-ly-1.0.0b0/src/controllably/misc/templates/configs/
--rw-rw-rw-   0        0        0        0 2023-02-23 14:08:10.000000 control-lab-ly-1.0.0b0/src/controllably/misc/templates/configs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.830516 control-lab-ly-1.0.0b0/src/controllably/misc/templates/configs/plugins/
--rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b0/src/controllably/misc/templates/configs/plugins/__init__.py
--rw-rw-rw-   0        0        0     1091 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/misc/templates/configs/plugins/plugin_template.py
--rw-rw-rw-   0        0        0      439 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/misc/templates/configs/registry.yaml
-drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.854517 control-lab-ly-1.0.0b0/src/controllably/misc/templates/setup/
--rw-rw-rw-   0        0        0      772 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/misc/templates/setup/__init__.py
--rw-rw-rw-   0        0        0     1434 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/misc/templates/setup/config.yaml
--rw-rw-rw-   0        0        0      987 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/misc/templates/setup/layout.json
-drwxrwxrwx   0        0        0        0 2023-04-12 15:59:31.004546 control-lab-ly-1.0.0b0/tests/
--rw-rw-rw-   0        0        0      189 2023-04-11 09:35:43.000000 control-lab-ly-1.0.0b0/tests/test_camera_optical.py
--rw-rw-rw-   0        0        0      230 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b0/tests/test_camera_thermal.py
--rw-rw-rw-   0        0        0      509 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b0/tests/test_cartesian_ender.py
--rw-rw-rw-   0        0        0      429 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b0/tests/test_cartesian_primitiv.py
--rw-rw-rw-   0        0        0      585 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b0/tests/test_compound_liquidmover.py
--rw-rw-rw-   0        0        0      801 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b0/tests/test_compound_spin_printer.py
--rw-rw-rw-   0        0        0      616 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b0/tests/test_dobot_m1pro.py
--rw-rw-rw-   0        0        0      651 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b0/tests/test_dobot_mg400.py
--rw-rw-rw-   0        0        0      324 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b0/tests/test_electrical_keithley.py
--rw-rw-rw-   0        0        0      392 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b0/tests/test_film_spin.py
--rw-rw-rw-   0        0        0      587 2023-04-11 09:21:52.000000 control-lab-ly-1.0.0b0/tests/test_heat_peltier.py
--rw-rw-rw-   0        0        0      349 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b0/tests/test_light_led_array.py
--rw-rw-rw-   0        0        0      362 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b0/tests/test_liquid_sartorius.py
--rw-rw-rw-   0        0        0      412 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b0/tests/test_liquid_syringe_assembly.py
--rw-rw-rw-   0        0        0      538 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/tests/test_liquid_tricontinent.py
--rw-rw-rw-   0        0        0      239 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b0/tests/test_mechanical_piezorobotics.py
--rw-rw-rw-   0        0        0      268 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b0/tests/test_panels.py
--rw-rw-rw-   0        0        0      273 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b0/tests/test_physical_balance.py
--rw-rw-rw-   0        0        0      337 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b0/tests/test_pump_peristaltic.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:17:50.171707 control-lab-ly-1.0.0b1/
+-rw-rw-rw-   0        0        0     1093 2023-02-24 13:59:16.000000 control-lab-ly-1.0.0b1/LICENSE.md
+-rw-rw-rw-   0        0        0       17 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b1/MANIFEST.in
+-rw-rw-rw-   0        0        0    17453 2023-04-12 16:17:50.171707 control-lab-ly-1.0.0b1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-12 16:17:48.838090 control-lab-ly-1.0.0b1/docs/
+-rw-rw-rw-   0        0        0     4263 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/docs/CHANGELOG.md
+-rw-rw-rw-   0        0        0     5356 2023-02-24 14:06:11.000000 control-lab-ly-1.0.0b1/docs/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0        0        0       33 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0b1/docs/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0     1093 2023-02-24 13:59:16.000000 control-lab-ly-1.0.0b1/docs/LICENSE.md
+-rw-rw-rw-   0        0        0    12070 2023-04-12 16:03:24.000000 control-lab-ly-1.0.0b1/docs/README.md
+-rw-rw-rw-   0        0        0      108 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0b1/pyproject.toml
+-rw-rw-rw-   0        0        0     1561 2023-04-12 16:17:50.179682 control-lab-ly-1.0.0b1/setup.cfg
+-rw-rw-rw-   0        0        0       37 2023-03-10 02:02:34.000000 control-lab-ly-1.0.0b1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:17:48.471823 control-lab-ly-1.0.0b1/src/
+drwxrwxrwx   0        0        0        0 2023-04-12 16:17:48.876290 control-lab-ly-1.0.0b1/src/control_lab_ly.egg-info/
+-rw-rw-rw-   0        0        0    17453 2023-04-12 16:17:48.000000 control-lab-ly-1.0.0b1/src/control_lab_ly.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7306 2023-04-12 16:17:48.000000 control-lab-ly-1.0.0b1/src/control_lab_ly.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 16:17:48.000000 control-lab-ly-1.0.0b1/src/control_lab_ly.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      214 2023-04-12 16:17:48.000000 control-lab-ly-1.0.0b1/src/control_lab_ly.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-12 16:17:48.000000 control-lab-ly-1.0.0b1/src/control_lab_ly.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 16:17:48.888031 control-lab-ly-1.0.0b1/src/controllably/
+drwxrwxrwx   0        0        0        0 2023-04-12 16:17:48.888531 control-lab-ly-1.0.0b1/src/controllably/Analyse/
+drwxrwxrwx   0        0        0        0 2023-04-12 16:17:48.900491 control-lab-ly-1.0.0b1/src/controllably/Analyse/Data/
+drwxrwxrwx   0        0        0        0 2023-04-12 16:17:48.913840 control-lab-ly-1.0.0b1/src/controllably/Analyse/Data/Database/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b1/src/controllably/Analyse/Data/Database/__init__.py
+-rw-rw-rw-   0        0        0     3029 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b1/src/controllably/Analyse/Data/Database/database_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:17:48.969298 control-lab-ly-1.0.0b1/src/controllably/Analyse/Data/Types/
+-rw-rw-rw-   0        0        0      277 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b1/src/controllably/Analyse/Data/Types/__init__.py
+-rw-rw-rw-   0        0        0     6448 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b1/src/controllably/Analyse/Data/Types/circuit_datatype.py
+-rw-rw-rw-   0        0        0    26583 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b1/src/controllably/Analyse/Data/Types/eis_datatype.py
+-rw-rw-rw-   0        0        0      956 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b1/src/controllably/Analyse/Data/Types/eis_test_circuits.yaml
+-rw-rw-rw-   0        0        0     1585 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b1/src/controllably/Analyse/Data/Types/eis_tests.json
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b1/src/controllably/Analyse/Data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:17:48.986690 control-lab-ly-1.0.0b1/src/controllably/Analyse/Visualisation/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b1/src/controllably/Analyse/Visualisation/__init__.py
+-rw-rw-rw-   0        0        0      830 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b1/src/controllably/Analyse/Visualisation/visualisation_utils.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b1/src/controllably/Analyse/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.000168 control-lab-ly-1.0.0b1/src/controllably/Compound/
+drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.008764 control-lab-ly-1.0.0b1/src/controllably/Compound/LiquidMover/
+drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.032998 control-lab-ly-1.0.0b1/src/controllably/Compound/LiquidMover/Opentrons/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b1/src/controllably/Compound/LiquidMover/Opentrons/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b1/src/controllably/Compound/LiquidMover/Opentrons/opentrons_utils.py
+-rw-rw-rw-   0        0        0      259 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Compound/LiquidMover/__init__.py
+-rw-rw-rw-   0        0        0    14057 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Compound/LiquidMover/liquidmover_utils.py
+-rw-rw-rw-   0        0        0      241 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Compound/__init__.py
+-rw-rw-rw-   0        0        0     8733 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Compound/compound_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.041011 control-lab-ly-1.0.0b1/src/controllably/Control/
+drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.088431 control-lab-ly-1.0.0b1/src/controllably/Control/GUI/
+-rw-rw-rw-   0        0        0      516 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Control/GUI/__init__.py
+-rw-rw-rw-   0        0        0    30932 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b1/src/controllably/Control/GUI/_guibuilder.py
+-rw-rw-rw-   0        0        0    17704 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Control/GUI/gui_utils.py
+-rw-rw-rw-   0        0        0      886 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Control/GUI/loader_panel.py
+-rw-rw-rw-   0        0        0     8608 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Control/GUI/measurer_panel.py
+-rw-rw-rw-   0        0        0    15405 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Control/GUI/mover_panel.py
+-rw-rw-rw-   0        0        0     3624 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Control/GUI/viewer_panel.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.104577 control-lab-ly-1.0.0b1/src/controllably/Control/Schedule/
+-rw-rw-rw-   0        0        0      147 2023-04-11 14:01:57.000000 control-lab-ly-1.0.0b1/src/controllably/Control/Schedule/__init__.py
+-rw-rw-rw-   0        0        0     1868 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Control/Schedule/schedule_utils.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b1/src/controllably/Control/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.138113 control-lab-ly-1.0.0b1/src/controllably/Make/
+drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.161937 control-lab-ly-1.0.0b1/src/controllably/Make/Heat/
+-rw-rw-rw-   0        0        0      225 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Make/Heat/__init__.py
+-rw-rw-rw-   0        0        0    10393 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Make/Heat/peltier_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.180861 control-lab-ly-1.0.0b1/src/controllably/Make/Light/
+-rw-rw-rw-   0        0        0      218 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Make/Light/__init__.py
+-rw-rw-rw-   0        0        0     9094 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Make/Light/led_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.192798 control-lab-ly-1.0.0b1/src/controllably/Make/Mixture/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b1/src/controllably/Make/Mixture/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.204931 control-lab-ly-1.0.0b1/src/controllably/Make/ThinFilm/
+-rw-rw-rw-   0        0        0      268 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Make/ThinFilm/__init__.py
+-rw-rw-rw-   0        0        0     9660 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Make/ThinFilm/spinner_utils.py
+-rw-rw-rw-   0        0        0      217 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Make/__init__.py
+-rw-rw-rw-   0        0        0     3956 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Make/make_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.242247 control-lab-ly-1.0.0b1/src/controllably/Measure/
+drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.258192 control-lab-ly-1.0.0b1/src/controllably/Measure/Electrical/
+drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.297193 control-lab-ly-1.0.0b1/src/controllably/Measure/Electrical/Keithley/
+-rw-rw-rw-   0        0        0      314 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Measure/Electrical/Keithley/__init__.py
+-rw-rw-rw-   0        0        0    18015 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Measure/Electrical/Keithley/keithley_device.py
+-rw-rw-rw-   0        0        0     7492 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Measure/Electrical/Keithley/keithley_lib.py
+-rw-rw-rw-   0        0        0     2102 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Measure/Electrical/Keithley/keithley_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.347618 control-lab-ly-1.0.0b1/src/controllably/Measure/Electrical/Keithley/programs/
+-rw-rw-rw-   0        0        0      401 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Measure/Electrical/Keithley/programs/__init__.py
+-rw-rw-rw-   0        0        0    10256 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Measure/Electrical/Keithley/programs/base_programs.py
+-rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b1/src/controllably/Measure/Electrical/__init__.py
+-rw-rw-rw-   0        0        0      298 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Measure/Electrical/electrical_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.364957 control-lab-ly-1.0.0b1/src/controllably/Measure/Mechanical/
+drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.400897 control-lab-ly-1.0.0b1/src/controllably/Measure/Mechanical/PiezoRobotics/
+-rw-rw-rw-   0        0        0      334 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Measure/Mechanical/PiezoRobotics/__init__.py
+-rw-rw-rw-   0        0        0    10329 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_device.py
+-rw-rw-rw-   0        0        0     3163 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_lib.py
+-rw-rw-rw-   0        0        0     2093 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.427094 control-lab-ly-1.0.0b1/src/controllably/Measure/Mechanical/PiezoRobotics/programs/
+-rw-rw-rw-   0        0        0      350 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Measure/Mechanical/PiezoRobotics/programs/__init__.py
+-rw-rw-rw-   0        0        0     3973 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Measure/Mechanical/PiezoRobotics/programs/base_programs.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b1/src/controllably/Measure/Mechanical/__init__.py
+-rw-rw-rw-   0        0        0      298 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Measure/Mechanical/mechanical_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.439540 control-lab-ly-1.0.0b1/src/controllably/Measure/Physical/
+-rw-rw-rw-   0        0        0      249 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Measure/Physical/__init__.py
+-rw-rw-rw-   0        0        0     7972 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Measure/Physical/balance_utils.py
+-rw-rw-rw-   0        0        0      535 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Measure/__init__.py
+-rw-rw-rw-   0        0        0     5398 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Measure/instrument_utils.py
+-rw-rw-rw-   0        0        0    13804 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Measure/measure_utils.py
+-rw-rw-rw-   0        0        0     4176 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Measure/program_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.453245 control-lab-ly-1.0.0b1/src/controllably/Move/
+drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.488972 control-lab-ly-1.0.0b1/src/controllably/Move/Cartesian/
+-rw-rw-rw-   0        0        0      346 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Move/Cartesian/__init__.py
+-rw-rw-rw-   0        0        0     9049 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Move/Cartesian/cartesian_utils.py
+-rw-rw-rw-   0        0        0     3402 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Move/Cartesian/ender_utils.py
+-rw-rw-rw-   0        0        0     2853 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Move/Cartesian/primitiv_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.497074 control-lab-ly-1.0.0b1/src/controllably/Move/Jointed/
+drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.528975 control-lab-ly-1.0.0b1/src/controllably/Move/Jointed/Dobot/
+-rw-rw-rw-   0        0        0      336 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Move/Jointed/Dobot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.543968 control-lab-ly-1.0.0b1/src/controllably/Move/Jointed/Dobot/dobot_api/
+-rw-rw-rw-   0        0        0       62 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b1/src/controllably/Move/Jointed/Dobot/dobot_api/__init__.py
+-rw-rw-rw-   0        0        0    24262 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b1/src/controllably/Move/Jointed/Dobot/dobot_api/dobot_api.py
+-rw-rw-rw-   0        0        0    15851 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Move/Jointed/Dobot/dobot_utils.py
+-rw-rw-rw-   0        0        0     7030 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Move/Jointed/Dobot/m1pro_utils.py
+-rw-rw-rw-   0        0        0     4325 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Move/Jointed/Dobot/mg400_utils.py
+-rw-rw-rw-   0        0        0      233 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Move/Jointed/__init__.py
+-rw-rw-rw-   0        0        0    10507 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Move/Jointed/jointed_utils.py
+-rw-rw-rw-   0        0        0      217 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Move/__init__.py
+-rw-rw-rw-   0        0        0    32152 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Move/move_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.563012 control-lab-ly-1.0.0b1/src/controllably/Transfer/
+drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.594517 control-lab-ly-1.0.0b1/src/controllably/Transfer/Liquid/
+drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.612438 control-lab-ly-1.0.0b1/src/controllably/Transfer/Liquid/Pumps/
+drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.637624 control-lab-ly-1.0.0b1/src/controllably/Transfer/Liquid/Pumps/TriContinent/
+-rw-rw-rw-   0        0        0      255 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Transfer/Liquid/Pumps/TriContinent/__init__.py
+-rw-rw-rw-   0        0        0     3460 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_lib.py
+-rw-rw-rw-   0        0        0    29831 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_utils.py
+-rw-rw-rw-   0        0        0      332 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Transfer/Liquid/Pumps/__init__.py
+-rw-rw-rw-   0        0        0     9064 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Transfer/Liquid/Pumps/peristaltic_utils.py
+-rw-rw-rw-   0        0        0     3097 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Transfer/Liquid/Pumps/pump_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.669182 control-lab-ly-1.0.0b1/src/controllably/Transfer/Liquid/Sartorius/
+-rw-rw-rw-   0        0        0      252 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Transfer/Liquid/Sartorius/__init__.py
+-rw-rw-rw-   0        0        0     3210 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Transfer/Liquid/Sartorius/sartorius_lib.py
+-rw-rw-rw-   0        0        0    30582 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Transfer/Liquid/Sartorius/sartorius_utils.py
+-rw-rw-rw-   0        0        0      364 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Transfer/Liquid/__init__.py
+-rw-rw-rw-   0        0        0    13126 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Transfer/Liquid/liquid_utils.py
+-rw-rw-rw-   0        0        0     3413 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Transfer/Liquid/syringe_lib.py
+-rw-rw-rw-   0        0        0    14619 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Transfer/Liquid/syringe_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.677392 control-lab-ly-1.0.0b1/src/controllably/Transfer/Powder/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b1/src/controllably/Transfer/Powder/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.691909 control-lab-ly-1.0.0b1/src/controllably/Transfer/Substrate/
+drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.709325 control-lab-ly-1.0.0b1/src/controllably/Transfer/Substrate/Dobot/
+-rw-rw-rw-   0        0        0      348 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Transfer/Substrate/Dobot/__init__.py
+-rw-rw-rw-   0        0        0     8255 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Transfer/Substrate/Dobot/dobot_attachments.py
+-rw-rw-rw-   0        0        0      238 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Transfer/Substrate/__init__.py
+-rw-rw-rw-   0        0        0     1032 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/Transfer/Substrate/substrate_utils.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b1/src/controllably/Transfer/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b1/src/controllably/Transfer/transfer_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.726902 control-lab-ly-1.0.0b1/src/controllably/View/
+drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.789816 control-lab-ly-1.0.0b1/src/controllably/View/Classifiers/
+-rw-rw-rw-   0        0        0      333 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/View/Classifiers/__init__.py
+-rw-rw-rw-   0        0        0     2586 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/View/Classifiers/classifier_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.807821 control-lab-ly-1.0.0b1/src/controllably/View/Optical/
+-rw-rw-rw-   0        0        0      219 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/View/Optical/__init__.py
+-rw-rw-rw-   0        0        0     3163 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/View/Optical/optical_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.822632 control-lab-ly-1.0.0b1/src/controllably/View/Optical/placeholders/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b1/src/controllably/View/Optical/placeholders/__init__.py
+-rw-rw-rw-   0        0        0    15567 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0b1/src/controllably/View/Optical/placeholders/optical_camera.png
+drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.840468 control-lab-ly-1.0.0b1/src/controllably/View/Thermal/
+drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.840468 control-lab-ly-1.0.0b1/src/controllably/View/Thermal/Flir/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0b1/src/controllably/View/Thermal/Flir/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.892068 control-lab-ly-1.0.0b1/src/controllably/View/Thermal/Flir/ax8/
+-rw-rw-rw-   0        0        0       33 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0b1/src/controllably/View/Thermal/Flir/ax8/__init__.py
+-rw-rw-rw-   0        0        0    10147 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0b1/src/controllably/View/Thermal/Flir/ax8/ax8.py
+-rw-rw-rw-   0        0        0     3821 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0b1/src/controllably/View/Thermal/Flir/ax8/ax8_camera_feed.py
+-rw-rw-rw-   0        0        0      636 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0b1/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_regs.py
+-rw-rw-rw-   0        0        0      819 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0b1/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_utils.py
+-rw-rw-rw-   0        0        0      219 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/View/Thermal/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.901301 control-lab-ly-1.0.0b1/src/controllably/View/Thermal/placeholders/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0b1/src/controllably/View/Thermal/placeholders/__init__.py
+-rw-rw-rw-   0        0        0   148660 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0b1/src/controllably/View/Thermal/placeholders/infrared_camera.png
+-rw-rw-rw-   0        0        0     2983 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/View/Thermal/thermal_utils.py
+-rw-rw-rw-   0        0        0      294 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/View/__init__.py
+-rw-rw-rw-   0        0        0    15729 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/View/image_utils.py
+-rw-rw-rw-   0        0        0    17366 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/View/view_utils.py
+-rw-rw-rw-   0        0        0       98 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.953432 control-lab-ly-1.0.0b1/src/controllably/misc/
+-rw-rw-rw-   0        0        0      586 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/misc/__init__.py
+-rw-rw-rw-   0        0        0     2522 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/misc/decorators.py
+-rw-rw-rw-   0        0        0    10014 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/misc/factory.py
+-rw-rw-rw-   0        0        0     6551 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/misc/helper.py
+-rw-rw-rw-   0        0        0    17274 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/misc/layout.py
+-rw-rw-rw-   0        0        0     2867 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/misc/logger.py
+-rw-rw-rw-   0        0        0     4576 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/misc/misc_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.961830 control-lab-ly-1.0.0b1/src/controllably/misc/templates/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0b1/src/controllably/misc/templates/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.970917 control-lab-ly-1.0.0b1/src/controllably/misc/templates/configs/
+-rw-rw-rw-   0        0        0        0 2023-02-23 14:08:10.000000 control-lab-ly-1.0.0b1/src/controllably/misc/templates/configs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:17:49.996091 control-lab-ly-1.0.0b1/src/controllably/misc/templates/configs/plugins/
+-rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b1/src/controllably/misc/templates/configs/plugins/__init__.py
+-rw-rw-rw-   0        0        0     1091 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/misc/templates/configs/plugins/plugin_template.py
+-rw-rw-rw-   0        0        0      439 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/misc/templates/configs/registry.yaml
+drwxrwxrwx   0        0        0        0 2023-04-12 16:17:50.018630 control-lab-ly-1.0.0b1/src/controllably/misc/templates/setup/
+-rw-rw-rw-   0        0        0      772 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/misc/templates/setup/__init__.py
+-rw-rw-rw-   0        0        0     1434 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/misc/templates/setup/config.yaml
+-rw-rw-rw-   0        0        0      987 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/src/controllably/misc/templates/setup/layout.json
+drwxrwxrwx   0        0        0        0 2023-04-12 16:17:50.163669 control-lab-ly-1.0.0b1/tests/
+-rw-rw-rw-   0        0        0      189 2023-04-11 09:35:43.000000 control-lab-ly-1.0.0b1/tests/test_camera_optical.py
+-rw-rw-rw-   0        0        0      230 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b1/tests/test_camera_thermal.py
+-rw-rw-rw-   0        0        0      509 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b1/tests/test_cartesian_ender.py
+-rw-rw-rw-   0        0        0      429 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b1/tests/test_cartesian_primitiv.py
+-rw-rw-rw-   0        0        0      585 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b1/tests/test_compound_liquidmover.py
+-rw-rw-rw-   0        0        0      801 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b1/tests/test_compound_spin_printer.py
+-rw-rw-rw-   0        0        0      616 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b1/tests/test_dobot_m1pro.py
+-rw-rw-rw-   0        0        0      651 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b1/tests/test_dobot_mg400.py
+-rw-rw-rw-   0        0        0      324 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b1/tests/test_electrical_keithley.py
+-rw-rw-rw-   0        0        0      392 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b1/tests/test_film_spin.py
+-rw-rw-rw-   0        0        0      587 2023-04-11 09:21:52.000000 control-lab-ly-1.0.0b1/tests/test_heat_peltier.py
+-rw-rw-rw-   0        0        0      349 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b1/tests/test_light_led_array.py
+-rw-rw-rw-   0        0        0      362 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b1/tests/test_liquid_sartorius.py
+-rw-rw-rw-   0        0        0      412 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b1/tests/test_liquid_syringe_assembly.py
+-rw-rw-rw-   0        0        0      538 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b1/tests/test_liquid_tricontinent.py
+-rw-rw-rw-   0        0        0      239 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b1/tests/test_mechanical_piezorobotics.py
+-rw-rw-rw-   0        0        0      268 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b1/tests/test_panels.py
+-rw-rw-rw-   0        0        0      273 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b1/tests/test_physical_balance.py
+-rw-rw-rw-   0        0        0      337 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b1/tests/test_pump_peristaltic.py
```

### Comparing `control-lab-ly-1.0.0b0/LICENSE.md` & `control-lab-ly-1.0.0b1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/PKG-INFO` & `control-lab-ly-1.0.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: control-lab-ly
-Version: 1.0.0b0
+Version: 1.0.0b1
 Summary: Lab Equipment Automation Package
 Home-page: https://github.com/kylejeanlewis/control-lab-le
 Author: Chang Jie Leong
 Author-email: changjie.leong@outlook.com
 License: MIT
 Project-URL: GitHub, https://github.com/kylejeanlewis/control-lab-le
 Project-URL: Documentation, https://github.com/kylejeanlewis/control-lab-le/blob/main/docs/README.md
@@ -89,15 +89,15 @@
 ```shell
 $ python -m pydoc controllably.Move
 ```
 
 >Tip: when using Interactive Python (IPython) (e.g. Jupyter notebooks), add a exclamation mark (`!`) in front of the shell command
 ```python
 >>> !python -m pydoc controllably.Move
->>> !python -m pydoc -b                 # Generates a static HTML site to browse package documentation
+>>> !python -m pydoc -b   # Generates a static HTML site to browse package documentation
 ```
 For basic usage, this is all you need to know. Check the documentation for more details on each respective class.
 
 ---
 
 ## Advanced Usage
 For more advanced uses, Control.lab.ly provides a host of tools to streamline the development of lab equipment automation.
@@ -128,20 +128,20 @@
 print(lab.Helper.get_node())
 ```
 
 A template of `registry.yaml` has also been added to the folder to hold the machine-specific addresses of your connected devices (i.e. COM ports).\
 Populate the YAML file in the format shown below.
 ```yaml
 ### registry.yaml ###
-'012345678901234':              # insert your machine's 15-digit ID here (from the above step)
-    cam_index:                  # camera index of the connected imaging devices
-      __cam_01__: 1             # keep the leading and trailing double underscores
+'012345678901234':          # insert your machine's 15-digit ID here (from the above step)
+    cam_index:              # camera index of the connected imaging devices
+      __cam_01__: 1         # keep the leading and trailing double underscores
       __cam_02__: 0
-    port:                       # addresses of serial COM ports
-      __device_01__: COM3       # keep the leading and trailing double underscores
+    port:                   # addresses of serial COM ports
+      __device_01__: COM3   # keep the leading and trailing double underscores
       __device_02__: COM16
 ```
 
 To find the COM port address(es) of the device(s) that is/are currently connected to your machine, use:
 ```python
 lab.Helper.get_ports()
 ```
@@ -166,30 +166,30 @@
     port: __device_01__                         # port addresses defined in registry.yaml
     _setting_A_: {'tuple': [300,0,200]}         # use keys to define the type of iterable
     _setting_B_: {'array': [[0,1,0],[-1,0,0]]}  # only tuple and np.array supported
 ```
 
 `Compound` devices are similarly configured. The configuration values for its component devices are defined under the `component_config` setting. The structure of the configuration values for the component devices are similar to that shown above, except indented to fall under the indentation of the `component_config` setting.
 ```yaml
-_Device02_:                                     # name of 'Compound' device (user-defined)
+_Device02_:                                 # name of 'Compound' device (user-defined)
   module: Compound                            
   class: _submodule_2A_._class_2A_
   settings:
-    _setting_C_: 1                              # other settings for your 'Compound' device
-    component_config:                           # nest component configuration settings here
-      _Component01_:                            # name of component
+    _setting_C_: 1                          # other settings for your 'Compound' device
+    component_config:                       # nest component configuration settings here
+      _Component01_:                        # name of component
         module: _module_name_03_
         class: _submodule_3A_._class_3A_
         settings:
-          ip_address: '192.0.0.1'               # IP addresses do not vary between machines
+          ip_address: '192.0.0.1'           # IP addresses do not vary between machines
       _Component02_: 
         module: _module_name_04_
         class: _submodule_4A_._class_4A_
         settings:
-          _setting_D_: 2                        # settings for your component device
+          _setting_D_: 2                    # settings for your component device
 ```
 
 Lastly, you can define shortcuts to quickly access components of `Compound` devices.
 ```yaml
 SHORTCUTS:
   _Nickname1_: '_Device02_._Component01_'
   _Nickname2_: '_Device02_._Component02_'
```

### Comparing `control-lab-ly-1.0.0b0/docs/CHANGELOG.md` & `control-lab-ly-1.0.0b1/docs/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/docs/CODE_OF_CONDUCT.md` & `control-lab-ly-1.0.0b1/docs/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/docs/LICENSE.md` & `control-lab-ly-1.0.0b1/docs/LICENSE.md`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/docs/README.md` & `control-lab-ly-1.0.0b1/docs/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 ```shell
 $ python -m pydoc controllably.Move
 ```
 
 >Tip: when using Interactive Python (IPython) (e.g. Jupyter notebooks), add a exclamation mark (`!`) in front of the shell command
 ```python
 >>> !python -m pydoc controllably.Move
->>> !python -m pydoc -b                 # Generates a static HTML site to browse package documentation
+>>> !python -m pydoc -b   # Generates a static HTML site to browse package documentation
 ```
 For basic usage, this is all you need to know. Check the documentation for more details on each respective class.
 
 ---
 
 ## Advanced Usage
 For more advanced uses, Control.lab.ly provides a host of tools to streamline the development of lab equipment automation.
@@ -103,20 +103,20 @@
 print(lab.Helper.get_node())
 ```
 
 A template of `registry.yaml` has also been added to the folder to hold the machine-specific addresses of your connected devices (i.e. COM ports).\
 Populate the YAML file in the format shown below.
 ```yaml
 ### registry.yaml ###
-'012345678901234':              # insert your machine's 15-digit ID here (from the above step)
-    cam_index:                  # camera index of the connected imaging devices
-      __cam_01__: 1             # keep the leading and trailing double underscores
+'012345678901234':          # insert your machine's 15-digit ID here (from the above step)
+    cam_index:              # camera index of the connected imaging devices
+      __cam_01__: 1         # keep the leading and trailing double underscores
       __cam_02__: 0
-    port:                       # addresses of serial COM ports
-      __device_01__: COM3       # keep the leading and trailing double underscores
+    port:                   # addresses of serial COM ports
+      __device_01__: COM3   # keep the leading and trailing double underscores
       __device_02__: COM16
 ```
 
 To find the COM port address(es) of the device(s) that is/are currently connected to your machine, use:
 ```python
 lab.Helper.get_ports()
 ```
@@ -141,30 +141,30 @@
     port: __device_01__                         # port addresses defined in registry.yaml
     _setting_A_: {'tuple': [300,0,200]}         # use keys to define the type of iterable
     _setting_B_: {'array': [[0,1,0],[-1,0,0]]}  # only tuple and np.array supported
 ```
 
 `Compound` devices are similarly configured. The configuration values for its component devices are defined under the `component_config` setting. The structure of the configuration values for the component devices are similar to that shown above, except indented to fall under the indentation of the `component_config` setting.
 ```yaml
-_Device02_:                                     # name of 'Compound' device (user-defined)
+_Device02_:                                 # name of 'Compound' device (user-defined)
   module: Compound                            
   class: _submodule_2A_._class_2A_
   settings:
-    _setting_C_: 1                              # other settings for your 'Compound' device
-    component_config:                           # nest component configuration settings here
-      _Component01_:                            # name of component
+    _setting_C_: 1                          # other settings for your 'Compound' device
+    component_config:                       # nest component configuration settings here
+      _Component01_:                        # name of component
         module: _module_name_03_
         class: _submodule_3A_._class_3A_
         settings:
-          ip_address: '192.0.0.1'               # IP addresses do not vary between machines
+          ip_address: '192.0.0.1'           # IP addresses do not vary between machines
       _Component02_: 
         module: _module_name_04_
         class: _submodule_4A_._class_4A_
         settings:
-          _setting_D_: 2                        # settings for your component device
+          _setting_D_: 2                    # settings for your component device
 ```
 
 Lastly, you can define shortcuts to quickly access components of `Compound` devices.
 ```yaml
 SHORTCUTS:
   _Nickname1_: '_Device02_._Component01_'
   _Nickname2_: '_Device02_._Component02_'
```

### Comparing `control-lab-ly-1.0.0b0/setup.cfg` & `control-lab-ly-1.0.0b1/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,98 +1,98 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2063 6f6e 7472 6f6c 2d6c 6162 2d6c   = control-lab-l
 00000020: 790d 0a76 6572 7369 6f6e 203d 2031 2e30  y..version = 1.0
-00000030: 2e30 2d62 0d0a 6465 7363 7269 7074 696f  .0-b..descriptio
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
+00000030: 2e30 2d62 2e31 0d0a 6465 7363 7269 7074  .0-b.1..descript
+00000040: 696f 6e20 3d20 4c61 6220 4571 7569 706d  ion = Lab Equipm
+00000050: 656e 7420 4175 746f 6d61 7469 6f6e 2050  ent Automation P
+00000060: 6163 6b61 6765 0d0a 6c6f 6e67 5f64 6573  ackage..long_des
+00000070: 6372 6970 7469 6f6e 203d 2066 696c 653a  cription = file:
+00000080: 2064 6f63 732f 5245 4144 4d45 2e6d 642c   docs/README.md,
+00000090: 2064 6f63 732f 4348 414e 4745 4c4f 472e   docs/CHANGELOG.
+000000a0: 6d64 0d0a 6c6f 6e67 5f64 6573 6372 6970  md..long_descrip
+000000b0: 7469 6f6e 5f63 6f6e 7465 6e74 5f74 7970  tion_content_typ
+000000c0: 6520 3d20 7465 7874 2f6d 6172 6b64 6f77  e = text/markdow
+000000d0: 6e0d 0a61 7574 686f 7220 3d20 4368 616e  n..author = Chan
+000000e0: 6720 4a69 6520 4c65 6f6e 670d 0a61 7574  g Jie Leong..aut
+000000f0: 686f 725f 656d 6169 6c20 3d20 6368 616e  hor_email = chan
+00000100: 676a 6965 2e6c 656f 6e67 406f 7574 6c6f  gjie.leong@outlo
+00000110: 6f6b 2e63 6f6d 0d0a 7572 6c20 3d20 6874  ok.com..url = ht
+00000120: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000130: 2f6b 796c 656a 6561 6e6c 6577 6973 2f63  /kylejeanlewis/c
+00000140: 6f6e 7472 6f6c 2d6c 6162 2d6c 650d 0a70  ontrol-lab-le..p
+00000150: 726f 6a65 6374 5f75 726c 7320 3d20 0d0a  roject_urls = ..
+00000160: 0947 6974 4875 6220 3d20 6874 7470 733a  .GitHub = https:
+00000170: 2f2f 6769 7468 7562 2e63 6f6d 2f6b 796c  //github.com/kyl
+00000180: 656a 6561 6e6c 6577 6973 2f63 6f6e 7472  ejeanlewis/contr
+00000190: 6f6c 2d6c 6162 2d6c 650d 0a09 446f 6375  ol-lab-le...Docu
+000001a0: 6d65 6e74 6174 696f 6e20 3d20 6874 7470  mentation = http
+000001b0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6b  s://github.com/k
+000001c0: 796c 656a 6561 6e6c 6577 6973 2f63 6f6e  ylejeanlewis/con
+000001d0: 7472 6f6c 2d6c 6162 2d6c 652f 626c 6f62  trol-lab-le/blob
+000001e0: 2f6d 6169 6e2f 646f 6373 2f52 4541 444d  /main/docs/READM
+000001f0: 452e 6d64 0d0a 0943 6861 6e67 656c 6f67  E.md...Changelog
+00000200: 203d 2068 7474 7073 3a2f 2f67 6974 6875   = https://githu
+00000210: 622e 636f 6d2f 6b79 6c65 6a65 616e 6c65  b.com/kylejeanle
+00000220: 7769 732f 636f 6e74 726f 6c2d 6c61 622d  wis/control-lab-
+00000230: 6c65 2f62 6c6f 622f 6d61 696e 2f64 6f63  le/blob/main/doc
+00000240: 732f 4348 414e 4745 4c4f 472e 6d64 0d0a  s/CHANGELOG.md..
+00000250: 0954 7261 636b 6572 203d 2068 7474 7073  .Tracker = https
+00000260: 3a2f 2f67 6974 6875 622e 636f 6d2f 6b79  ://github.com/ky
+00000270: 6c65 6a65 616e 6c65 7769 732f 636f 6e74  lejeanlewis/cont
+00000280: 726f 6c2d 6c61 622d 6c65 2f69 7373 7565  rol-lab-le/issue
+00000290: 730d 0a6c 6963 656e 7365 203d 204d 4954  s..license = MIT
+000002a0: 0d0a 6b65 7977 6f72 6473 203d 200d 0a09  ..keywords = ...
+000002b0: 7079 7468 6f6e 0d0a 096c 6162 2061 7574  python...lab aut
+000002c0: 6f6d 6174 696f 6e0d 0a63 6c61 7373 6966  omation..classif
+000002d0: 6965 7273 203d 200d 0a09 4465 7665 6c6f  iers = ...Develo
+000002e0: 706d 656e 7420 5374 6174 7573 203a 3a20  pment Status :: 
+000002f0: 3320 2d20 416c 7068 610d 0a09 496e 7465  3 - Alpha...Inte
+00000300: 6e64 6564 2041 7564 6965 6e63 6520 3a3a  nded Audience ::
+00000310: 2044 6576 656c 6f70 6572 730d 0a09 496e   Developers...In
+00000320: 7465 6e64 6564 2041 7564 6965 6e63 6520  tended Audience 
+00000330: 3a3a 2053 6369 656e 6365 2f52 6573 6561  :: Science/Resea
+00000340: 7263 680d 0a09 4c69 6365 6e73 6520 3a3a  rch...License ::
+00000350: 204f 5349 2041 7070 726f 7665 6420 3a3a   OSI Approved ::
+00000360: 204d 4954 204c 6963 656e 7365 0d0a 094f   MIT License...O
+00000370: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
+00000380: 3a3a 204d 6963 726f 736f 6674 203a 3a20  :: Microsoft :: 
+00000390: 5769 6e64 6f77 730d 0a09 5072 6f67 7261  Windows...Progra
+000003a0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+000003b0: 3a20 5079 7468 6f6e 203a 3a20 330d 0a09  : Python :: 3...
+000003c0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+000003d0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+000003e0: 3a20 332e 380d 0a09 546f 7069 6320 3a3a  : 3.8...Topic ::
+000003f0: 2053 6369 656e 7469 6669 632f 456e 6769   Scientific/Engi
+00000400: 6e65 6572 696e 670d 0a0d 0a5b 6f70 7469  neering....[opti
+00000410: 6f6e 735d 0d0a 7061 636b 6167 655f 6469  ons]..package_di
+00000420: 7220 3d20 0d0a 093d 2073 7263 0d0a 7061  r = ...= src..pa
+00000430: 636b 6167 6573 203d 2066 696e 643a 0d0a  ckages = find:..
+00000440: 696e 636c 7564 655f 7061 636b 6167 655f  include_package_
+00000450: 6461 7461 203d 2054 7275 650d 0a70 7974  data = True..pyt
+00000460: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
+00000470: 3d33 2e38 0d0a 696e 7374 616c 6c5f 7265  =3.8..install_re
+00000480: 7175 6972 6573 203d 200d 0a09 6461 7368  quires = ...dash
+00000490: 3e3d 322e 370d 0a09 696d 7065 6461 6e63  >=2.7...impedanc
+000004a0: 653e 3d31 2e34 0d0a 0969 6d75 7469 6c73  e>=1.4...imutils
+000004b0: 3e3d 302e 350d 0a09 6d61 7470 6c6f 746c  >=0.5...matplotl
+000004c0: 6962 3e3d 332e 330d 0a09 6e65 7374 5f61  ib>=3.3...nest_a
+000004d0: 7379 6e63 696f 3e3d 312e 350d 0a09 6e75  syncio>=1.5...nu
+000004e0: 6d70 793e 3d31 2e31 390d 0a09 6f70 656e  mpy>=1.19...open
+000004f0: 6376 5f70 7974 686f 6e3e 3d34 2e35 2e30  cv_python>=4.5.0
+00000500: 0d0a 0970 616e 6461 733e 3d31 2e32 0d0a  ...pandas>=1.2..
+00000510: 0970 6c6f 746c 793e 3d35 2e33 0d0a 0970  .plotly>=5.3...p
+00000520: 794d 6f64 6275 7354 4350 3e3d 302e 320d  yModbusTCP>=0.2.
+00000530: 0a09 7079 7365 7269 616c 3e3d 332e 350d  ..pyserial>=3.5.
+00000540: 0a09 5079 5369 6d70 6c65 4755 493e 3d34  ..PySimpleGUI>=4
+00000550: 2e36 300d 0a09 5079 5649 5341 3e3d 312e  .60...PyVISA>=1.
+00000560: 3132 0d0a 0950 7959 414d 4c3e 3d36 2e30  12...PyYAML>=6.0
+00000570: 0d0a 0973 6369 7079 3e3d 312e 360d 0a0d  ...scipy>=1.6...
+00000580: 0a5b 6f70 7469 6f6e 732e 7061 636b 6167  .[options.packag
+00000590: 6573 2e66 696e 645d 0d0a 7768 6572 6520  es.find]..where 
+000005a0: 3d20 7372 630d 0a65 7863 6c75 6465 203d  = src..exclude =
+000005b0: 2074 6573 7473 0d0a 0d0a 5b6f 7074 696f   tests....[optio
+000005c0: 6e73 2e70 6163 6b61 6765 5f64 6174 615d  ns.package_data]
+000005d0: 0d0a 2a20 3d20 2a2e 6a73 6f6e 2c20 2a2e  ..* = *.json, *.
+000005e0: 7961 6d6c 2c20 2a2e 706e 670d 0a0d 0a5b  yaml, *.png....[
+000005f0: 6567 675f 696e 666f 5d0d 0a74 6167 5f62  egg_info]..tag_b
+00000600: 7569 6c64 203d 200d 0a74 6167 5f64 6174  uild = ..tag_dat
+00000610: 6520 3d20 300d 0a0d 0a                   e = 0....
```

### Comparing `control-lab-ly-1.0.0b0/src/control_lab_ly.egg-info/PKG-INFO` & `control-lab-ly-1.0.0b1/src/control_lab_ly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: control-lab-ly
-Version: 1.0.0b0
+Version: 1.0.0b1
 Summary: Lab Equipment Automation Package
 Home-page: https://github.com/kylejeanlewis/control-lab-le
 Author: Chang Jie Leong
 Author-email: changjie.leong@outlook.com
 License: MIT
 Project-URL: GitHub, https://github.com/kylejeanlewis/control-lab-le
 Project-URL: Documentation, https://github.com/kylejeanlewis/control-lab-le/blob/main/docs/README.md
@@ -89,15 +89,15 @@
 ```shell
 $ python -m pydoc controllably.Move
 ```
 
 >Tip: when using Interactive Python (IPython) (e.g. Jupyter notebooks), add a exclamation mark (`!`) in front of the shell command
 ```python
 >>> !python -m pydoc controllably.Move
->>> !python -m pydoc -b                 # Generates a static HTML site to browse package documentation
+>>> !python -m pydoc -b   # Generates a static HTML site to browse package documentation
 ```
 For basic usage, this is all you need to know. Check the documentation for more details on each respective class.
 
 ---
 
 ## Advanced Usage
 For more advanced uses, Control.lab.ly provides a host of tools to streamline the development of lab equipment automation.
@@ -128,20 +128,20 @@
 print(lab.Helper.get_node())
 ```
 
 A template of `registry.yaml` has also been added to the folder to hold the machine-specific addresses of your connected devices (i.e. COM ports).\
 Populate the YAML file in the format shown below.
 ```yaml
 ### registry.yaml ###
-'012345678901234':              # insert your machine's 15-digit ID here (from the above step)
-    cam_index:                  # camera index of the connected imaging devices
-      __cam_01__: 1             # keep the leading and trailing double underscores
+'012345678901234':          # insert your machine's 15-digit ID here (from the above step)
+    cam_index:              # camera index of the connected imaging devices
+      __cam_01__: 1         # keep the leading and trailing double underscores
       __cam_02__: 0
-    port:                       # addresses of serial COM ports
-      __device_01__: COM3       # keep the leading and trailing double underscores
+    port:                   # addresses of serial COM ports
+      __device_01__: COM3   # keep the leading and trailing double underscores
       __device_02__: COM16
 ```
 
 To find the COM port address(es) of the device(s) that is/are currently connected to your machine, use:
 ```python
 lab.Helper.get_ports()
 ```
@@ -166,30 +166,30 @@
     port: __device_01__                         # port addresses defined in registry.yaml
     _setting_A_: {'tuple': [300,0,200]}         # use keys to define the type of iterable
     _setting_B_: {'array': [[0,1,0],[-1,0,0]]}  # only tuple and np.array supported
 ```
 
 `Compound` devices are similarly configured. The configuration values for its component devices are defined under the `component_config` setting. The structure of the configuration values for the component devices are similar to that shown above, except indented to fall under the indentation of the `component_config` setting.
 ```yaml
-_Device02_:                                     # name of 'Compound' device (user-defined)
+_Device02_:                                 # name of 'Compound' device (user-defined)
   module: Compound                            
   class: _submodule_2A_._class_2A_
   settings:
-    _setting_C_: 1                              # other settings for your 'Compound' device
-    component_config:                           # nest component configuration settings here
-      _Component01_:                            # name of component
+    _setting_C_: 1                          # other settings for your 'Compound' device
+    component_config:                       # nest component configuration settings here
+      _Component01_:                        # name of component
         module: _module_name_03_
         class: _submodule_3A_._class_3A_
         settings:
-          ip_address: '192.0.0.1'               # IP addresses do not vary between machines
+          ip_address: '192.0.0.1'           # IP addresses do not vary between machines
       _Component02_: 
         module: _module_name_04_
         class: _submodule_4A_._class_4A_
         settings:
-          _setting_D_: 2                        # settings for your component device
+          _setting_D_: 2                    # settings for your component device
 ```
 
 Lastly, you can define shortcuts to quickly access components of `Compound` devices.
 ```yaml
 SHORTCUTS:
   _Nickname1_: '_Device02_._Component01_'
   _Nickname2_: '_Device02_._Component02_'
```

### Comparing `control-lab-ly-1.0.0b0/src/control_lab_ly.egg-info/SOURCES.txt` & `control-lab-ly-1.0.0b1/src/control_lab_ly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/Analyse/Data/Database/database_utils.py` & `control-lab-ly-1.0.0b1/src/controllably/Analyse/Data/Database/database_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/Analyse/Data/Types/circuit_datatype.py` & `control-lab-ly-1.0.0b1/src/controllably/Analyse/Data/Types/circuit_datatype.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/Analyse/Data/Types/eis_datatype.py` & `control-lab-ly-1.0.0b1/src/controllably/Analyse/Data/Types/eis_datatype.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/Analyse/Data/Types/eis_test_circuits.yaml` & `control-lab-ly-1.0.0b1/src/controllably/Analyse/Data/Types/eis_test_circuits.yaml`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/Analyse/Data/Types/eis_tests.json` & `control-lab-ly-1.0.0b1/src/controllably/Analyse/Data/Types/eis_tests.json`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/Analyse/Visualisation/visualisation_utils.py` & `control-lab-ly-1.0.0b1/src/controllably/Analyse/Visualisation/visualisation_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/Compound/LiquidMover/liquidmover_utils.py` & `control-lab-ly-1.0.0b1/src/controllably/Compound/LiquidMover/liquidmover_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/Compound/compound_utils.py` & `control-lab-ly-1.0.0b1/src/controllably/Compound/compound_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/Control/GUI/__init__.py` & `control-lab-ly-1.0.0b1/src/controllably/Control/GUI/__init__.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/Control/GUI/_guibuilder.py` & `control-lab-ly-1.0.0b1/src/controllably/Control/GUI/_guibuilder.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/Control/GUI/gui_utils.py` & `control-lab-ly-1.0.0b1/src/controllably/Control/GUI/gui_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/Control/GUI/loader_panel.py` & `control-lab-ly-1.0.0b1/src/controllably/Control/GUI/loader_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/Control/GUI/measurer_panel.py` & `control-lab-ly-1.0.0b1/src/controllably/Control/GUI/measurer_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/Control/GUI/mover_panel.py` & `control-lab-ly-1.0.0b1/src/controllably/Control/GUI/mover_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/Control/GUI/viewer_panel.py` & `control-lab-ly-1.0.0b1/src/controllably/Control/GUI/viewer_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/Control/Schedule/schedule_utils.py` & `control-lab-ly-1.0.0b1/src/controllably/Control/Schedule/schedule_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/Make/Heat/peltier_utils.py` & `control-lab-ly-1.0.0b1/src/controllably/Make/Heat/peltier_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/Make/Light/led_utils.py` & `control-lab-ly-1.0.0b1/src/controllably/Make/Light/led_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/Make/ThinFilm/spinner_utils.py` & `control-lab-ly-1.0.0b1/src/controllably/Make/ThinFilm/spinner_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/Make/make_utils.py` & `control-lab-ly-1.0.0b1/src/controllably/Make/make_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/Measure/Electrical/Keithley/keithley_device.py` & `control-lab-ly-1.0.0b1/src/controllably/Measure/Electrical/Keithley/keithley_device.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/Measure/Electrical/Keithley/keithley_lib.py` & `control-lab-ly-1.0.0b1/src/controllably/Measure/Electrical/Keithley/keithley_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/Measure/Electrical/Keithley/keithley_utils.py` & `control-lab-ly-1.0.0b1/src/controllably/Measure/Electrical/Keithley/keithley_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/Measure/Electrical/Keithley/programs/base_programs.py` & `control-lab-ly-1.0.0b1/src/controllably/Measure/Electrical/Keithley/programs/base_programs.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_device.py` & `control-lab-ly-1.0.0b1/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_device.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_lib.py` & `control-lab-ly-1.0.0b1/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_utils.py` & `control-lab-ly-1.0.0b1/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/Measure/Mechanical/PiezoRobotics/programs/base_programs.py` & `control-lab-ly-1.0.0b1/src/controllably/Measure/Mechanical/PiezoRobotics/programs/base_programs.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/Measure/Physical/balance_utils.py` & `control-lab-ly-1.0.0b1/src/controllably/Measure/Physical/balance_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/Measure/__init__.py` & `control-lab-ly-1.0.0b1/src/controllably/Measure/__init__.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/Measure/instrument_utils.py` & `control-lab-ly-1.0.0b1/src/controllably/Measure/instrument_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/Measure/measure_utils.py` & `control-lab-ly-1.0.0b1/src/controllably/Measure/measure_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/Measure/program_utils.py` & `control-lab-ly-1.0.0b1/src/controllably/Measure/program_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/Move/Cartesian/cartesian_utils.py` & `control-lab-ly-1.0.0b1/src/controllably/Move/Cartesian/cartesian_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/Move/Cartesian/ender_utils.py` & `control-lab-ly-1.0.0b1/src/controllably/Move/Cartesian/ender_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/Move/Cartesian/primitiv_utils.py` & `control-lab-ly-1.0.0b1/src/controllably/Move/Cartesian/primitiv_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/Move/Jointed/Dobot/dobot_api/dobot_api.py` & `control-lab-ly-1.0.0b1/src/controllably/Move/Jointed/Dobot/dobot_api/dobot_api.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/Move/Jointed/Dobot/dobot_utils.py` & `control-lab-ly-1.0.0b1/src/controllably/Move/Jointed/Dobot/dobot_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/Move/Jointed/Dobot/m1pro_utils.py` & `control-lab-ly-1.0.0b1/src/controllably/Move/Jointed/Dobot/m1pro_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/Move/Jointed/Dobot/mg400_utils.py` & `control-lab-ly-1.0.0b1/src/controllably/Move/Jointed/Dobot/mg400_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/Move/Jointed/jointed_utils.py` & `control-lab-ly-1.0.0b1/src/controllably/Move/Jointed/jointed_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/Move/move_utils.py` & `control-lab-ly-1.0.0b1/src/controllably/Move/move_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_lib.py` & `control-lab-ly-1.0.0b1/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_utils.py` & `control-lab-ly-1.0.0b1/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/Transfer/Liquid/Pumps/peristaltic_utils.py` & `control-lab-ly-1.0.0b1/src/controllably/Transfer/Liquid/Pumps/peristaltic_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/Transfer/Liquid/Pumps/pump_utils.py` & `control-lab-ly-1.0.0b1/src/controllably/Transfer/Liquid/Pumps/pump_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/Transfer/Liquid/Sartorius/sartorius_lib.py` & `control-lab-ly-1.0.0b1/src/controllably/Transfer/Liquid/Sartorius/sartorius_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/Transfer/Liquid/Sartorius/sartorius_utils.py` & `control-lab-ly-1.0.0b1/src/controllably/Transfer/Liquid/Sartorius/sartorius_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/Transfer/Liquid/liquid_utils.py` & `control-lab-ly-1.0.0b1/src/controllably/Transfer/Liquid/liquid_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/Transfer/Liquid/syringe_lib.py` & `control-lab-ly-1.0.0b1/src/controllably/Transfer/Liquid/syringe_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/Transfer/Liquid/syringe_utils.py` & `control-lab-ly-1.0.0b1/src/controllably/Transfer/Liquid/syringe_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/Transfer/Substrate/Dobot/dobot_attachments.py` & `control-lab-ly-1.0.0b1/src/controllably/Transfer/Substrate/Dobot/dobot_attachments.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/Transfer/Substrate/substrate_utils.py` & `control-lab-ly-1.0.0b1/src/controllably/Transfer/Substrate/substrate_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/View/Classifiers/classifier_utils.py` & `control-lab-ly-1.0.0b1/src/controllably/View/Classifiers/classifier_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/View/Optical/optical_utils.py` & `control-lab-ly-1.0.0b1/src/controllably/View/Optical/optical_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/View/Optical/placeholders/optical_camera.png` & `control-lab-ly-1.0.0b1/src/controllably/View/Optical/placeholders/optical_camera.png`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/View/Thermal/Flir/ax8/ax8.py` & `control-lab-ly-1.0.0b1/src/controllably/View/Thermal/Flir/ax8/ax8.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/View/Thermal/Flir/ax8/ax8_camera_feed.py` & `control-lab-ly-1.0.0b1/src/controllably/View/Thermal/Flir/ax8/ax8_camera_feed.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_regs.py` & `control-lab-ly-1.0.0b1/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_regs.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_utils.py` & `control-lab-ly-1.0.0b1/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/View/Thermal/placeholders/infrared_camera.png` & `control-lab-ly-1.0.0b1/src/controllably/View/Thermal/placeholders/infrared_camera.png`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/View/Thermal/thermal_utils.py` & `control-lab-ly-1.0.0b1/src/controllably/View/Thermal/thermal_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/View/image_utils.py` & `control-lab-ly-1.0.0b1/src/controllably/View/image_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/View/view_utils.py` & `control-lab-ly-1.0.0b1/src/controllably/View/view_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/misc/__init__.py` & `control-lab-ly-1.0.0b1/src/controllably/misc/__init__.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/misc/decorators.py` & `control-lab-ly-1.0.0b1/src/controllably/misc/decorators.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/misc/factory.py` & `control-lab-ly-1.0.0b1/src/controllably/misc/factory.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/misc/helper.py` & `control-lab-ly-1.0.0b1/src/controllably/misc/helper.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/misc/layout.py` & `control-lab-ly-1.0.0b1/src/controllably/misc/layout.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/misc/logger.py` & `control-lab-ly-1.0.0b1/src/controllably/misc/logger.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/misc/misc_utils.py` & `control-lab-ly-1.0.0b1/src/controllably/misc/misc_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/misc/templates/configs/plugins/plugin_template.py` & `control-lab-ly-1.0.0b1/src/controllably/misc/templates/configs/plugins/plugin_template.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/misc/templates/setup/__init__.py` & `control-lab-ly-1.0.0b1/src/controllably/misc/templates/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/misc/templates/setup/config.yaml` & `control-lab-ly-1.0.0b1/src/controllably/misc/templates/setup/config.yaml`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/src/controllably/misc/templates/setup/layout.json` & `control-lab-ly-1.0.0b1/src/controllably/misc/templates/setup/layout.json`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/tests/test_compound_liquidmover.py` & `control-lab-ly-1.0.0b1/tests/test_compound_liquidmover.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/tests/test_compound_spin_printer.py` & `control-lab-ly-1.0.0b1/tests/test_compound_spin_printer.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/tests/test_dobot_m1pro.py` & `control-lab-ly-1.0.0b1/tests/test_dobot_m1pro.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/tests/test_dobot_mg400.py` & `control-lab-ly-1.0.0b1/tests/test_dobot_mg400.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/tests/test_heat_peltier.py` & `control-lab-ly-1.0.0b1/tests/test_heat_peltier.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0b0/tests/test_liquid_tricontinent.py` & `control-lab-ly-1.0.0b1/tests/test_liquid_tricontinent.py`

 * *Files identical despite different names*

