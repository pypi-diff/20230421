# Comparing `tmp/z3_target_bigquery-0.6.3.tar.gz` & `tmp/z3_target_bigquery-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "z3_target_bigquery-0.6.3.tar", max compression
+gzip compressed data, was "z3_target_bigquery-0.6.6.tar", max compression
```

## Comparing `z3_target_bigquery-0.6.3.tar` & `z3_target_bigquery-0.6.6.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0     1078 2023-02-04 09:27:15.696724 z3_target_bigquery-0.6.3/LICENSE
--rw-r--r--   0        0        0    16973 2023-03-15 22:08:34.909700 z3_target_bigquery-0.6.3/README.md
--rw-r--r--   0        0        0     2091 2023-03-15 22:24:21.219475 z3_target_bigquery-0.6.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-04 09:27:15.698113 z3_target_bigquery-0.6.3/target_bigquery/__init__.py
--rw-r--r--   0        0        0     4965 2023-03-15 21:49:44.364864 z3_target_bigquery-0.6.3/target_bigquery/batch_job.py
--rw-r--r--   0        0        0     2575 2023-02-04 09:27:15.698445 z3_target_bigquery-0.6.3/target_bigquery/constants.py
--rw-r--r--   0        0        0    37483 2023-03-15 21:55:13.835395 z3_target_bigquery-0.6.3/target_bigquery/core.py
--rw-r--r--   0        0        0     9442 2023-03-15 21:49:44.422697 z3_target_bigquery-0.6.3/target_bigquery/gcs_stage.py
--rw-r--r--   0        0        0     4986 2023-02-04 09:27:15.698952 z3_target_bigquery-0.6.3/target_bigquery/proto_gen.py
--rw-r--r--   0        0        0    13091 2023-03-15 22:31:31.386472 z3_target_bigquery-0.6.3/target_bigquery/storage_write.py
--rw-r--r--   0        0        0     4468 2023-03-15 22:30:28.748172 z3_target_bigquery-0.6.3/target_bigquery/streaming_insert.py
--rw-r--r--   0        0        0    21731 2023-03-15 22:30:01.256841 z3_target_bigquery-0.6.3/target_bigquery/target.py
--rw-r--r--   0        0        0    18454 1970-01-01 00:00:00.000000 z3_target_bigquery-0.6.3/setup.py
--rw-r--r--   0        0        0    18488 1970-01-01 00:00:00.000000 z3_target_bigquery-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-01-20 23:36:48.960193 z3_target_bigquery-0.6.6/LICENSE
+-rw-r--r--   0        0        0    20800 2023-04-20 22:31:15.806538 z3_target_bigquery-0.6.6/README.md
+-rw-r--r--   0        0        0     2099 2023-04-20 19:59:59.743672 z3_target_bigquery-0.6.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-06-20 18:27:41.011352 z3_target_bigquery-0.6.6/target_bigquery/__init__.py
+-rw-r--r--   0        0        0     4965 2023-04-02 03:16:22.076367 z3_target_bigquery-0.6.6/target_bigquery/batch_job.py
+-rw-r--r--   0        0        0     2575 2023-04-02 03:16:22.077092 z3_target_bigquery-0.6.6/target_bigquery/constants.py
+-rw-r--r--   0        0        0    42167 2023-04-20 22:07:12.619047 z3_target_bigquery-0.6.6/target_bigquery/core.py
+-rw-r--r--   0        0        0     9442 2023-04-02 03:16:22.078271 z3_target_bigquery-0.6.6/target_bigquery/gcs_stage.py
+-rw-r--r--   0        0        0     4986 2023-04-02 03:16:22.079246 z3_target_bigquery-0.6.6/target_bigquery/proto_gen.py
+-rw-r--r--   0        0        0    13091 2023-04-02 03:16:22.079767 z3_target_bigquery-0.6.6/target_bigquery/storage_write.py
+-rw-r--r--   0        0        0     4468 2023-04-02 03:16:22.080448 z3_target_bigquery-0.6.6/target_bigquery/streaming_insert.py
+-rw-r--r--   0        0        0    22149 2023-04-20 22:02:47.844135 z3_target_bigquery-0.6.6/target_bigquery/target.py
+-rw-r--r--   0        0        0    22323 1970-01-01 00:00:00.000000 z3_target_bigquery-0.6.6/PKG-INFO
```

### Comparing `z3_target_bigquery-0.6.3/LICENSE` & `z3_target_bigquery-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `z3_target_bigquery-0.6.3/README.md` & `z3_target_bigquery-0.6.6/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -42,14 +42,38 @@
 ```bash
 # Use pipx or pip
 pipx install z3-target-bigquery
 # Verify it is installed
 target-bigquery --version
 ```
 
+## Usage Notes
+
+### Denormalization
+
+So denormalized is a loaded term, so lets clarify here what we mean by it:
+
+> In the context of JSON objects, denormalization refers to the process of flattening a hierarchical or nested JSON object into a simpler, more "denormalized" structure that can be easier to work with for certain use cases.
+
+Denormalized=False (default) means we load all data into a single `JSON` column. This means all access requires an accessor such as `SELECT data.my_column FROM table` instead of `SELECT my_column FROM table`. Hence the term denormalized is relative to the `data` column which is the default for this target. This is a tradeoff between convenience/resilience and performance. This is the default because most _resilient_. IE a load will **never** fail due to a schema change or an invalid schema. You can always denormalize later via `dbt`. However, it is not the most performant and slower to transform. If your tap has a high quality and consistent schema, denormalization is the way to go to get the best performance and start modeling quickly.
+
+Denormalized=True means we unpack the data into a schema which is derived from the tap schema. It does _not_ mean we will flatten the data. There is a separate option for flattening. We will convert arrays to repeated fields and records to structs. All top level keys will end up as columns which is was you might expect from more typical targets.
+
+#### Resolver Versions
+
+There are 2 resolver versions. The config option `schema_resolver_version` lets you select which version you want to use. This versioning exists because we want to support evolving how we resolve schemas whilst not creating breaking changes for long-time users dependent on how a schema is resolved. The default is `1` which behaves very similarly to existing flavors of `target-bigquery`. It works well enough but has plenty of edge cases where it simply cannot resolve valid jsonschemas to a bq schema. The new version `2` is much more robust and will resolve most, if not all schemas due to it falling back to `JSON` when in doubt. You must opt-in to this version by setting `schema_resolver_version: 2` in your config. 
+
+### Overwrite vs Append
+
+Sometimes you want to overwrite a table on every load. This can be achieved by either setting `overwrite: true` which will full refresh ALL tables **or** setting `overwrite: [table1, table2, table_*_other, !table_v1_other]` which will only overwrite the specified tables and supports pattern matching. This is useful if you have a table which is a lookup table and you want to overwrite it on every load. You can also set `overwrite: false` which will append to the table. This is the default behavior.
+
+### Upsert (aka Merge)
+
+If you want to merge data into a table, you can set `merge: true` which will use the `MERGE` statement to upsert data. This supports pattern matching like the above setting. It requires `denormalized: true` takes precedence over `overwrite`. It will only work on tables which have a primary key as defined by the `key_properties` sent by the tap. There is a supporting config option called `dedupe_before_upsert` which will dedupe the data before upserting. This is useful if you are replicating data which has a primary key but is not unique. This occurs when you are replicating data from a source which has a primary key but does not enforce it. This is the case for MongoDB. It can also happen when moving data from a data lake in S3/GCS to a database. This is not the default behavior because it is slower and requires more resources.
+
 ## Features ✨
 
 - Autoscaling self-healing worker pool using either threads (default) or multiprocessing, configurable by the user for the _fastest_ possible data ingestion. Particularly when leveraging colocated compute in GCP.
 - Denormalized load pattern where data is unpacked in flight into a statically typed BigQuery schema derived from the input stream json schemas.
 - Fix schema load pattern where all data is loaded into a `JSON` column which has been GA in BigQuery since mid 2022.
 - Autogenerated `VIEW` support for fixed schema load patterns which essentially overlays a statically typed schema allowing you to get the best of both worlds when using fixed schema ingestion.
 - JIT compilation of protobuf schemas allowing the Storage Write API to use a denormalized load pattern. 
@@ -120,14 +144,15 @@
 | column_name_transforms.lower                       |  False   |       None        | Lowercase column names. |
 | column_name_transforms.quote                       |  False   |       None        | Quote column names in any generated DDL. |
 | column_name_transforms.add_underscore_when_invalid |  False   |       None        | Add an underscore to the column name if it starts with a digit to make it valid. |
 | column_name_transforms.snake_case                  |  False   |       None        | Snake case all incoming column names. Does not apply to fixed schema loads but _does_ apply to the view auto-generated over them. |
 | options.storage_write_batch_mode                   |  False   |       None        | By default, we use the default stream (Committed mode) in the [storage_write_api](https://cloud.google.com/bigquery/docs/write-api) load method which results in streaming records which are immediately available and is generally fastest. If this is set to true, we will use the application created streams (pending mode) to transactionally batch data on STATE messages and at end of pipe. |
 | options.process_pool                               |  False   |       None        | By default we use an autoscaling threadpool to write to BigQuery. If set to true, we will use a process pool. |
 | options.max_workers                                |  False   |       None        | By default, each sink type has a preconfigured max worker pool limit. This sets an override for maximum number of workers in the pool. |
+| schema_resolver_version                            |  False   |       1           | The version of the schema resolver to use. Defaults to 1. Version 2 uses JSON as a fallback during denormalization. This only has an effect if denormalized=true |
 | stream_maps                                        |  False   |       None        | Config object for stream maps capability. For more information check out [Stream Maps](https://sdk.meltano.com/en/latest/stream_maps.html). |
 | stream_map_config                                  |  False   |       None        | User-defined config values to be used within map expressions. |
 | flattening_enabled                                 |  False   |       None        | 'True' to enable schema flattening and automatically expand nested properties. |
 | flattening_max_depth                               |  False   |       None        | The max depth to flatten schemas. |
 
 A full list of supported settings and capabilities is available by running: `target-bigquery --about`
```

#### html2text {}

```diff
@@ -21,170 +21,220 @@
 Denormalized, Overwrite - Legacy Streaming API, Denormalized, Upsert - Legacy
 Streaming API, Denormalized, Append - Legacy Streaming API, Fixed Schema,
 Overwrite - Legacy Streaming API, Fixed Schema, Append ## Installation ð The
 package on pypi is named `z3-target-bigquery` but the executable it ships with
 is simply `target-bigquery`. This allows me to release work without concerns of
 naming conflicts on the package index. ```bash # Use pipx or pip pipx install
 z3-target-bigquery # Verify it is installed target-bigquery --version ``` ##
-Features â¨ - Autoscaling self-healing worker pool using either threads
-(default) or multiprocessing, configurable by the user for the _fastest_
-possible data ingestion. Particularly when leveraging colocated compute in GCP.
-- Denormalized load pattern where data is unpacked in flight into a statically
-typed BigQuery schema derived from the input stream json schemas. - Fix schema
-load pattern where all data is loaded into a `JSON` column which has been GA in
-BigQuery since mid 2022. - Autogenerated `VIEW` support for fixed schema load
-patterns which essentially overlays a statically typed schema allowing you to
-get the best of both worlds when using fixed schema ingestion. - JIT
-compilation of protobuf schemas allowing the Storage Write API to use a
-denormalized load pattern. - BATCH message support ð ## Load Patterns ð -
-`Batch Load Job` ingestion pattern using in memory compression (fixed schema +
-denormalized) - `Storage Write API` ingestion pattern using gRPC and protocol
-buffers supporting both streaming and batch patterns. Capable of JIT
-compilation of BQ schemas to protobuf to enable denormalized loads of input
-structures only known at runtime. (fixed schema + denormalized ð) - `GCS
-Staging` ingestion pattern using in memory compression and a GCS staging layer
-which generates a well organized data lake which backs the data warehouse
-providing additional failsafes and data sources (fixed schema + denormalized) -
-`Legacy Streaming` ingestion pattern which emphasizes simplicity and fast start
-up / tear down. I would highly recommend the storage write API instead unless
-data volume is small (fixed schema + denormalized) **Choosing between
-denormalized and fixed schema (JSON support)?** ðð¾ââï¸ The gap
-between the methods is closed due in part to the target's ability to
-automatically generating a `VIEW` which will unpack (or rather provide typing
-as a more accurate take) a JSON based ingestion source for you. Unless
-operating at tens of millions of rows with JSON objects containing multiple
-hundreds of keys, its quite performant. Particularly if accessing a small
-subset of keys. It does however fall off (quite hard) given enough scale as I
-mentioned (I've pushed it to the limits). Denormalized is recommended for high
-volume where the schema is fairly consistent. Fixed is recommended for lower
-volume, inconsistent schemas or for taps which are inherently schemaless in
-which case its the ideal (only...) logical pattern. Fixed schema can also be
-used for taps which routinely break down on BQ due to json schemas being
-inexpressible in a static way (ie patternProperties, additionalProperties...)
-**Old Header (still true, here for posterity)** ð§ª This is the first truly
-unstructured sink for BigQuery leveraging the recent GA feature in BigQuery for
-JSON support. This allows this target to load from essentially any tap
-regardless of the quality or explicitness of its jsonschema. Observations in
-existing taps note things such as `patternProperties` used in jsonschema
-objects which break down on all existing BigQuery taps due to the previous need
-for strong typing. Also taps such as MongoDB which inherently deal with
-unstructured data are seamlessly enabled by this target without klutzy
-collection scraping of a sample of records which we _hope_ are repesentative of
-all documents. Built with the [Meltano Target SDK](https://sdk.meltano.com). ##
-Configuration ð¨ ### Settings First a valid example to give context to the
-below including a nested key example (denoted via a `.` in the setting path) as
-seen with `column_name_transforms.snake_case` ```json { "project": "my-bq-
-project", "method": "storage_write_api", "denormalized": true,
-"credentials_path": "...", "dataset": "my_dataset", "location": "us-central1",
-"batch_size": 500, "column_name_transforms": { "snake_case": true } } ``` |
-Setting | Required | Default | Description | |:--------------------------------
--------------------|:--------:|:-----------------:|:---------------------------
+Usage Notes ### Denormalization So denormalized is a loaded term, so lets
+clarify here what we mean by it: > In the context of JSON objects,
+denormalization refers to the process of flattening a hierarchical or nested
+JSON object into a simpler, more "denormalized" structure that can be easier to
+work with for certain use cases. Denormalized=False (default) means we load all
+data into a single `JSON` column. This means all access requires an accessor
+such as `SELECT data.my_column FROM table` instead of `SELECT my_column FROM
+table`. Hence the term denormalized is relative to the `data` column which is
+the default for this target. This is a tradeoff between convenience/resilience
+and performance. This is the default because most _resilient_. IE a load will
+**never** fail due to a schema change or an invalid schema. You can always
+denormalize later via `dbt`. However, it is not the most performant and slower
+to transform. If your tap has a high quality and consistent schema,
+denormalization is the way to go to get the best performance and start modeling
+quickly. Denormalized=True means we unpack the data into a schema which is
+derived from the tap schema. It does _not_ mean we will flatten the data. There
+is a separate option for flattening. We will convert arrays to repeated fields
+and records to structs. All top level keys will end up as columns which is was
+you might expect from more typical targets. #### Resolver Versions There are 2
+resolver versions. The config option `schema_resolver_version` lets you select
+which version you want to use. This versioning exists because we want to
+support evolving how we resolve schemas whilst not creating breaking changes
+for long-time users dependent on how a schema is resolved. The default is `1`
+which behaves very similarly to existing flavors of `target-bigquery`. It works
+well enough but has plenty of edge cases where it simply cannot resolve valid
+jsonschemas to a bq schema. The new version `2` is much more robust and will
+resolve most, if not all schemas due to it falling back to `JSON` when in
+doubt. You must opt-in to this version by setting `schema_resolver_version: 2`
+in your config. ### Overwrite vs Append Sometimes you want to overwrite a table
+on every load. This can be achieved by either setting `overwrite: true` which
+will full refresh ALL tables **or** setting `overwrite: [table1, table2,
+table_*_other, !table_v1_other]` which will only overwrite the specified tables
+and supports pattern matching. This is useful if you have a table which is a
+lookup table and you want to overwrite it on every load. You can also set
+`overwrite: false` which will append to the table. This is the default
+behavior. ### Upsert (aka Merge) If you want to merge data into a table, you
+can set `merge: true` which will use the `MERGE` statement to upsert data. This
+supports pattern matching like the above setting. It requires `denormalized:
+true` takes precedence over `overwrite`. It will only work on tables which have
+a primary key as defined by the `key_properties` sent by the tap. There is a
+supporting config option called `dedupe_before_upsert` which will dedupe the
+data before upserting. This is useful if you are replicating data which has a
+primary key but is not unique. This occurs when you are replicating data from a
+source which has a primary key but does not enforce it. This is the case for
+MongoDB. It can also happen when moving data from a data lake in S3/GCS to a
+database. This is not the default behavior because it is slower and requires
+more resources. ## Features â¨ - Autoscaling self-healing worker pool using
+either threads (default) or multiprocessing, configurable by the user for the
+_fastest_ possible data ingestion. Particularly when leveraging colocated
+compute in GCP. - Denormalized load pattern where data is unpacked in flight
+into a statically typed BigQuery schema derived from the input stream json
+schemas. - Fix schema load pattern where all data is loaded into a `JSON`
+column which has been GA in BigQuery since mid 2022. - Autogenerated `VIEW`
+support for fixed schema load patterns which essentially overlays a statically
+typed schema allowing you to get the best of both worlds when using fixed
+schema ingestion. - JIT compilation of protobuf schemas allowing the Storage
+Write API to use a denormalized load pattern. - BATCH message support ð ##
+Load Patterns ð - `Batch Load Job` ingestion pattern using in memory
+compression (fixed schema + denormalized) - `Storage Write API` ingestion
+pattern using gRPC and protocol buffers supporting both streaming and batch
+patterns. Capable of JIT compilation of BQ schemas to protobuf to enable
+denormalized loads of input structures only known at runtime. (fixed schema +
+denormalized ð) - `GCS Staging` ingestion pattern using in memory
+compression and a GCS staging layer which generates a well organized data lake
+which backs the data warehouse providing additional failsafes and data sources
+(fixed schema + denormalized) - `Legacy Streaming` ingestion pattern which
+emphasizes simplicity and fast start up / tear down. I would highly recommend
+the storage write API instead unless data volume is small (fixed schema +
+denormalized) **Choosing between denormalized and fixed schema (JSON
+support)?** ðð¾ââï¸ The gap between the methods is closed due in part
+to the target's ability to automatically generating a `VIEW` which will unpack
+(or rather provide typing as a more accurate take) a JSON based ingestion
+source for you. Unless operating at tens of millions of rows with JSON objects
+containing multiple hundreds of keys, its quite performant. Particularly if
+accessing a small subset of keys. It does however fall off (quite hard) given
+enough scale as I mentioned (I've pushed it to the limits). Denormalized is
+recommended for high volume where the schema is fairly consistent. Fixed is
+recommended for lower volume, inconsistent schemas or for taps which are
+inherently schemaless in which case its the ideal (only...) logical pattern.
+Fixed schema can also be used for taps which routinely break down on BQ due to
+json schemas being inexpressible in a static way (ie patternProperties,
+additionalProperties...) **Old Header (still true, here for posterity)** ð§ª
+This is the first truly unstructured sink for BigQuery leveraging the recent GA
+feature in BigQuery for JSON support. This allows this target to load from
+essentially any tap regardless of the quality or explicitness of its
+jsonschema. Observations in existing taps note things such as
+`patternProperties` used in jsonschema objects which break down on all existing
+BigQuery taps due to the previous need for strong typing. Also taps such as
+MongoDB which inherently deal with unstructured data are seamlessly enabled by
+this target without klutzy collection scraping of a sample of records which we
+_hope_ are repesentative of all documents. Built with the [Meltano Target SDK]
+(https://sdk.meltano.com). ## Configuration ð¨ ### Settings First a valid
+example to give context to the below including a nested key example (denoted
+via a `.` in the setting path) as seen with `column_name_transforms.snake_case`
+```json { "project": "my-bq-project", "method": "storage_write_api",
+"denormalized": true, "credentials_path": "...", "dataset": "my_dataset",
+"location": "us-central1", "batch_size": 500, "column_name_transforms":
+{ "snake_case": true } } ``` | Setting | Required | Default | Description | |:-
+--------------------------------------------------|:--------:|:----------------
+-:|:---------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
----------------------------------------------------------------------------| |
-credentials_path | False | None | The path to a gcp credentials json file. | |
-credentials_json | False | None | A JSON string of your service account JSON
-file. | | project | True | None | The target GCP project to materialize data
-into. | | dataset | True | None | The target dataset to materialize data into.
-| | location | False | US | The target dataset location to materialize data
-into. Applies also to the GCS bucket if using `gcs_stage` load method. | |
-batch_size | False | 500 | The maximum number of rows to send in a single batch
-to the worker. This should be configured based on load method. For
-`storage_write_api` and `streaming_insert` it should be `<=500`, for the
-LoadJob sinks, it can be much higher, ie `>100,000` | | timeout | False | 600 |
-Default timeout for batch_job and gcs_stage derived LoadJobs. | | fail_fast |
-False | True | Fail the entire load job if any row fails to insert. | |
-denormalized | False | False | Determines whether to denormalize the data
-before writing to BigQuery. A false value will write data using a fixed JSON
-column based schema, while a true value will write data using a dynamic schema
-derived from the tap. | | method | True | storage_write_api | The method to use
-for writing to BigQuery. Must be one of `batch_job`, `storage_write_api`,
-`gcs_stage`, `streaming_insert` | | generate_view | False | False | Determines
-whether to generate a view based on the SCHEMA message parsed from the tap.
-Only valid if denormalized=false meaning you are using the fixed JSON column
-based schema. | | upsert | False | False | Determines if we should upsert.
-Defaults to false. A value of true will write to a temporary table and then
-merge into the target table (upsert). This requires the target table to be
-unique on the key properties. A value of false will write to the target table
-directly (append). A value of an array of strings will evaluate the strings in
-order using fnmatch. At the end of the array, the value of the last match will
-be used. If not matched, the default value is false (append). | | overwrite |
-False | False | Determines if the target table should be overwritten on load.
-Defaults to false. A value of true will write to a temporary table and then
-overwrite the target table inside a transaction (so it is safe). A value of
-false will write to the target table directly (append). A value of an array of
+---------------------------| | credentials_path | False | None | The path to a
+gcp credentials json file. | | credentials_json | False | None | A JSON string
+of your service account JSON file. | | project | True | None | The target GCP
+project to materialize data into. | | dataset | True | None | The target
+dataset to materialize data into. | | location | False | US | The target
+dataset location to materialize data into. Applies also to the GCS bucket if
+using `gcs_stage` load method. | | batch_size | False | 500 | The maximum
+number of rows to send in a single batch to the worker. This should be
+configured based on load method. For `storage_write_api` and `streaming_insert`
+it should be `<=500`, for the LoadJob sinks, it can be much higher, ie
+`>100,000` | | timeout | False | 600 | Default timeout for batch_job and
+gcs_stage derived LoadJobs. | | fail_fast | False | True | Fail the entire load
+job if any row fails to insert. | | denormalized | False | False | Determines
+whether to denormalize the data before writing to BigQuery. A false value will
+write data using a fixed JSON column based schema, while a true value will
+write data using a dynamic schema derived from the tap. | | method | True |
+storage_write_api | The method to use for writing to BigQuery. Must be one of
+`batch_job`, `storage_write_api`, `gcs_stage`, `streaming_insert` | |
+generate_view | False | False | Determines whether to generate a view based on
+the SCHEMA message parsed from the tap. Only valid if denormalized=false
+meaning you are using the fixed JSON column based schema. | | upsert | False |
+False | Determines if we should upsert. Defaults to false. A value of true will
+write to a temporary table and then merge into the target table (upsert). This
+requires the target table to be unique on the key properties. A value of false
+will write to the target table directly (append). A value of an array of
 strings will evaluate the strings in order using fnmatch. At the end of the
 array, the value of the last match will be used. If not matched, the default
-value is false. This is mutually exclusive with the `upsert` option. If both
-are set, `upsert` will take precedence. | | dedupe_before_upsert | False |
-False | This option is only used if `upsert` is enabled for a stream. The
-selection criteria for the stream's candidacy is the same as upsert. If the
-stream is marked for deduping before upsert, we will create a _session scoped
-temporary table during the merge transaction to dedupe the ingested records.
-This is useful for streams that are not unique on the key properties during an
-ingest but are unique in the source system. Data lake ingestion is often a good
-example of this where the same unique record may exist in the lake at different
-points in time from different extracts. | | bucket | False | None | The GCS
-bucket to use for staging data. Only used if method is gcs_stage. | |
-cluster_on_key_properties | False | 0 | Determines whether to cluster on the
-key properties from the tap. Defaults to false. When false, clustering will be
-based on _sdc_batched_at instead. | | partition_granularity | False | "month" |
-Indicates the granularity of the created table partitioning scheme which is
-based on `_sdc_batched_at`. By default the granularity is monthly. Must be one
-of: "hour", "day", "month", "year". | | column_name_transforms.lower | False |
-None | Lowercase column names. | | column_name_transforms.quote | False | None
-| Quote column names in any generated DDL. | |
-column_name_transforms.add_underscore_when_invalid | False | None | Add an
-underscore to the column name if it starts with a digit to make it valid. | |
-column_name_transforms.snake_case | False | None | Snake case all incoming
-column names. Does not apply to fixed schema loads but _does_ apply to the view
-auto-generated over them. | | options.storage_write_batch_mode | False | None |
-By default, we use the default stream (Committed mode) in the
-[storage_write_api](https://cloud.google.com/bigquery/docs/write-api) load
-method which results in streaming records which are immediately available and
-is generally fastest. If this is set to true, we will use the application
-created streams (pending mode) to transactionally batch data on STATE messages
-and at end of pipe. | | options.process_pool | False | None | By default we use
-an autoscaling threadpool to write to BigQuery. If set to true, we will use a
-process pool. | | options.max_workers | False | None | By default, each sink
-type has a preconfigured max worker pool limit. This sets an override for
-maximum number of workers in the pool. | | stream_maps | False | None | Config
-object for stream maps capability. For more information check out [Stream Maps]
-(https://sdk.meltano.com/en/latest/stream_maps.html). | | stream_map_config |
-False | None | User-defined config values to be used within map expressions. |
-| flattening_enabled | False | None | 'True' to enable schema flattening and
-automatically expand nested properties. | | flattening_max_depth | False | None
-| The max depth to flatten schemas. | A full list of supported settings and
-capabilities is available by running: `target-bigquery --about` ### Configure
-using environment variables âï¸ This Singer target will automatically import
-any environment variables within the working directory's `.env` if the `--
-config=ENV` is provided, such that config values will be considered if a
-matching environment variable is set either in the terminal context or in the
-`.env` file. ### Source Authentication and Authorization ð®ð½ââï¸
-Authenticate via service account key file or Application Default Credentials
-(ADC) https://cloud.google.com/bigquery/docs/authentication ## Capabilities â¨
-* `about` * `stream-maps` * `schema-flattening` * `batch` ## Usage
-ð·ââï¸ You can easily run `target-bigquery` by itself or in a pipeline
-using [Meltano](https://meltano.com/). ### Executing the Target Directly ð§
-```bash target-bigquery --version target-bigquery --help # Test using the
-"Carbon Intensity" sample: tap-carbon-intensity | target-bigquery --config /
-path/to/target-bigquery-config.json ``` ## Developer Resources ð©ð¼âð»
-### Initialize your Development Environment ```bash pipx install poetry poetry
-install ``` ### Create and Run Tests Create tests within the `target_bigquery/
-tests` subfolder and then run: ```bash poetry run pytest ``` You can also test
-the `target-bigquery` CLI interface directly using `poetry run`: ```bash poetry
-run target-bigquery --help ``` ### Testing with [Meltano](https://meltano.com/
-) _**Note:** This target will work in any Singer environment and does not
-require Meltano. Examples here are for convenience and to streamline end-to-end
-orchestration scenarios._ Next, install Meltano (if you haven't already) and
-any needed plugins: ```bash # Install meltano pipx install meltano # Initialize
-meltano within this directory cd target-bigquery meltano install ``` Now you
-can test and orchestrate using Meltano: ```bash # Test invocation: meltano
-invoke target-bigquery --version # OR run a test `elt` pipeline with the Carbon
+value is false (append). | | overwrite | False | False | Determines if the
+target table should be overwritten on load. Defaults to false. A value of true
+will write to a temporary table and then overwrite the target table inside a
+transaction (so it is safe). A value of false will write to the target table
+directly (append). A value of an array of strings will evaluate the strings in
+order using fnmatch. At the end of the array, the value of the last match will
+be used. If not matched, the default value is false. This is mutually exclusive
+with the `upsert` option. If both are set, `upsert` will take precedence. | |
+dedupe_before_upsert | False | False | This option is only used if `upsert` is
+enabled for a stream. The selection criteria for the stream's candidacy is the
+same as upsert. If the stream is marked for deduping before upsert, we will
+create a _session scoped temporary table during the merge transaction to dedupe
+the ingested records. This is useful for streams that are not unique on the key
+properties during an ingest but are unique in the source system. Data lake
+ingestion is often a good example of this where the same unique record may
+exist in the lake at different points in time from different extracts. | |
+bucket | False | None | The GCS bucket to use for staging data. Only used if
+method is gcs_stage. | | cluster_on_key_properties | False | 0 | Determines
+whether to cluster on the key properties from the tap. Defaults to false. When
+false, clustering will be based on _sdc_batched_at instead. | |
+partition_granularity | False | "month" | Indicates the granularity of the
+created table partitioning scheme which is based on `_sdc_batched_at`. By
+default the granularity is monthly. Must be one of: "hour", "day", "month",
+"year". | | column_name_transforms.lower | False | None | Lowercase column
+names. | | column_name_transforms.quote | False | None | Quote column names in
+any generated DDL. | | column_name_transforms.add_underscore_when_invalid |
+False | None | Add an underscore to the column name if it starts with a digit
+to make it valid. | | column_name_transforms.snake_case | False | None | Snake
+case all incoming column names. Does not apply to fixed schema loads but _does_
+apply to the view auto-generated over them. | |
+options.storage_write_batch_mode | False | None | By default, we use the
+default stream (Committed mode) in the [storage_write_api](https://
+cloud.google.com/bigquery/docs/write-api) load method which results in
+streaming records which are immediately available and is generally fastest. If
+this is set to true, we will use the application created streams (pending mode)
+to transactionally batch data on STATE messages and at end of pipe. | |
+options.process_pool | False | None | By default we use an autoscaling
+threadpool to write to BigQuery. If set to true, we will use a process pool. |
+| options.max_workers | False | None | By default, each sink type has a
+preconfigured max worker pool limit. This sets an override for maximum number
+of workers in the pool. | | schema_resolver_version | False | 1 | The version
+of the schema resolver to use. Defaults to 1. Version 2 uses JSON as a fallback
+during denormalization. This only has an effect if denormalized=true | |
+stream_maps | False | None | Config object for stream maps capability. For more
+information check out [Stream Maps](https://sdk.meltano.com/en/latest/
+stream_maps.html). | | stream_map_config | False | None | User-defined config
+values to be used within map expressions. | | flattening_enabled | False | None
+| 'True' to enable schema flattening and automatically expand nested
+properties. | | flattening_max_depth | False | None | The max depth to flatten
+schemas. | A full list of supported settings and capabilities is available by
+running: `target-bigquery --about` ### Configure using environment variables
+âï¸ This Singer target will automatically import any environment variables
+within the working directory's `.env` if the `--config=ENV` is provided, such
+that config values will be considered if a matching environment variable is set
+either in the terminal context or in the `.env` file. ### Source Authentication
+and Authorization ð®ð½ââï¸ Authenticate via service account key file
+or Application Default Credentials (ADC) https://cloud.google.com/bigquery/
+docs/authentication ## Capabilities â¨ * `about` * `stream-maps` * `schema-
+flattening` * `batch` ## Usage ð·ââï¸ You can easily run `target-
+bigquery` by itself or in a pipeline using [Meltano](https://meltano.com/). ###
+Executing the Target Directly ð§ ```bash target-bigquery --version target-
+bigquery --help # Test using the "Carbon Intensity" sample: tap-carbon-
+intensity | target-bigquery --config /path/to/target-bigquery-config.json ```
+## Developer Resources ð©ð¼âð» ### Initialize your Development
+Environment ```bash pipx install poetry poetry install ``` ### Create and Run
+Tests Create tests within the `target_bigquery/tests` subfolder and then run:
+```bash poetry run pytest ``` You can also test the `target-bigquery` CLI
+interface directly using `poetry run`: ```bash poetry run target-bigquery --
+help ``` ### Testing with [Meltano](https://meltano.com/) _**Note:** This
+target will work in any Singer environment and does not require Meltano.
+Examples here are for convenience and to streamline end-to-end orchestration
+scenarios._ Next, install Meltano (if you haven't already) and any needed
+plugins: ```bash # Install meltano pipx install meltano # Initialize meltano
+within this directory cd target-bigquery meltano install ``` Now you can test
+and orchestrate using Meltano: ```bash # Test invocation: meltano invoke
+target-bigquery --version # OR run a test `elt` pipeline with the Carbon
 Intensity sample tap: meltano elt tap-carbon-intensity target-bigquery ``` ###
 SDK Dev Guide See the [dev guide](https://sdk.meltano.com/en/latest/
 dev_guide.html) for more instructions on how to use the Meltano SDK to develop
 your own Singer taps and targets.
```

### Comparing `z3_target_bigquery-0.6.3/pyproject.toml` & `z3_target_bigquery-0.6.6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "z3-target-bigquery"
-version = "0.6.3"
+version = "0.6.6"
 description = "z3-target-bigquery is a Singer target for BigQuery. It supports storage write, GCS, streaming, and batch load methods. Built with the Meltano SDK."
 authors = ["Alex Butler <butler.alex2010@gmail.com>"]
 keywords = ["ELT", "BigQuery"]
 license = "MIT"
 include = ["target_bigquery/*.py", "README.md", "LICENSE"]
 homepage = "https://github.com/z3z1ma/target-bigquery"
 repository = "https://github.com/z3z1ma/target-bigquery"
@@ -26,15 +26,15 @@
     { include = "README.md" },
     { include = "LICENSE" },
 ]
 
 [tool.poetry.dependencies]
 python = "<3.11,>=3.8"
 requests = ">=2.25.1"
-singer-sdk = ">=0.16.0"
+singer-sdk = ">=0.22.0,<0.23.0"
 google-cloud-bigquery = { version = ">=3.4.1,<4", extras = ["bqstorage"] }
 orjson = ">=3.7.2,<4"
 tenacity = ">=8.0.1,<9"
 grpcio-tools = ">=1.51.1,<2"
 google-cloud-storage = ">=2.7.0,<3"
 grpcio-status = ">=1.51.1,<2"
```

### Comparing `z3_target_bigquery-0.6.3/target_bigquery/batch_job.py` & `z3_target_bigquery-0.6.6/target_bigquery/batch_job.py`

 * *Files identical despite different names*

### Comparing `z3_target_bigquery-0.6.3/target_bigquery/constants.py` & `z3_target_bigquery-0.6.6/target_bigquery/constants.py`

 * *Files identical despite different names*

### Comparing `z3_target_bigquery-0.6.3/target_bigquery/core.py` & `z3_target_bigquery-0.6.6/target_bigquery/core.py`

 * *Files 15% similar despite different names*

```diff
@@ -65,45 +65,61 @@
     "YEAR": TimePartitioningType.YEAR,
     "MONTH": TimePartitioningType.MONTH,
     "DAY": TimePartitioningType.DAY,
     "HOUR": TimePartitioningType.HOUR,
 }
 
 
+class SchemaResolverVersion(Enum):
+    """The schema resolver version to use."""
+
+    V1 = 1
+    V2 = 2
+
+    def __str__(self) -> str:
+        return str(self.value)
+
+
 @dataclass
 class BigQueryTable:
     name: str
     """The name of the table."""
     dataset: str
     """The dataset that this table belongs to."""
     project: str
     """The project that this table belongs to."""
     jsonschema: Dict[str, Any]
     """The jsonschema for this table."""
     ingestion_strategy: IngestionStrategy
     """The ingestion strategy for this table."""
     transforms: Dict[str, bool] = field(default_factory=dict)
     """A dict of transformation rules to apply to the table schema."""
+    schema_resolver_version: SchemaResolverVersion = SchemaResolverVersion.V1
 
     @property
     def schema_translator(self) -> "SchemaTranslator":
         """Returns a SchemaTranslator instance for this table."""
         if not hasattr(self, "_schema_translator"):
             self._schema_translator = SchemaTranslator(
                 schema=self.jsonschema,
                 transforms=self.transforms,
+                resolver_version=self.schema_resolver_version,
             )
         return self._schema_translator
 
     def get_schema(self, apply_transforms: bool = False) -> List[bigquery.SchemaField]:
         """Returns the jsonschema to bigquery schema translation for this table."""
         if apply_transforms:
             return self.schema_translator.translated_schema_transformed
         return self.schema_translator.translated_schema
 
+    def get_escaped_name(self, suffix: str = '') -> str:
+        """Returns the table name as as escaped SQL string."""
+        return f"`{self.project}`.`{self.dataset}`.`{self.name}{suffix}`"
+
     def get_resolved_schema(self, apply_transforms: bool = False) -> List[bigquery.SchemaField]:
         """Returns the schema for this table after factoring in the ingestion strategy."""
         if self.ingestion_strategy is IngestionStrategy.FIXED:
             return DEFAULT_SCHEMA
         elif self.ingestion_strategy is IngestionStrategy.DENORMALIZED:
             return self.get_schema(apply_transforms)
 
@@ -277,14 +293,15 @@
         self.client = bigquery_client_factory(self._credentials)
         opts = {
             "project": self.config["project"],
             "dataset": self.config["dataset"],
             "jsonschema": self.schema,
             "transforms": self.config.get("column_name_transforms", {}),
             "ingestion_strategy": self.ingestion_strategy,
+            "schema_resolver_version": SchemaResolverVersion(self.config.get("schema_resolver_version", 1)),
         }
         self.table = BigQueryTable(name=self.table_name, **opts)
         self.create_target(key_properties=key_properties)
         self.update_schema()
         self.merge_target: Optional[BigQueryTable] = None
         self.overwrite_target: Optional[BigQueryTable] = None
         # In absence of dedupe or overwrite candidacy, we append to the target table directly
@@ -449,15 +466,15 @@
         )
         kwargs["dataset"]["location"] = location
         # Create the table
         self.table.create_table(self.client, self.apply_transforms, **kwargs)
         if self.generate_view:
             self.client.query(
                 self.table.schema_translator.generate_view_statement(
-                    str(self.table),
+                    self.table,
                 )
             ).result()
 
     def update_schema(self) -> None:
         """Update the target schema in BigQuery."""
         pass
 
@@ -485,15 +502,15 @@
                 # a _SESSION scoped intermediate table.
                 tmp = f"{target.name}__tmp"
                 dedupe_query = (
                     f"SELECT * FROM {self.table} "
                     f"QUALIFY ROW_NUMBER() OVER (PARTITION BY {', '.join(self.key_properties)} "
                     f"ORDER BY COALESCE({', '.join(date_columns)}) DESC) = 1"
                 )
-                ctas_tmp = f"CREATE OR REPLACE TEMP TABLE {tmp} AS {dedupe_query}"
+                ctas_tmp = f"CREATE OR REPLACE TEMP TABLE `{tmp}` AS {dedupe_query}"
             merge_clause = (
                 f"MERGE `{self.merge_target}` AS target USING `{tmp or self.table}` AS source ON "
                 + " AND ".join(f"target.`{f}` = source.`{f}`" for f in self.key_properties)
             )
             update_clause = "UPDATE SET " + ", ".join(
                 f"target.`{f.name}` = source.`{f.name}`" for f in target.schema
             )
@@ -501,27 +518,27 @@
                 f"INSERT ({', '.join(f.name for f in target.schema)}) "
                 f"VALUES ({', '.join(f'source.`{f.name}`' for f in target.schema)})"
             )
             self.client.query(
                 f"{ctas_tmp}; {merge_clause} "
                 f"WHEN MATCHED THEN {update_clause} "
                 f"WHEN NOT MATCHED THEN {insert_clause}; "
-                f"DROP TABLE IF EXISTS {self.table};"
+                f"DROP TABLE IF EXISTS {self.table.get_escaped_name()};"
             ).result()
             self.table = self.merge_target
             self.merge_target = None
         elif self.overwrite_target is not None:
             # We must overwrite the target table with the temp table.
             # Do it in a transaction to avoid partial writes.
             target = self.overwrite_target.as_table()
             self.client.query(
-                f"DROP TABLE IF EXISTS {self.overwrite_target}; "
-                f"CREATE TABLE {self.overwrite_target} LIKE {self.table} AS "
-                f"SELECT * FROM {self.table};"
-                f"DROP TABLE IF EXISTS {self.table};"
+                f"DROP TABLE IF EXISTS {self.overwrite_target.get_escaped_name()}; "
+                f"CREATE TABLE {self.overwrite_target} LIKE {self.table.get_escaped_name()} AS "
+                f"SELECT * FROM {self.table.get_escaped_name()};"
+                f"DROP TABLE IF EXISTS {self.table.get_escaped_name()};"
             ).result()
             self.table = self.merge_target
             self.merge_target = None
 
 
 class Denormalized:
     """This class provides common overrides for denormalized sinks and should be subclassed
@@ -570,27 +587,33 @@
         sys.path = original_sys_path
 
 
 @cache
 def bigquery_client_factory(creds: BigQueryCredentials) -> bigquery.Client:
     """Get a BigQuery client."""
     if creds.path:
-        return bigquery.Client.from_service_account_json(creds.path)
+        return bigquery.Client.from_service_account_json(creds.path,
+            project=creds.project
+        )
     elif creds.json:
-        return bigquery.Client.from_service_account_info(json.loads(creds.json))
+        return bigquery.Client.from_service_account_info(
+            json.loads(creds.json), project=creds.project
+        )
     return bigquery.Client(project=creds.project)
 
 
 @cache
 def gcs_client_factory(creds: BigQueryCredentials) -> storage.Client:
     """Get a GCS client."""
     if creds.path:
-        return storage.Client.from_service_account_json(creds.path)
+        return storage.Client.from_service_account_json(creds.path, project=creds.project)
     elif creds.json:
-        return storage.Client.from_service_account_info(json.loads(creds.json))
+        return storage.Client.from_service_account_info(
+            json.loads(creds.json), project=creds.project
+        )
     return storage.Client(project=creds.project)
 
 
 @cache
 def storage_client_factory(
     creds: BigQueryCredentials,
 ) -> bigquery_storage_v1.BigQueryWriteClient:
@@ -599,23 +622,38 @@
         return bigquery_storage_v1.BigQueryWriteClient.from_service_account_file(creds.path)
     elif creds.json:
         return bigquery_storage_v1.BigQueryWriteClient.from_service_account_info(
             json.loads(creds.json)
         )
     return bigquery_storage_v1.BigQueryWriteClient()
 
+@dataclass
+class _FieldProjection:
+    projection: str
+    alias: str
+
+    def as_sql(self) -> str:
+        """Return the SQL representation of this projection"""
+        return f'{self.projection} as {self.alias.lstrip()},\n'
+
 
 # This class translates a JSON schema into a BigQuery schema.
 # It also uses the translated schema to generate a CREATE VIEW statement.
 class SchemaTranslator:
     """Translate a JSON schema into a BigQuery schema."""
 
-    def __init__(self, schema: Dict[str, Any], transforms: Dict[str, bool]):
+    def __init__(
+        self,
+        schema: Dict[str, Any],
+        transforms: Dict[str, bool],
+        resolver_version: SchemaResolverVersion = SchemaResolverVersion.V1,
+    ) -> None:
         self.schema = schema
         self.transforms = transforms
+        self.resolver_version = resolver_version
         # Used by fixed schema strategy where we defer transformation
         # to the view statement
         self._translated_schema = None
         # Used by the denormalized strategy where we eagerly transform
         # the target schema
         self._translated_schema_transformed = None
 
@@ -656,163 +694,211 @@
                 for i, inner in enumerate(v):
                     if isinstance(inner, dict):
                         output[k][i] = self.translate_record(inner)
             if isinstance(v, dict):
                 output[k] = self.translate_record(v)
         return output
 
-    def generate_view_statement(self, table_name: str) -> str:
+    def generate_view_statement(self, table_name: BigQueryTable) -> str:
         """Generate a CREATE VIEW statement for the SchemaTranslator `schema`."""
         projection = ""
         for field_ in self.translated_schema[:]:
             if field_.mode == "REPEATED":
                 projection += indent(self._wrap_json_array(field_, path="$", depth=1), " " * 4)
             else:
-                projection += indent(self._bigquery_field_to_projection(field_), " " * 4)
+                projection += indent(self._bigquery_field_to_projection(field_).as_sql(), " " * 4)
 
         return (
-            f"CREATE OR REPLACE VIEW {table_name}_view AS \nSELECT \n{projection} FROM {table_name}"
+            f"CREATE OR REPLACE VIEW {table_name.get_escaped_name('_view')} AS \nSELECT \n{projection} FROM {table_name.get_escaped_name()}"
         )
 
     def _jsonschema_property_to_bigquery_column(
         self, name: str, schema_property: dict
     ) -> SchemaField:
-        """Translate a JSON schema property into a BigQuery column."""
-        if "anyOf" in schema_property and len(schema_property["anyOf"]) > 0:
-            # I have only seen this used in the wild with tap-salesforce, which
-            # is incidentally an important one so lets handle the anyOf case
-            # by giving the 0th index priority.
-            property_type = schema_property["anyOf"][0].get("type", "string")
-            property_format = schema_property["anyOf"][0].get("format", None)
-        else:
-            property_type = schema_property.get("type", "string")
-            property_format = schema_property.get("format", None)
+        """Translate a JSON schema property into a BigQuery column.
+        
+        The v1 resolver is very similar to how existing target-bigquery implementations worked.
+        The v2 resolver uses JSON in all cases the schema property is unresolvable making it _much_
+        more flexible though the denormalization can only be said to be partial if a type is not
+        resolved. Most of the time this is fine but for the sake of consistency, we default to v1.
+        """
+        if self.resolver_version == SchemaResolverVersion.V1:
+            # This is the original resolver, which is used by the denormalized strategy
+            if "anyOf" in schema_property and len(schema_property["anyOf"]) > 0:
+                # I have only seen this used in the wild with tap-salesforce, which
+                # is incidentally an important one so lets handle the anyOf case
+                # by giving the 0th index priority.
+                property_type = schema_property["anyOf"][0].get("type", "string")
+                property_format = schema_property["anyOf"][0].get("format", None)
+            else:
+                property_type = schema_property.get("type", "string")
+                property_format = schema_property.get("format", None)
+
+            if "array" in property_type:
+                if "items" not in schema_property:
+                    return SchemaField(name, "JSON", "REPEATED")
+                items_schema: dict = schema_property["items"]
+                items_type = bigquery_type(items_schema["type"], items_schema.get("format", None))
+                if items_type == "record":
+                    return self._translate_record_to_bigquery_schema(name, items_schema, "REPEATED")
+                return SchemaField(name, items_type, "REPEATED")
+            elif "object" in property_type:
+                return self._translate_record_to_bigquery_schema(name, schema_property)
+            else:
+                result_type = bigquery_type(property_type, property_format)
+                return SchemaField(name, result_type, "NULLABLE")
+        elif self.resolver_version == SchemaResolverVersion.V2:
+            # This is the new resolver, which is far more lenient and falls back to JSON
+            # if it doesn't know how to translate a property.
+            try:
+                if "anyOf" in schema_property and len(schema_property["anyOf"]) > 0:
+                    # I have only seen this used in the wild with tap-salesforce, which
+                    # is incidentally an important one so lets handle the anyOf case
+                    # by giving the 0th index priority.
+                    property_type = schema_property["anyOf"][0].get("type", "string")
+                    property_format = schema_property["anyOf"][0].get("format", None)
+                else:
+                    property_type = schema_property["type"]
+                    property_format = schema_property.get("format", None)
+
+                if "array" in property_type:
+                    if "items" not in schema_property or "type" not in schema_property["items"]:
+                        return SchemaField(name, "JSON", "REPEATED")
+                    items_schema: dict = schema_property["items"]
+                    if "patternProperties" in items_schema:
+                        return SchemaField(name, "JSON", "REPEATED")
+                    items_type = bigquery_type(items_schema["type"], items_schema.get("format", None))
+                    if items_type == "record":
+                        return self._translate_record_to_bigquery_schema(name, items_schema, "REPEATED")
+                    return SchemaField(name, items_type, "REPEATED")
+                elif "object" in property_type:
+                    if "properties" not in schema_property or len(schema_property["properties"]) == 0 or "patternProperties" in schema_property:
+                        return SchemaField(name, "JSON", "NULLABLE")
+                    return self._translate_record_to_bigquery_schema(name, schema_property)
+                else:
+                    if "patternProperties" in schema_property:
+                        return SchemaField(name, "JSON", "NULLABLE")
+                    result_type = bigquery_type(property_type, property_format)
+                    return SchemaField(name, result_type, "NULLABLE")
+            except Exception:
+                return SchemaField(name, "JSON", "NULLABLE")
 
-        if "array" in property_type:
-            if "items" not in schema_property:
-                return SchemaField(name, "JSON", "REPEATED")
-            items_schema: dict = schema_property["items"]
-            items_type = bigquery_type(items_schema["type"], items_schema.get("format", None))
-            if items_type == "record":
-                return self._translate_record_to_bigquery_schema(name, items_schema, "REPEATED")
-            return SchemaField(name, items_type, "REPEATED")
-        elif "object" in property_type:
-            return self._translate_record_to_bigquery_schema(name, schema_property)
-        else:
-            result_type = bigquery_type(property_type, property_format)
-            return SchemaField(name, result_type, "NULLABLE")
 
     def _translate_record_to_bigquery_schema(
         self, name: str, schema_property: dict, mode: str = "NULLABLE"
     ) -> SchemaField:
         """Translate a JSON schema record into a BigQuery schema."""
         fields = [
             self._jsonschema_property_to_bigquery_column(col, t)
             for col, t in schema_property.get("properties", {}).items()
         ]
         return SchemaField(name, "RECORD", mode, fields=fields)
 
     def _bigquery_field_to_projection(
         self, field: SchemaField, path: str = "$", depth: int = 0, base: str = "data"
-    ) -> str:
+    ) -> _FieldProjection:
         """Translate a BigQuery schema field into a SQL projection."""
         # Pass-through _sdc columns into the projection as-is
         if field.name.startswith("_sdc_"):
-            return f"{field.name},\n"
+            return _FieldProjection(field.name, field.name)
 
         scalar = f"{base}.{field.name}"
         from_base = f"{path}.{field.name}" if base == "data" else "$"
 
         # Records are handled recursively
         if field.field_type.upper() == "RECORD":
-            return (
+            return _FieldProjection(
                 (" " * depth * 2)
                 + "STRUCT(\n{}\n".format(
                     "".join(
                         [
                             (
                                 self._bigquery_field_to_projection(
                                     f, path=from_base, depth=depth + 1, base=base
-                                )
+                                ).as_sql()
                                 if not f.mode == "REPEATED"
                                 else self._wrap_json_array(
                                     f, path=from_base, depth=depth, base=base
                                 )
                             )
                             for f in field.fields
                         ]
                     ).rstrip(",\n"),
                 )
                 + (" " * depth * 2)
-                + f") as {transform_column_name(field.name, **self.transforms)},\n"
+                + ")", f"{transform_column_name(field.name, **self.transforms)}"
             )
         # Nullable fields require a JSON_VALUE call which creates a 2-stage cast
         elif field.is_nullable:
-            return (" " * depth * 2) + self._wrap_nullable_json_value(field, path=path, base=base)
+            _field = self._wrap_nullable_json_value(field, path=path, base=base)
+            return _FieldProjection((" " * depth * 2) + _field.projection, _field.alias)
         # These are not nullable so if the type is known, we can do a 1-stage extract & cast
         elif field.field_type.upper() == "STRING":
-            return (
+            return _FieldProjection((
                 " " * depth * 2
-            ) + f"STRING({scalar}) as {transform_column_name(field.name, **self.transforms)},\n"
+            ) + f"STRING({scalar})", f"{transform_column_name(field.name, **self.transforms)}")
         elif field.field_type.upper() == "INTEGER":
-            return (
+            return _FieldProjection((
                 " " * depth * 2
-            ) + f"INT64({scalar}) as {transform_column_name(field.name, **self.transforms)},\n"
+            ) + f"INT64({scalar})", f"{transform_column_name(field.name, **self.transforms)}")
         elif field.field_type.upper() == "FLOAT":
-            return (
+            return _FieldProjection(
                 (" " * depth * 2)
-                + f"FLOAT64({scalar}) as {transform_column_name(field.name, **self.transforms)},\n"
+                + f"FLOAT64({scalar})", f"{transform_column_name(field.name, **self.transforms)}"
             )
         elif field.field_type.upper() == "BOOLEAN":
-            return (
+            return _FieldProjection((
                 " " * depth * 2
-            ) + f"BOOL({scalar}) as {transform_column_name(field.name, **self.transforms)},\n"
+            ) + f"BOOL({scalar})", f"{transform_column_name(field.name, **self.transforms)}")
         # Fallback to a 2-stage extract & cast
         else:
-            return (" " * depth * 2) + self._wrap_nullable_json_value(field, path, base)
+            _field =  self._wrap_nullable_json_value(field, path, base)
+            return _FieldProjection((" " * depth * 2) + _field.projection, _field.alias)
 
     def _wrap_json_array(
         self, field: SchemaField, path: str, depth: int = 0, base: str = "data"
     ) -> str:
         """Translate a BigQuery schema field into a SQL projection for a repeated field."""
-        v = self._bigquery_field_to_projection(
+        _v = self._bigquery_field_to_projection(
             field, path="$", depth=depth, base=f"{field.name}__rows"
-        ).rstrip(", \n")
+        )
+        v = _v.as_sql().rstrip(", \n")
         return (" " * depth * 2) + indent(
             dedent(
                 f"""
         ARRAY(
             SELECT {v}
             FROM UNNEST(
                 JSON_QUERY_ARRAY({base}, '{path}.{field.name}')
             ) AS {field.name}__rows
+            WHERE {_v.projection} IS NOT NULL
         """
                 + (" " * depth * 2)
                 + f") AS {field.name},\n"
             ).lstrip(),
             " " * depth * 2,
         )
 
     def _wrap_nullable_json_value(
         self, field: SchemaField, path: str = "$", base: str = "data"
-    ) -> str:
+    ) -> _FieldProjection:
         """Translate a BigQuery schema field into a SQL projection for a nullable field."""
         typ = field.field_type.upper()
         if typ == "STRING":
-            return (
-                f"JSON_VALUE({base}, '{path}.{field.name}') as"
-                f" {transform_column_name(field.name, **self.transforms)},\n"
+            return _FieldProjection(
+                f"JSON_VALUE({base}, '{path}.{field.name}')",
+                f" {transform_column_name(field.name, **self.transforms)}"
             )
         if typ == "FLOAT":
             typ = "FLOAT64"
         if typ in ("INT", "INTEGER"):
             typ = "INT64"
-        return (
-            f"CAST(JSON_VALUE({base}, '{path}.{field.name}') as {typ}) as"
-            f" {transform_column_name(field.name, **self.transforms)},\n"
+        return _FieldProjection(
+            f"CAST(JSON_VALUE({base}, '{path}.{field.name}') as {typ})",
+            f" {transform_column_name(field.name, **self.transforms)}"
         )
 
 
 class Compressor:
     """Compresses streams of bytes using gzip."""
 
     def __init__(self) -> None:
```

### Comparing `z3_target_bigquery-0.6.3/target_bigquery/gcs_stage.py` & `z3_target_bigquery-0.6.6/target_bigquery/gcs_stage.py`

 * *Files identical despite different names*

### Comparing `z3_target_bigquery-0.6.3/target_bigquery/proto_gen.py` & `z3_target_bigquery-0.6.6/target_bigquery/proto_gen.py`

 * *Files identical despite different names*

### Comparing `z3_target_bigquery-0.6.3/target_bigquery/storage_write.py` & `z3_target_bigquery-0.6.6/target_bigquery/storage_write.py`

 * *Files identical despite different names*

### Comparing `z3_target_bigquery-0.6.3/target_bigquery/streaming_insert.py` & `z3_target_bigquery-0.6.6/target_bigquery/streaming_insert.py`

 * *Files identical despite different names*

### Comparing `z3_target_bigquery-0.6.3/target_bigquery/target.py` & `z3_target_bigquery-0.6.6/target_bigquery/target.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,17 @@
 # substantial portions of the Software.
 """BigQuery target class."""
 import copy
 import time
 import uuid
 from typing import TYPE_CHECKING, Callable, Dict, List, Optional, Tuple, Type, Union
 
+from singer_sdk import Sink
 from singer_sdk import typing as th
-from singer_sdk.target_base import Sink, Target
+from singer_sdk.target_base import Target
 
 from target_bigquery.batch_job import BigQueryBatchJobDenormalizedSink, BigQueryBatchJobSink
 from target_bigquery.core import BaseBigQuerySink, BaseWorker, BigQueryCredentials, ParType
 from target_bigquery.gcs_stage import BigQueryGcsStagingDenormalizedSink, BigQueryGcsStagingSink
 from target_bigquery.storage_write import (
     BigQueryStorageWriteDenormalizedSink,
     BigQueryStorageWriteSink,
@@ -295,14 +296,24 @@
                 " table during the merge transaction to dedupe the ingested records. This is useful"
                 " for streams that are not unique on the key properties during an ingest but are"
                 " unique in the source system. Data lake ingestion is often a good example of this"
                 " where the same unique record may exist in the lake at different points in time"
                 " from different extracts."
             ),
         ),
+        th.Property(
+            "schema_resolver_version",
+            th.IntegerType,
+            default=1,
+            description=(
+                "The version of the schema resolver to use. Defaults to 1. Version 2 uses JSON as a"
+                " fallback during denormalization. This only has an effect if denormalized=true"
+            ),
+            allowed_values=[1, 2],
+        ),
     ).to_dict()
 
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         self.max_parallelism = 1
         (
             self.proc_cls,
```

### Comparing `z3_target_bigquery-0.6.3/setup.py` & `z3_target_bigquery-0.6.6/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,45 +1,279 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: z3-target-bigquery
+Version: 0.6.6
+Summary: z3-target-bigquery is a Singer target for BigQuery. It supports storage write, GCS, streaming, and batch load methods. Built with the Meltano SDK.
+Home-page: https://github.com/z3z1ma/target-bigquery
+License: MIT
+Keywords: ELT,BigQuery
+Author: Alex Butler
+Author-email: butler.alex2010@gmail.com
+Requires-Python: >=3.8,<3.11
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Typing :: Typed
+Requires-Dist: google-cloud-bigquery[bqstorage] (>=3.4.1,<4)
+Requires-Dist: google-cloud-storage (>=2.7.0,<3)
+Requires-Dist: grpcio-status (>=1.51.1,<2)
+Requires-Dist: grpcio-tools (>=1.51.1,<2)
+Requires-Dist: orjson (>=3.7.2,<4)
+Requires-Dist: requests (>=2.25.1)
+Requires-Dist: singer-sdk (>=0.22.0,<0.23.0)
+Requires-Dist: tenacity (>=8.0.1,<9)
+Project-URL: Repository, https://github.com/z3z1ma/target-bigquery
+Description-Content-Type: text/markdown
 
-packages = \
-['target_bigquery', 'target_bigquery.tests']
+<h1 align="center">Target-BigQuery</h1>
 
-package_data = \
-{'': ['*']}
+<p align="center">
+<a href="https://github.com/z3z1ma/target-bigquery/actions/"><img alt="Actions Status" src="https://github.com/z3z1ma/target-bigquery/actions/workflows/ci.yml/badge.svg"></a>
+<a href="https://github.com/z3z1ma/target-bigquery/blob/main/LICENSE"><img alt="License: MIT" src="https://img.shields.io/badge/License-MIT-yellow.svg"></a>
+<a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
+</p>
 
-modules = \
-['README', 'LICENSE']
-install_requires = \
-['google-cloud-bigquery[bqstorage]>=3.4.1,<4',
- 'google-cloud-storage>=2.7.0,<3',
- 'grpcio-status>=1.51.1,<2',
- 'grpcio-tools>=1.51.1,<2',
- 'orjson>=3.7.2,<4',
- 'requests>=2.25.1',
- 'singer-sdk>=0.16.0',
- 'tenacity>=8.0.1,<9']
-
-entry_points = \
-{'console_scripts': ['target-bigquery = '
-                     'target_bigquery.target:TargetBigQuery.cli']}
-
-setup_kwargs = {
-    'name': 'z3-target-bigquery',
-    'version': '0.6.3',
-    'description': 'z3-target-bigquery is a Singer target for BigQuery. It supports storage write, GCS, streaming, and batch load methods. Built with the Meltano SDK.',
-    'long_description': '<h1 align="center">Target-BigQuery</h1>\n\n<p align="center">\n<a href="https://github.com/z3z1ma/target-bigquery/actions/"><img alt="Actions Status" src="https://github.com/z3z1ma/target-bigquery/actions/workflows/ci.yml/badge.svg"></a>\n<a href="https://github.com/z3z1ma/target-bigquery/blob/main/LICENSE"><img alt="License: MIT" src="https://img.shields.io/badge/License-MIT-yellow.svg"></a>\n<a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>\n</p>\n\n**A rare 💎 you have stumbled upon**\n\n`target-bigquery` is a Singer target for BigQuery.\n\nIt is the most versatile target for BigQuery. Extremely performant, resource efficient, and fast in all configurations enabling 20 different ingestion patterns. Denormalized variants indicate data is unpacked during load with a resultant schema in BigQuery based on the tap schema. Non-denormalized means we have a fixed schema which loads all data into an unstructured `JSON` column. They are both useful patterns. The latter allowing BigQuery to work with schemaless or rapidly changing sources such as MongoDB instantly, while the former is more performant and convenient to start modeling quickly.\n\n**Patterns** 🛠 (more details below)\n\n- Batch Job, Denormalized, Overwrite\n- Batch Job, Denormalized, Upsert\n- Batch Job, Denormalized, Append\n- Batch Job, Fixed Schema, Overwrite\n- Batch Job, Fixed Schema, Append\n- GCS Staging Data Lake, Denormalized, Overwrite\n- GCS Staging Data Lake, Denormalized, Upsert\n- GCS Staging Data Lake, Denormalized, Append\n- GCS Staging Data Lake, Fixed Schema, Overwrite\n- GCS Staging Data Lake, Fixed Schema, Append\n- Storage Write API, Denormalized, Overwrite\n- Storage Write API, Denormalized, Upsert\n- Storage Write API, Denormalized, Append\n- Storage Write API, Fixed Schema, Overwrite\n- Storage Write API, Fixed Schema, Append\n- Legacy Streaming API, Denormalized, Overwrite\n- Legacy Streaming API, Denormalized, Upsert\n- Legacy Streaming API, Denormalized, Append\n- Legacy Streaming API, Fixed Schema, Overwrite\n- Legacy Streaming API, Fixed Schema, Append\n\n## Installation 📈\n\nThe package on pypi is named `z3-target-bigquery` but the executable it ships with is simply `target-bigquery`. This allows me to release work without concerns of naming conflicts on the package index.\n\n```bash\n# Use pipx or pip\npipx install z3-target-bigquery\n# Verify it is installed\ntarget-bigquery --version\n```\n\n## Features ✨\n\n- Autoscaling self-healing worker pool using either threads (default) or multiprocessing, configurable by the user for the _fastest_ possible data ingestion. Particularly when leveraging colocated compute in GCP.\n- Denormalized load pattern where data is unpacked in flight into a statically typed BigQuery schema derived from the input stream json schemas.\n- Fix schema load pattern where all data is loaded into a `JSON` column which has been GA in BigQuery since mid 2022.\n- Autogenerated `VIEW` support for fixed schema load patterns which essentially overlays a statically typed schema allowing you to get the best of both worlds when using fixed schema ingestion.\n- JIT compilation of protobuf schemas allowing the Storage Write API to use a denormalized load pattern. \n- BATCH message support 😎\n\n## Load Patterns 🏎\n\n- `Batch Load Job` ingestion pattern using in memory compression (fixed schema + denormalized)\n- `Storage Write API` ingestion pattern using gRPC and protocol buffers supporting both streaming and batch patterns. Capable of JIT compilation of BQ schemas to protobuf to enable denormalized loads of input structures only known at runtime. (fixed schema + denormalized 🎉)\n- `GCS Staging` ingestion pattern using in memory compression and a GCS staging layer which generates a well organized data lake which backs the data warehouse providing additional failsafes and data sources (fixed schema + denormalized)\n- `Legacy Streaming` ingestion pattern which emphasizes simplicity and fast start up / tear down. I would highly recommend the storage write API instead unless data volume is small (fixed schema + denormalized)\n\n\n**Choosing between denormalized and fixed schema (JSON support)?** 🙇🏾\u200d♂️\n\nThe gap between the methods is closed due in part to the target\'s ability to  automatically generating a `VIEW` which will unpack (or rather provide typing as a more accurate take) a JSON based ingestion source for you. Unless operating at tens of millions of rows with JSON objects containing multiple hundreds of keys, its quite performant. Particularly if accessing a small subset of keys. It does however fall off (quite hard) given enough scale as I mentioned (I\'ve pushed it to the limits). Denormalized is recommended for high volume where the schema is fairly consistent. Fixed is recommended for lower volume, inconsistent schemas or for taps which are inherently schemaless in which case its the ideal (only...) logical pattern. Fixed schema can also be used for taps which routinely break down on BQ due to json schemas being inexpressible in a static way (ie patternProperties, additionalProperties...)\n\n\n**Old Header (still true, here for posterity)** 🧪\n\nThis is the first truly unstructured sink for BigQuery leveraging the recent GA feature in BigQuery for JSON support. This allows this target to load from essentially any tap regardless of the quality or explicitness of its jsonschema. Observations in existing taps note things such as `patternProperties` used in jsonschema objects which break down on all existing BigQuery taps due to the previous need for strong typing. Also taps such as MongoDB which inherently deal with unstructured data are seamlessly enabled by this target without klutzy collection scraping of a sample of records which we _hope_ are repesentative of all documents.\n\n\nBuilt with the [Meltano Target SDK](https://sdk.meltano.com).\n\n\n## Configuration 🔨\n\n### Settings\n\nFirst a valid example to give context to the below including a nested key example (denoted via a `.` in the setting path) as seen with `column_name_transforms.snake_case`\n\n```json\n{\n    "project": "my-bq-project",\n    "method": "storage_write_api",\n    "denormalized": true,\n    "credentials_path": "...",\n    "dataset": "my_dataset",\n    "location": "us-central1",\n    "batch_size": 500,\n    "column_name_transforms": {\n      "snake_case": true\n    }\n}\n```\n\n\n| Setting                                            | Required |      Default      | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |\n|:---------------------------------------------------|:--------:|:-----------------:|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|\n| credentials_path                                   |  False   |       None        | The path to a gcp credentials json file. |\n| credentials_json                                   |  False   |       None        | A JSON string of your service account JSON file. |\n| project                                            |   True   |       None        | The target GCP project to materialize data into. |\n| dataset                                            |   True   |       None        | The target dataset to materialize data into. |\n| location                                           |  False   |        US         | The target dataset location to materialize data into. Applies also to the GCS bucket if using `gcs_stage` load method. |\n| batch_size                                         |  False   |        500        | The maximum number of rows to send in a single batch to the worker. This should be configured based on load method. For `storage_write_api` and `streaming_insert` it should be `<=500`, for the LoadJob sinks, it can be much higher, ie `>100,000` |\n| timeout                                            |  False   |        600        | Default timeout for batch_job and gcs_stage derived LoadJobs. |\n| fail_fast                                          |  False   |        True       | Fail the entire load job if any row fails to insert. |\n| denormalized                                       |  False   |       False       | Determines whether to denormalize the data before writing to BigQuery. A false value will write data using a fixed JSON column based schema, while a true value will write data using a dynamic schema derived from the tap. |\n| method                                             |   True   | storage_write_api | The method to use for writing to BigQuery. Must be one of `batch_job`, `storage_write_api`, `gcs_stage`, `streaming_insert` |\n| generate_view                                      |  False   |       False       | Determines whether to generate a view based on the SCHEMA message parsed from the tap. Only valid if denormalized=false meaning you are using the fixed JSON column based schema. |\n| upsert                                             |  False   |       False       | Determines if we should upsert. Defaults to false. A value of true will write to a temporary table and then merge into the target table (upsert). This requires the target table to be unique on the key properties. A value of false will write to the target table directly (append). A value of an array of strings will evaluate the strings in order using fnmatch. At the end of the array, the value of the last match will be used. If not matched, the default value is false (append). |\n| overwrite                                          |  False   |       False       | Determines if the target table should be overwritten on load. Defaults to false. A value of true will write to a temporary table and then overwrite the target table inside a transaction (so it is safe). A value of false will write to the target table directly (append). A value of an array of strings will evaluate the strings in order using fnmatch. At the end of the array, the value of the last match will be used. If not matched, the default value is false. This is mutually exclusive with the `upsert` option. If both are set, `upsert` will take precedence. |\n| dedupe_before_upsert                               |  False   |       False       | This option is only used if `upsert` is enabled for a stream. The selection criteria for the stream\'s candidacy is the same as upsert. If the stream is marked for deduping before upsert, we will create a _session scoped temporary table during the merge transaction to dedupe the ingested records. This is useful for streams that are not unique on the key properties during an ingest but are unique in the source system. Data lake ingestion is often a good example of this where the same unique record may exist in the lake at different points in time from different extracts. |\n| bucket                                             |  False   |       None        | The GCS bucket to use for staging data. Only used if method is gcs_stage. |\n| cluster_on_key_properties                          |  False   |         0         | Determines whether to cluster on the key properties from the tap. Defaults to false. When false, clustering will be based on _sdc_batched_at instead. |\n| partition_granularity                              |  False   |      "month"      | Indicates the granularity of the created table partitioning scheme which is based on `_sdc_batched_at`. By default the granularity is monthly. Must be one of: "hour", "day", "month", "year". |\n| column_name_transforms.lower                       |  False   |       None        | Lowercase column names. |\n| column_name_transforms.quote                       |  False   |       None        | Quote column names in any generated DDL. |\n| column_name_transforms.add_underscore_when_invalid |  False   |       None        | Add an underscore to the column name if it starts with a digit to make it valid. |\n| column_name_transforms.snake_case                  |  False   |       None        | Snake case all incoming column names. Does not apply to fixed schema loads but _does_ apply to the view auto-generated over them. |\n| options.storage_write_batch_mode                   |  False   |       None        | By default, we use the default stream (Committed mode) in the [storage_write_api](https://cloud.google.com/bigquery/docs/write-api) load method which results in streaming records which are immediately available and is generally fastest. If this is set to true, we will use the application created streams (pending mode) to transactionally batch data on STATE messages and at end of pipe. |\n| options.process_pool                               |  False   |       None        | By default we use an autoscaling threadpool to write to BigQuery. If set to true, we will use a process pool. |\n| options.max_workers                                |  False   |       None        | By default, each sink type has a preconfigured max worker pool limit. This sets an override for maximum number of workers in the pool. |\n| stream_maps                                        |  False   |       None        | Config object for stream maps capability. For more information check out [Stream Maps](https://sdk.meltano.com/en/latest/stream_maps.html). |\n| stream_map_config                                  |  False   |       None        | User-defined config values to be used within map expressions. |\n| flattening_enabled                                 |  False   |       None        | \'True\' to enable schema flattening and automatically expand nested properties. |\n| flattening_max_depth                               |  False   |       None        | The max depth to flatten schemas. |\n\nA full list of supported settings and capabilities is available by running: `target-bigquery --about`\n\n### Configure using environment variables ✏️\n\nThis Singer target will automatically import any environment variables within the working directory\'s\n`.env` if the `--config=ENV` is provided, such that config values will be considered if a matching\nenvironment variable is set either in the terminal context or in the `.env` file.\n\n### Source Authentication and Authorization 👮🏽\u200d♂️\n\nAuthenticate via service account key file or Application Default Credentials (ADC)\nhttps://cloud.google.com/bigquery/docs/authentication\n\n## Capabilities ✨\n\n* `about`\n* `stream-maps`\n* `schema-flattening`\n* `batch`\n\n## Usage 👷\u200d♀️\n\nYou can easily run `target-bigquery` by itself or in a pipeline using [Meltano](https://meltano.com/).\n\n\n### Executing the Target Directly 🚧\n\n```bash\ntarget-bigquery --version\ntarget-bigquery --help\n# Test using the "Carbon Intensity" sample:\ntap-carbon-intensity | target-bigquery --config /path/to/target-bigquery-config.json\n```\n\n## Developer Resources 👩🏼\u200d💻\n\n\n### Initialize your Development Environment\n\n```bash\npipx install poetry\npoetry install\n```\n\n### Create and Run Tests\n\nCreate tests within the `target_bigquery/tests` subfolder and\n  then run:\n\n```bash\npoetry run pytest\n```\n\nYou can also test the `target-bigquery` CLI interface directly using `poetry run`:\n\n```bash\npoetry run target-bigquery --help\n```\n\n### Testing with [Meltano](https://meltano.com/)\n\n_**Note:** This target will work in any Singer environment and does not require Meltano.\nExamples here are for convenience and to streamline end-to-end orchestration scenarios._\n\nNext, install Meltano (if you haven\'t already) and any needed plugins:\n\n```bash\n# Install meltano\npipx install meltano\n# Initialize meltano within this directory\ncd target-bigquery\nmeltano install\n```\n\nNow you can test and orchestrate using Meltano:\n\n```bash\n# Test invocation:\nmeltano invoke target-bigquery --version\n# OR run a test `elt` pipeline with the Carbon Intensity sample tap:\nmeltano elt tap-carbon-intensity target-bigquery\n```\n\n### SDK Dev Guide\n\nSee the [dev guide](https://sdk.meltano.com/en/latest/dev_guide.html) for more instructions on how to use the Meltano SDK to\ndevelop your own Singer taps and targets.\n',
-    'author': 'Alex Butler',
-    'author_email': 'butler.alex2010@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/z3z1ma/target-bigquery',
-    'packages': packages,
-    'package_data': package_data,
-    'py_modules': modules,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<3.11',
+**A rare 💎 you have stumbled upon**
+
+`target-bigquery` is a Singer target for BigQuery.
+
+It is the most versatile target for BigQuery. Extremely performant, resource efficient, and fast in all configurations enabling 20 different ingestion patterns. Denormalized variants indicate data is unpacked during load with a resultant schema in BigQuery based on the tap schema. Non-denormalized means we have a fixed schema which loads all data into an unstructured `JSON` column. They are both useful patterns. The latter allowing BigQuery to work with schemaless or rapidly changing sources such as MongoDB instantly, while the former is more performant and convenient to start modeling quickly.
+
+**Patterns** 🛠 (more details below)
+
+- Batch Job, Denormalized, Overwrite
+- Batch Job, Denormalized, Upsert
+- Batch Job, Denormalized, Append
+- Batch Job, Fixed Schema, Overwrite
+- Batch Job, Fixed Schema, Append
+- GCS Staging Data Lake, Denormalized, Overwrite
+- GCS Staging Data Lake, Denormalized, Upsert
+- GCS Staging Data Lake, Denormalized, Append
+- GCS Staging Data Lake, Fixed Schema, Overwrite
+- GCS Staging Data Lake, Fixed Schema, Append
+- Storage Write API, Denormalized, Overwrite
+- Storage Write API, Denormalized, Upsert
+- Storage Write API, Denormalized, Append
+- Storage Write API, Fixed Schema, Overwrite
+- Storage Write API, Fixed Schema, Append
+- Legacy Streaming API, Denormalized, Overwrite
+- Legacy Streaming API, Denormalized, Upsert
+- Legacy Streaming API, Denormalized, Append
+- Legacy Streaming API, Fixed Schema, Overwrite
+- Legacy Streaming API, Fixed Schema, Append
+
+## Installation 📈
+
+The package on pypi is named `z3-target-bigquery` but the executable it ships with is simply `target-bigquery`. This allows me to release work without concerns of naming conflicts on the package index.
+
+```bash
+# Use pipx or pip
+pipx install z3-target-bigquery
+# Verify it is installed
+target-bigquery --version
+```
+
+## Usage Notes
+
+### Denormalization
+
+So denormalized is a loaded term, so lets clarify here what we mean by it:
+
+> In the context of JSON objects, denormalization refers to the process of flattening a hierarchical or nested JSON object into a simpler, more "denormalized" structure that can be easier to work with for certain use cases.
+
+Denormalized=False (default) means we load all data into a single `JSON` column. This means all access requires an accessor such as `SELECT data.my_column FROM table` instead of `SELECT my_column FROM table`. Hence the term denormalized is relative to the `data` column which is the default for this target. This is a tradeoff between convenience/resilience and performance. This is the default because most _resilient_. IE a load will **never** fail due to a schema change or an invalid schema. You can always denormalize later via `dbt`. However, it is not the most performant and slower to transform. If your tap has a high quality and consistent schema, denormalization is the way to go to get the best performance and start modeling quickly.
+
+Denormalized=True means we unpack the data into a schema which is derived from the tap schema. It does _not_ mean we will flatten the data. There is a separate option for flattening. We will convert arrays to repeated fields and records to structs. All top level keys will end up as columns which is was you might expect from more typical targets.
+
+#### Resolver Versions
+
+There are 2 resolver versions. The config option `schema_resolver_version` lets you select which version you want to use. This versioning exists because we want to support evolving how we resolve schemas whilst not creating breaking changes for long-time users dependent on how a schema is resolved. The default is `1` which behaves very similarly to existing flavors of `target-bigquery`. It works well enough but has plenty of edge cases where it simply cannot resolve valid jsonschemas to a bq schema. The new version `2` is much more robust and will resolve most, if not all schemas due to it falling back to `JSON` when in doubt. You must opt-in to this version by setting `schema_resolver_version: 2` in your config. 
+
+### Overwrite vs Append
+
+Sometimes you want to overwrite a table on every load. This can be achieved by either setting `overwrite: true` which will full refresh ALL tables **or** setting `overwrite: [table1, table2, table_*_other, !table_v1_other]` which will only overwrite the specified tables and supports pattern matching. This is useful if you have a table which is a lookup table and you want to overwrite it on every load. You can also set `overwrite: false` which will append to the table. This is the default behavior.
+
+### Upsert (aka Merge)
+
+If you want to merge data into a table, you can set `merge: true` which will use the `MERGE` statement to upsert data. This supports pattern matching like the above setting. It requires `denormalized: true` takes precedence over `overwrite`. It will only work on tables which have a primary key as defined by the `key_properties` sent by the tap. There is a supporting config option called `dedupe_before_upsert` which will dedupe the data before upserting. This is useful if you are replicating data which has a primary key but is not unique. This occurs when you are replicating data from a source which has a primary key but does not enforce it. This is the case for MongoDB. It can also happen when moving data from a data lake in S3/GCS to a database. This is not the default behavior because it is slower and requires more resources.
+
+## Features ✨
+
+- Autoscaling self-healing worker pool using either threads (default) or multiprocessing, configurable by the user for the _fastest_ possible data ingestion. Particularly when leveraging colocated compute in GCP.
+- Denormalized load pattern where data is unpacked in flight into a statically typed BigQuery schema derived from the input stream json schemas.
+- Fix schema load pattern where all data is loaded into a `JSON` column which has been GA in BigQuery since mid 2022.
+- Autogenerated `VIEW` support for fixed schema load patterns which essentially overlays a statically typed schema allowing you to get the best of both worlds when using fixed schema ingestion.
+- JIT compilation of protobuf schemas allowing the Storage Write API to use a denormalized load pattern. 
+- BATCH message support 😎
+
+## Load Patterns 🏎
+
+- `Batch Load Job` ingestion pattern using in memory compression (fixed schema + denormalized)
+- `Storage Write API` ingestion pattern using gRPC and protocol buffers supporting both streaming and batch patterns. Capable of JIT compilation of BQ schemas to protobuf to enable denormalized loads of input structures only known at runtime. (fixed schema + denormalized 🎉)
+- `GCS Staging` ingestion pattern using in memory compression and a GCS staging layer which generates a well organized data lake which backs the data warehouse providing additional failsafes and data sources (fixed schema + denormalized)
+- `Legacy Streaming` ingestion pattern which emphasizes simplicity and fast start up / tear down. I would highly recommend the storage write API instead unless data volume is small (fixed schema + denormalized)
+
+
+**Choosing between denormalized and fixed schema (JSON support)?** 🙇🏾‍♂️
+
+The gap between the methods is closed due in part to the target's ability to  automatically generating a `VIEW` which will unpack (or rather provide typing as a more accurate take) a JSON based ingestion source for you. Unless operating at tens of millions of rows with JSON objects containing multiple hundreds of keys, its quite performant. Particularly if accessing a small subset of keys. It does however fall off (quite hard) given enough scale as I mentioned (I've pushed it to the limits). Denormalized is recommended for high volume where the schema is fairly consistent. Fixed is recommended for lower volume, inconsistent schemas or for taps which are inherently schemaless in which case its the ideal (only...) logical pattern. Fixed schema can also be used for taps which routinely break down on BQ due to json schemas being inexpressible in a static way (ie patternProperties, additionalProperties...)
+
+
+**Old Header (still true, here for posterity)** 🧪
+
+This is the first truly unstructured sink for BigQuery leveraging the recent GA feature in BigQuery for JSON support. This allows this target to load from essentially any tap regardless of the quality or explicitness of its jsonschema. Observations in existing taps note things such as `patternProperties` used in jsonschema objects which break down on all existing BigQuery taps due to the previous need for strong typing. Also taps such as MongoDB which inherently deal with unstructured data are seamlessly enabled by this target without klutzy collection scraping of a sample of records which we _hope_ are repesentative of all documents.
+
+
+Built with the [Meltano Target SDK](https://sdk.meltano.com).
+
+
+## Configuration 🔨
+
+### Settings
+
+First a valid example to give context to the below including a nested key example (denoted via a `.` in the setting path) as seen with `column_name_transforms.snake_case`
+
+```json
+{
+    "project": "my-bq-project",
+    "method": "storage_write_api",
+    "denormalized": true,
+    "credentials_path": "...",
+    "dataset": "my_dataset",
+    "location": "us-central1",
+    "batch_size": 500,
+    "column_name_transforms": {
+      "snake_case": true
+    }
 }
+```
+
+
+| Setting                                            | Required |      Default      | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
+|:---------------------------------------------------|:--------:|:-----------------:|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| credentials_path                                   |  False   |       None        | The path to a gcp credentials json file. |
+| credentials_json                                   |  False   |       None        | A JSON string of your service account JSON file. |
+| project                                            |   True   |       None        | The target GCP project to materialize data into. |
+| dataset                                            |   True   |       None        | The target dataset to materialize data into. |
+| location                                           |  False   |        US         | The target dataset location to materialize data into. Applies also to the GCS bucket if using `gcs_stage` load method. |
+| batch_size                                         |  False   |        500        | The maximum number of rows to send in a single batch to the worker. This should be configured based on load method. For `storage_write_api` and `streaming_insert` it should be `<=500`, for the LoadJob sinks, it can be much higher, ie `>100,000` |
+| timeout                                            |  False   |        600        | Default timeout for batch_job and gcs_stage derived LoadJobs. |
+| fail_fast                                          |  False   |        True       | Fail the entire load job if any row fails to insert. |
+| denormalized                                       |  False   |       False       | Determines whether to denormalize the data before writing to BigQuery. A false value will write data using a fixed JSON column based schema, while a true value will write data using a dynamic schema derived from the tap. |
+| method                                             |   True   | storage_write_api | The method to use for writing to BigQuery. Must be one of `batch_job`, `storage_write_api`, `gcs_stage`, `streaming_insert` |
+| generate_view                                      |  False   |       False       | Determines whether to generate a view based on the SCHEMA message parsed from the tap. Only valid if denormalized=false meaning you are using the fixed JSON column based schema. |
+| upsert                                             |  False   |       False       | Determines if we should upsert. Defaults to false. A value of true will write to a temporary table and then merge into the target table (upsert). This requires the target table to be unique on the key properties. A value of false will write to the target table directly (append). A value of an array of strings will evaluate the strings in order using fnmatch. At the end of the array, the value of the last match will be used. If not matched, the default value is false (append). |
+| overwrite                                          |  False   |       False       | Determines if the target table should be overwritten on load. Defaults to false. A value of true will write to a temporary table and then overwrite the target table inside a transaction (so it is safe). A value of false will write to the target table directly (append). A value of an array of strings will evaluate the strings in order using fnmatch. At the end of the array, the value of the last match will be used. If not matched, the default value is false. This is mutually exclusive with the `upsert` option. If both are set, `upsert` will take precedence. |
+| dedupe_before_upsert                               |  False   |       False       | This option is only used if `upsert` is enabled for a stream. The selection criteria for the stream's candidacy is the same as upsert. If the stream is marked for deduping before upsert, we will create a _session scoped temporary table during the merge transaction to dedupe the ingested records. This is useful for streams that are not unique on the key properties during an ingest but are unique in the source system. Data lake ingestion is often a good example of this where the same unique record may exist in the lake at different points in time from different extracts. |
+| bucket                                             |  False   |       None        | The GCS bucket to use for staging data. Only used if method is gcs_stage. |
+| cluster_on_key_properties                          |  False   |         0         | Determines whether to cluster on the key properties from the tap. Defaults to false. When false, clustering will be based on _sdc_batched_at instead. |
+| partition_granularity                              |  False   |      "month"      | Indicates the granularity of the created table partitioning scheme which is based on `_sdc_batched_at`. By default the granularity is monthly. Must be one of: "hour", "day", "month", "year". |
+| column_name_transforms.lower                       |  False   |       None        | Lowercase column names. |
+| column_name_transforms.quote                       |  False   |       None        | Quote column names in any generated DDL. |
+| column_name_transforms.add_underscore_when_invalid |  False   |       None        | Add an underscore to the column name if it starts with a digit to make it valid. |
+| column_name_transforms.snake_case                  |  False   |       None        | Snake case all incoming column names. Does not apply to fixed schema loads but _does_ apply to the view auto-generated over them. |
+| options.storage_write_batch_mode                   |  False   |       None        | By default, we use the default stream (Committed mode) in the [storage_write_api](https://cloud.google.com/bigquery/docs/write-api) load method which results in streaming records which are immediately available and is generally fastest. If this is set to true, we will use the application created streams (pending mode) to transactionally batch data on STATE messages and at end of pipe. |
+| options.process_pool                               |  False   |       None        | By default we use an autoscaling threadpool to write to BigQuery. If set to true, we will use a process pool. |
+| options.max_workers                                |  False   |       None        | By default, each sink type has a preconfigured max worker pool limit. This sets an override for maximum number of workers in the pool. |
+| schema_resolver_version                            |  False   |       1           | The version of the schema resolver to use. Defaults to 1. Version 2 uses JSON as a fallback during denormalization. This only has an effect if denormalized=true |
+| stream_maps                                        |  False   |       None        | Config object for stream maps capability. For more information check out [Stream Maps](https://sdk.meltano.com/en/latest/stream_maps.html). |
+| stream_map_config                                  |  False   |       None        | User-defined config values to be used within map expressions. |
+| flattening_enabled                                 |  False   |       None        | 'True' to enable schema flattening and automatically expand nested properties. |
+| flattening_max_depth                               |  False   |       None        | The max depth to flatten schemas. |
+
+A full list of supported settings and capabilities is available by running: `target-bigquery --about`
+
+### Configure using environment variables ✏️
+
+This Singer target will automatically import any environment variables within the working directory's
+`.env` if the `--config=ENV` is provided, such that config values will be considered if a matching
+environment variable is set either in the terminal context or in the `.env` file.
+
+### Source Authentication and Authorization 👮🏽‍♂️
+
+Authenticate via service account key file or Application Default Credentials (ADC)
+https://cloud.google.com/bigquery/docs/authentication
+
+## Capabilities ✨
+
+* `about`
+* `stream-maps`
+* `schema-flattening`
+* `batch`
+
+## Usage 👷‍♀️
+
+You can easily run `target-bigquery` by itself or in a pipeline using [Meltano](https://meltano.com/).
+
+
+### Executing the Target Directly 🚧
+
+```bash
+target-bigquery --version
+target-bigquery --help
+# Test using the "Carbon Intensity" sample:
+tap-carbon-intensity | target-bigquery --config /path/to/target-bigquery-config.json
+```
+
+## Developer Resources 👩🏼‍💻
+
+
+### Initialize your Development Environment
+
+```bash
+pipx install poetry
+poetry install
+```
+
+### Create and Run Tests
+
+Create tests within the `target_bigquery/tests` subfolder and
+  then run:
+
+```bash
+poetry run pytest
+```
+
+You can also test the `target-bigquery` CLI interface directly using `poetry run`:
+
+```bash
+poetry run target-bigquery --help
+```
+
+### Testing with [Meltano](https://meltano.com/)
+
+_**Note:** This target will work in any Singer environment and does not require Meltano.
+Examples here are for convenience and to streamline end-to-end orchestration scenarios._
+
+Next, install Meltano (if you haven't already) and any needed plugins:
+
+```bash
+# Install meltano
+pipx install meltano
+# Initialize meltano within this directory
+cd target-bigquery
+meltano install
+```
+
+Now you can test and orchestrate using Meltano:
+
+```bash
+# Test invocation:
+meltano invoke target-bigquery --version
+# OR run a test `elt` pipeline with the Carbon Intensity sample tap:
+meltano elt tap-carbon-intensity target-bigquery
+```
+
+### SDK Dev Guide
 
+See the [dev guide](https://sdk.meltano.com/en/latest/dev_guide.html) for more instructions on how to use the Meltano SDK to
+develop your own Singer taps and targets.
 
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,212 +1,260 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \
-['target_bigquery', 'target_bigquery.tests'] package_data = \ {'': ['*']}
-modules = \ ['README', 'LICENSE'] install_requires = \ ['google-cloud-bigquery
-[bqstorage]>=3.4.1,<4', 'google-cloud-storage>=2.7.0,<3', 'grpcio-
-status>=1.51.1,<2', 'grpcio-tools>=1.51.1,<2', 'orjson>=3.7.2,<4',
-'requests>=2.25.1', 'singer-sdk>=0.16.0', 'tenacity>=8.0.1,<9'] entry_points =
-\ {'console_scripts': ['target-bigquery = ' 'target_bigquery.target:
-TargetBigQuery.cli']} setup_kwargs = { 'name': 'z3-target-bigquery', 'version':
-'0.6.3', 'description': 'z3-target-bigquery is a Singer target for BigQuery. It
-supports storage write, GCS, streaming, and batch load methods. Built with the
-Meltano SDK.', 'long_description': '
+Metadata-Version: 2.1 Name: z3-target-bigquery Version: 0.6.6 Summary: z3-
+target-bigquery is a Singer target for BigQuery. It supports storage write,
+GCS, streaming, and batch load methods. Built with the Meltano SDK. Home-page:
+https://github.com/z3z1ma/target-bigquery License: MIT Keywords: ELT,BigQuery
+Author: Alex Butler Author-email: butler.alex2010@gmail.com Requires-Python:
+>=3.8,<3.11 Classifier: Development Status :: 4 - Beta Classifier: Environment
+:: Console Classifier: Intended Audience :: Developers Classifier: License ::
+OSI Approved :: MIT License Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Topic :: Software
+Development :: Libraries :: Python Modules Classifier: Typing :: Typed
+Requires-Dist: google-cloud-bigquery[bqstorage] (>=3.4.1,<4) Requires-Dist:
+google-cloud-storage (>=2.7.0,<3) Requires-Dist: grpcio-status (>=1.51.1,<2)
+Requires-Dist: grpcio-tools (>=1.51.1,<2) Requires-Dist: orjson (>=3.7.2,<4)
+Requires-Dist: requests (>=2.25.1) Requires-Dist: singer-sdk (>=0.22.0,<0.23.0)
+Requires-Dist: tenacity (>=8.0.1,<9) Project-URL: Repository, https://
+github.com/z3z1ma/target-bigquery Description-Content-Type: text/markdown
                          ****** Target-BigQuery ******
-\n\n
-           \n[Actions_Status]\n[License:_MIT]\n[Code_style:_black]\n
-\n\n**A rare ð you have stumbled upon**\n\n`target-bigquery` is a Singer
-target for BigQuery.\n\nIt is the most versatile target for BigQuery. Extremely
-performant, resource efficient, and fast in all configurations enabling 20
-different ingestion patterns. Denormalized variants indicate data is unpacked
-during load with a resultant schema in BigQuery based on the tap schema. Non-
-denormalized means we have a fixed schema which loads all data into an
-unstructured `JSON` column. They are both useful patterns. The latter allowing
-BigQuery to work with schemaless or rapidly changing sources such as MongoDB
-instantly, while the former is more performant and convenient to start modeling
-quickly.\n\n**Patterns** ð  (more details below)\n\n- Batch Job,
-Denormalized, Overwrite\n- Batch Job, Denormalized, Upsert\n- Batch Job,
-Denormalized, Append\n- Batch Job, Fixed Schema, Overwrite\n- Batch Job, Fixed
-Schema, Append\n- GCS Staging Data Lake, Denormalized, Overwrite\n- GCS Staging
-Data Lake, Denormalized, Upsert\n- GCS Staging Data Lake, Denormalized,
-Append\n- GCS Staging Data Lake, Fixed Schema, Overwrite\n- GCS Staging Data
-Lake, Fixed Schema, Append\n- Storage Write API, Denormalized, Overwrite\n-
-Storage Write API, Denormalized, Upsert\n- Storage Write API, Denormalized,
-Append\n- Storage Write API, Fixed Schema, Overwrite\n- Storage Write API,
-Fixed Schema, Append\n- Legacy Streaming API, Denormalized, Overwrite\n- Legacy
-Streaming API, Denormalized, Upsert\n- Legacy Streaming API, Denormalized,
-Append\n- Legacy Streaming API, Fixed Schema, Overwrite\n- Legacy Streaming
-API, Fixed Schema, Append\n\n## Installation ð\n\nThe package on pypi is
-named `z3-target-bigquery` but the executable it ships with is simply `target-
-bigquery`. This allows me to release work without concerns of naming conflicts
-on the package index.\n\n```bash\n# Use pipx or pip\npipx install z3-target-
-bigquery\n# Verify it is installed\ntarget-bigquery --version\n```\n\n##
-Features â¨\n\n- Autoscaling self-healing worker pool using either threads
-(default) or multiprocessing, configurable by the user for the _fastest_
-possible data ingestion. Particularly when leveraging colocated compute in
-GCP.\n- Denormalized load pattern where data is unpacked in flight into a
-statically typed BigQuery schema derived from the input stream json schemas.\n-
-Fix schema load pattern where all data is loaded into a `JSON` column which has
-been GA in BigQuery since mid 2022.\n- Autogenerated `VIEW` support for fixed
-schema load patterns which essentially overlays a statically typed schema
-allowing you to get the best of both worlds when using fixed schema
-ingestion.\n- JIT compilation of protobuf schemas allowing the Storage Write
-API to use a denormalized load pattern. \n- BATCH message support ð\n\n##
-Load Patterns ð\n\n- `Batch Load Job` ingestion pattern using in memory
-compression (fixed schema + denormalized)\n- `Storage Write API` ingestion
+              [Actions_Status] [License:_MIT] [Code_style:_black]
+**A rare ð you have stumbled upon** `target-bigquery` is a Singer target for
+BigQuery. It is the most versatile target for BigQuery. Extremely performant,
+resource efficient, and fast in all configurations enabling 20 different
+ingestion patterns. Denormalized variants indicate data is unpacked during load
+with a resultant schema in BigQuery based on the tap schema. Non-denormalized
+means we have a fixed schema which loads all data into an unstructured `JSON`
+column. They are both useful patterns. The latter allowing BigQuery to work
+with schemaless or rapidly changing sources such as MongoDB instantly, while
+the former is more performant and convenient to start modeling quickly.
+**Patterns** ð  (more details below) - Batch Job, Denormalized, Overwrite -
+Batch Job, Denormalized, Upsert - Batch Job, Denormalized, Append - Batch Job,
+Fixed Schema, Overwrite - Batch Job, Fixed Schema, Append - GCS Staging Data
+Lake, Denormalized, Overwrite - GCS Staging Data Lake, Denormalized, Upsert -
+GCS Staging Data Lake, Denormalized, Append - GCS Staging Data Lake, Fixed
+Schema, Overwrite - GCS Staging Data Lake, Fixed Schema, Append - Storage Write
+API, Denormalized, Overwrite - Storage Write API, Denormalized, Upsert -
+Storage Write API, Denormalized, Append - Storage Write API, Fixed Schema,
+Overwrite - Storage Write API, Fixed Schema, Append - Legacy Streaming API,
+Denormalized, Overwrite - Legacy Streaming API, Denormalized, Upsert - Legacy
+Streaming API, Denormalized, Append - Legacy Streaming API, Fixed Schema,
+Overwrite - Legacy Streaming API, Fixed Schema, Append ## Installation ð The
+package on pypi is named `z3-target-bigquery` but the executable it ships with
+is simply `target-bigquery`. This allows me to release work without concerns of
+naming conflicts on the package index. ```bash # Use pipx or pip pipx install
+z3-target-bigquery # Verify it is installed target-bigquery --version ``` ##
+Usage Notes ### Denormalization So denormalized is a loaded term, so lets
+clarify here what we mean by it: > In the context of JSON objects,
+denormalization refers to the process of flattening a hierarchical or nested
+JSON object into a simpler, more "denormalized" structure that can be easier to
+work with for certain use cases. Denormalized=False (default) means we load all
+data into a single `JSON` column. This means all access requires an accessor
+such as `SELECT data.my_column FROM table` instead of `SELECT my_column FROM
+table`. Hence the term denormalized is relative to the `data` column which is
+the default for this target. This is a tradeoff between convenience/resilience
+and performance. This is the default because most _resilient_. IE a load will
+**never** fail due to a schema change or an invalid schema. You can always
+denormalize later via `dbt`. However, it is not the most performant and slower
+to transform. If your tap has a high quality and consistent schema,
+denormalization is the way to go to get the best performance and start modeling
+quickly. Denormalized=True means we unpack the data into a schema which is
+derived from the tap schema. It does _not_ mean we will flatten the data. There
+is a separate option for flattening. We will convert arrays to repeated fields
+and records to structs. All top level keys will end up as columns which is was
+you might expect from more typical targets. #### Resolver Versions There are 2
+resolver versions. The config option `schema_resolver_version` lets you select
+which version you want to use. This versioning exists because we want to
+support evolving how we resolve schemas whilst not creating breaking changes
+for long-time users dependent on how a schema is resolved. The default is `1`
+which behaves very similarly to existing flavors of `target-bigquery`. It works
+well enough but has plenty of edge cases where it simply cannot resolve valid
+jsonschemas to a bq schema. The new version `2` is much more robust and will
+resolve most, if not all schemas due to it falling back to `JSON` when in
+doubt. You must opt-in to this version by setting `schema_resolver_version: 2`
+in your config. ### Overwrite vs Append Sometimes you want to overwrite a table
+on every load. This can be achieved by either setting `overwrite: true` which
+will full refresh ALL tables **or** setting `overwrite: [table1, table2,
+table_*_other, !table_v1_other]` which will only overwrite the specified tables
+and supports pattern matching. This is useful if you have a table which is a
+lookup table and you want to overwrite it on every load. You can also set
+`overwrite: false` which will append to the table. This is the default
+behavior. ### Upsert (aka Merge) If you want to merge data into a table, you
+can set `merge: true` which will use the `MERGE` statement to upsert data. This
+supports pattern matching like the above setting. It requires `denormalized:
+true` takes precedence over `overwrite`. It will only work on tables which have
+a primary key as defined by the `key_properties` sent by the tap. There is a
+supporting config option called `dedupe_before_upsert` which will dedupe the
+data before upserting. This is useful if you are replicating data which has a
+primary key but is not unique. This occurs when you are replicating data from a
+source which has a primary key but does not enforce it. This is the case for
+MongoDB. It can also happen when moving data from a data lake in S3/GCS to a
+database. This is not the default behavior because it is slower and requires
+more resources. ## Features â¨ - Autoscaling self-healing worker pool using
+either threads (default) or multiprocessing, configurable by the user for the
+_fastest_ possible data ingestion. Particularly when leveraging colocated
+compute in GCP. - Denormalized load pattern where data is unpacked in flight
+into a statically typed BigQuery schema derived from the input stream json
+schemas. - Fix schema load pattern where all data is loaded into a `JSON`
+column which has been GA in BigQuery since mid 2022. - Autogenerated `VIEW`
+support for fixed schema load patterns which essentially overlays a statically
+typed schema allowing you to get the best of both worlds when using fixed
+schema ingestion. - JIT compilation of protobuf schemas allowing the Storage
+Write API to use a denormalized load pattern. - BATCH message support ð ##
+Load Patterns ð - `Batch Load Job` ingestion pattern using in memory
+compression (fixed schema + denormalized) - `Storage Write API` ingestion
 pattern using gRPC and protocol buffers supporting both streaming and batch
 patterns. Capable of JIT compilation of BQ schemas to protobuf to enable
 denormalized loads of input structures only known at runtime. (fixed schema +
-denormalized ð)\n- `GCS Staging` ingestion pattern using in memory
+denormalized ð) - `GCS Staging` ingestion pattern using in memory
 compression and a GCS staging layer which generates a well organized data lake
 which backs the data warehouse providing additional failsafes and data sources
-(fixed schema + denormalized)\n- `Legacy Streaming` ingestion pattern which
+(fixed schema + denormalized) - `Legacy Streaming` ingestion pattern which
 emphasizes simplicity and fast start up / tear down. I would highly recommend
 the storage write API instead unless data volume is small (fixed schema +
-denormalized)\n\n\n**Choosing between denormalized and fixed schema (JSON
-support)?** ðð¾\u200dâï¸\n\nThe gap between the methods is closed due
-in part to the target\'s ability to automatically generating a `VIEW` which
-will unpack (or rather provide typing as a more accurate take) a JSON based
-ingestion source for you. Unless operating at tens of millions of rows with
-JSON objects containing multiple hundreds of keys, its quite performant.
-Particularly if accessing a small subset of keys. It does however fall off
-(quite hard) given enough scale as I mentioned (I\'ve pushed it to the limits).
-Denormalized is recommended for high volume where the schema is fairly
-consistent. Fixed is recommended for lower volume, inconsistent schemas or for
-taps which are inherently schemaless in which case its the ideal (only...)
-logical pattern. Fixed schema can also be used for taps which routinely break
-down on BQ due to json schemas being inexpressible in a static way (ie
-patternProperties, additionalProperties...)\n\n\n**Old Header (still true, here
-for posterity)** ð§ª\n\nThis is the first truly unstructured sink for BigQuery
-leveraging the recent GA feature in BigQuery for JSON support. This allows this
-target to load from essentially any tap regardless of the quality or
-explicitness of its jsonschema. Observations in existing taps note things such
-as `patternProperties` used in jsonschema objects which break down on all
-existing BigQuery taps due to the previous need for strong typing. Also taps
-such as MongoDB which inherently deal with unstructured data are seamlessly
-enabled by this target without klutzy collection scraping of a sample of
-records which we _hope_ are repesentative of all documents.\n\n\nBuilt with the
-[Meltano Target SDK](https://sdk.meltano.com).\n\n\n## Configuration
-ð¨\n\n### Settings\n\nFirst a valid example to give context to the below
-including a nested key example (denoted via a `.` in the setting path) as seen
-with `column_name_transforms.snake_case`\n\n```json\n{\n "project": "my-bq-
-project",\n "method": "storage_write_api",\n "denormalized": true,\n
-"credentials_path": "...",\n "dataset": "my_dataset",\n "location": "us-
-central1",\n "batch_size": 500,\n "column_name_transforms": {\n "snake_case":
-true\n }\n}\n```\n\n\n| Setting | Required | Default | Description |\n|:-------
---------------------------------------------|:--------:|:-----------------:|:--
+denormalized) **Choosing between denormalized and fixed schema (JSON
+support)?** ðð¾ââï¸ The gap between the methods is closed due in part
+to the target's ability to automatically generating a `VIEW` which will unpack
+(or rather provide typing as a more accurate take) a JSON based ingestion
+source for you. Unless operating at tens of millions of rows with JSON objects
+containing multiple hundreds of keys, its quite performant. Particularly if
+accessing a small subset of keys. It does however fall off (quite hard) given
+enough scale as I mentioned (I've pushed it to the limits). Denormalized is
+recommended for high volume where the schema is fairly consistent. Fixed is
+recommended for lower volume, inconsistent schemas or for taps which are
+inherently schemaless in which case its the ideal (only...) logical pattern.
+Fixed schema can also be used for taps which routinely break down on BQ due to
+json schemas being inexpressible in a static way (ie patternProperties,
+additionalProperties...) **Old Header (still true, here for posterity)** ð§ª
+This is the first truly unstructured sink for BigQuery leveraging the recent GA
+feature in BigQuery for JSON support. This allows this target to load from
+essentially any tap regardless of the quality or explicitness of its
+jsonschema. Observations in existing taps note things such as
+`patternProperties` used in jsonschema objects which break down on all existing
+BigQuery taps due to the previous need for strong typing. Also taps such as
+MongoDB which inherently deal with unstructured data are seamlessly enabled by
+this target without klutzy collection scraping of a sample of records which we
+_hope_ are repesentative of all documents. Built with the [Meltano Target SDK]
+(https://sdk.meltano.com). ## Configuration ð¨ ### Settings First a valid
+example to give context to the below including a nested key example (denoted
+via a `.` in the setting path) as seen with `column_name_transforms.snake_case`
+```json { "project": "my-bq-project", "method": "storage_write_api",
+"denormalized": true, "credentials_path": "...", "dataset": "my_dataset",
+"location": "us-central1", "batch_size": 500, "column_name_transforms":
+{ "snake_case": true } } ``` | Setting | Required | Default | Description | |:-
+--------------------------------------------------|:--------:|:----------------
+-:|:---------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
--------------------------------------------------------------------------------
----------------------|\n| credentials_path | False | None | The path to a gcp
-credentials json file. |\n| credentials_json | False | None | A JSON string of
-your service account JSON file. |\n| project | True | None | The target GCP
-project to materialize data into. |\n| dataset | True | None | The target
-dataset to materialize data into. |\n| location | False | US | The target
+---------------------------| | credentials_path | False | None | The path to a
+gcp credentials json file. | | credentials_json | False | None | A JSON string
+of your service account JSON file. | | project | True | None | The target GCP
+project to materialize data into. | | dataset | True | None | The target
+dataset to materialize data into. | | location | False | US | The target
 dataset location to materialize data into. Applies also to the GCS bucket if
-using `gcs_stage` load method. |\n| batch_size | False | 500 | The maximum
+using `gcs_stage` load method. | | batch_size | False | 500 | The maximum
 number of rows to send in a single batch to the worker. This should be
 configured based on load method. For `storage_write_api` and `streaming_insert`
 it should be `<=500`, for the LoadJob sinks, it can be much higher, ie
-`>100,000` |\n| timeout | False | 600 | Default timeout for batch_job and
-gcs_stage derived LoadJobs. |\n| fail_fast | False | True | Fail the entire
-load job if any row fails to insert. |\n| denormalized | False | False |
-Determines whether to denormalize the data before writing to BigQuery. A false
-value will write data using a fixed JSON column based schema, while a true
-value will write data using a dynamic schema derived from the tap. |\n| method
-| True | storage_write_api | The method to use for writing to BigQuery. Must be
-one of `batch_job`, `storage_write_api`, `gcs_stage`, `streaming_insert` |\n|
+`>100,000` | | timeout | False | 600 | Default timeout for batch_job and
+gcs_stage derived LoadJobs. | | fail_fast | False | True | Fail the entire load
+job if any row fails to insert. | | denormalized | False | False | Determines
+whether to denormalize the data before writing to BigQuery. A false value will
+write data using a fixed JSON column based schema, while a true value will
+write data using a dynamic schema derived from the tap. | | method | True |
+storage_write_api | The method to use for writing to BigQuery. Must be one of
+`batch_job`, `storage_write_api`, `gcs_stage`, `streaming_insert` | |
 generate_view | False | False | Determines whether to generate a view based on
 the SCHEMA message parsed from the tap. Only valid if denormalized=false
-meaning you are using the fixed JSON column based schema. |\n| upsert | False |
+meaning you are using the fixed JSON column based schema. | | upsert | False |
 False | Determines if we should upsert. Defaults to false. A value of true will
 write to a temporary table and then merge into the target table (upsert). This
 requires the target table to be unique on the key properties. A value of false
 will write to the target table directly (append). A value of an array of
 strings will evaluate the strings in order using fnmatch. At the end of the
 array, the value of the last match will be used. If not matched, the default
-value is false (append). |\n| overwrite | False | False | Determines if the
+value is false (append). | | overwrite | False | False | Determines if the
 target table should be overwritten on load. Defaults to false. A value of true
 will write to a temporary table and then overwrite the target table inside a
 transaction (so it is safe). A value of false will write to the target table
 directly (append). A value of an array of strings will evaluate the strings in
 order using fnmatch. At the end of the array, the value of the last match will
 be used. If not matched, the default value is false. This is mutually exclusive
-with the `upsert` option. If both are set, `upsert` will take precedence. |\n|
+with the `upsert` option. If both are set, `upsert` will take precedence. | |
 dedupe_before_upsert | False | False | This option is only used if `upsert` is
-enabled for a stream. The selection criteria for the stream\'s candidacy is the
+enabled for a stream. The selection criteria for the stream's candidacy is the
 same as upsert. If the stream is marked for deduping before upsert, we will
 create a _session scoped temporary table during the merge transaction to dedupe
 the ingested records. This is useful for streams that are not unique on the key
 properties during an ingest but are unique in the source system. Data lake
 ingestion is often a good example of this where the same unique record may
-exist in the lake at different points in time from different extracts. |\n|
+exist in the lake at different points in time from different extracts. | |
 bucket | False | None | The GCS bucket to use for staging data. Only used if
-method is gcs_stage. |\n| cluster_on_key_properties | False | 0 | Determines
+method is gcs_stage. | | cluster_on_key_properties | False | 0 | Determines
 whether to cluster on the key properties from the tap. Defaults to false. When
-false, clustering will be based on _sdc_batched_at instead. |\n|
+false, clustering will be based on _sdc_batched_at instead. | |
 partition_granularity | False | "month" | Indicates the granularity of the
 created table partitioning scheme which is based on `_sdc_batched_at`. By
 default the granularity is monthly. Must be one of: "hour", "day", "month",
-"year". |\n| column_name_transforms.lower | False | None | Lowercase column
-names. |\n| column_name_transforms.quote | False | None | Quote column names in
-any generated DDL. |\n| column_name_transforms.add_underscore_when_invalid |
+"year". | | column_name_transforms.lower | False | None | Lowercase column
+names. | | column_name_transforms.quote | False | None | Quote column names in
+any generated DDL. | | column_name_transforms.add_underscore_when_invalid |
 False | None | Add an underscore to the column name if it starts with a digit
-to make it valid. |\n| column_name_transforms.snake_case | False | None | Snake
+to make it valid. | | column_name_transforms.snake_case | False | None | Snake
 case all incoming column names. Does not apply to fixed schema loads but _does_
-apply to the view auto-generated over them. |\n|
+apply to the view auto-generated over them. | |
 options.storage_write_batch_mode | False | None | By default, we use the
 default stream (Committed mode) in the [storage_write_api](https://
 cloud.google.com/bigquery/docs/write-api) load method which results in
 streaming records which are immediately available and is generally fastest. If
 this is set to true, we will use the application created streams (pending mode)
-to transactionally batch data on STATE messages and at end of pipe. |\n|
+to transactionally batch data on STATE messages and at end of pipe. | |
 options.process_pool | False | None | By default we use an autoscaling
-threadpool to write to BigQuery. If set to true, we will use a process pool.
-|\n| options.max_workers | False | None | By default, each sink type has a
+threadpool to write to BigQuery. If set to true, we will use a process pool. |
+| options.max_workers | False | None | By default, each sink type has a
 preconfigured max worker pool limit. This sets an override for maximum number
-of workers in the pool. |\n| stream_maps | False | None | Config object for
-stream maps capability. For more information check out [Stream Maps](https://
-sdk.meltano.com/en/latest/stream_maps.html). |\n| stream_map_config | False |
-None | User-defined config values to be used within map expressions. |\n|
-flattening_enabled | False | None | \'True\' to enable schema flattening and
-automatically expand nested properties. |\n| flattening_max_depth | False |
-None | The max depth to flatten schemas. |\n\nA full list of supported settings
-and capabilities is available by running: `target-bigquery --about`\n\n###
-Configure using environment variables âï¸\n\nThis Singer target will
-automatically import any environment variables within the working
-directory\'s\n`.env` if the `--config=ENV` is provided, such that config values
-will be considered if a matching\nenvironment variable is set either in the
-terminal context or in the `.env` file.\n\n### Source Authentication and
-Authorization ð®ð½\u200dâï¸\n\nAuthenticate via service account key file
-or Application Default Credentials (ADC)\nhttps://cloud.google.com/bigquery/
-docs/authentication\n\n## Capabilities â¨\n\n* `about`\n* `stream-maps`\n*
-`schema-flattening`\n* `batch`\n\n## Usage ð·\u200dâï¸\n\nYou can easily
-run `target-bigquery` by itself or in a pipeline using [Meltano](https://
-meltano.com/).\n\n\n### Executing the Target Directly ð§\n\n```bash\ntarget-
-bigquery --version\ntarget-bigquery --help\n# Test using the "Carbon Intensity"
-sample:\ntap-carbon-intensity | target-bigquery --config /path/to/target-
-bigquery-config.json\n```\n\n## Developer Resources ð©ð¼\u200dð»\n\n\n###
-Initialize your Development Environment\n\n```bash\npipx install poetry\npoetry
-install\n```\n\n### Create and Run Tests\n\nCreate tests within the
-`target_bigquery/tests` subfolder and\n then run:\n\n```bash\npoetry run
-pytest\n```\n\nYou can also test the `target-bigquery` CLI interface directly
-using `poetry run`:\n\n```bash\npoetry run target-bigquery --help\n```\n\n###
-Testing with [Meltano](https://meltano.com/)\n\n_**Note:** This target will
-work in any Singer environment and does not require Meltano.\nExamples here are
-for convenience and to streamline end-to-end orchestration scenarios._\n\nNext,
-install Meltano (if you haven\'t already) and any needed plugins:\n\n```bash\n#
-Install meltano\npipx install meltano\n# Initialize meltano within this
-directory\ncd target-bigquery\nmeltano install\n```\n\nNow you can test and
-orchestrate using Meltano:\n\n```bash\n# Test invocation:\nmeltano invoke
-target-bigquery --version\n# OR run a test `elt` pipeline with the Carbon
-Intensity sample tap:\nmeltano elt tap-carbon-intensity target-
-bigquery\n```\n\n### SDK Dev Guide\n\nSee the [dev guide](https://
-sdk.meltano.com/en/latest/dev_guide.html) for more instructions on how to use
-the Meltano SDK to\ndevelop your own Singer taps and targets.\n', 'author':
-'Alex Butler', 'author_email': 'butler.alex2010@gmail.com', 'maintainer':
-'None', 'maintainer_email': 'None', 'url': 'https://github.com/z3z1ma/target-
-bigquery', 'packages': packages, 'package_data': package_data, 'py_modules':
-modules, 'install_requires': install_requires, 'entry_points': entry_points,
-'python_requires': '>=3.8,<3.11', } setup(**setup_kwargs)
+of workers in the pool. | | schema_resolver_version | False | 1 | The version
+of the schema resolver to use. Defaults to 1. Version 2 uses JSON as a fallback
+during denormalization. This only has an effect if denormalized=true | |
+stream_maps | False | None | Config object for stream maps capability. For more
+information check out [Stream Maps](https://sdk.meltano.com/en/latest/
+stream_maps.html). | | stream_map_config | False | None | User-defined config
+values to be used within map expressions. | | flattening_enabled | False | None
+| 'True' to enable schema flattening and automatically expand nested
+properties. | | flattening_max_depth | False | None | The max depth to flatten
+schemas. | A full list of supported settings and capabilities is available by
+running: `target-bigquery --about` ### Configure using environment variables
+âï¸ This Singer target will automatically import any environment variables
+within the working directory's `.env` if the `--config=ENV` is provided, such
+that config values will be considered if a matching environment variable is set
+either in the terminal context or in the `.env` file. ### Source Authentication
+and Authorization ð®ð½ââï¸ Authenticate via service account key file
+or Application Default Credentials (ADC) https://cloud.google.com/bigquery/
+docs/authentication ## Capabilities â¨ * `about` * `stream-maps` * `schema-
+flattening` * `batch` ## Usage ð·ââï¸ You can easily run `target-
+bigquery` by itself or in a pipeline using [Meltano](https://meltano.com/). ###
+Executing the Target Directly ð§ ```bash target-bigquery --version target-
+bigquery --help # Test using the "Carbon Intensity" sample: tap-carbon-
+intensity | target-bigquery --config /path/to/target-bigquery-config.json ```
+## Developer Resources ð©ð¼âð» ### Initialize your Development
+Environment ```bash pipx install poetry poetry install ``` ### Create and Run
+Tests Create tests within the `target_bigquery/tests` subfolder and then run:
+```bash poetry run pytest ``` You can also test the `target-bigquery` CLI
+interface directly using `poetry run`: ```bash poetry run target-bigquery --
+help ``` ### Testing with [Meltano](https://meltano.com/) _**Note:** This
+target will work in any Singer environment and does not require Meltano.
+Examples here are for convenience and to streamline end-to-end orchestration
+scenarios._ Next, install Meltano (if you haven't already) and any needed
+plugins: ```bash # Install meltano pipx install meltano # Initialize meltano
+within this directory cd target-bigquery meltano install ``` Now you can test
+and orchestrate using Meltano: ```bash # Test invocation: meltano invoke
+target-bigquery --version # OR run a test `elt` pipeline with the Carbon
+Intensity sample tap: meltano elt tap-carbon-intensity target-bigquery ``` ###
+SDK Dev Guide See the [dev guide](https://sdk.meltano.com/en/latest/
+dev_guide.html) for more instructions on how to use the Meltano SDK to develop
+your own Singer taps and targets.
```

