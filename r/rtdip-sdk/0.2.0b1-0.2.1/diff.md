# Comparing `tmp/rtdip_sdk-0.2.0b1-py3-none-any.whl.zip` & `tmp/rtdip_sdk-0.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,71 +1,81 @@
-Zip file size: 76037 bytes, number of entries: 69
--rw-r--r--  2.0 unx      571 b- defN 23-Mar-30 10:26 rtdip_sdk/__init__.py
--rw-r--r--  2.0 unx      571 b- defN 23-Mar-30 10:26 rtdip_sdk/authentication/__init__.py
--rw-r--r--  2.0 unx     7210 b- defN 23-Mar-30 10:26 rtdip_sdk/authentication/authenticate.py
--rw-r--r--  2.0 unx      571 b- defN 23-Mar-30 10:26 rtdip_sdk/functions/__init__.py
--rw-r--r--  2.0 unx     8746 b- defN 23-Mar-30 10:26 rtdip_sdk/functions/_query_builder.py
--rw-r--r--  2.0 unx     2908 b- defN 23-Mar-30 10:26 rtdip_sdk/functions/interpolate.py
--rw-r--r--  2.0 unx     2293 b- defN 23-Mar-30 10:26 rtdip_sdk/functions/metadata.py
--rw-r--r--  2.0 unx     2786 b- defN 23-Mar-30 10:26 rtdip_sdk/functions/raw.py
--rw-r--r--  2.0 unx     3052 b- defN 23-Mar-30 10:26 rtdip_sdk/functions/resample.py
--rw-r--r--  2.0 unx     8921 b- defN 23-Mar-30 10:26 rtdip_sdk/functions/time_weighted_average.py
--rw-r--r--  2.0 unx      571 b- defN 23-Mar-30 10:26 rtdip_sdk/odbc/__init__.py
--rw-r--r--  2.0 unx      934 b- defN 23-Mar-30 10:26 rtdip_sdk/odbc/connection_interface.py
--rw-r--r--  2.0 unx      952 b- defN 23-Mar-30 10:26 rtdip_sdk/odbc/cursor_interface.py
--rw-r--r--  2.0 unx     3498 b- defN 23-Mar-30 10:26 rtdip_sdk/odbc/db_sql_connector.py
--rw-r--r--  2.0 unx     4228 b- defN 23-Mar-30 10:26 rtdip_sdk/odbc/pyodbc_sql_connector.py
--rw-r--r--  2.0 unx     4432 b- defN 23-Mar-30 10:26 rtdip_sdk/odbc/turbodbc_sql_connector.py
--rw-r--r--  2.0 unx      569 b- defN 23-Mar-30 10:26 rtdip_sdk/pipelines/__init__.py
--rw-r--r--  2.0 unx     1035 b- defN 23-Mar-30 10:26 rtdip_sdk/pipelines/interfaces.py
--rw-r--r--  2.0 unx      569 b- defN 23-Mar-30 10:26 rtdip_sdk/pipelines/_pipeline_utils/__init__.py
--rw-r--r--  2.0 unx     2059 b- defN 23-Mar-30 10:26 rtdip_sdk/pipelines/_pipeline_utils/constants.py
--rw-r--r--  2.0 unx     2434 b- defN 23-Mar-30 10:26 rtdip_sdk/pipelines/_pipeline_utils/models.py
--rw-r--r--  2.0 unx     3295 b- defN 23-Mar-30 10:26 rtdip_sdk/pipelines/_pipeline_utils/spark.py
--rw-r--r--  2.0 unx      603 b- defN 23-Mar-30 10:26 rtdip_sdk/pipelines/converters/__init__.py
--rw-r--r--  2.0 unx      697 b- defN 23-Mar-30 10:26 rtdip_sdk/pipelines/converters/interfaces.py
--rw-r--r--  2.0 unx     3424 b- defN 23-Mar-30 10:26 rtdip_sdk/pipelines/converters/pipeline_job_json.py
--rw-r--r--  2.0 unx      571 b- defN 23-Mar-30 10:26 rtdip_sdk/pipelines/deploy/__init__.py
--rw-r--r--  2.0 unx    13229 b- defN 23-Mar-30 10:26 rtdip_sdk/pipelines/deploy/databricks.py
--rw-r--r--  2.0 unx      751 b- defN 23-Mar-30 10:26 rtdip_sdk/pipelines/deploy/interfaces.py
--rw-r--r--  2.0 unx      571 b- defN 23-Mar-30 10:26 rtdip_sdk/pipelines/deploy/dbx/__init__.py
--rw-r--r--  2.0 unx     1114 b- defN 23-Mar-30 10:26 rtdip_sdk/pipelines/deploy/dbx/setup.py
--rw-r--r--  2.0 unx      571 b- defN 23-Mar-30 10:26 rtdip_sdk/pipelines/deploy/dbx/rtdip/__init__.py
--rw-r--r--  2.0 unx      571 b- defN 23-Mar-30 10:26 rtdip_sdk/pipelines/deploy/dbx/rtdip/tasks/__init__.py
--rw-r--r--  2.0 unx     3310 b- defN 23-Mar-30 10:26 rtdip_sdk/pipelines/deploy/dbx/rtdip/tasks/common.py
--rw-r--r--  2.0 unx     1686 b- defN 23-Mar-30 10:26 rtdip_sdk/pipelines/deploy/dbx/rtdip/tasks/pipeline_task.py
--rw-r--r--  2.0 unx      571 b- defN 23-Mar-30 10:26 rtdip_sdk/pipelines/deploy/models/__init__.py
--rw-r--r--  2.0 unx     7897 b- defN 23-Mar-30 10:26 rtdip_sdk/pipelines/deploy/models/databricks.py
--rw-r--r--  2.0 unx      627 b- defN 23-Mar-30 10:26 rtdip_sdk/pipelines/destinations/__init__.py
--rw-r--r--  2.0 unx      427 b- defN 23-Mar-30 10:26 rtdip_sdk/pipelines/destinations/interfaces.py
--rw-r--r--  2.0 unx      569 b- defN 23-Mar-30 10:26 rtdip_sdk/pipelines/destinations/spark/__init__.py
--rw-r--r--  2.0 unx     5093 b- defN 23-Mar-30 10:26 rtdip_sdk/pipelines/destinations/spark/delta.py
--rw-r--r--  2.0 unx     4516 b- defN 23-Mar-30 10:26 rtdip_sdk/pipelines/destinations/spark/eventhub.py
--rw-r--r--  2.0 unx      611 b- defN 23-Mar-30 10:26 rtdip_sdk/pipelines/execute/__init__.py
--rw-r--r--  2.0 unx     1448 b- defN 23-Mar-30 10:26 rtdip_sdk/pipelines/execute/container.py
--rw-r--r--  2.0 unx     8378 b- defN 23-Mar-30 10:26 rtdip_sdk/pipelines/execute/job.py
--rw-r--r--  2.0 unx     3037 b- defN 23-Mar-30 10:26 rtdip_sdk/pipelines/execute/models.py
--rw-r--r--  2.0 unx      596 b- defN 23-Mar-30 10:26 rtdip_sdk/pipelines/secrets/__init__.py
--rw-r--r--  2.0 unx     2227 b- defN 23-Mar-30 10:26 rtdip_sdk/pipelines/secrets/databricks.py
--rw-r--r--  2.0 unx      824 b- defN 23-Mar-30 10:26 rtdip_sdk/pipelines/secrets/interfaces.py
--rw-r--r--  2.0 unx      887 b- defN 23-Mar-30 10:26 rtdip_sdk/pipelines/secrets/models.py
--rw-r--r--  2.0 unx      694 b- defN 23-Mar-30 10:26 rtdip_sdk/pipelines/sources/__init__.py
--rw-r--r--  2.0 unx      993 b- defN 23-Mar-30 10:26 rtdip_sdk/pipelines/sources/interfaces.py
--rw-r--r--  2.0 unx      569 b- defN 23-Mar-30 10:26 rtdip_sdk/pipelines/sources/spark/__init__.py
--rw-r--r--  2.0 unx     3400 b- defN 23-Mar-30 10:26 rtdip_sdk/pipelines/sources/spark/autoloader.py
--rw-r--r--  2.0 unx     4487 b- defN 23-Mar-30 10:26 rtdip_sdk/pipelines/sources/spark/delta.py
--rw-r--r--  2.0 unx     4459 b- defN 23-Mar-30 10:26 rtdip_sdk/pipelines/sources/spark/delta_sharing.py
--rw-r--r--  2.0 unx     5322 b- defN 23-Mar-30 10:26 rtdip_sdk/pipelines/sources/spark/eventhub.py
--rw-r--r--  2.0 unx      600 b- defN 23-Mar-30 10:26 rtdip_sdk/pipelines/transformers/__init__.py
--rw-r--r--  2.0 unx      946 b- defN 23-Mar-30 10:26 rtdip_sdk/pipelines/transformers/interfaces.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-30 10:26 rtdip_sdk/pipelines/transformers/spark/__init__.py
--rw-r--r--  2.0 unx     1715 b- defN 23-Mar-30 10:26 rtdip_sdk/pipelines/transformers/spark/eventhub.py
--rw-r--r--  2.0 unx      569 b- defN 23-Mar-30 10:26 rtdip_sdk/pipelines/utilities/__init__.py
--rw-r--r--  2.0 unx      773 b- defN 23-Mar-30 10:26 rtdip_sdk/pipelines/utilities/interfaces.py
--rw-r--r--  2.0 unx      569 b- defN 23-Mar-30 10:26 rtdip_sdk/pipelines/utilities/spark/__init__.py
--rw-r--r--  2.0 unx     3857 b- defN 23-Mar-30 10:26 rtdip_sdk/pipelines/utilities/spark/delta_table_create.py
--rw-r--r--  2.0 unx    10172 b- defN 23-Mar-30 10:27 rtdip_sdk-0.2.0b1.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     3012 b- defN 23-Mar-30 10:27 rtdip_sdk-0.2.0b1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-30 10:27 rtdip_sdk-0.2.0b1.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Mar-30 10:27 rtdip_sdk-0.2.0b1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     6687 b- defN 23-Mar-30 10:27 rtdip_sdk-0.2.0b1.dist-info/RECORD
-69 files, 175937 bytes uncompressed, 65083 bytes compressed:  63.0%
+Zip file size: 92459 bytes, number of entries: 79
+-rw-r--r--  2.0 unx      571 b- defN 23-Apr-21 15:32 rtdip_sdk/__init__.py
+-rw-r--r--  2.0 unx      571 b- defN 23-Apr-21 15:32 rtdip_sdk/authentication/__init__.py
+-rw-r--r--  2.0 unx     7210 b- defN 23-Apr-21 15:32 rtdip_sdk/authentication/authenticate.py
+-rw-r--r--  2.0 unx      571 b- defN 23-Apr-21 15:32 rtdip_sdk/functions/__init__.py
+-rw-r--r--  2.0 unx     8746 b- defN 23-Apr-21 15:32 rtdip_sdk/functions/_query_builder.py
+-rw-r--r--  2.0 unx     2908 b- defN 23-Apr-21 15:32 rtdip_sdk/functions/interpolate.py
+-rw-r--r--  2.0 unx     2293 b- defN 23-Apr-21 15:32 rtdip_sdk/functions/metadata.py
+-rw-r--r--  2.0 unx     2786 b- defN 23-Apr-21 15:32 rtdip_sdk/functions/raw.py
+-rw-r--r--  2.0 unx     3052 b- defN 23-Apr-21 15:32 rtdip_sdk/functions/resample.py
+-rw-r--r--  2.0 unx     8921 b- defN 23-Apr-21 15:32 rtdip_sdk/functions/time_weighted_average.py
+-rw-r--r--  2.0 unx      571 b- defN 23-Apr-21 15:32 rtdip_sdk/odbc/__init__.py
+-rw-r--r--  2.0 unx      934 b- defN 23-Apr-21 15:32 rtdip_sdk/odbc/connection_interface.py
+-rw-r--r--  2.0 unx      952 b- defN 23-Apr-21 15:32 rtdip_sdk/odbc/cursor_interface.py
+-rw-r--r--  2.0 unx     3498 b- defN 23-Apr-21 15:32 rtdip_sdk/odbc/db_sql_connector.py
+-rw-r--r--  2.0 unx     4228 b- defN 23-Apr-21 15:32 rtdip_sdk/odbc/pyodbc_sql_connector.py
+-rw-r--r--  2.0 unx     4432 b- defN 23-Apr-21 15:32 rtdip_sdk/odbc/turbodbc_sql_connector.py
+-rw-r--r--  2.0 unx      569 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/__init__.py
+-rw-r--r--  2.0 unx     1035 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/interfaces.py
+-rw-r--r--  2.0 unx      569 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/_pipeline_utils/__init__.py
+-rw-r--r--  2.0 unx     1485 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/_pipeline_utils/constants.py
+-rw-r--r--  2.0 unx     2434 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/_pipeline_utils/models.py
+-rw-r--r--  2.0 unx     5327 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/_pipeline_utils/spark.py
+-rw-r--r--  2.0 unx      603 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/converters/__init__.py
+-rw-r--r--  2.0 unx      697 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/converters/interfaces.py
+-rw-r--r--  2.0 unx     3424 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/converters/pipeline_job_json.py
+-rw-r--r--  2.0 unx      630 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/deploy/__init__.py
+-rw-r--r--  2.0 unx    13189 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/deploy/databricks.py
+-rw-r--r--  2.0 unx      751 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/deploy/interfaces.py
+-rw-r--r--  2.0 unx      571 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/deploy/dbx/__init__.py
+-rw-r--r--  2.0 unx     1114 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/deploy/dbx/setup.py
+-rw-r--r--  2.0 unx      571 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/deploy/dbx/conf/__init__.py
+-rw-r--r--  2.0 unx      571 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/deploy/dbx/rtdip/__init__.py
+-rw-r--r--  2.0 unx      571 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/deploy/dbx/rtdip/tasks/__init__.py
+-rw-r--r--  2.0 unx     3310 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/deploy/dbx/rtdip/tasks/common.py
+-rw-r--r--  2.0 unx     1686 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/deploy/dbx/rtdip/tasks/pipeline_task.py
+-rw-r--r--  2.0 unx      571 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/deploy/models/__init__.py
+-rw-r--r--  2.0 unx     7897 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/deploy/models/databricks.py
+-rw-r--r--  2.0 unx      684 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/destinations/__init__.py
+-rw-r--r--  2.0 unx      427 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/destinations/interfaces.py
+-rw-r--r--  2.0 unx      569 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/destinations/spark/__init__.py
+-rw-r--r--  2.0 unx     5112 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/destinations/spark/delta.py
+-rw-r--r--  2.0 unx     4781 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/destinations/spark/eventhub.py
+-rw-r--r--  2.0 unx     3903 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/destinations/spark/kafka.py
+-rw-r--r--  2.0 unx     3659 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/destinations/spark/kinesis.py
+-rw-r--r--  2.0 unx      611 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/execute/__init__.py
+-rw-r--r--  2.0 unx     1448 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/execute/container.py
+-rw-r--r--  2.0 unx     8378 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/execute/job.py
+-rw-r--r--  2.0 unx     3037 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/execute/models.py
+-rw-r--r--  2.0 unx      618 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/secrets/__init__.py
+-rw-r--r--  2.0 unx     2227 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/secrets/databricks.py
+-rw-r--r--  2.0 unx      824 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/secrets/interfaces.py
+-rw-r--r--  2.0 unx      887 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/secrets/models.py
+-rw-r--r--  2.0 unx      779 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/sources/__init__.py
+-rw-r--r--  2.0 unx      993 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/sources/interfaces.py
+-rw-r--r--  2.0 unx      569 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/sources/spark/__init__.py
+-rw-r--r--  2.0 unx     3420 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/sources/spark/autoloader.py
+-rw-r--r--  2.0 unx     4501 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/sources/spark/delta.py
+-rw-r--r--  2.0 unx     4473 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/sources/spark/delta_sharing.py
+-rw-r--r--  2.0 unx     5259 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/sources/spark/eventhub.py
+-rw-r--r--  2.0 unx     5240 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/sources/spark/iot_hub.py
+-rw-r--r--  2.0 unx     8114 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/sources/spark/kafka.py
+-rw-r--r--  2.0 unx     3793 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/sources/spark/kinesis.py
+-rw-r--r--  2.0 unx      692 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/transformers/__init__.py
+-rw-r--r--  2.0 unx      946 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/transformers/interfaces.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/transformers/spark/__init__.py
+-rw-r--r--  2.0 unx     1715 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/transformers/spark/eventhub.py
+-rw-r--r--  2.0 unx     2900 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/transformers/spark/json_to_opcua.py
+-rw-r--r--  2.0 unx     3560 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/transformers/spark/opcua_to_process_control_data_model.py
+-rw-r--r--  2.0 unx      692 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/utilities/__init__.py
+-rw-r--r--  2.0 unx      773 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/utilities/interfaces.py
+-rw-r--r--  2.0 unx      569 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/utilities/spark/__init__.py
+-rw-r--r--  2.0 unx     3857 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/utilities/spark/delta_table_create.py
+-rw-r--r--  2.0 unx     3119 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/utilities/spark/delta_table_optimize.py
+-rw-r--r--  2.0 unx     2602 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/utilities/spark/delta_table_vacuum.py
+-rw-r--r--  2.0 unx    10172 b- defN 23-Apr-21 15:32 rtdip_sdk-0.2.1.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     2709 b- defN 23-Apr-21 15:32 rtdip_sdk-0.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-21 15:32 rtdip_sdk-0.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Apr-21 15:32 rtdip_sdk-0.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     7767 b- defN 23-Apr-21 15:32 rtdip_sdk-0.2.1.dist-info/RECORD
+79 files, 216300 bytes uncompressed, 79723 bytes compressed:  63.1%
```

## zipnote {}

```diff
@@ -84,14 +84,17 @@
 
 Filename: rtdip_sdk/pipelines/deploy/dbx/__init__.py
 Comment: 
 
 Filename: rtdip_sdk/pipelines/deploy/dbx/setup.py
 Comment: 
 
+Filename: rtdip_sdk/pipelines/deploy/dbx/conf/__init__.py
+Comment: 
+
 Filename: rtdip_sdk/pipelines/deploy/dbx/rtdip/__init__.py
 Comment: 
 
 Filename: rtdip_sdk/pipelines/deploy/dbx/rtdip/tasks/__init__.py
 Comment: 
 
 Filename: rtdip_sdk/pipelines/deploy/dbx/rtdip/tasks/common.py
@@ -117,14 +120,20 @@
 
 Filename: rtdip_sdk/pipelines/destinations/spark/delta.py
 Comment: 
 
 Filename: rtdip_sdk/pipelines/destinations/spark/eventhub.py
 Comment: 
 
+Filename: rtdip_sdk/pipelines/destinations/spark/kafka.py
+Comment: 
+
+Filename: rtdip_sdk/pipelines/destinations/spark/kinesis.py
+Comment: 
+
 Filename: rtdip_sdk/pipelines/execute/__init__.py
 Comment: 
 
 Filename: rtdip_sdk/pipelines/execute/container.py
 Comment: 
 
 Filename: rtdip_sdk/pipelines/execute/job.py
@@ -162,47 +171,68 @@
 
 Filename: rtdip_sdk/pipelines/sources/spark/delta_sharing.py
 Comment: 
 
 Filename: rtdip_sdk/pipelines/sources/spark/eventhub.py
 Comment: 
 
+Filename: rtdip_sdk/pipelines/sources/spark/iot_hub.py
+Comment: 
+
+Filename: rtdip_sdk/pipelines/sources/spark/kafka.py
+Comment: 
+
+Filename: rtdip_sdk/pipelines/sources/spark/kinesis.py
+Comment: 
+
 Filename: rtdip_sdk/pipelines/transformers/__init__.py
 Comment: 
 
 Filename: rtdip_sdk/pipelines/transformers/interfaces.py
 Comment: 
 
 Filename: rtdip_sdk/pipelines/transformers/spark/__init__.py
 Comment: 
 
 Filename: rtdip_sdk/pipelines/transformers/spark/eventhub.py
 Comment: 
 
+Filename: rtdip_sdk/pipelines/transformers/spark/json_to_opcua.py
+Comment: 
+
+Filename: rtdip_sdk/pipelines/transformers/spark/opcua_to_process_control_data_model.py
+Comment: 
+
 Filename: rtdip_sdk/pipelines/utilities/__init__.py
 Comment: 
 
 Filename: rtdip_sdk/pipelines/utilities/interfaces.py
 Comment: 
 
 Filename: rtdip_sdk/pipelines/utilities/spark/__init__.py
 Comment: 
 
 Filename: rtdip_sdk/pipelines/utilities/spark/delta_table_create.py
 Comment: 
 
-Filename: rtdip_sdk-0.2.0b1.dist-info/LICENSE.md
+Filename: rtdip_sdk/pipelines/utilities/spark/delta_table_optimize.py
+Comment: 
+
+Filename: rtdip_sdk/pipelines/utilities/spark/delta_table_vacuum.py
+Comment: 
+
+Filename: rtdip_sdk-0.2.1.dist-info/LICENSE.md
 Comment: 
 
-Filename: rtdip_sdk-0.2.0b1.dist-info/METADATA
+Filename: rtdip_sdk-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: rtdip_sdk-0.2.0b1.dist-info/WHEEL
+Filename: rtdip_sdk-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: rtdip_sdk-0.2.0b1.dist-info/top_level.txt
+Filename: rtdip_sdk-0.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: rtdip_sdk-0.2.0b1.dist-info/RECORD
+Filename: rtdip_sdk-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rtdip_sdk/functions/interpolate.py

```diff
@@ -25,15 +25,15 @@
     This function requires the user to input a dictionary of parameters. (See Attributes table below.)
 
     Args:
         connection: Connection chosen by the user (Databricks SQL Connect, PYODBC SQL Connect, TURBODBC SQL Connect)
         parameters_dict: A dictionary of parameters (see Attributes table below)
 
     Attributes:
-        buisness_unit (str): Business unit of the data
+        business_unit (str): Business unit of the data
         region (str): Region
         asset (str):  Asset
         data_security_level (str): Level of data security 
         data_type (str): Type of the data (float, integer, double, string)
         tag_names (list): List of tagname or tagnames ["tag_1", "tag_2"]
         start_date (str): Start date (Either a date in the format YY-MM-DD or a datetime in the format YYY-MM-DDTHH:MM:SS)
         end_date (str): End date (Either a date in the format YY-MM-DD or a datetime in the format YYY-MM-DDTHH:MM:SS)
```

## rtdip_sdk/functions/metadata.py

```diff
@@ -27,15 +27,15 @@
     This function requires the user to input a dictionary of parameters. (See Attributes table below)
     
     Args:
         connection: Connection chosen by the user (Databricks SQL Connect, PYODBC SQL Connect, TURBODBC SQL Connect)
         parameters_dict: A dictionary of parameters (see Attributes table below)
 
     Attributes:
-        buisness_unit (str): Business unit
+        business_unit (str): Business unit
         region (str): Region
         asset (str): Asset 
         data_security_level (str): Level of data security
         tag_names (list): (Optional) Either pass a list of tagname/tagnames ["tag_1", "tag_2"] or leave the list blank [] or leave the parameter out completely
 
     Returns:
         DataFrame: A dataframe of metadata.
```

## rtdip_sdk/functions/raw.py

```diff
@@ -28,15 +28,15 @@
     This function requires the user to input a dictionary of parameters. (See Attributes table below)
     
     Args:
         connection: Connection chosen by the user (Databricks SQL Connect, PYODBC SQL Connect, TURBODBC SQL Connect)
         parameters_dict: A dictionary of parameters (see Attributes table below)
 
     Attributes:
-        buisness_unit (str): Business unit 
+        business_unit (str): Business unit 
         region (str): Region
         asset (str): Asset 
         data_security_level (str): Level of data security
         data_type (str): Type of the data (float, integer, double, string)
         tag_names (list): List of tagname or tagnames ["tag_1", "tag_2"]
         start_date (str): Start date (Either a date in the format YY-MM-DD or a datetime in the format YYY-MM-DDTHH:MM:SS)
         end_date (str): End date (Either a date in the format YY-MM-DD or a datetime in the format YYY-MM-DDTHH:MM:SS)
```

## rtdip_sdk/functions/resample.py

```diff
@@ -27,15 +27,15 @@
     This function requires the user to input a dictionary of parameters. (See Attributes table below)
 
     Args:
         connection: Connection chosen by the user (Databricks SQL Connect, PYODBC SQL Connect, TURBODBC SQL Connect)
         parameters_dict: A dictionary of parameters (see Attributes table below)
 
     Attributes:
-        buisness_unit (str): Business unit of the data
+        business_unit (str): Business unit of the data
         region (str): Region
         asset (str):  Asset
         data_security_level (str): Level of data security
         data_type (str): Type of the data (float, integer, double, string)
         tag_names (list): List of tagname or tagnames ["tag_1", "tag_2"]
         start_date (str): Start date (Either a date in the format YY-MM-DD or a datetime in the format YYY-MM-DDTHH:MM:SS)
         end_date (str): End date (Either a date in the format YY-MM-DD or a datetime in the format YYY-MM-DDTHH:MM:SS)
```

## rtdip_sdk/pipelines/_pipeline_utils/constants.py

```diff
@@ -9,42 +9,34 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from .models import MavenLibrary, PyPiLibrary
-from pyspark.sql.types import StructType, StructField, TimestampType, StringType, BinaryType, LongType, MapType
 
 DEFAULT_PACKAGES = {
     "spark_delta_core": MavenLibrary(
                 group_id="io.delta",
                 artifact_id="delta-core_2.12",
-                version="2.2.0"
+                version="2.3.0"
             ),
     "spark_delta_sharing": MavenLibrary(
                 group_id="io.delta",
                 artifact_id="delta-sharing-spark_2.12",
-                version="0.6.2"
+                version="0.6.3"
             ),
     "spark_azure_eventhub": MavenLibrary(
                 group_id="com.microsoft.azure", 
                 artifact_id="azure-eventhubs-spark_2.12",
                 version="2.3.22"
             ),
+    "spark_sql_kafka": MavenLibrary(
+                group_id="org.apache.spark", 
+                artifact_id="spark-sql-kafka-0-10_2.12",
+                version="3.4.0"
+            ),
     "rtdip_sdk": PyPiLibrary(
                 name="rtdip_sdk",
-                version="0.1.7"
+                version="0.2.0"
             )
 }
-
-EVENTHUB_SCHEMA = StructType(
-            [StructField('body', BinaryType(), True), 
-             StructField('partition', StringType(), True), 
-             StructField('offset', StringType(), True), 
-             StructField('sequenceNumber', LongType(), True), 
-             StructField('enqueuedTime', TimestampType(), True), 
-             StructField('publisher', StringType(), True), 
-             StructField('partitionKey', StringType(), True), 
-             StructField('properties', MapType(StringType(), StringType(), True), True), 
-             StructField('systemProperties', MapType(StringType(), StringType(), True), True)]
-        )
```

## rtdip_sdk/pipelines/_pipeline_utils/spark.py

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import logging
 from pyspark.sql import SparkSession
+from pyspark.sql.types import StructType, StructField, TimestampType, StringType, BinaryType, LongType, MapType, IntegerType
 from .models import Libraries
 
 class SparkClient():
     spark_configuration: dict
     spark_libraries: Libraries
     spark_session: SparkSession
     
@@ -78,8 +79,53 @@
 #     def onQueryStarted(self, event):
 #         logging.info("Query started: {} {}".format(event.id, event.name))
 
 #     def onQueryProgress(self, event):
 #         logging.info("Query Progress: {}".format(event))
 
 #     def onQueryTerminated(self, event):
-#         logging.info("Query terminated: {} {}".format(event.id, event.name))
+#         logging.info("Query terminated: {} {}".format(event.id, event.name))
+
+EVENTHUB_SCHEMA = StructType([
+    StructField('body', BinaryType(), True), 
+    StructField('partition', StringType(), True), 
+    StructField('offset', StringType(), True), 
+    StructField('sequenceNumber', LongType(), True), 
+    StructField('enqueuedTime', TimestampType(), True), 
+    StructField('publisher', StringType(), True), 
+    StructField('partitionKey', StringType(), True), 
+    StructField('properties', MapType(StringType(), StringType(), True), True), 
+    StructField('systemProperties', MapType(StringType(), StringType(), True), True)
+])
+
+OPCUA_SCHEMA = StructType([
+    StructField('ApplicationUri',StringType(),True),
+    StructField('DisplayName',StringType(),True),
+    StructField('NodeId', StringType(),True),
+    StructField('Value', StructType([
+        StructField('SourceTimestamp',StringType(),True),
+        StructField('StatusCode', StructType([
+            StructField('Code', LongType(),True),
+            StructField('Symbol', StringType(),True)
+        ]), True),
+        StructField('Value',StringType(),True)
+    ]),True)
+])
+
+KAFKA_SCHEMA = StructType(
+           [StructField('key', BinaryType(), True),
+            StructField('value', BinaryType(), True),
+            StructField('topic', StringType(), True),
+            StructField('partition', IntegerType(), True),
+            StructField('offset', LongType(), True),
+            StructField('timestamp', TimestampType(), True),
+            StructField('timestampType', IntegerType(), True)]
+       )
+
+KINESIS_SCHEMA = StructType(
+           [StructField('partitionKey', StringType(), True),
+            StructField('data', BinaryType(), True),
+            StructField('stream', StringType(), True),
+            StructField('shardId', StringType(), True),
+            StructField('sequenceNumber', StringType(), True),
+            StructField('approximateArrivalTimestamp', TimestampType(), True)]
+       )
```

## rtdip_sdk/pipelines/deploy/__init__.py

```diff
@@ -8,7 +8,9 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from .databricks import *
+from .models.databricks import *
```

## rtdip_sdk/pipelines/deploy/databricks.py

```diff
@@ -92,17 +92,14 @@
     Args:
         pipeline_job (PipelineJob): Pipeline Job containing tasks and steps that are to be deployed
         databricks_job_for_pipeline_job (DatabricksJobForPipelineJob): Contains Databricks specific information required for deploying the RTDIP Pipeline Job to Databricks, such as cluster and workflow scheduling information. This can be any field in the [Databricks Jobs REST API v2.1](https://docs.databricks.com/dev-tools/api/latest/jobs.html)
         host (str): Databricks URL
         token (str): Token for authenticating with Databricks such as a Databricks PAT Token or Azure AD Token
         workspace_directory (str, optional): Determines the folder location in the Databricks Workspace. Defaults to /rtdip 
         artifacts_directory (str, optional): Determines the folder location in the Databricks Workspace. Defaults to dbfs:/rtdip/projects
-
-
-
     '''
     pipeline_job: PipelineJob
     databricks_job_for_pipeline_job: DatabricksJobForPipelineJob
     host: str
     token: str
     workspace_directory: str
     artifacts_directory: str
@@ -166,15 +163,15 @@
             try:
                 rtdip_version = version("rtdip-sdk")
                 databricks_job_task.libraries.append(DatabricksLibraries(pypi=DatbricksLibrariesPypi(package="rtdip-sdk[pipelines]=={}".format(rtdip_version))))
             except PackageNotFoundError as e:
                 databricks_job_task.libraries.append(DatabricksLibraries(pypi=DatbricksLibrariesPypi(package="rtdip-sdk[pipelines]")))
 
             databricks_job_task.spark_python_task = DatabricksSparkPythonTask(
-                python_file="file://{}".format("rtdip/tasks/pipeline_task.py"), #.format(task_python_file_location),
+                python_file="file://{}".format("rtdip/tasks/pipeline_task.py"),
                 parameters=[PipelineJobToJson(self.pipeline_job).convert()]
             )
             databricks_tasks.append(databricks_job_task)
 
         databricks_job = DatabricksJob(name=self.pipeline_job.name, tasks=databricks_tasks)
         databricks_job.__dict__.update(self.databricks_job_for_pipeline_job.__dict__)
         databricks_job.__dict__.pop("databricks_task_for_pipeline_task_list", None)
```

## rtdip_sdk/pipelines/destinations/__init__.py

```diff
@@ -9,8 +9,10 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from .spark.delta import *
-from .spark.eventhub import *
+from .spark.eventhub import *
+from .spark.kafka import *
+from .spark.kinesis import *
```

## rtdip_sdk/pipelines/destinations/spark/delta.py

```diff
@@ -22,17 +22,17 @@
 from ..._pipeline_utils.constants import DEFAULT_PACKAGES
 
 class SparkDeltaDestination(DestinationInterface):
     '''
     The Spark Delta Source is used to write data to a Delta table. 
 
     Args:
-        table_name: Name of the Hive Metastore or Unity Catalog Delta Table
-        options: Options that can be specified for a Delta Table read operation (See Attributes table below). Further information on the options is available for [batch](https://docs.delta.io/latest/delta-batch.html#write-to-a-table){ target="_blank" } and [streaming](https://docs.delta.io/latest/delta-streaming.html#delta-table-as-a-sink){ target="_blank" }.
-        mode: Method of writing to Delta Table - append/overwrite (batch), append/complete (stream)
+        table_name (str): Name of the Hive Metastore or Unity Catalog Delta Table
+        options (dict): Options that can be specified for a Delta Table read operation (See Attributes table below). Further information on the options is available for [batch](https://docs.delta.io/latest/delta-batch.html#write-to-a-table){ target="_blank" } and [streaming](https://docs.delta.io/latest/delta-streaming.html#delta-table-as-a-sink){ target="_blank" }.
+        mode (str): Method of writing to Delta Table - append/overwrite (batch), append/complete (stream)
         trigger (str): Frequency of the write operation
         query_name (str): Unique name for the query in associated SparkSession
 
     Attributes:
         checkpointLocation (str): Path to checkpoint files. (Streaming)
         txnAppId (str): A unique string that you can pass on each DataFrame write. (Batch & Streaming)
         txnVersion (str): A monotonically increasing number that acts as transaction version. (Batch & Streaming)
@@ -116,15 +116,15 @@
                 .options(**self.options)
                 .toTable(self.table_name)
             )
             
             while query.isActive:
                 if query.lastProgress:
                     logging.info(query.lastProgress)
-                time.sleep(30)
+                time.sleep(10)
 
         except Py4JJavaError as e:
             logging.exception(e.errmsg)
             raise e
         except Exception as e:
             logging.exception(str(e))
             raise e
```

## rtdip_sdk/pipelines/destinations/spark/eventhub.py

```diff
@@ -10,30 +10,32 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import logging
 import time
-from pyspark.sql import DataFrame, SparkSession
+from pyspark.sql import DataFrame
 from py4j.protocol import Py4JJavaError
 
 from ..interfaces import DestinationInterface
-from ..._pipeline_utils.models import Libraries, MavenLibrary, SystemType
+from ..._pipeline_utils.models import Libraries, SystemType
 from ..._pipeline_utils.constants import DEFAULT_PACKAGES
 
 class SparkEventhubDestination(DestinationInterface):
     '''
     This Spark destination class is used to write batch or streaming data to Eventhubs. Eventhub configurations need to be specified as options in a dictionary.
-    Additionally, there are more optional configuration which can be found [here.](https://github.com/Azure/azure-event-hubs-spark/blob/master/docs/PySpark/structured-streaming-pyspark.md#event-hubs-configuration){ target="_blank" }
+    Additionally, there are more optional configurations which can be found [here.](https://github.com/Azure/azure-event-hubs-spark/blob/master/docs/PySpark/structured-streaming-pyspark.md#event-hubs-configuration){ target="_blank" }
     If using startingPosition or endingPosition make sure to check out **Event Position** section for more details and examples.
+
     Args:
-        options: A dictionary of Eventhub configurations (See Attributes table below)
+        options (dict): A dictionary of Eventhub configurations (See Attributes table below). All Configuration options for Eventhubs can be found [here.](https://github.com/Azure/azure-event-hubs-spark/blob/master/docs/PySpark/structured-streaming-pyspark.md#event-hubs-configuration){ target="_blank" }
 
     Attributes:
+        checkpointLocation (str): Path to checkpoint files. (Streaming)
         eventhubs.connectionString (str):  Eventhubs connection string is required to connect to the Eventhubs service. (Streaming and Batch)
         eventhubs.consumerGroup (str): A consumer group is a view of an entire eventhub. Consumer groups enable multiple consuming applications to each have a separate view of the event stream, and to read the stream independently at their own pace and with their own offsets. (Streaming and Batch)
         eventhubs.startingPosition (JSON str): The starting position for your Structured Streaming job. If a specific EventPosition is not set for a partition using startingPositions, then we use the EventPosition set in startingPosition. If nothing is set in either option, we will begin consuming from the end of the partition. (Streaming and Batch)
         eventhubs.endingPosition: (JSON str): The ending position of a batch query. This works the same as startingPosition. (Batch)
         maxEventsPerTrigger (long): Rate limit on maximum number of events processed per trigger interval. The specified total number of events will be proportionally split across partitions of different volume. (Stream)
     '''
     options: dict
@@ -95,15 +97,15 @@
                 .format("eventhubs")
                 .options(**self.options)
                 .start()
             )
             while query.isActive:
                 if query.lastProgress:
                     logging.info(query.lastProgress)
-                time.sleep(30)
+                time.sleep(10)
 
         except Py4JJavaError as e:
             logging.exception(e.errmsg)
             raise e
         except Exception as e:
             logging.exception(str(e))
             raise e
```

## rtdip_sdk/pipelines/secrets/__init__.py

```diff
@@ -8,8 +8,9 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from .models import *
 from .databricks import *
```

## rtdip_sdk/pipelines/sources/__init__.py

```diff
@@ -11,8 +11,11 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from .spark.autoloader import *
 from .spark.delta import *
 from .spark.delta_sharing import *
-from .spark.eventhub import *
+from .spark.eventhub import *
+from .spark.iot_hub import *
+from .spark.kafka import *
+from .spark.kinesis import *
```

## rtdip_sdk/pipelines/sources/spark/autoloader.py

```diff
@@ -12,26 +12,26 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import logging
 from pyspark.sql import DataFrame, SparkSession
 
 from ..interfaces import SourceInterface
-from ..._pipeline_utils.models import Libraries, MavenLibrary, SystemType
+from ..._pipeline_utils.models import Libraries, SystemType
 from ..._pipeline_utils.constants import DEFAULT_PACKAGES
 
 class DataBricksAutoLoaderSource(SourceInterface):
     '''
     The Spark Auto Loader is used to read new data files as they arrive in cloud storage. Further information on Auto Loader is available [here](https://docs.databricks.com/ingestion/auto-loader/index.html)
     
     Args:
-        spark: Spark Session required to read data from cloud storage
-        options: Options that can be specified for configuring the Auto Loader. Further information on the options available are [here](https://docs.databricks.com/ingestion/auto-loader/options.html)
-        path: The cloud storage path
-        format: Specifies the file format to be read. Supported formats are available [here](https://docs.databricks.com/ingestion/auto-loader/options.html#file-format-options)
+        spark (SparkSession): Spark Session required to read data from cloud storage
+        options (dict): Options that can be specified for configuring the Auto Loader. Further information on the options available are [here](https://docs.databricks.com/ingestion/auto-loader/options.html)
+        path (str): The cloud storage path
+        format (str): Specifies the file format to be read. Supported formats are available [here](https://docs.databricks.com/ingestion/auto-loader/options.html#file-format-options)
     ''' 
     spark: SparkSession
     options: dict
     path: str
 
     def __init__(self, spark: SparkSession, options: dict, path: str, format: str) -> None:
         self.spark = spark
```

## rtdip_sdk/pipelines/sources/spark/delta.py

```diff
@@ -13,25 +13,25 @@
 # limitations under the License.
 
 import logging
 from py4j.protocol import Py4JJavaError
 from pyspark.sql import DataFrame, SparkSession
 
 from ..interfaces import SourceInterface
-from ..._pipeline_utils.models import Libraries, MavenLibrary, SystemType
+from ..._pipeline_utils.models import Libraries, SystemType
 from ..._pipeline_utils.constants import DEFAULT_PACKAGES
 
 class SparkDeltaSource(SourceInterface):
     '''
     The Spark Delta Source is used to read data from a Delta table. 
 
     Args:
-        spark: Spark Session required to read data from a Delta table
-        options: Options that can be specified for a Delta Table read operation (See Attributes table below). Further information on the options is available for [batch](https://docs.delta.io/latest/delta-batch.html#read-a-table){ target="_blank" } and [streaming](https://docs.delta.io/latest/delta-streaming.html#delta-table-as-a-source){ target="_blank" }.
-        table_name: Name of the Hive Metastore or Unity Catalog Delta Table
+        spark (SparkSession): Spark Session required to read data from a Delta table
+        options (dict): Options that can be specified for a Delta Table read operation (See Attributes table below). Further information on the options is available for [batch](https://docs.delta.io/latest/delta-batch.html#read-a-table){ target="_blank" } and [streaming](https://docs.delta.io/latest/delta-streaming.html#delta-table-as-a-source){ target="_blank" }.
+        table_name (str): Name of the Hive Metastore or Unity Catalog Delta Table
 
     Attributes:
         maxFilesPerTrigger (int): How many new files to be considered in every micro-batch. The default is 1000. (Streaming)
         maxBytesPerTrigger (int): How much data gets processed in each micro-batch. (Streaming)
         ignoreDeletes (bool str): Ignore transactions that delete data at partition boundaries. (Streaming)
         ignoreChanges (bool str): Pre-process updates if files had to be rewritten in the source table due to a data changing operation. (Streaming)
         startingVersion (int str): The Delta Lake version to start from. (Streaming)
```

## rtdip_sdk/pipelines/sources/spark/delta_sharing.py

```diff
@@ -13,25 +13,25 @@
 # limitations under the License.
 
 import logging
 from pyspark.sql import DataFrame, SparkSession
 from py4j.protocol import Py4JJavaError
 
 from ..interfaces import SourceInterface
-from ..._pipeline_utils.models import Libraries, MavenLibrary, SystemType
+from ..._pipeline_utils.models import Libraries, SystemType
 from ..._pipeline_utils.constants import DEFAULT_PACKAGES
 
 class SparkDeltaSharingSource(SourceInterface):
     '''
     The Spark Delta Sharing Source is used to read data from a Delta table where Delta sharing is configured 
 
     Args:
-        spark: Spark Session required to read data from a Delta table
-        options: Options that can be specified for a Delta Table read operation (See Attributes table below). Further information on the options is available [here](https://docs.databricks.com/data-sharing/read-data-open.html#apache-spark-read-shared-data){ target="_blank" }
-        table_path: Path to credentials file and Delta table to query
+        spark (SparkSession): Spark Session required to read data from a Delta table
+        options (dict): Options that can be specified for a Delta Table read operation (See Attributes table below). Further information on the options is available [here](https://docs.databricks.com/data-sharing/read-data-open.html#apache-spark-read-shared-data){ target="_blank" }
+        table_path (str): Path to credentials file and Delta table to query
 
     Attributes:
         ignoreDeletes (bool str): Ignore transactions that delete data at partition boundaries. (Streaming)
         ignoreChanges (bool str): Pre-process updates if files had to be rewritten in the source table due to a data changing operation. (Streaming)
         startingVersion (int str): The Delta Lake version to start from. (Streaming)
         startingTimestamp (datetime str): The timestamp to start from. (Streaming)
         maxFilesPerTrigger (int): How many new files to be considered in every micro-batch. The default is 1000. (Streaming)
```

## rtdip_sdk/pipelines/sources/spark/eventhub.py

```diff
@@ -11,28 +11,28 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import logging
 from py4j.protocol import Py4JJavaError
 from pyspark.sql import DataFrame, SparkSession
-from pyspark.sql.types import StructType, StructField, BinaryType, StringType, LongType, TimestampType, MapType
 
 from ..interfaces import SourceInterface
-from ..._pipeline_utils.models import Libraries, MavenLibrary, SystemType
-from ..._pipeline_utils.constants import DEFAULT_PACKAGES, EVENTHUB_SCHEMA
+from ..._pipeline_utils.models import Libraries, SystemType
+from ..._pipeline_utils.constants import DEFAULT_PACKAGES
+from ..._pipeline_utils.spark import EVENTHUB_SCHEMA
 
 class SparkEventhubSource(SourceInterface):
     '''
     This Spark source class is used to read batch or streaming data from Eventhubs. Eventhub configurations need to be specified as options in a dictionary.
-    Additionally, there are more optional configuration which can be found [here.](https://github.com/Azure/azure-event-hubs-spark/blob/master/docs/PySpark/structured-streaming-pyspark.md#event-hubs-configuration){ target="_blank" }
-    If using startingPosition or endingPosition make sure to check out **Event Position** section for more details and examples.
+    Additionally, there are more optional configurations which can be found [here.](https://github.com/Azure/azure-event-hubs-spark/blob/master/docs/PySpark/structured-streaming-pyspark.md#event-hubs-configuration){ target="_blank" }
+    If using startingPosition or endingPosition make sure to check out the **Event Position** section for more details and examples.
     Args:
-        spark: Spark Session
-        options: A dictionary of Eventhub configurations (See Attributes table below)
+        spark (SparkSession): Spark Session
+        options (dict): A dictionary of Eventhub configurations (See Attributes table below)
 
     Attributes:
         eventhubs.connectionString (str):  Eventhubs connection string is required to connect to the Eventhubs service. (Streaming and Batch)
         eventhubs.consumerGroup (str): A consumer group is a view of an entire eventhub. Consumer groups enable multiple consuming applications to each have a separate view of the event stream, and to read the stream independently at their own pace and with their own offsets. (Streaming and Batch)
         eventhubs.startingPosition (JSON str): The starting position for your Structured Streaming job. If a specific EventPosition is not set for a partition using startingPositions, then we use the EventPosition set in startingPosition. If nothing is set in either option, we will begin consuming from the end of the partition. (Streaming and Batch)
         eventhubs.endingPosition: (JSON str): The ending position of a batch query. This works the same as startingPosition. (Batch)
         maxEventsPerTrigger (long): Rate limit on maximum number of events processed per trigger interval. The specified total number of events will be proportionally split across partitions of different volume. (Stream)
```

## rtdip_sdk/pipelines/transformers/__init__.py

```diff
@@ -8,8 +8,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .spark.eventhub import *
+from .spark.eventhub import *
+from .spark.json_to_opcua import *
+from .spark.opcua_to_process_control_data_model import *
```

## rtdip_sdk/pipelines/utilities/__init__.py

```diff
@@ -6,8 +6,12 @@
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
-# limitations under the License.
+# limitations under the License.
+
+from .spark.delta_table_create import *
+from .spark.delta_table_optimize import *
+from .spark.delta_table_vacuum import *
```

## Comparing `rtdip_sdk-0.2.0b1.dist-info/LICENSE.md` & `rtdip_sdk-0.2.1.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `rtdip_sdk-0.2.0b1.dist-info/METADATA` & `rtdip_sdk-0.2.1.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 Metadata-Version: 2.1
 Name: rtdip-sdk
-Version: 0.2.0b1
+Version: 0.2.1
 Home-page: https://github.com/rtdip/core
 Project-URL: Issue Tracker, https://github.com/rtdip/core/issues
 Project-URL: Source, https://github.com/rtdip/core/
 Project-URL: Documentation, https://www.rtdip.io/
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8, <=3.10
+Requires-Python: >=3.8, <3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: databricks-sql-connector (==2.4.0)
 Requires-Dist: azure-identity (==1.11.0)
 Requires-Dist: pyodbc (==4.0.34)
 Requires-Dist: pandas (==1.5.2)
 Requires-Dist: jinja2 (==3.0.3)
 Requires-Dist: jinjasql (==0.1.8)
 Provides-Extra: pipelines
 Requires-Dist: dependency-injector (==4.41.0) ; extra == 'pipelines'
 Requires-Dist: dbx (==0.8.10) ; extra == 'pipelines'
 Requires-Dist: pydantic (==1.10.6) ; extra == 'pipelines'
 Provides-Extra: pyspark
 Requires-Dist: pyspark (==3.3.2) ; extra == 'pyspark'
-Requires-Dist: delta-spark (==2.2.0) ; extra == 'pyspark'
-Requires-Dist: openjdk (==11.0.15) ; extra == 'pyspark'
+Requires-Dist: delta-spark (==2.3.0) ; extra == 'pyspark'
 
 <p align="center"><img src=https://raw.githubusercontent.com/rtdip/core/develop/docs/getting-started/images/rtdip-horizontal-color.png alt="rtdip" width=50% height=50%/></p>
 
 # What is the RTDIP SDK?
 
-​​**Real Time Data Ingestion Platform (RTDIP) SDK** is a software development kit built to easily access some of RTDIP's transformation functions.
+​​**Real Time Data Ingestion Platform (RTDIP) SDK** is a python software development kit built to provide users, data scientists and developers with the ability to interact with components of the Real Time Data Ingestion Platform, including:
 
-The RTDIP SDK will give the end user the power to use some of the convenience methods for frequency conversions and resampling of Pi data all through a self-service platform. RTDIP is offering a flexible product with the ability to authenticate and connect to Databricks SQL Warehouses given the end users preferences. RTDIP have taken the initiative to cut out the middle man and instead wrap these commonly requested methods in a simple python module so that you can instead focus on the data. 
+- Building, Executing and Deploying Ingestion Pipelines
+- Execution of queries on RTDIP data
+- Authentication to securely interact with environments and data
 
 See [RTDIP Documentation](https://www.rtdip.io/) for more information on how to use the SDK.
 
 # Licensing
 
 Distributed under the Apache 2.0 License. See [LICENSE.md](https://github.com/rtdip/core/blob/develop/LICENSE.md) for more information.
```

## Comparing `rtdip_sdk-0.2.0b1.dist-info/RECORD` & `rtdip_sdk-0.2.1.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,69 +1,79 @@
 rtdip_sdk/__init__.py,sha256=eIke9C2leBQU1ezpJHbkoWUl7ExNw9QmxvZFbCyVomE,571
 rtdip_sdk/authentication/__init__.py,sha256=eIke9C2leBQU1ezpJHbkoWUl7ExNw9QmxvZFbCyVomE,571
 rtdip_sdk/authentication/authenticate.py,sha256=GPd7ftHVZjrGq3n9Gj7dwEjrSxpCwlSODzvQggIpfts,7210
 rtdip_sdk/functions/__init__.py,sha256=eIke9C2leBQU1ezpJHbkoWUl7ExNw9QmxvZFbCyVomE,571
 rtdip_sdk/functions/_query_builder.py,sha256=m29X24I9U_WrgMmg9PyViEIPQ1vMWTKzdHrRG2CNLGU,8746
-rtdip_sdk/functions/interpolate.py,sha256=bFwZYCuZSeOcM5G_ihdgmLfAlIb7afWiaU5WcsVKC4Q,2908
-rtdip_sdk/functions/metadata.py,sha256=sR342MQmTYpB8xMIFuNKAOqmXPEdBM28ZJeYQ8jFzM4,2293
-rtdip_sdk/functions/raw.py,sha256=LQRojeUmYBJqIPQ2P9r62R001wnHEwDCaa6fRzx6Q_4,2786
-rtdip_sdk/functions/resample.py,sha256=HqcYE71bVjV2cE8kVadGpvaXt5bXFbCfq-tsj9Z3Ukk,3052
+rtdip_sdk/functions/interpolate.py,sha256=R5mAUWMU24oyC_DfbL3GoJE0nx4ddyBuYeTNCh2tdR8,2908
+rtdip_sdk/functions/metadata.py,sha256=DNy2X--PGw5ERj5sA2KuCJxChJ3uLN8TTgeIdLLWRcg,2293
+rtdip_sdk/functions/raw.py,sha256=O4Rg-DMSNx8iRxqyjfjnkzfn3Gf5l8TJOeI0ESLnOqw,2786
+rtdip_sdk/functions/resample.py,sha256=NT3bA1Ia8u834C1HC9dUQ1AaLy4PN2Yc51KN1Qee0wc,3052
 rtdip_sdk/functions/time_weighted_average.py,sha256=quQCHCpHT-zxW-SCNFV0U6vUQfV1FzJybXbXtjL1PKw,8921
 rtdip_sdk/odbc/__init__.py,sha256=eIke9C2leBQU1ezpJHbkoWUl7ExNw9QmxvZFbCyVomE,571
 rtdip_sdk/odbc/connection_interface.py,sha256=7FnrbBSvsCGNjutxutGvFYZfktY2hcDhyfLnCcCh-hQ,934
 rtdip_sdk/odbc/cursor_interface.py,sha256=JEWb1W72PXibztG8koTj-tOuejvoDsJh8k7mFvH-C6k,952
 rtdip_sdk/odbc/db_sql_connector.py,sha256=I6d8K3mm_ykIPh8-EjkNQDmdRGvCdFyROHsl8ErBY-g,3498
 rtdip_sdk/odbc/pyodbc_sql_connector.py,sha256=9Ap6Qh73enYXS6GnmrybN2mVH2CUCWCwUjxq7mrmtaQ,4228
 rtdip_sdk/odbc/turbodbc_sql_connector.py,sha256=Uv4DRn1y1QOiggN5nAVPB3RrS1hUuI56OsAAHspZqq0,4432
 rtdip_sdk/pipelines/__init__.py,sha256=cLARnwRfLDutJ3PTR19AhwFxmrpjsYuxojv2GhlMlCU,569
 rtdip_sdk/pipelines/interfaces.py,sha256=RdiawOPSQ5Vxch6htM03MMKhyMBtU4RVtnTdl0jVBBU,1035
 rtdip_sdk/pipelines/_pipeline_utils/__init__.py,sha256=cLARnwRfLDutJ3PTR19AhwFxmrpjsYuxojv2GhlMlCU,569
-rtdip_sdk/pipelines/_pipeline_utils/constants.py,sha256=09zlcYGntgAa_AhhSMzrh9FCcp3J6m379mHxPCwzXJ8,2059
+rtdip_sdk/pipelines/_pipeline_utils/constants.py,sha256=insI6NqDXf80_tzyKlTnmQ_p09yp1_0X__UVuogCzd4,1485
 rtdip_sdk/pipelines/_pipeline_utils/models.py,sha256=tvviN-pD1TBZQ_9t2icYGTP0LRnslore8NHlYaALlCw,2434
-rtdip_sdk/pipelines/_pipeline_utils/spark.py,sha256=9qX0_2JCEJvtK4KSpourKreBlFKcpUj1k6x5BWkMS28,3295
+rtdip_sdk/pipelines/_pipeline_utils/spark.py,sha256=SJYHa2HzZgj0VkDzYxqOC30zaYPaDC7IQ6yj25XyPDU,5327
 rtdip_sdk/pipelines/converters/__init__.py,sha256=hwO8Ac698lsn720_wfiyk7ss4cPWCFHMuNgJ7-YdMWQ,603
 rtdip_sdk/pipelines/converters/interfaces.py,sha256=wvm5Doxre6XJjc1nE9-l047MR4JjvyPCeGDIO3kUCt4,697
 rtdip_sdk/pipelines/converters/pipeline_job_json.py,sha256=8fm6NtsvN_bzDqaFiknzdfOlMjMMSMnpn9ZGDRAFd3E,3424
-rtdip_sdk/pipelines/deploy/__init__.py,sha256=eIke9C2leBQU1ezpJHbkoWUl7ExNw9QmxvZFbCyVomE,571
-rtdip_sdk/pipelines/deploy/databricks.py,sha256=oxd2CUE6jSVQY0TYc55aLFgO674oZH4-ZH8QV1Dym4w,13229
+rtdip_sdk/pipelines/deploy/__init__.py,sha256=8wwgnaMDh2h_Y6kMrHKXFsXBdPASIeoLssPDgHyVSgA,630
+rtdip_sdk/pipelines/deploy/databricks.py,sha256=rv9qIxujRiMD-j6Zv2N4DQECHItfKQQOsep8znZcsME,13189
 rtdip_sdk/pipelines/deploy/interfaces.py,sha256=s6FM0UjSFkF1LhPvBF52zOExuIIItXJql-1j9qiXvnQ,751
 rtdip_sdk/pipelines/deploy/dbx/__init__.py,sha256=eIke9C2leBQU1ezpJHbkoWUl7ExNw9QmxvZFbCyVomE,571
 rtdip_sdk/pipelines/deploy/dbx/setup.py,sha256=7VEAGmbQ_qAd73g9T85DitK1EvObixrzoatjiufbeDU,1114
+rtdip_sdk/pipelines/deploy/dbx/conf/__init__.py,sha256=eIke9C2leBQU1ezpJHbkoWUl7ExNw9QmxvZFbCyVomE,571
 rtdip_sdk/pipelines/deploy/dbx/rtdip/__init__.py,sha256=eIke9C2leBQU1ezpJHbkoWUl7ExNw9QmxvZFbCyVomE,571
 rtdip_sdk/pipelines/deploy/dbx/rtdip/tasks/__init__.py,sha256=eIke9C2leBQU1ezpJHbkoWUl7ExNw9QmxvZFbCyVomE,571
 rtdip_sdk/pipelines/deploy/dbx/rtdip/tasks/common.py,sha256=f7q1C5OvcHNrRNp1iAU461DKF4XnVi-dOFVs19Oj7bQ,3310
 rtdip_sdk/pipelines/deploy/dbx/rtdip/tasks/pipeline_task.py,sha256=sXMSI_gnEC3LTT-2ekEMKclZ3XXli8CbH8gIeu4xB9c,1686
 rtdip_sdk/pipelines/deploy/models/__init__.py,sha256=eIke9C2leBQU1ezpJHbkoWUl7ExNw9QmxvZFbCyVomE,571
 rtdip_sdk/pipelines/deploy/models/databricks.py,sha256=BaVaRGHGoGiUiG_1ouBuAUOHc4t0nLCaLIIIj56Annc,7897
-rtdip_sdk/pipelines/destinations/__init__.py,sha256=o-3p0_ikvbbOqXFm5k4OF1lwjKF5dyYHwDtuuvi9k_g,627
+rtdip_sdk/pipelines/destinations/__init__.py,sha256=oPnFMRb6Y1__25uf5yfR_ETeKDGfvn-hUAQupySWuV8,684
 rtdip_sdk/pipelines/destinations/interfaces.py,sha256=IjIYhBInHDAvtf52Z7zcvux9q0_ni8KkHj5kD1I6LP4,427
 rtdip_sdk/pipelines/destinations/spark/__init__.py,sha256=cLARnwRfLDutJ3PTR19AhwFxmrpjsYuxojv2GhlMlCU,569
-rtdip_sdk/pipelines/destinations/spark/delta.py,sha256=xYBpbTdHH4mC_1L3Lg18I7_4l_08TyegLbXNJCxr2aE,5093
-rtdip_sdk/pipelines/destinations/spark/eventhub.py,sha256=N9_SeAsh6OvR1QBkiGIcrZxgrmdxUbsvtL-OcOKjJDw,4516
+rtdip_sdk/pipelines/destinations/spark/delta.py,sha256=WjMzdnEyZUVOS0DG-YoqVZ1FvKf1qVbOikl2VDXMi9g,5112
+rtdip_sdk/pipelines/destinations/spark/eventhub.py,sha256=12C5NvjzSctJytKv7iBoR5Qc1zxK0CM41JZQqQ5Ycqc,4781
+rtdip_sdk/pipelines/destinations/spark/kafka.py,sha256=DEZApzSLTamM7sqiPKxVLpWNpOBZY2O1ysrTYSI24AQ,3903
+rtdip_sdk/pipelines/destinations/spark/kinesis.py,sha256=gx6BhFe_M797mp-j_OMDmTooI8HoBLq2ZqBTi0Mzk8I,3659
 rtdip_sdk/pipelines/execute/__init__.py,sha256=NrQH7iM8LSCgnkbVmIWx_Gd67SxbdnJYGacS1iKshM0,611
 rtdip_sdk/pipelines/execute/container.py,sha256=0u-YsNbgMD2iyZob2W_OuxrVuGlpqGUm4Atz1jg6cA4,1448
 rtdip_sdk/pipelines/execute/job.py,sha256=UZV3mA0pVvauPcc6q4Pgyws34pxEKjaBZUOt3IKoIkE,8378
 rtdip_sdk/pipelines/execute/models.py,sha256=TQxpDl0G3EuciPREYzOo_C0gv_HvE-1uzwze9-WYdlA,3037
-rtdip_sdk/pipelines/secrets/__init__.py,sha256=Ol-9E4LXblVhu-IZixJZ4Ui4shBZ50JbTuHW9RV9E7Q,596
+rtdip_sdk/pipelines/secrets/__init__.py,sha256=wz5k9b3FvKaXT_Yxy374H_ZNqUgV5ekhffRPpSrHUC0,618
 rtdip_sdk/pipelines/secrets/databricks.py,sha256=pXVC_wtPVBbLUqwd04hISiAk273DLCDtmOXz4CtNgmQ,2227
 rtdip_sdk/pipelines/secrets/interfaces.py,sha256=VoSDAhP63SrLs8DgHihZEFMi3hHgivhCDtha9xQxjO0,824
 rtdip_sdk/pipelines/secrets/models.py,sha256=wf7mqWTcgdIznuD6hBI1zpwsKOewMZUUu2rUwV2uehU,887
-rtdip_sdk/pipelines/sources/__init__.py,sha256=CfB0epGPI3Ejmp9l11oJF4dFsTjhktKTmvOqaB8BcpE,694
+rtdip_sdk/pipelines/sources/__init__.py,sha256=hPl8ifI25qmvN9IOghCOIoXjvCR0dLVke0atab6bvGg,779
 rtdip_sdk/pipelines/sources/interfaces.py,sha256=FnhgvVMd2IpizhuITFavf7oKvo9HeJwazSIQ2jihO8c,993
 rtdip_sdk/pipelines/sources/spark/__init__.py,sha256=cLARnwRfLDutJ3PTR19AhwFxmrpjsYuxojv2GhlMlCU,569
-rtdip_sdk/pipelines/sources/spark/autoloader.py,sha256=1l1aDOqwZbRfzJm7TCZmGERf6yewYlZPbjW-SCK4yCA,3400
-rtdip_sdk/pipelines/sources/spark/delta.py,sha256=JfuaXC4EMdtYqGARLuiKduu08u05uz4p9eWPs2DGJsg,4487
-rtdip_sdk/pipelines/sources/spark/delta_sharing.py,sha256=8KLEDak2MRsZ1ZWJhzr9Ylw5ltYuXJ7hwrqBrLn9NFU,4459
-rtdip_sdk/pipelines/sources/spark/eventhub.py,sha256=6-Q47on1T9BNIkoatkfhSfz9Zqj5Wew9JIuBlBImRRA,5322
-rtdip_sdk/pipelines/transformers/__init__.py,sha256=w34SHEbKonbYb105Yod3u1owOl4khNXl7rK8ikrNq_0,600
+rtdip_sdk/pipelines/sources/spark/autoloader.py,sha256=rL0t5jd-RSowkpklhdSd__6adfrVD0c8LKmKvmqYBY0,3420
+rtdip_sdk/pipelines/sources/spark/delta.py,sha256=BuWtKZPDxRfe7XA6x7pJTTL8TxjJoMXEaPAomdrEdt8,4501
+rtdip_sdk/pipelines/sources/spark/delta_sharing.py,sha256=Mbb4Be4yN1X6biLDB-S6CDDos0SdKDTA97_sMY4W-1o,4473
+rtdip_sdk/pipelines/sources/spark/eventhub.py,sha256=jgUecN1ZkBKoAyVCM52SgbAPbdRl1Nknfbp-SozCRz0,5259
+rtdip_sdk/pipelines/sources/spark/iot_hub.py,sha256=LdVZkc-xOSTyq6y4sD1nmpef5zlSySJNwwtP4tXaMao,5240
+rtdip_sdk/pipelines/sources/spark/kafka.py,sha256=7OGqTZtkvNI8TaBB7hptYywclJOAzmHxOync_1jUayE,8114
+rtdip_sdk/pipelines/sources/spark/kinesis.py,sha256=uarSt6bVe-2amI8qaLd2lwabLnVcasMnrFu86KXyIDo,3793
+rtdip_sdk/pipelines/transformers/__init__.py,sha256=S_qtKJIha2LCb3oAfj_gOfgieVZCr5l1TMyvdZUc0ps,692
 rtdip_sdk/pipelines/transformers/interfaces.py,sha256=KZUm93QHDARxMobPg989HijfiBjSpOI8oVILSJlK30g,946
 rtdip_sdk/pipelines/transformers/spark/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 rtdip_sdk/pipelines/transformers/spark/eventhub.py,sha256=Kxvb65UYOzt_bTTVs3gw9HfKG6gwvcdGMnJk6rVRWZo,1715
-rtdip_sdk/pipelines/utilities/__init__.py,sha256=cLARnwRfLDutJ3PTR19AhwFxmrpjsYuxojv2GhlMlCU,569
+rtdip_sdk/pipelines/transformers/spark/json_to_opcua.py,sha256=CWgNn91Mj3Txlq9JKdwfJSXaaLCMNC7Sbfmc0VQ9C5M,2900
+rtdip_sdk/pipelines/transformers/spark/opcua_to_process_control_data_model.py,sha256=3bw6qZgKpCJp7EyyG8w1_fzFsuhijsByTn-Pk3BcQ3Y,3560
+rtdip_sdk/pipelines/utilities/__init__.py,sha256=vGjc2wBsYJ9F6AXcZ6TC9wMnDp-vEHo8RSTH1WPjb7U,692
 rtdip_sdk/pipelines/utilities/interfaces.py,sha256=jHlDdFAgbUL9alAmU3Ncye_2iqywJLglFbZ04zaqNTQ,773
 rtdip_sdk/pipelines/utilities/spark/__init__.py,sha256=cLARnwRfLDutJ3PTR19AhwFxmrpjsYuxojv2GhlMlCU,569
 rtdip_sdk/pipelines/utilities/spark/delta_table_create.py,sha256=NvPxUZapqt2_CZ3arKHkCUKcRnhdyruIBHmz3Jtok0k,3857
-rtdip_sdk-0.2.0b1.dist-info/LICENSE.md,sha256=WYmcYJG1QFgu1hfo7qrEkZ3Jhcz8NUWe6XUraZvlIFs,10172
-rtdip_sdk-0.2.0b1.dist-info/METADATA,sha256=K13IuiaeGsEOWnJj8V3WySPyUHVqINV-QLOmr6ShLB8,3012
-rtdip_sdk-0.2.0b1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-rtdip_sdk-0.2.0b1.dist-info/top_level.txt,sha256=DFRWw2FYwSXWlH6UsWDVt1G8Bq6QjRWN0GJ8BS4o2dg,10
-rtdip_sdk-0.2.0b1.dist-info/RECORD,,
+rtdip_sdk/pipelines/utilities/spark/delta_table_optimize.py,sha256=8mBCct4mmhkypW41eFDbLYhWZEnlii1ANz5kwtWyNkM,3119
+rtdip_sdk/pipelines/utilities/spark/delta_table_vacuum.py,sha256=BvMUPC1NCFPXz4oN9XxsCnAsZ0vdiZTNp7bFsx7dFfg,2602
+rtdip_sdk-0.2.1.dist-info/LICENSE.md,sha256=WYmcYJG1QFgu1hfo7qrEkZ3Jhcz8NUWe6XUraZvlIFs,10172
+rtdip_sdk-0.2.1.dist-info/METADATA,sha256=aBJv_kKLezbJ33Mi_VwWHNraLKzWkl5tq79q9zR84cU,2709
+rtdip_sdk-0.2.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+rtdip_sdk-0.2.1.dist-info/top_level.txt,sha256=DFRWw2FYwSXWlH6UsWDVt1G8Bq6QjRWN0GJ8BS4o2dg,10
+rtdip_sdk-0.2.1.dist-info/RECORD,,
```

