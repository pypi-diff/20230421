# Comparing `tmp/openmsistream-1.3.2.tar.gz` & `tmp/openmsistream-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openmsistream-1.3.2.tar", last modified: Fri Apr 21 18:05:02 2023, max compression
+gzip compressed data, was "openmsistream-1.3.3.tar", last modified: Fri Apr 21 18:39:25 2023, max compression
```

## Comparing `openmsistream-1.3.2.tar` & `openmsistream-1.3.3.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 18:05:02.809967 openmsistream-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (122)    35148 2023-04-21 18:04:53.000000 openmsistream-1.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      116 2023-04-21 18:04:53.000000 openmsistream-1.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2191 2023-04-21 18:05:02.809967 openmsistream-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2878 2023-04-21 18:04:53.000000 openmsistream-1.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 18:05:02.801967 openmsistream-1.3.2/openmsistream/
--rw-r--r--   0 runner    (1001) docker     (122)     2085 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 18:05:02.801967 openmsistream-1.3.2/openmsistream/data_file_io/
--rw-r--r--   0 runner    (1001) docker     (122)      546 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/data_file_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 18:05:02.801967 openmsistream-1.3.2/openmsistream/data_file_io/actor/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/data_file_io/actor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7014 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/data_file_io/actor/data_file_chunk_handlers.py
--rw-r--r--   0 runner    (1001) docker     (122)     9321 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/data_file_io/actor/data_file_download_directory.py
--rw-r--r--   0 runner    (1001) docker     (122)     6431 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/data_file_io/actor/data_file_stream_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)    11858 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/data_file_io/actor/data_file_stream_processor.py
--rw-r--r--   0 runner    (1001) docker     (122)    17173 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/data_file_io/actor/data_file_stream_reproducer.py
--rw-r--r--   0 runner    (1001) docker     (122)    27293 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/data_file_io/actor/data_file_upload_directory.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 18:05:02.801967 openmsistream-1.3.2/openmsistream/data_file_io/actor/file_registry/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/data_file_io/actor/file_registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13045 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/data_file_io/actor/file_registry/producer_file_registry.py
--rw-r--r--   0 runner    (1001) docker     (122)    17858 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/data_file_io/actor/file_registry/stream_handler_registries.py
--rw-r--r--   0 runner    (1001) docker     (122)     1590 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/data_file_io/config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 18:05:02.801967 openmsistream-1.3.2/openmsistream/data_file_io/entity/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/data_file_io/entity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      542 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/data_file_io/entity/data_file.py
--rw-r--r--   0 runner    (1001) docker     (122)     9797 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/data_file_io/entity/data_file_chunk.py
--rw-r--r--   0 runner    (1001) docker     (122)      559 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/data_file_io/entity/data_file_directory.py
--rw-r--r--   0 runner    (1001) docker     (122)    10963 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/data_file_io/entity/download_data_file.py
--rw-r--r--   0 runner    (1001) docker     (122)     1749 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/data_file_io/entity/reproducer_message.py
--rw-r--r--   0 runner    (1001) docker     (122)    16756 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/data_file_io/entity/upload_data_file.py
--rw-r--r--   0 runner    (1001) docker     (122)     2073 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/data_file_io/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 18:05:02.805967 openmsistream-1.3.2/openmsistream/kafka_wrapper/
--rw-r--r--   0 runner    (1001) docker     (122)      698 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/kafka_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6249 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/kafka_wrapper/config_file_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 18:05:02.805967 openmsistream-1.3.2/openmsistream/kafka_wrapper/config_files/
--rw-r--r--   0 runner    (1001) docker     (122)      137 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/kafka_wrapper/config_files/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      447 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/kafka_wrapper/config_files/local_broker_test.config
--rw-r--r--   0 runner    (1001) docker     (122)      484 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/kafka_wrapper/config_files/local_broker_test_encrypted.config
--rw-r--r--   0 runner    (1001) docker     (122)      486 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/kafka_wrapper/config_files/local_broker_test_encrypted_2.config
--rw-r--r--   0 runner    (1001) docker     (122)      189 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/kafka_wrapper/config_files/local_broker_test_metadata_rep_consumer.config
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/kafka_wrapper/config_files/local_broker_test_s3_transfer.config
--rw-r--r--   0 runner    (1001) docker     (122)      601 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/kafka_wrapper/config_files/prod.config
--rw-r--r--   0 runner    (1001) docker     (122)      600 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/kafka_wrapper/config_files/test.config
--rw-r--r--   0 runner    (1001) docker     (122)      637 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/kafka_wrapper/config_files/test_encrypted.config
--rw-r--r--   0 runner    (1001) docker     (122)      639 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/kafka_wrapper/config_files/test_encrypted_2.config
--rw-r--r--   0 runner    (1001) docker     (122)      342 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/kafka_wrapper/config_files/test_metadata_rep_consumer.config
--rw-r--r--   0 runner    (1001) docker     (122)      714 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/kafka_wrapper/config_files/test_s3_transfer.config
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 18:05:02.805967 openmsistream-1.3.2/openmsistream/kafka_wrapper/config_files/testing_node/
--rw-r--r--   0 runner    (1001) docker     (122)     3030 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/kafka_wrapper/config_files/testing_node/testing_node.config
--rw-r--r--   0 runner    (1001) docker     (122)      105 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/kafka_wrapper/config_files/testing_node/testing_node.crypto
--rw-r--r--   0 runner    (1001) docker     (122)       36 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/kafka_wrapper/config_files/testing_node/testing_node.seed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 18:05:02.805967 openmsistream-1.3.2/openmsistream/kafka_wrapper/config_files/testing_node_2/
--rw-r--r--   0 runner    (1001) docker     (122)     1230 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/kafka_wrapper/config_files/testing_node_2/testing_node_2.config
--rw-r--r--   0 runner    (1001) docker     (122)      105 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/kafka_wrapper/config_files/testing_node_2/testing_node_2.crypto
--rw-r--r--   0 runner    (1001) docker     (122)       36 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/kafka_wrapper/config_files/testing_node_2/testing_node_2.seed
--rw-r--r--   0 runner    (1001) docker     (122)     3755 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/kafka_wrapper/consumer_and_producer_group.py
--rw-r--r--   0 runner    (1001) docker     (122)     7533 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/kafka_wrapper/consumer_group.py
--rw-r--r--   0 runner    (1001) docker     (122)     5999 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/kafka_wrapper/controlled_message_processor.py
--rw-r--r--   0 runner    (1001) docker     (122)     9280 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/kafka_wrapper/controlled_message_reproducer.py
--rw-r--r--   0 runner    (1001) docker     (122)    16995 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/kafka_wrapper/openmsistream_consumer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2849 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/kafka_wrapper/openmsistream_kafka_crypto.py
--rw-r--r--   0 runner    (1001) docker     (122)    15524 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/kafka_wrapper/openmsistream_producer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2330 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/kafka_wrapper/producer_group.py
--rw-r--r--   0 runner    (1001) docker     (122)     1407 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/kafka_wrapper/producible.py
--rw-r--r--   0 runner    (1001) docker     (122)     8894 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/kafka_wrapper/serialization.py
--rw-r--r--   0 runner    (1001) docker     (122)     2927 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/kafka_wrapper/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 18:05:02.805967 openmsistream-1.3.2/openmsistream/metadata_extraction/
--rw-r--r--   0 runner    (1001) docker     (122)      151 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/metadata_extraction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      675 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/metadata_extraction/metadata_json_message.py
--rw-r--r--   0 runner    (1001) docker     (122)     6645 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/metadata_extraction/metadata_json_reproducer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 18:05:02.805967 openmsistream-1.3.2/openmsistream/s3_buckets/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/s3_buckets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      607 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/s3_buckets/config_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (122)     1387 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/s3_buckets/s3_data_transfer.py
--rw-r--r--   0 runner    (1001) docker     (122)     4039 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/s3_buckets/s3_service.py
--rw-r--r--   0 runner    (1001) docker     (122)     6595 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/s3_buckets/s3_transfer_stream_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 18:05:02.805967 openmsistream-1.3.2/openmsistream/services/
--rw-r--r--   0 runner    (1001) docker     (122)      281 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2476 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/services/config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 18:05:02.805967 openmsistream-1.3.2/openmsistream/services/examples/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/services/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1149 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/services/examples/runnable_example.py
--rw-r--r--   0 runner    (1001) docker     (122)     1191 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/services/examples/script_example.py
--rw-r--r--   0 runner    (1001) docker     (122)     2250 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/services/install_service.py
--rw-r--r--   0 runner    (1001) docker     (122)     8319 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/services/linux_service_manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     1482 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/services/manage_service.py
--rw-r--r--   0 runner    (1001) docker     (122)    20850 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/services/service_manager_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     5051 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/services/utilities.py
--rw-r--r--   0 runner    (1001) docker     (122)    11005 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/services/windows_service_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 18:05:02.809967 openmsistream-1.3.2/openmsistream/utilities/
--rw-r--r--   0 runner    (1001) docker     (122)      917 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    18903 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/utilities/argument_parsing.py
--rw-r--r--   0 runner    (1001) docker     (122)      597 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/utilities/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     3244 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/utilities/config_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (122)     3812 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/utilities/controlled_process.py
--rw-r--r--   0 runner    (1001) docker     (122)     5774 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/utilities/controlled_process_multi_threaded.py
--rw-r--r--   0 runner    (1001) docker     (122)      993 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/utilities/controlled_process_single_thread.py
--rw-r--r--   0 runner    (1001) docker     (122)    21412 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/utilities/dataclass_table.py
--rw-r--r--   0 runner    (1001) docker     (122)     1103 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/utilities/exception_tracking_thread.py
--rw-r--r--   0 runner    (1001) docker     (122)      456 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/utilities/has_argument_parser.py
--rw-r--r--   0 runner    (1001) docker     (122)      817 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/utilities/has_arguments.py
--rw-r--r--   0 runner    (1001) docker     (122)     9121 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/utilities/logging.py
--rw-r--r--   0 runner    (1001) docker     (122)     4025 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/utilities/misc.py
--rw-r--r--   0 runner    (1001) docker     (122)     6319 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/utilities/provision_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (122)     1863 2023-04-21 18:04:53.000000 openmsistream-1.3.2/openmsistream/utilities/runnable.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 18:05:02.801967 openmsistream-1.3.2/openmsistream.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2191 2023-04-21 18:05:02.000000 openmsistream-1.3.2/openmsistream.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4861 2023-04-21 18:05:02.000000 openmsistream-1.3.2/openmsistream.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-21 18:05:02.000000 openmsistream-1.3.2/openmsistream.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      547 2023-04-21 18:05:02.000000 openmsistream-1.3.2/openmsistream.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      403 2023-04-21 18:05:02.000000 openmsistream-1.3.2/openmsistream.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       14 2023-04-21 18:05:02.000000 openmsistream-1.3.2/openmsistream.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-04-21 18:05:02.809967 openmsistream-1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     3084 2023-04-21 18:04:53.000000 openmsistream-1.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:39:25.465002 openmsistream-1.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-04-21 18:39:18.000000 openmsistream-1.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-21 18:39:18.000000 openmsistream-1.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-04-21 18:39:25.465002 openmsistream-1.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-04-21 18:39:18.000000 openmsistream-1.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:39:25.457002 openmsistream-1.3.3/openmsistream/
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:39:25.457002 openmsistream-1.3.3/openmsistream/data_file_io/
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/data_file_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:39:25.457002 openmsistream-1.3.3/openmsistream/data_file_io/actor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/data_file_io/actor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/data_file_io/actor/data_file_chunk_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9321 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/data_file_io/actor/data_file_download_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/data_file_io/actor/data_file_stream_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11858 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/data_file_io/actor/data_file_stream_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17173 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/data_file_io/actor/data_file_stream_reproducer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27293 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/data_file_io/actor/data_file_upload_directory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:39:25.457002 openmsistream-1.3.3/openmsistream/data_file_io/actor/file_registry/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/data_file_io/actor/file_registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13045 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/data_file_io/actor/file_registry/producer_file_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17858 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/data_file_io/actor/file_registry/stream_handler_registries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/data_file_io/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:39:25.457002 openmsistream-1.3.3/openmsistream/data_file_io/entity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/data_file_io/entity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/data_file_io/entity/data_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9797 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/data_file_io/entity/data_file_chunk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/data_file_io/entity/data_file_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10963 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/data_file_io/entity/download_data_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/data_file_io/entity/reproducer_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16756 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/data_file_io/entity/upload_data_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/data_file_io/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:39:25.461002 openmsistream-1.3.3/openmsistream/kafka_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/kafka_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6249 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/kafka_wrapper/config_file_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:39:25.461002 openmsistream-1.3.3/openmsistream/kafka_wrapper/config_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/kafka_wrapper/config_files/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/kafka_wrapper/config_files/local_broker_test.config
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/kafka_wrapper/config_files/local_broker_test_encrypted.config
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/kafka_wrapper/config_files/local_broker_test_encrypted_2.config
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/kafka_wrapper/config_files/local_broker_test_metadata_rep_consumer.config
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/kafka_wrapper/config_files/local_broker_test_s3_transfer.config
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/kafka_wrapper/config_files/prod.config
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/kafka_wrapper/config_files/test.config
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/kafka_wrapper/config_files/test_encrypted.config
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/kafka_wrapper/config_files/test_encrypted_2.config
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/kafka_wrapper/config_files/test_metadata_rep_consumer.config
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/kafka_wrapper/config_files/test_s3_transfer.config
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:39:25.461002 openmsistream-1.3.3/openmsistream/kafka_wrapper/config_files/testing_node/
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/kafka_wrapper/config_files/testing_node/testing_node.config
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/kafka_wrapper/config_files/testing_node/testing_node.crypto
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/kafka_wrapper/config_files/testing_node/testing_node.seed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:39:25.461002 openmsistream-1.3.3/openmsistream/kafka_wrapper/config_files/testing_node_2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/kafka_wrapper/config_files/testing_node_2/testing_node_2.config
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/kafka_wrapper/config_files/testing_node_2/testing_node_2.crypto
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/kafka_wrapper/config_files/testing_node_2/testing_node_2.seed
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/kafka_wrapper/consumer_and_producer_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7533 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/kafka_wrapper/consumer_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/kafka_wrapper/controlled_message_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9280 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/kafka_wrapper/controlled_message_reproducer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16995 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/kafka_wrapper/openmsistream_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/kafka_wrapper/openmsistream_kafka_crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15524 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/kafka_wrapper/openmsistream_producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/kafka_wrapper/producer_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/kafka_wrapper/producible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8894 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/kafka_wrapper/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/kafka_wrapper/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:39:25.461002 openmsistream-1.3.3/openmsistream/metadata_extraction/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/metadata_extraction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/metadata_extraction/metadata_json_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/metadata_extraction/metadata_json_reproducer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:39:25.461002 openmsistream-1.3.3/openmsistream/s3_buckets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/s3_buckets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/s3_buckets/config_file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/s3_buckets/s3_data_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/s3_buckets/s3_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/s3_buckets/s3_transfer_stream_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:39:25.465002 openmsistream-1.3.3/openmsistream/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/services/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:39:25.465002 openmsistream-1.3.3/openmsistream/services/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/services/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/services/examples/runnable_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/services/examples/script_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/services/install_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8319 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/services/linux_service_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/services/manage_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20850 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/services/service_manager_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/services/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11005 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/services/windows_service_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:39:25.465002 openmsistream-1.3.3/openmsistream/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18903 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/utilities/argument_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/utilities/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/utilities/config_file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/utilities/controlled_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/utilities/controlled_process_multi_threaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/utilities/controlled_process_single_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21412 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/utilities/dataclass_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/utilities/exception_tracking_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/utilities/has_argument_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/utilities/has_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9121 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/utilities/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/utilities/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6319 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/utilities/provision_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-04-21 18:39:18.000000 openmsistream-1.3.3/openmsistream/utilities/runnable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:39:25.457002 openmsistream-1.3.3/openmsistream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-04-21 18:39:25.000000 openmsistream-1.3.3/openmsistream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-04-21 18:39:25.000000 openmsistream-1.3.3/openmsistream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 18:39:25.000000 openmsistream-1.3.3/openmsistream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-21 18:39:25.000000 openmsistream-1.3.3/openmsistream.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-21 18:39:25.000000 openmsistream-1.3.3/openmsistream.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-21 18:39:25.000000 openmsistream-1.3.3/openmsistream.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-21 18:39:25.465002 openmsistream-1.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-04-21 18:39:18.000000 openmsistream-1.3.3/setup.py
```

### Comparing `openmsistream-1.3.2/LICENSE` & `openmsistream-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/PKG-INFO` & `openmsistream-1.3.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 Metadata-Version: 2.1
 Name: openmsistream
-Version: 1.3.2
+Version: 1.3.3
 Summary: Python applications for materials data streaming using Apache Kafka. Developed for Open MSI (NSF DMREF award #1921959)
 Home-page: https://github.com/openmsi/openmsistream
-Download-URL: https://github.com/openmsi/openmsistream/archive/refs/tags/v1.3.2.tar.gz
 Author: OpenMSIStream
 Author-email: openmsistream@gmail.com
 License: GNU GPLv3
+Download-URL: https://github.com/openmsi/openmsistream/archive/refs/tags/v1.3.3.tar.gz
 Keywords: data_streaming,stream_processing,apache_kafka,materials,data_science
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7,<3.10
 Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: docs
-Provides-Extra: dev
 Provides-Extra: all
+Provides-Extra: dev
+Provides-Extra: docs
+Provides-Extra: test
 License-File: LICENSE
 
 
 [![JOSS DOI](https://joss.theoj.org/papers/10.21105/joss.04896/status.svg)](https://doi.org/10.21105/joss.04896) ![PyPI](https://img.shields.io/pypi/v/openmsistream) ![License](https://img.shields.io/github/license/openmsi/openmsistream) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/openmsistream) ![GitHub Release Date](https://img.shields.io/github/release-date/openmsi/openmsistream) ![GitHub last commit](https://img.shields.io/github/last-commit/openmsi/openmsistream) ![CircleCI](https://img.shields.io/circleci/build/github/openmsi/openmsistream/main) [![Documentation Status](https://readthedocs.org/projects/openmsistream/badge/?version=latest)](https://openmsistream.readthedocs.io/en/latest/?badge=latest) [![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/PyCQA/pylint)
 
 Applications for laboratory, analysis, and computational materials data streaming using [Apache Kafka](https://kafka.apache.org/)
 
 Available on PyPI at https://pypi.org/project/openmsistream and GitHub at https://github.com/openmsi/openmsistream 
 
 Official documentation at https://openmsistream.readthedocs.io/en/latest/
 
 Developed for Open MSI (NSF DMREF award #1921959); published in the [Journal of Open Source Software](https://doi.org/10.21105/joss.04896)
+
+
```

### Comparing `openmsistream-1.3.2/README.md` & `openmsistream-1.3.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # <div align="center"> OpenMSIStream </div>
-#### <div align="center">***v1.3.2***</div>
+#### <div align="center">***v1.3.3***</div>
 
 #### <div align="center">Maggie Eminizer<sup>1</sup>, Sam Tabrisky<sup>2,3,4</sup>, Amir Sharifzadeh<sup>1</sup>, Christopher DiMarco<sup>4</sup>, Jacob M. Diamond<sup>4,6</sup>, K.T. Ramesh<sup>4</sup>, Todd C. Hufnagel<sup>4,5,6</sup>, Tyrel M. McQueen<sup>4,5,7,8</sup>, David Elbert<sup>1,4</sup></div>
 
  <div align="center"><sup>1</sup> Institute for Data Intensive Engineering and Science (IDIES), The Johns Hopkins University, Baltimore, MD, USA </div>
  <div align="center"><sup>2</sup> Department of Biology, Dartmouth College, Hanover, NH, USA </div>
  <div align="center"><sup>3</sup> Department of Computer Science, Dartmouth College, Hanover, NH, USA </div>
  <div align="center"><sup>4</sup> Hopkins Extreme Materials Institute (HEMI), The Johns Hopkins University, Baltimore, MD, USA </div>
```

### Comparing `openmsistream-1.3.2/openmsistream/__init__.py` & `openmsistream-1.3.3/openmsistream/__init__.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/data_file_io/__init__.py` & `openmsistream-1.3.3/openmsistream/data_file_io/__init__.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/data_file_io/actor/data_file_chunk_handlers.py` & `openmsistream-1.3.3/openmsistream/data_file_io/actor/data_file_chunk_handlers.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/data_file_io/actor/data_file_download_directory.py` & `openmsistream-1.3.3/openmsistream/data_file_io/actor/data_file_download_directory.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/data_file_io/actor/data_file_stream_handler.py` & `openmsistream-1.3.3/openmsistream/data_file_io/actor/data_file_stream_handler.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/data_file_io/actor/data_file_stream_processor.py` & `openmsistream-1.3.3/openmsistream/data_file_io/actor/data_file_stream_processor.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/data_file_io/actor/data_file_stream_reproducer.py` & `openmsistream-1.3.3/openmsistream/data_file_io/actor/data_file_stream_reproducer.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/data_file_io/actor/data_file_upload_directory.py` & `openmsistream-1.3.3/openmsistream/data_file_io/actor/data_file_upload_directory.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/data_file_io/actor/file_registry/producer_file_registry.py` & `openmsistream-1.3.3/openmsistream/data_file_io/actor/file_registry/producer_file_registry.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/data_file_io/actor/file_registry/stream_handler_registries.py` & `openmsistream-1.3.3/openmsistream/data_file_io/actor/file_registry/stream_handler_registries.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/data_file_io/config.py` & `openmsistream-1.3.3/openmsistream/data_file_io/config.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/data_file_io/entity/data_file.py` & `openmsistream-1.3.3/openmsistream/data_file_io/entity/data_file.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/data_file_io/entity/data_file_chunk.py` & `openmsistream-1.3.3/openmsistream/data_file_io/entity/data_file_chunk.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/data_file_io/entity/data_file_directory.py` & `openmsistream-1.3.3/openmsistream/data_file_io/entity/data_file_directory.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/data_file_io/entity/download_data_file.py` & `openmsistream-1.3.3/openmsistream/data_file_io/entity/download_data_file.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/data_file_io/entity/reproducer_message.py` & `openmsistream-1.3.3/openmsistream/data_file_io/entity/reproducer_message.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/data_file_io/entity/upload_data_file.py` & `openmsistream-1.3.3/openmsistream/data_file_io/entity/upload_data_file.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/data_file_io/utilities.py` & `openmsistream-1.3.3/openmsistream/data_file_io/utilities.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/kafka_wrapper/__init__.py` & `openmsistream-1.3.3/openmsistream/kafka_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/kafka_wrapper/config_file_parser.py` & `openmsistream-1.3.3/openmsistream/kafka_wrapper/config_file_parser.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/kafka_wrapper/config_files/local_broker_test_s3_transfer.config` & `openmsistream-1.3.3/openmsistream/kafka_wrapper/config_files/local_broker_test_s3_transfer.config`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/kafka_wrapper/config_files/prod.config` & `openmsistream-1.3.3/openmsistream/kafka_wrapper/config_files/prod.config`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/kafka_wrapper/config_files/test.config` & `openmsistream-1.3.3/openmsistream/kafka_wrapper/config_files/test.config`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/kafka_wrapper/config_files/test_encrypted.config` & `openmsistream-1.3.3/openmsistream/kafka_wrapper/config_files/test_encrypted.config`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/kafka_wrapper/config_files/test_encrypted_2.config` & `openmsistream-1.3.3/openmsistream/kafka_wrapper/config_files/test_encrypted_2.config`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/kafka_wrapper/config_files/test_s3_transfer.config` & `openmsistream-1.3.3/openmsistream/kafka_wrapper/config_files/test_s3_transfer.config`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/kafka_wrapper/config_files/testing_node/testing_node.config` & `openmsistream-1.3.3/openmsistream/kafka_wrapper/config_files/testing_node/testing_node.config`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/kafka_wrapper/config_files/testing_node_2/testing_node_2.config` & `openmsistream-1.3.3/openmsistream/kafka_wrapper/config_files/testing_node_2/testing_node_2.config`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/kafka_wrapper/consumer_and_producer_group.py` & `openmsistream-1.3.3/openmsistream/kafka_wrapper/consumer_and_producer_group.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/kafka_wrapper/consumer_group.py` & `openmsistream-1.3.3/openmsistream/kafka_wrapper/consumer_group.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/kafka_wrapper/controlled_message_processor.py` & `openmsistream-1.3.3/openmsistream/kafka_wrapper/controlled_message_processor.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/kafka_wrapper/controlled_message_reproducer.py` & `openmsistream-1.3.3/openmsistream/kafka_wrapper/controlled_message_reproducer.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/kafka_wrapper/openmsistream_consumer.py` & `openmsistream-1.3.3/openmsistream/kafka_wrapper/openmsistream_consumer.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/kafka_wrapper/openmsistream_kafka_crypto.py` & `openmsistream-1.3.3/openmsistream/kafka_wrapper/openmsistream_kafka_crypto.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/kafka_wrapper/openmsistream_producer.py` & `openmsistream-1.3.3/openmsistream/kafka_wrapper/openmsistream_producer.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/kafka_wrapper/producer_group.py` & `openmsistream-1.3.3/openmsistream/kafka_wrapper/producer_group.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/kafka_wrapper/producible.py` & `openmsistream-1.3.3/openmsistream/kafka_wrapper/producible.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/kafka_wrapper/serialization.py` & `openmsistream-1.3.3/openmsistream/kafka_wrapper/serialization.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/kafka_wrapper/utilities.py` & `openmsistream-1.3.3/openmsistream/kafka_wrapper/utilities.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/metadata_extraction/metadata_json_message.py` & `openmsistream-1.3.3/openmsistream/metadata_extraction/metadata_json_message.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/metadata_extraction/metadata_json_reproducer.py` & `openmsistream-1.3.3/openmsistream/metadata_extraction/metadata_json_reproducer.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/s3_buckets/config_file_parser.py` & `openmsistream-1.3.3/openmsistream/s3_buckets/config_file_parser.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/s3_buckets/s3_data_transfer.py` & `openmsistream-1.3.3/openmsistream/s3_buckets/s3_data_transfer.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/s3_buckets/s3_service.py` & `openmsistream-1.3.3/openmsistream/s3_buckets/s3_service.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/s3_buckets/s3_transfer_stream_processor.py` & `openmsistream-1.3.3/openmsistream/s3_buckets/s3_transfer_stream_processor.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/services/config.py` & `openmsistream-1.3.3/openmsistream/services/config.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/services/examples/runnable_example.py` & `openmsistream-1.3.3/openmsistream/services/examples/runnable_example.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/services/examples/script_example.py` & `openmsistream-1.3.3/openmsistream/services/examples/script_example.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/services/install_service.py` & `openmsistream-1.3.3/openmsistream/services/install_service.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/services/linux_service_manager.py` & `openmsistream-1.3.3/openmsistream/services/linux_service_manager.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/services/manage_service.py` & `openmsistream-1.3.3/openmsistream/services/manage_service.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/services/service_manager_base.py` & `openmsistream-1.3.3/openmsistream/services/service_manager_base.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/services/utilities.py` & `openmsistream-1.3.3/openmsistream/services/utilities.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/services/windows_service_manager.py` & `openmsistream-1.3.3/openmsistream/services/windows_service_manager.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/utilities/__init__.py` & `openmsistream-1.3.3/openmsistream/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/utilities/argument_parsing.py` & `openmsistream-1.3.3/openmsistream/utilities/argument_parsing.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/utilities/config.py` & `openmsistream-1.3.3/openmsistream/utilities/config.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/utilities/config_file_parser.py` & `openmsistream-1.3.3/openmsistream/utilities/config_file_parser.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/utilities/controlled_process.py` & `openmsistream-1.3.3/openmsistream/utilities/controlled_process.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/utilities/controlled_process_multi_threaded.py` & `openmsistream-1.3.3/openmsistream/utilities/controlled_process_multi_threaded.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/utilities/controlled_process_single_thread.py` & `openmsistream-1.3.3/openmsistream/utilities/controlled_process_single_thread.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/utilities/dataclass_table.py` & `openmsistream-1.3.3/openmsistream/utilities/dataclass_table.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/utilities/exception_tracking_thread.py` & `openmsistream-1.3.3/openmsistream/utilities/exception_tracking_thread.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/utilities/has_arguments.py` & `openmsistream-1.3.3/openmsistream/utilities/has_arguments.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/utilities/logging.py` & `openmsistream-1.3.3/openmsistream/utilities/logging.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/utilities/misc.py` & `openmsistream-1.3.3/openmsistream/utilities/misc.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/utilities/provision_wrapper.py` & `openmsistream-1.3.3/openmsistream/utilities/provision_wrapper.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream/utilities/runnable.py` & `openmsistream-1.3.3/openmsistream/utilities/runnable.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream.egg-info/PKG-INFO` & `openmsistream-1.3.3/openmsistream.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 Metadata-Version: 2.1
 Name: openmsistream
-Version: 1.3.2
+Version: 1.3.3
 Summary: Python applications for materials data streaming using Apache Kafka. Developed for Open MSI (NSF DMREF award #1921959)
 Home-page: https://github.com/openmsi/openmsistream
-Download-URL: https://github.com/openmsi/openmsistream/archive/refs/tags/v1.3.2.tar.gz
 Author: OpenMSIStream
 Author-email: openmsistream@gmail.com
 License: GNU GPLv3
+Download-URL: https://github.com/openmsi/openmsistream/archive/refs/tags/v1.3.3.tar.gz
 Keywords: data_streaming,stream_processing,apache_kafka,materials,data_science
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7,<3.10
 Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: docs
-Provides-Extra: dev
 Provides-Extra: all
+Provides-Extra: dev
+Provides-Extra: docs
+Provides-Extra: test
 License-File: LICENSE
 
 
 [![JOSS DOI](https://joss.theoj.org/papers/10.21105/joss.04896/status.svg)](https://doi.org/10.21105/joss.04896) ![PyPI](https://img.shields.io/pypi/v/openmsistream) ![License](https://img.shields.io/github/license/openmsi/openmsistream) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/openmsistream) ![GitHub Release Date](https://img.shields.io/github/release-date/openmsi/openmsistream) ![GitHub last commit](https://img.shields.io/github/last-commit/openmsi/openmsistream) ![CircleCI](https://img.shields.io/circleci/build/github/openmsi/openmsistream/main) [![Documentation Status](https://readthedocs.org/projects/openmsistream/badge/?version=latest)](https://openmsistream.readthedocs.io/en/latest/?badge=latest) [![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/PyCQA/pylint)
 
 Applications for laboratory, analysis, and computational materials data streaming using [Apache Kafka](https://kafka.apache.org/)
 
 Available on PyPI at https://pypi.org/project/openmsistream and GitHub at https://github.com/openmsi/openmsistream 
 
 Official documentation at https://openmsistream.readthedocs.io/en/latest/
 
 Developed for Open MSI (NSF DMREF award #1921959); published in the [Journal of Open Source Software](https://doi.org/10.21105/joss.04896)
+
+
```

### Comparing `openmsistream-1.3.2/openmsistream.egg-info/SOURCES.txt` & `openmsistream-1.3.3/openmsistream.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.2/openmsistream.egg-info/entry_points.txt` & `openmsistream-1.3.3/openmsistream.egg-info/entry_points.txt`

 * *Files 0% similar despite different names*

```diff
@@ -2,7 +2,8 @@
 DataFileDownloadDirectory = openmsistream.data_file_io.actor.data_file_download_directory:main
 DataFileUploadDirectory = openmsistream.data_file_io.actor.data_file_upload_directory:main
 InstallService = openmsistream.services.install_service:main
 ManageService = openmsistream.services.manage_service:main
 ProvisionNode = openmsistream.utilities.provision_wrapper:main
 S3TransferStreamProcessor = openmsistream.s3_buckets.s3_transfer_stream_processor:main
 UploadDataFile = openmsistream.data_file_io.entity.upload_data_file:main
+
```

### Comparing `openmsistream-1.3.2/setup.py` & `openmsistream-1.3.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #imports
 import setuptools
 
 #version tag
-version = '1.3.2'
+version = '1.3.3'
 
 long_description = ''
 with open('README.md', 'r') as readme :
     for il,line in enumerate(readme.readlines(),start=1) :
         if il>=18 :
             long_description+=line
```

