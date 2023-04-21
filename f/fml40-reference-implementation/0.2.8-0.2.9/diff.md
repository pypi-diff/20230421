# Comparing `tmp/fml40_reference_implementation-0.2.8-py3-none-any.whl.zip` & `tmp/fml40_reference_implementation-0.2.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,23 @@
-Zip file size: 198449 bytes, number of entries: 439
+Zip file size: 204015 bytes, number of entries: 451
 -rw-r--r--  2.0 unx        0 b- defN 23-Mar-22 16:18 dt_templates/__init__.py
 -rw-r--r--  2.0 unx      979 b- defN 23-Mar-24 14:23 dt_templates/chainsaw.py
+-rw-r--r--  2.0 unx      986 b- defN 23-Apr-21 15:17 dt_templates/forest_owner.py
 -rw-r--r--  2.0 unx     2259 b- defN 23-Mar-22 16:18 dt_templates/forwarder.py
 -rw-r--r--  2.0 unx      996 b- defN 23-Apr-11 07:53 dt_templates/forwarding_agency.py
 -rw-r--r--  2.0 unx     2139 b- defN 23-Mar-22 16:18 dt_templates/harvester.py
+-rw-r--r--  2.0 unx      989 b- defN 23-Apr-21 15:17 dt_templates/production_team.py
 -rw-r--r--  2.0 unx      988 b- defN 23-Apr-11 07:53 dt_templates/sawmill_entry.py
 -rw-r--r--  2.0 unx      979 b- defN 23-Apr-11 07:53 dt_templates/supplier.py
 -rw-r--r--  2.0 unx     2119 b- defN 23-Mar-24 14:23 dt_templates/truck.py
 -rw-r--r--  2.0 unx      360 b- defN 22-Jan-23 19:54 ml/__init__.py
 -rw-r--r--  2.0 unx     1039 b- defN 23-Jan-26 11:14 ml/app_logger.py
 -rw-r--r--  2.0 unx     2934 b- defN 23-Jan-26 11:14 ml/callback.py
 -rw-r--r--  2.0 unx      693 b- defN 23-Jan-26 11:14 ml/ditto_feature.py
--rw-r--r--  2.0 unx    33091 b- defN 23-Apr-11 07:53 ml/dt_factory.py
+-rw-r--r--  2.0 unx    33891 b- defN 23-Apr-21 15:17 ml/dt_factory.py
 -rw-r--r--  2.0 unx     6088 b- defN 23-Mar-22 16:18 ml/entry.py
 -rw-r--r--  2.0 unx     3794 b- defN 23-Jan-26 11:14 ml/feature.py
 -rw-r--r--  2.0 unx     1254 b- defN 23-Jan-26 11:14 ml/identifier.py
 -rw-r--r--  2.0 unx     4598 b- defN 23-Jan-26 11:14 ml/parameters.py
 -rw-r--r--  2.0 unx     2120 b- defN 23-Jan-26 11:14 ml/role.py
 -rw-r--r--  2.0 unx     8249 b- defN 22-Jan-23 19:54 ml/s3i_tools.py
 -rw-r--r--  2.0 unx    32710 b- defN 23-Mar-22 16:18 ml/thing.py
@@ -33,15 +35,16 @@
 -rw-r--r--  2.0 unx      501 b- defN 21-Dec-16 08:43 ml/fml40/features/functionalities/accepts_passability_report.py
 -rw-r--r--  2.0 unx      712 b- defN 21-Dec-16 08:43 ml/fml40/features/functionalities/accepts_proximity_alert.py
 -rw-r--r--  2.0 unx      994 b- defN 21-Dec-16 08:43 ml/fml40/features/functionalities/accepts_shield_commands.py
 -rw-r--r--  2.0 unx      583 b- defN 21-Dec-16 08:43 ml/fml40/features/functionalities/accepts_single_tree_felling_jobs.py
 -rw-r--r--  2.0 unx      992 b- defN 21-Dec-16 08:43 ml/fml40/features/functionalities/accepts_winch_command.py
 -rw-r--r--  2.0 unx      404 b- defN 23-Mar-22 16:18 ml/fml40/features/functionalities/calculates_machine_operation_cost.py
 -rw-r--r--  2.0 unx      830 b- defN 21-Dec-16 08:43 ml/fml40/features/functionalities/classifies_tree_species.py
--rw-r--r--  2.0 unx      357 b- defN 23-Apr-11 07:53 ml/fml40/features/functionalities/controls_sawmill_production.py
+-rw-r--r--  2.0 unx      464 b- defN 23-Apr-21 15:17 ml/fml40/features/functionalities/controls_forest_production.py
+-rw-r--r--  2.0 unx      373 b- defN 23-Apr-21 15:17 ml/fml40/features/functionalities/controls_sawmill_production.py
 -rw-r--r--  2.0 unx      314 b- defN 21-Dec-16 08:43 ml/fml40/features/functionalities/converts_data_formats.py
 -rw-r--r--  2.0 unx      333 b- defN 21-Dec-16 08:43 ml/fml40/features/functionalities/converts_forest_gml.py
 -rw-r--r--  2.0 unx      333 b- defN 22-Nov-17 10:47 ml/fml40/features/functionalities/converts_shapefile.py
 -rw-r--r--  2.0 unx      498 b- defN 21-Dec-16 08:43 ml/fml40/features/functionalities/cuts.py
 -rw-r--r--  2.0 unx     1646 b- defN 21-Dec-16 08:43 ml/fml40/features/functionalities/determines_passability.py
 -rw-r--r--  2.0 unx      544 b- defN 21-Dec-16 08:43 ml/fml40/features/functionalities/displays_health_alarms.py
 -rw-r--r--  2.0 unx      316 b- defN 21-Dec-16 08:43 ml/fml40/features/functionalities/evaluates_forest_rating.py
@@ -104,14 +107,16 @@
 -rw-r--r--  2.0 unx      307 b- defN 23-Apr-11 07:53 ml/fml40/features/properties/values/sawmill_delivery_parking_area_status.py
 -rw-r--r--  2.0 unx      304 b- defN 23-Apr-11 07:53 ml/fml40/features/properties/values/sawmill_entry_parking_area_status.py
 -rw-r--r--  2.0 unx      268 b- defN 21-Dec-16 08:43 ml/fml40/features/properties/values/stand_attribute_set.py
 -rw-r--r--  2.0 unx     1502 b- defN 21-Dec-16 08:43 ml/fml40/features/properties/values/stem_segment_properties.py
 -rw-r--r--  2.0 unx      657 b- defN 22-Nov-17 10:47 ml/fml40/features/properties/values/stock_volume.py
 -rw-r--r--  2.0 unx      312 b- defN 23-Mar-22 16:18 ml/fml40/features/properties/values/suitable_tree_species.py
 -rw-r--r--  2.0 unx      287 b- defN 21-Dec-16 08:43 ml/fml40/features/properties/values/thickness_class.py
+-rw-r--r--  2.0 unx      307 b- defN 23-Apr-21 15:17 ml/fml40/features/properties/values/timber_harvesting_capacity.py
+-rw-r--r--  2.0 unx      291 b- defN 23-Apr-21 15:17 ml/fml40/features/properties/values/timber_harvesting_cost.py
 -rw-r--r--  2.0 unx      281 b- defN 21-Dec-16 08:43 ml/fml40/features/properties/values/tree_data.py
 -rw-r--r--  2.0 unx      700 b- defN 23-Mar-22 16:18 ml/fml40/features/properties/values/tree_species.py
 -rw-r--r--  2.0 unx      684 b- defN 21-Dec-16 08:43 ml/fml40/features/properties/values/tree_type.py
 -rw-r--r--  2.0 unx     3165 b- defN 22-Nov-17 10:47 ml/fml40/features/properties/values/vegetationindex.py
 -rw-r--r--  2.0 unx      649 b- defN 21-Dec-16 08:43 ml/fml40/features/properties/values/vitality_status.py
 -rw-r--r--  2.0 unx      284 b- defN 21-Dec-16 08:43 ml/fml40/features/properties/values/wood_quality.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Nov-09 12:38 ml/fml40/features/properties/values/documents/__init__.py
@@ -198,14 +203,15 @@
 -rw-r--r--  2.0 unx        0 b- defN 21-Nov-09 12:38 ml/fml40/roles/services/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Nov-09 12:38 ml/ml40/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Nov-09 12:38 ml/ml40/features/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Nov-09 12:38 ml/ml40/features/functionalities/__init__.py
 -rw-r--r--  2.0 unx      680 b- defN 21-Dec-16 08:43 ml/ml40/features/functionalities/accepts_jobs.py
 -rw-r--r--  2.0 unx      471 b- defN 21-Dec-16 08:43 ml/ml40/features/functionalities/accepts_reports.py
 -rw-r--r--  2.0 unx      427 b- defN 21-Dec-16 08:43 ml/ml40/features/functionalities/clears_jobs.py
+-rw-r--r--  2.0 unx      376 b- defN 23-Apr-21 15:17 ml/ml40/features/functionalities/controls_production.py
 -rw-r--r--  2.0 unx      330 b- defN 21-Dec-16 08:43 ml/ml40/features/functionalities/functionality.py
 -rw-r--r--  2.0 unx      633 b- defN 21-Dec-16 08:43 ml/ml40/features/functionalities/manages_jobs.py
 -rw-r--r--  2.0 unx      510 b- defN 21-Dec-16 08:43 ml/ml40/features/functionalities/plans_routes.py
 -rw-r--r--  2.0 unx      377 b- defN 23-Apr-11 07:53 ml/ml40/features/functionalities/predicts_consumption.py
 -rw-r--r--  2.0 unx      377 b- defN 22-Nov-17 10:47 ml/ml40/features/functionalities/predicts_maintenance.py
 -rw-r--r--  2.0 unx      327 b- defN 23-Mar-22 16:18 ml/ml40/features/functionalities/predicts_purchase.py
 -rw-r--r--  2.0 unx      387 b- defN 23-Mar-22 16:18 ml/ml40/features/functionalities/provides_emissions_data.py
@@ -227,14 +233,15 @@
 -rw-r--r--  2.0 unx      996 b- defN 21-Dec-16 08:43 ml/ml40/features/properties/values/address.py
 -rw-r--r--  2.0 unx      537 b- defN 23-Mar-22 16:18 ml/ml40/features/properties/values/air_pressure.py
 -rw-r--r--  2.0 unx      528 b- defN 23-Mar-22 16:18 ml/ml40/features/properties/values/air_volume.py
 -rw-r--r--  2.0 unx      276 b- defN 21-Dec-16 08:43 ml/ml40/features/properties/values/area.py
 -rw-r--r--  2.0 unx      769 b- defN 23-Apr-11 07:53 ml/ml40/features/properties/values/bank_account.py
 -rw-r--r--  2.0 unx      516 b- defN 23-Mar-22 16:18 ml/ml40/features/properties/values/brand.py
 -rw-r--r--  2.0 unx      282 b- defN 21-Dec-16 08:43 ml/ml40/features/properties/values/brightness.py
+-rw-r--r--  2.0 unx      491 b- defN 23-Apr-21 15:17 ml/ml40/features/properties/values/capacity.py
 -rw-r--r--  2.0 unx      315 b- defN 23-Apr-11 07:53 ml/ml40/features/properties/values/contacts.py
 -rw-r--r--  2.0 unx      515 b- defN 23-Mar-22 16:18 ml/ml40/features/properties/values/cost.py
 -rw-r--r--  2.0 unx      795 b- defN 21-Dec-16 08:43 ml/ml40/features/properties/values/count.py
 -rw-r--r--  2.0 unx      280 b- defN 23-Mar-22 16:18 ml/ml40/features/properties/values/current_load.py
 -rw-r--r--  2.0 unx      288 b- defN 23-Mar-22 16:18 ml/ml40/features/properties/values/current_weight.py
 -rw-r--r--  2.0 unx      526 b- defN 23-Mar-22 16:18 ml/ml40/features/properties/values/description.py
 -rw-r--r--  2.0 unx      524 b- defN 23-Apr-11 07:53 ml/ml40/features/properties/values/diameter.py
@@ -310,14 +317,18 @@
 -rw-r--r--  2.0 unx      703 b- defN 23-Mar-22 16:18 ml/ml40/features/properties/values/velocity.py
 -rw-r--r--  2.0 unx      522 b- defN 23-Apr-11 07:53 ml/ml40/features/properties/values/volume.py
 -rw-r--r--  2.0 unx     2793 b- defN 22-Aug-03 12:25 ml/ml40/features/properties/values/weatherdata.py
 -rw-r--r--  2.0 unx      669 b- defN 21-Dec-16 08:43 ml/ml40/features/properties/values/weight.py
 -rw-r--r--  2.0 unx      309 b- defN 21-Dec-16 08:43 ml/ml40/features/properties/values/white_level.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Nov-09 12:38 ml/ml40/features/properties/values/documents/__init__.py
 -rw-r--r--  2.0 unx      280 b- defN 21-Dec-16 08:43 ml/ml40/features/properties/values/documents/document.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-21 15:17 ml/ml40/features/properties/values/documents/contacts/__init__.py
+-rw-r--r--  2.0 unx     1016 b- defN 23-Apr-21 15:17 ml/ml40/features/properties/values/documents/contacts/contact.py
+-rw-r--r--  2.0 unx      555 b- defN 23-Apr-21 15:17 ml/ml40/features/properties/values/documents/contacts/organizational_contact.py
+-rw-r--r--  2.0 unx      913 b- defN 23-Apr-21 15:17 ml/ml40/features/properties/values/documents/contacts/personal_contact.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 07:53 ml/ml40/features/properties/values/documents/contracts/__init__.py
 -rw-r--r--  2.0 unx      299 b- defN 23-Apr-11 07:53 ml/ml40/features/properties/values/documents/contracts/contract.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Nov-09 12:38 ml/ml40/features/properties/values/documents/jobs/__init__.py
 -rw-r--r--  2.0 unx      695 b- defN 21-Dec-16 08:43 ml/ml40/features/properties/values/documents/jobs/generic_job.py
 -rw-r--r--  2.0 unx      782 b- defN 23-Mar-22 16:18 ml/ml40/features/properties/values/documents/jobs/job.py
 -rw-r--r--  2.0 unx      288 b- defN 21-Dec-16 08:43 ml/ml40/features/properties/values/documents/jobs/job_list.py
 -rw-r--r--  2.0 unx       99 b- defN 21-Nov-09 12:38 ml/ml40/features/properties/values/documents/jobs/job_status.py
@@ -347,14 +358,15 @@
 -rw-r--r--  2.0 unx      274 b- defN 21-Dec-16 08:43 ml/ml40/roles/dts/parts/scale.py
 -rw-r--r--  2.0 unx      272 b- defN 21-Dec-16 08:43 ml/ml40/roles/dts/parts/tank.py
 -rw-r--r--  2.0 unx      274 b- defN 23-Mar-22 16:18 ml/ml40/roles/dts/parts/wheel.py
 -rw-r--r--  2.0 unx      274 b- defN 23-Mar-22 16:18 ml/ml40/roles/dts/parts/winch.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Nov-09 12:38 ml/ml40/roles/dts/persons/__init__.py
 -rw-r--r--  2.0 unx      302 b- defN 21-Dec-16 08:43 ml/ml40/roles/dts/persons/machine_operator.py
 -rw-r--r--  2.0 unx      242 b- defN 21-Dec-16 08:43 ml/ml40/roles/dts/persons/person.py
+-rw-r--r--  2.0 unx      277 b- defN 23-Apr-21 15:17 ml/ml40/roles/dts/persons/precinct_leader.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Nov-09 12:38 ml/ml40/roles/dts/sensors/__init__.py
 -rw-r--r--  2.0 unx      279 b- defN 21-Dec-16 08:43 ml/ml40/roles/dts/sensors/accelerometer.py
 -rw-r--r--  2.0 unx      290 b- defN 21-Dec-16 08:43 ml/ml40/roles/dts/sensors/air_sensor.py
 -rw-r--r--  2.0 unx      298 b- defN 23-Apr-11 07:53 ml/ml40/roles/dts/sensors/counter_sensor.py
 -rw-r--r--  2.0 unx      290 b- defN 21-Dec-16 08:43 ml/ml40/roles/dts/sensors/gyroscope.py
 -rw-r--r--  2.0 unx      274 b- defN 21-Nov-09 12:38 ml/ml40/roles/dts/sensors/high_speed_camera.py
 -rw-r--r--  2.0 unx      295 b- defN 21-Nov-09 12:38 ml/ml40/roles/dts/sensors/imu.py
@@ -429,13 +441,13 @@
 -rw-r--r--  2.0 unx      252 b- defN 22-Aug-03 12:25 ml/wml40/roles/dts/water/water.py
 -rw-r--r--  2.0 unx      277 b- defN 22-Aug-03 12:25 ml/wml40/roles/dts/water/waterreservoir.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Aug-03 12:25 ml/wml40/roles/hmis/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Aug-03 12:25 ml/wml40/roles/services/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Nov-09 12:38 tests/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Nov-09 12:38 tests/test_async.py
 -rw-r--r--  2.0 unx       48 b- defN 22-Aug-03 12:25 tests/test_entry.py
--rw-rw-rw-  2.0 unx     7651 b- defN 23-Apr-11 08:02 fml40_reference_implementation-0.2.8.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     8893 b- defN 23-Apr-11 08:02 fml40_reference_implementation-0.2.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-11 08:02 fml40_reference_implementation-0.2.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       22 b- defN 23-Apr-11 08:02 fml40_reference_implementation-0.2.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    45031 b- defN 23-Apr-11 08:02 fml40_reference_implementation-0.2.8.dist-info/RECORD
-439 files, 356503 bytes uncompressed, 123853 bytes compressed:  65.3%
+-rw-rw-rw-  2.0 unx     7651 b- defN 23-Apr-21 15:27 fml40_reference_implementation-0.2.9.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     8893 b- defN 23-Apr-21 15:27 fml40_reference_implementation-0.2.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-21 15:27 fml40_reference_implementation-0.2.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       22 b- defN 23-Apr-21 15:27 fml40_reference_implementation-0.2.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    46376 b- defN 23-Apr-21 15:27 fml40_reference_implementation-0.2.9.dist-info/RECORD
+451 files, 365329 bytes uncompressed, 127159 bytes compressed:  65.2%
```

## zipnote {}

```diff
@@ -1,22 +1,28 @@
 Filename: dt_templates/__init__.py
 Comment: 
 
 Filename: dt_templates/chainsaw.py
 Comment: 
 
+Filename: dt_templates/forest_owner.py
+Comment: 
+
 Filename: dt_templates/forwarder.py
 Comment: 
 
 Filename: dt_templates/forwarding_agency.py
 Comment: 
 
 Filename: dt_templates/harvester.py
 Comment: 
 
+Filename: dt_templates/production_team.py
+Comment: 
+
 Filename: dt_templates/sawmill_entry.py
 Comment: 
 
 Filename: dt_templates/supplier.py
 Comment: 
 
 Filename: dt_templates/truck.py
@@ -108,14 +114,17 @@
 
 Filename: ml/fml40/features/functionalities/calculates_machine_operation_cost.py
 Comment: 
 
 Filename: ml/fml40/features/functionalities/classifies_tree_species.py
 Comment: 
 
+Filename: ml/fml40/features/functionalities/controls_forest_production.py
+Comment: 
+
 Filename: ml/fml40/features/functionalities/controls_sawmill_production.py
 Comment: 
 
 Filename: ml/fml40/features/functionalities/converts_data_formats.py
 Comment: 
 
 Filename: ml/fml40/features/functionalities/converts_forest_gml.py
@@ -321,14 +330,20 @@
 
 Filename: ml/fml40/features/properties/values/suitable_tree_species.py
 Comment: 
 
 Filename: ml/fml40/features/properties/values/thickness_class.py
 Comment: 
 
+Filename: ml/fml40/features/properties/values/timber_harvesting_capacity.py
+Comment: 
+
+Filename: ml/fml40/features/properties/values/timber_harvesting_cost.py
+Comment: 
+
 Filename: ml/fml40/features/properties/values/tree_data.py
 Comment: 
 
 Filename: ml/fml40/features/properties/values/tree_species.py
 Comment: 
 
 Filename: ml/fml40/features/properties/values/tree_type.py
@@ -603,14 +618,17 @@
 
 Filename: ml/ml40/features/functionalities/accepts_reports.py
 Comment: 
 
 Filename: ml/ml40/features/functionalities/clears_jobs.py
 Comment: 
 
+Filename: ml/ml40/features/functionalities/controls_production.py
+Comment: 
+
 Filename: ml/ml40/features/functionalities/functionality.py
 Comment: 
 
 Filename: ml/ml40/features/functionalities/manages_jobs.py
 Comment: 
 
 Filename: ml/ml40/features/functionalities/plans_routes.py
@@ -690,14 +708,17 @@
 
 Filename: ml/ml40/features/properties/values/brand.py
 Comment: 
 
 Filename: ml/ml40/features/properties/values/brightness.py
 Comment: 
 
+Filename: ml/ml40/features/properties/values/capacity.py
+Comment: 
+
 Filename: ml/ml40/features/properties/values/contacts.py
 Comment: 
 
 Filename: ml/ml40/features/properties/values/cost.py
 Comment: 
 
 Filename: ml/ml40/features/properties/values/count.py
@@ -939,14 +960,26 @@
 
 Filename: ml/ml40/features/properties/values/documents/__init__.py
 Comment: 
 
 Filename: ml/ml40/features/properties/values/documents/document.py
 Comment: 
 
+Filename: ml/ml40/features/properties/values/documents/contacts/__init__.py
+Comment: 
+
+Filename: ml/ml40/features/properties/values/documents/contacts/contact.py
+Comment: 
+
+Filename: ml/ml40/features/properties/values/documents/contacts/organizational_contact.py
+Comment: 
+
+Filename: ml/ml40/features/properties/values/documents/contacts/personal_contact.py
+Comment: 
+
 Filename: ml/ml40/features/properties/values/documents/contracts/__init__.py
 Comment: 
 
 Filename: ml/ml40/features/properties/values/documents/contracts/contract.py
 Comment: 
 
 Filename: ml/ml40/features/properties/values/documents/jobs/__init__.py
@@ -1050,14 +1083,17 @@
 
 Filename: ml/ml40/roles/dts/persons/machine_operator.py
 Comment: 
 
 Filename: ml/ml40/roles/dts/persons/person.py
 Comment: 
 
+Filename: ml/ml40/roles/dts/persons/precinct_leader.py
+Comment: 
+
 Filename: ml/ml40/roles/dts/sensors/__init__.py
 Comment: 
 
 Filename: ml/ml40/roles/dts/sensors/accelerometer.py
 Comment: 
 
 Filename: ml/ml40/roles/dts/sensors/air_sensor.py
@@ -1296,23 +1332,23 @@
 
 Filename: tests/test_async.py
 Comment: 
 
 Filename: tests/test_entry.py
 Comment: 
 
-Filename: fml40_reference_implementation-0.2.8.dist-info/LICENSE.txt
+Filename: fml40_reference_implementation-0.2.9.dist-info/LICENSE.txt
 Comment: 
 
-Filename: fml40_reference_implementation-0.2.8.dist-info/METADATA
+Filename: fml40_reference_implementation-0.2.9.dist-info/METADATA
 Comment: 
 
-Filename: fml40_reference_implementation-0.2.8.dist-info/WHEEL
+Filename: fml40_reference_implementation-0.2.9.dist-info/WHEEL
 Comment: 
 
-Filename: fml40_reference_implementation-0.2.8.dist-info/top_level.txt
+Filename: fml40_reference_implementation-0.2.9.dist-info/top_level.txt
 Comment: 
 
-Filename: fml40_reference_implementation-0.2.8.dist-info/RECORD
+Filename: fml40_reference_implementation-0.2.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ml/dt_factory.py

```diff
@@ -28,14 +28,15 @@
 from ml.ml40.roles.dts.parts.engine import Engine
 from ml.ml40.roles.dts.parts.scale import Scale
 from ml.ml40.roles.dts.parts.tank import Tank
 from ml.ml40.roles.dts.parts.winch import Winch
 from ml.ml40.roles.dts.parts.wheel import Wheel
 from ml.ml40.roles.dts.persons.machine_operator import MachineOperator
 from ml.ml40.roles.dts.persons.person import Person
+from ml.ml40.roles.dts.persons.precinct_leader import PrecinctLeader
 from ml.ml40.roles.dts.sensors.sensor import Sensor
 from ml.ml40.roles.dts.sensors.air_sensor import AirSensor
 from ml.ml40.roles.dts.sensors.accelerometer import Accelerometer
 from ml.ml40.roles.dts.sensors.counter_sensor import CounterSensor
 from ml.ml40.roles.dts.sensors.gyroscope import Gyroscope
 from ml.ml40.roles.dts.sensors.high_speed_camera import HighSpeedCamera
 from ml.ml40.roles.dts.sensors.imu import IMU
@@ -116,14 +117,15 @@
 from ml.ml40.features.properties.property import Property
 from ml.ml40.features.properties.associations.shared import Shared
 from ml.ml40.features.properties.values.acceleration import Acceleration
 from ml.ml40.features.properties.values.address import Address
 from ml.ml40.features.properties.values.air_volume import AirVolume
 from ml.ml40.features.properties.values.bank_account import BankAccount
 from ml.ml40.features.properties.values.brand import Brand
+from ml.ml40.features.properties.values.capacity import Capacity
 from ml.ml40.features.properties.values.contacts import Contacts
 from ml.ml40.features.properties.values.cost import Cost
 from ml.ml40.features.properties.values.count import Count
 from ml.ml40.features.properties.values.current_load import CurrentLoad
 from ml.ml40.features.properties.values.current_weight import CurrentWeight
 from ml.ml40.features.properties.values.description import Description
 from ml.ml40.features.properties.values.diameter import Diameter
@@ -186,14 +188,17 @@
 from ml.ml40.features.properties.values.torque import Torque
 from ml.ml40.features.properties.values.type import Type
 from ml.ml40.features.properties.values.unit import Unit
 from ml.ml40.features.properties.values.velocity import Velocity
 from ml.ml40.features.properties.values.volume import Volume
 from ml.ml40.features.properties.values.weatherdata import WeatherData
 from ml.ml40.features.properties.values.weight import Weight
+from ml.ml40.features.properties.values.documents.contacts.contact import Contact
+from ml.ml40.features.properties.values.documents.contacts.organizational_contact import OrganizationalContact
+from ml.ml40.features.properties.values.documents.contacts.personal_contact import PersonalContact
 from ml.ml40.features.properties.values.documents.contracts.contract import Contract
 from ml.ml40.features.properties.values.documents.jobs.generic_job import GenericJob
 from ml.ml40.features.properties.values.documents.jobs.job import Job
 from ml.ml40.features.properties.values.documents.jobs.job_list import JobList
 from ml.ml40.features.properties.values.documents.jobs.job_status import JobStatus
 from ml.ml40.features.properties.values.documents.notes.note import Note
 from ml.ml40.features.properties.values.documents.reports.report import Report
@@ -224,14 +229,16 @@
 from ml.fml40.features.properties.values.sawing_processing_time import SawingProcessingTime
 from ml.fml40.features.properties.values.sawing_setup_time import SawingSetupTime
 from ml.fml40.features.properties.values.sawmill_delivery_parking_area_status import SawmillDeliveryParkingAreaStatus
 from ml.fml40.features.properties.values.sawmill_entry_parking_area_status import SawmillEntryParkingAreaStatus
 from ml.fml40.features.properties.values.stem_segment_properties import StemSegmentProperties
 from ml.fml40.features.properties.values.stock_volume import StockVolume
 from ml.fml40.features.properties.values.suitable_tree_species import SuitableTreeSpecies
+from ml.fml40.features.properties.values.timber_harvesting_capacity import TimberHarvestingCapacity
+from ml.fml40.features.properties.values.timber_harvesting_cost import TimberHarvestingCost
 from ml.fml40.features.properties.values.thickness_class import ThicknessClass
 from ml.fml40.features.properties.values.tree_data import TreeData
 from ml.fml40.features.properties.values.tree_species import TreeSpecies
 from ml.fml40.features.properties.values.tree_type import TreeType
 from ml.fml40.features.properties.values.vegetationindex import VegetationIndex
 from ml.fml40.features.properties.values.vitality_status import VitalityStatus
 from ml.fml40.features.properties.values.wood_quality import WoodQuality
@@ -261,14 +268,15 @@
 from ml.wml40.features.properties.values.waterlevel import WaterLevel
 from ml.wml40.features.properties.values.waterquality import WaterQuality
 
 
 from ml.ml40.features.functionalities.accepts_jobs import AcceptsJobs
 from ml.ml40.features.functionalities.accepts_reports import AcceptsReports
 from ml.ml40.features.functionalities.clears_jobs import ClearsJobs
+from ml.ml40.features.functionalities.controls_production import ControlsProduction
 from ml.ml40.features.functionalities.functionality import Functionality
 from ml.ml40.features.functionalities.manages_jobs import ManagesJobs
 from ml.ml40.features.functionalities.plans_routes import PlansRoutes
 from ml.ml40.features.functionalities.predicts_consumption import PredictsConsumption
 from ml.ml40.features.functionalities.predicts_maintenance import PredictsMaintenance
 from ml.ml40.features.functionalities.predicts_purchase import PredictsPurchase
 from ml.ml40.features.functionalities.provides_emissions_data import ProvidesEmissionsData
@@ -290,14 +298,15 @@
 from ml.fml40.features.functionalities.accepts_passability_report import AcceptsPassabilityReport
 from ml.fml40.features.functionalities.accepts_proximity_alert import AcceptsProximityAlert
 from ml.fml40.features.functionalities.accepts_shield_commands import AcceptsShieldCommands
 from ml.fml40.features.functionalities.accepts_single_tree_felling_jobs import AcceptsSingleTreeFellingJobs
 from ml.fml40.features.functionalities.accepts_winch_command import AcceptsWinchCommands
 from ml.fml40.features.functionalities.calculates_machine_operation_cost import CalculatesMachineOperationCost
 from ml.fml40.features.functionalities.classifies_tree_species import ClassifiesTreeSpecies
+from ml.fml40.features.functionalities.controls_forest_production import ControlsForestProduction
 from ml.fml40.features.functionalities.controls_sawmill_production import ControlsSawmillProduction
 from ml.fml40.features.functionalities.converts_shapefile import ConvertsShapefile
 from ml.fml40.features.functionalities.cuts import Cuts
 from ml.fml40.features.functionalities.determines_passability import DeterminesPassability
 from ml.fml40.features.functionalities.displays_health_alarms import DisplaysHealthAlarms
 from ml.fml40.features.functionalities.evaluates_stand_attributes import EvaluatesStandAttributes
 from ml.fml40.features.functionalities.fells import Fells
```

## ml/fml40/features/functionalities/controls_sawmill_production.py

```diff
@@ -1,11 +1,11 @@
-from ml.ml40.features.functionalities.functionality import Functionality
+from ml.ml40.features.functionalities.controls_production import ControlsProduction
 
 
-class ControlsSawmillProduction(Functionality):
+class ControlsSawmillProduction(ControlsProduction):
     def __init__(self, namespace="fml40", name="", identifier="", parent=None):
         super().__init__(
             namespace=namespace, name=name, identifier=identifier, parent=parent
         )
 
     def control(self):
         pass
```

## Comparing `fml40_reference_implementation-0.2.8.dist-info/LICENSE.txt` & `fml40_reference_implementation-0.2.9.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `fml40_reference_implementation-0.2.8.dist-info/METADATA` & `fml40_reference_implementation-0.2.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fml40-reference-implementation
-Version: 0.2.8
+Version: 0.2.9
 Summary: fml40 reference implementation basic functions
 Home-page: https://www.kwh40.de/
 Author: Kompetenzzentrum Wald und Holz 4.0
 Author-email: s3i@kwh40.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Operating System :: OS Independent
```

## Comparing `fml40_reference_implementation-0.2.8.dist-info/RECORD` & `fml40_reference_implementation-0.2.9.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 dt_templates/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 dt_templates/chainsaw.py,sha256=ton9eRu5l5tL1mUuB_qPFVq_hFT9y1kBW5XHr54lI5M,979
+dt_templates/forest_owner.py,sha256=5AdFWmyS9Js1WpHFcxope4-gWfeN09eP6Pary8O4cPY,986
 dt_templates/forwarder.py,sha256=kLqICn3w3ld0uHQEf-NXAoKQcKRNY9VE0LMDfACTzFc,2259
 dt_templates/forwarding_agency.py,sha256=WtzUGqHobuvUcCDinJRP244aSlRx0ghX2geZ0kxlRgI,996
 dt_templates/harvester.py,sha256=RhAG2dMWpGKFR-V4AywtNnynDcJ86k_SLzILjWXIF5w,2139
+dt_templates/production_team.py,sha256=gTeh_jii1JsL6M0XiCCaF2BifM2Y_x3myvvvbQQcuRw,989
 dt_templates/sawmill_entry.py,sha256=oKpTDaM_x3wzufint70kvubJVbiKTmnKf11J6XaYv6U,988
 dt_templates/supplier.py,sha256=m2K2wCHrMev8eDl8lOaBJEl99rXE-mUn0PrE0xWEEI4,979
 dt_templates/truck.py,sha256=I1sZ67G0PEIn_GEAhXyMT3I_azZ_logNN9xi8t5WfSk,2119
 ml/__init__.py,sha256=QlspklRgPqi7uUxePGa-uJuTWPcwL0qHImVpbQJQKFs,360
 ml/app_logger.py,sha256=lsICIYTOADyMnisDaI2_KO1mGVFxkl1OYSsNK3JTlE4,1039
 ml/callback.py,sha256=PQxNdevMdI_fEUsAmRKNpZmnZs5MqY7ZTUx8vIZW1lw,2934
 ml/ditto_feature.py,sha256=OjvKNRSYYNxYW1QgbwSeLHPd2xxTFUud2CEFt2U46Fk,693
-ml/dt_factory.py,sha256=qYAiS5C-Oi2rkFt4oP7K5wgN-LCPXAKLG1tL0VPEaX8,33091
+ml/dt_factory.py,sha256=WAQe_espfm22N-A62mUmJDnZEXIrNU4hX_6_TEZLPXg,33891
 ml/entry.py,sha256=Q6OiJO8Vwj5ztCtYXaZSb3BzqmIyHgkdWp0iv6I3kGM,6088
 ml/feature.py,sha256=Z1q6sb0V0Buk3HvSSISOQfapZMsWxP2htKiIPv1g1xk,3794
 ml/identifier.py,sha256=4tVvLEH8fnLHAWe1rfuF3QuPd-TvMbaAElKvo7K5j3s,1254
 ml/parameters.py,sha256=GiK3n-AavnRy7Myz2LVlkvqSyZD7oJrPmqd0SfgNpHI,4598
 ml/role.py,sha256=gkK2-7QlARGICzjKwVxfcxvGm1BzZzTaPEVUbgXh71Q,2120
 ml/s3i_tools.py,sha256=e1TIqxspHw5-qOb3ptFbJb5hWVidI-0VMMVIqFvUXV8,8249
 ml/thing.py,sha256=TvVOyICgYLRLhBd_2s3TgnqiHFAQa0Q1rVs6tOTrMac,32710
@@ -32,15 +34,16 @@
 ml/fml40/features/functionalities/accepts_passability_report.py,sha256=a449SYeo5DMWTgVAW-zPSldwwhL2WJza1ypUDGh02dI,501
 ml/fml40/features/functionalities/accepts_proximity_alert.py,sha256=KrfSCbcLY8j5leHI__6rBHP1v-ok45XfsqpKRP1UN1I,712
 ml/fml40/features/functionalities/accepts_shield_commands.py,sha256=WuGYv-Y2MvtjYU8gXZIqOkdLnswDNoe0ZhycDl9gyvc,994
 ml/fml40/features/functionalities/accepts_single_tree_felling_jobs.py,sha256=RI0igTsjqrIWW9nK8G_RBF40dMNJDEp3iQmB6xFdNEQ,583
 ml/fml40/features/functionalities/accepts_winch_command.py,sha256=SKQ0aky32cKwqaK1Us_cHHuRpf2VY-FGZNw4FZ4_dXg,992
 ml/fml40/features/functionalities/calculates_machine_operation_cost.py,sha256=wVrnD5ijxGM17hj1mzdVK8cNwAp3icMBFRSkhAd9sjA,404
 ml/fml40/features/functionalities/classifies_tree_species.py,sha256=IGtyo2JJMo8W3LTY4VvLEP2uP-mrpqZ0aU_fjVBs_Hs,830
-ml/fml40/features/functionalities/controls_sawmill_production.py,sha256=F1ESPVIFr-ul6tZULcSIngZQDaxqeX-7eVkTPDnOHXA,357
+ml/fml40/features/functionalities/controls_forest_production.py,sha256=nL3dll2TQoLpHEe5_BEe8idcfJxplO3tzo2rr44ECzc,464
+ml/fml40/features/functionalities/controls_sawmill_production.py,sha256=Hw4ZhaKwBF4iO9xAJKi8hQwhsFYYClJwy7Dp1y_nwIk,373
 ml/fml40/features/functionalities/converts_data_formats.py,sha256=asiMttzY5r0Z0Ae2Iwbss7AjRKVGhJg13X1e28Dl3SY,314
 ml/fml40/features/functionalities/converts_forest_gml.py,sha256=4wUKKfQ0J4AnV6kB29Dc8HgJ4FxXHwWIaXLOYuc0_Ns,333
 ml/fml40/features/functionalities/converts_shapefile.py,sha256=-FTyWWqFYvzvZJSZobDltKWNgpZ3n7-vSYod0xiYfJU,333
 ml/fml40/features/functionalities/cuts.py,sha256=elyaf4IDS_63oq6jiqnniJxpaH9FR5vxTPLO945rRTs,498
 ml/fml40/features/functionalities/determines_passability.py,sha256=Wc1-kP6t4m8tXJS7TMLmmh98a2-Re04ZrGH5eKjcpNM,1646
 ml/fml40/features/functionalities/displays_health_alarms.py,sha256=U9y6GwBVho_Lg9AJA5iys5xZATnUqLsp9yKMkS2NPKA,544
 ml/fml40/features/functionalities/evaluates_forest_rating.py,sha256=UEwft8CY8jeXTrEmfZeUOU7hxMOhiHXpX4W6QJibXUE,316
@@ -103,14 +106,16 @@
 ml/fml40/features/properties/values/sawmill_delivery_parking_area_status.py,sha256=1cL7_72TWgOCGiibZVSUwbrNc9VB2emx5PjHpCYRdu4,307
 ml/fml40/features/properties/values/sawmill_entry_parking_area_status.py,sha256=FPH4rr_mH4bvxoYujJF63PqIrVc28hYUQ8hM8cjZRg4,304
 ml/fml40/features/properties/values/stand_attribute_set.py,sha256=wB0lXJkBTh6RjFr5nNAOIaJnf-DPHkrjkCy8LLoqh5g,268
 ml/fml40/features/properties/values/stem_segment_properties.py,sha256=TL_CKO-QqYtyGxD9kdzKsquiIPGdlPg_9c5dpHb07YE,1502
 ml/fml40/features/properties/values/stock_volume.py,sha256=jT1H1NONCDtbpGtvggoPlc8N8YKYhVV94z6o9TTuJKc,657
 ml/fml40/features/properties/values/suitable_tree_species.py,sha256=0prkntmaaoFufi-mcijw_gS4vei7bnwM86r6e4ayHxM,312
 ml/fml40/features/properties/values/thickness_class.py,sha256=tMhnDWmXpv9u7qddXpgNPgmZATHzUJIQmP9bJQfL6Fc,287
+ml/fml40/features/properties/values/timber_harvesting_capacity.py,sha256=ErU95UZkDvNVA4UP1qCAwKjvw_4FU07SVDFEyPGAEA4,307
+ml/fml40/features/properties/values/timber_harvesting_cost.py,sha256=PTnseJNF7QCJrOPinRfEcNa-yp9zJEgBbH-hItYkPM0,291
 ml/fml40/features/properties/values/tree_data.py,sha256=TLVkUsce2qIIggxNz62fYyDMulcgqAC-meLj5cTa0Jw,281
 ml/fml40/features/properties/values/tree_species.py,sha256=SVlhlsf4t6JGNwQXVk8EXfv4Z-5M_7NpBVUjBl1Hjrs,700
 ml/fml40/features/properties/values/tree_type.py,sha256=rpClFBJElYLKn_lwn5YymANRjJjAB4lYT1QEV04WEKs,684
 ml/fml40/features/properties/values/vegetationindex.py,sha256=A6n07rGC8InBMYrsQAI4m5bKqjUFQk1Fw_ogE9OHJjk,3165
 ml/fml40/features/properties/values/vitality_status.py,sha256=kXha5zwQknosLdyOiuZKWvwI7enpmRI7Nocs3d-p-VA,649
 ml/fml40/features/properties/values/wood_quality.py,sha256=zstocRCM_wKMLAN-slmUPAwWki1rh21zWH2gsBXSLiE,284
 ml/fml40/features/properties/values/documents/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -197,14 +202,15 @@
 ml/fml40/roles/services/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ml/ml40/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ml/ml40/features/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ml/ml40/features/functionalities/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ml/ml40/features/functionalities/accepts_jobs.py,sha256=MxfoCdi-ELnb7Cwqh2q9W6QbjrNBC0UhtFYBn3PdCyo,680
 ml/ml40/features/functionalities/accepts_reports.py,sha256=5ExZtfvs9K5dkvrSiF6QZDjHpfNzaZeTeOSVLyZZnyg,471
 ml/ml40/features/functionalities/clears_jobs.py,sha256=kXzb2WDAipPWjxHKh0y5qf6FlY98PO4Zs7wikxA4xh8,427
+ml/ml40/features/functionalities/controls_production.py,sha256=5lsvT2twJb1YINk_P7ImsR-Kh3tH8esEDBbXxMdDkAo,376
 ml/ml40/features/functionalities/functionality.py,sha256=hseOzQH126xKMurdFSVN_s2g_HUD_Ju7g6ZUTo3VUe0,330
 ml/ml40/features/functionalities/manages_jobs.py,sha256=33Jd3bPufS3-ED0xneQTx_DwIubN1ZGYBYoLLOJIzHE,633
 ml/ml40/features/functionalities/plans_routes.py,sha256=KWaKgLgdD0ScXrlI19bMHVzLj1x7OkPpZiNIijiPnps,510
 ml/ml40/features/functionalities/predicts_consumption.py,sha256=gYOZS9018MUg_dJ3XEYST1If7jSAgEcRACiSpVU1K8c,377
 ml/ml40/features/functionalities/predicts_maintenance.py,sha256=XD4QCnjSZGMaYRcMjFsVqhNnh2S95iYyxKqyLWZNLC8,377
 ml/ml40/features/functionalities/predicts_purchase.py,sha256=WxTWhiMrrBjjNJAM1EvlCLYVzMXjfjm9AnRujbBVD88,327
 ml/ml40/features/functionalities/provides_emissions_data.py,sha256=Ou_LzS3Jhmc2Db5WpRFZ4HBj3HJKNfBp8WONQLhqNpg,387
@@ -226,14 +232,15 @@
 ml/ml40/features/properties/values/address.py,sha256=UjrbKJMloafMO-lZhrF5FFh0WXAB7NTeudrkKQdcIDY,996
 ml/ml40/features/properties/values/air_pressure.py,sha256=XzJah_YWnQlJNRaqYftmuzKQ3SJbR8xE_tbX6kjPpJo,537
 ml/ml40/features/properties/values/air_volume.py,sha256=P9zP6XZSAY2v1TBb3oCoKjA28bI9Vxi4pY8e_lqVmNI,528
 ml/ml40/features/properties/values/area.py,sha256=0IBAtAeQtX8UwMTVK6JrC0-2Cj5qjD2rhxLWZe-qRzM,276
 ml/ml40/features/properties/values/bank_account.py,sha256=ZPihA14Zyi7JCRoYTwiGt_L3KP2P5Hg5G0og2jG9BVg,769
 ml/ml40/features/properties/values/brand.py,sha256=wxKk08jevADlf-ivC-OWcw2pUA1FY2PDgHb6r1n-GbM,516
 ml/ml40/features/properties/values/brightness.py,sha256=beMCxTOrKMoxaXkMFa-X5QSR_oNPKPDZ4xLMG_3ewFI,282
+ml/ml40/features/properties/values/capacity.py,sha256=Rf3I_Rha4aivmT3yOETiFTYD0_oPdhnXIdk26H_XA5Q,491
 ml/ml40/features/properties/values/contacts.py,sha256=dYC4Oxg-RPT0WfhkLTBifIWcNmQtpgI1ardOaPwgp50,315
 ml/ml40/features/properties/values/cost.py,sha256=2vgTf-umhBXHoWjLZcv8OEIoMpJsglHCkMN1lbzLcwk,515
 ml/ml40/features/properties/values/count.py,sha256=rxgydZ4hyHpuVNxkykpARNyIE_edwmOMbh0dKYtAu9g,795
 ml/ml40/features/properties/values/current_load.py,sha256=GAUth78GEQPJeW6JTTEDxJSThhF7HhwOQP7zpUuccDI,280
 ml/ml40/features/properties/values/current_weight.py,sha256=5j9NCco9k3iNblxXjNf0edhHPUkBHD-50sIi8-yaXds,288
 ml/ml40/features/properties/values/description.py,sha256=lhZA1OTrXnk3QBGfdeNxtOqFr_JWNiyQIF4HpehYkQc,526
 ml/ml40/features/properties/values/diameter.py,sha256=kLQi7P5U5jyVkDRkpfEraNHpXO20ycx4Fgf_YRqLhOY,524
@@ -309,14 +316,18 @@
 ml/ml40/features/properties/values/velocity.py,sha256=AVrl-c5HaOOkgGekQP8W4IsA0-nd9k5mJbsGGJKK_0Q,703
 ml/ml40/features/properties/values/volume.py,sha256=_NEZaarXQNHYpUHm4Ozuffaz2pO43hSXyi5guZrHT7E,522
 ml/ml40/features/properties/values/weatherdata.py,sha256=OxHVAiTDkd2GQPcb9aonsazsu_Ci0Johh40FbBqGJU8,2793
 ml/ml40/features/properties/values/weight.py,sha256=ci5RC8UAQkVO3YM5d2iSLBPtTufXicwyUU4W-d49KFE,669
 ml/ml40/features/properties/values/white_level.py,sha256=rlGQ9CVlTVf-yp2tTsBwkq_255E9MYM0drLt0Vl5ZFU,309
 ml/ml40/features/properties/values/documents/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ml/ml40/features/properties/values/documents/document.py,sha256=tUGqNBu690MWHly0QnPDR1bLOOBtFU5etM_tBhFlT4A,280
+ml/ml40/features/properties/values/documents/contacts/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ml/ml40/features/properties/values/documents/contacts/contact.py,sha256=KRaEs4Q9ihqRlCURXOTNc85GvVmK9o0RzkZBheYKDV4,1016
+ml/ml40/features/properties/values/documents/contacts/organizational_contact.py,sha256=gQdDlwcrJL913vs_qoNHkcufX3SxzvCedM6cm8xD2ZE,555
+ml/ml40/features/properties/values/documents/contacts/personal_contact.py,sha256=qrAxHq2O-_xu0LfVwfnA8LuLSJv7EQgfXcXEz8l43Wo,913
 ml/ml40/features/properties/values/documents/contracts/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ml/ml40/features/properties/values/documents/contracts/contract.py,sha256=XFb2iCKavtCCuLDyfooX0YpogZwlA7jkS3RZzMih8s0,299
 ml/ml40/features/properties/values/documents/jobs/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ml/ml40/features/properties/values/documents/jobs/generic_job.py,sha256=8j9iyYkyP_vDccLqXBOdCtDX3xdRUDRQ26DS9asIVEw,695
 ml/ml40/features/properties/values/documents/jobs/job.py,sha256=ouLcrOVA5tkB9NZufh3R3KEkhL25hZTK-4Ik18hxxsc,782
 ml/ml40/features/properties/values/documents/jobs/job_list.py,sha256=n6hS2-x4NLTZa4sGlyS6Q54oKZ5idoXBxjHf-SVv5pM,288
 ml/ml40/features/properties/values/documents/jobs/job_status.py,sha256=GoRxfx0nxiw3cZDBxGwPBOaqdhcx9-VuhVrLuf2BX30,99
@@ -346,14 +357,15 @@
 ml/ml40/roles/dts/parts/scale.py,sha256=0Q8onMR9dx2kvD9eZuwOSj5YzL5NFaZDfVTFuJLznq4,274
 ml/ml40/roles/dts/parts/tank.py,sha256=me9B25qLBBw6tvmmaM7LPHXY7wQ99rCB3DhDhImmeE4,272
 ml/ml40/roles/dts/parts/wheel.py,sha256=smsQznwaHy2D58_1r5tgAPG6Z-B1tk2Ayz5fJP7Dsx0,274
 ml/ml40/roles/dts/parts/winch.py,sha256=YQywNVwhPMfZqaa-QrNGrfOMoUV63uDW3D1DMJrVpEs,274
 ml/ml40/roles/dts/persons/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ml/ml40/roles/dts/persons/machine_operator.py,sha256=MZZ3Vss3nlm5DIHK8OpNBKI2uaOf1um2HvMDHbrRUs8,302
 ml/ml40/roles/dts/persons/person.py,sha256=arDzt_2VLq9uWflZ2FlOqhcsk-ldmxsFnROu86Qj7mQ,242
+ml/ml40/roles/dts/persons/precinct_leader.py,sha256=nDLTdGEalimcLQljWiJrs75MzWtTXqQqgrhTsiqKqkQ,277
 ml/ml40/roles/dts/sensors/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ml/ml40/roles/dts/sensors/accelerometer.py,sha256=fQQTS5YtmBPpkGd65-6QuSQ4f_aI2--R8Y7jtCPYx9E,279
 ml/ml40/roles/dts/sensors/air_sensor.py,sha256=6NRY9eFpWXD1z0BYBtFcT-OZ0s9nOOfAoCfIJw7Exjc,290
 ml/ml40/roles/dts/sensors/counter_sensor.py,sha256=XM1rjyA866ZmMJjGSKw9FqlSE9A1lNXuuSkMrtxNGbA,298
 ml/ml40/roles/dts/sensors/gyroscope.py,sha256=Fd4b_puUZ2cm6kS_0_AAVcliaZxulzblEMPWltVyyg0,290
 ml/ml40/roles/dts/sensors/high_speed_camera.py,sha256=L8ACQQx_q-HPXnd0WCxcTTtZEaoOA92_7H3aYZWKSNQ,274
 ml/ml40/roles/dts/sensors/imu.py,sha256=Y5AafN2HO8Ly-oa6sib6_Efv3CAY68-hxcx5cL4LDVw,295
@@ -428,12 +440,12 @@
 ml/wml40/roles/dts/water/water.py,sha256=EkIdLUwG6NFFk0eFuooIv2Aa_MZzGm7WXAblFktqQWw,252
 ml/wml40/roles/dts/water/waterreservoir.py,sha256=BiXgiP7EFtV43RiI_xwdsVyz9QFSzJj59r_a26Sd8ec,277
 ml/wml40/roles/hmis/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ml/wml40/roles/services/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/test_async.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/test_entry.py,sha256=r9lHxwSp6WbRu9fvh15q5hmMCEUC-P6MjlSekCiXibc,48
-fml40_reference_implementation-0.2.8.dist-info/LICENSE.txt,sha256=pWgb-bBdsU2Gd2kwAXxketnm5W_2u8_fIeWEgojfrxs,7651
-fml40_reference_implementation-0.2.8.dist-info/METADATA,sha256=NB-7wfVqrj6zj9kKMDhK8hUxH3l4bXyxbf_6pHEZci8,8893
-fml40_reference_implementation-0.2.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-fml40_reference_implementation-0.2.8.dist-info/top_level.txt,sha256=zi2IoIakYFZNb4sNVwCx-zsTTM-9E_fUQkhRTH7Tivs,22
-fml40_reference_implementation-0.2.8.dist-info/RECORD,,
+fml40_reference_implementation-0.2.9.dist-info/LICENSE.txt,sha256=pWgb-bBdsU2Gd2kwAXxketnm5W_2u8_fIeWEgojfrxs,7651
+fml40_reference_implementation-0.2.9.dist-info/METADATA,sha256=XvPBzuvVvNYASC7zLIPYnJkX6RIL1Uu-KXXvu5WpDe8,8893
+fml40_reference_implementation-0.2.9.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+fml40_reference_implementation-0.2.9.dist-info/top_level.txt,sha256=zi2IoIakYFZNb4sNVwCx-zsTTM-9E_fUQkhRTH7Tivs,22
+fml40_reference_implementation-0.2.9.dist-info/RECORD,,
```

