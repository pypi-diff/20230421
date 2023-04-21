# Comparing `tmp/ucam-identitylib-1.4.0.tar.gz` & `tmp/ucam-identitylib-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ucam-identitylib-1.4.0.tar", last modified: Wed Apr  5 16:01:05 2023, max compression
+gzip compressed data, was "ucam-identitylib-1.5.0.tar", last modified: Fri Apr 21 08:32:42 2023, max compression
```

## Comparing `ucam-identitylib-1.4.0.tar` & `ucam-identitylib-1.5.0.tar`

### file list

```diff
@@ -1,265 +1,268 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 16:01:05.449025 ucam-identitylib-1.4.0/
--rw-rw-rw-   0 root         (0) root         (0)       25 2023-03-30 12:21:35.000000 ucam-identitylib-1.4.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2699 2023-04-05 16:01:05.449025 ucam-identitylib-1.4.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2002 2023-03-30 12:21:35.000000 ucam-identitylib-1.4.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 16:01:05.381022 ucam-identitylib-1.4.0/identitylib/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-05 16:00:53.000000 ucam-identitylib-1.4.0/identitylib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2516 2023-03-30 12:21:35.000000 ucam-identitylib-1.4.0/identitylib/api_client_mixin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 16:01:05.381022 ucam-identitylib-1.4.0/identitylib/card_client/
--rw-r--r--   0 root         (0) root         (0)     8516 2023-04-05 16:00:36.000000 ucam-identitylib-1.4.0/identitylib/card_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 16:01:05.385022 ucam-identitylib-1.4.0/identitylib/card_client/api/
--rw-r--r--   0 root         (0) root         (0)      231 2023-04-05 16:00:36.000000 ucam-identitylib-1.4.0/identitylib/card_client/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13392 2023-04-05 16:00:36.000000 ucam-identitylib-1.4.0/identitylib/card_client/api/permissions_api.py
--rw-r--r--   0 root         (0) root         (0)   217309 2023-04-05 16:00:36.000000 ucam-identitylib-1.4.0/identitylib/card_client/api/v1beta1_api.py
--rw-r--r--   0 root         (0) root         (0)    13297 2023-04-05 16:00:36.000000 ucam-identitylib-1.4.0/identitylib/card_client/api/versions_api.py
--rw-r--r--   0 root         (0) root         (0)    46930 2023-04-05 16:00:36.000000 ucam-identitylib-1.4.0/identitylib/card_client/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 16:01:05.385022 ucam-identitylib-1.4.0/identitylib/card_client/apis/
--rw-r--r--   0 root         (0) root         (0)      643 2023-04-05 16:00:36.000000 ucam-identitylib-1.4.0/identitylib/card_client/apis/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24525 2023-04-05 16:00:36.000000 ucam-identitylib-1.4.0/identitylib/card_client/configuration.py
--rw-r--r--   0 root         (0) root         (0)    12776 2023-04-05 16:00:36.000000 ucam-identitylib-1.4.0/identitylib/card_client/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 16:01:05.401023 ucam-identitylib-1.4.0/identitylib/card_client/model/
--rw-r--r--   0 root         (0) root         (0)      357 2023-04-05 16:00:36.000000 ucam-identitylib-1.4.0/identitylib/card_client/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19212 2023-04-05 16:00:34.000000 ucam-identitylib-1.4.0/identitylib/card_client/model/api_exception.py
--rw-r--r--   0 root         (0) root         (0)    19855 2023-04-05 16:00:34.000000 ucam-identitylib-1.4.0/identitylib/card_client/model/available_barcode.py
--rw-r--r--   0 root         (0) root         (0)    19301 2023-04-05 16:00:34.000000 ucam-identitylib-1.4.0/identitylib/card_client/model/available_barcode_batch_request_type.py
--rw-r--r--   0 root         (0) root         (0)    19607 2023-04-05 16:00:34.000000 ucam-identitylib-1.4.0/identitylib/card_client/model/available_barcode_batch_response_type.py
--rw-r--r--   0 root         (0) root         (0)    19919 2023-04-05 16:00:34.000000 ucam-identitylib-1.4.0/identitylib/card_client/model/available_barcode_batch_response_type_details.py
--rw-r--r--   0 root         (0) root         (0)    19449 2023-04-05 16:00:34.000000 ucam-identitylib-1.4.0/identitylib/card_client/model/available_barcode_batch_response_type_details_invalid_inner.py
--rw-r--r--   0 root         (0) root         (0)    19216 2023-04-05 16:00:34.000000 ucam-identitylib-1.4.0/identitylib/card_client/model/available_barcode_create_request_type.py
--rw-r--r--   0 root         (0) root         (0)    25129 2023-04-05 16:00:34.000000 ucam-identitylib-1.4.0/identitylib/card_client/model/card.py
--rw-r--r--   0 root         (0) root         (0)    22257 2023-04-05 16:00:35.000000 ucam-identitylib-1.4.0/identitylib/card_client/model/card_filter_request_type.py
--rw-r--r--   0 root         (0) root         (0)    19875 2023-04-05 16:00:35.000000 ucam-identitylib-1.4.0/identitylib/card_client/model/card_filter_response_type.py
--rw-r--r--   0 root         (0) root         (0)    21301 2023-04-05 16:00:35.000000 ucam-identitylib-1.4.0/identitylib/card_client/model/card_identifier.py
--rw-r--r--   0 root         (0) root         (0)    19670 2023-04-05 16:00:35.000000 ucam-identitylib-1.4.0/identitylib/card_client/model/card_identifier_bulk_update_request_type.py
--rw-r--r--   0 root         (0) root         (0)    19747 2023-04-05 16:00:35.000000 ucam-identitylib-1.4.0/identitylib/card_client/model/card_identifier_bulk_update_request_type_updates_inner.py
--rw-r--r--   0 root         (0) root         (0)    19680 2023-04-05 16:00:35.000000 ucam-identitylib-1.4.0/identitylib/card_client/model/card_identifier_bulk_update_response_type.py
--rw-r--r--   0 root         (0) root         (0)    19600 2023-04-05 16:00:35.000000 ucam-identitylib-1.4.0/identitylib/card_client/model/card_identifier_bulk_update_response_type_details_inner.py
--rw-r--r--   0 root         (0) root         (0)    19209 2023-04-05 16:00:35.000000 ucam-identitylib-1.4.0/identitylib/card_client/model/card_identifier_destroy_response_type.py
--rw-r--r--   0 root         (0) root         (0)    19477 2023-04-05 16:00:35.000000 ucam-identitylib-1.4.0/identitylib/card_client/model/card_identifier_update_request_type.py
--rw-r--r--   0 root         (0) root         (0)    19206 2023-04-05 16:00:35.000000 ucam-identitylib-1.4.0/identitylib/card_client/model/card_identifier_update_response_type.py
--rw-r--r--   0 root         (0) root         (0)    21069 2023-04-05 16:00:35.000000 ucam-identitylib-1.4.0/identitylib/card_client/model/card_logo.py
--rw-r--r--   0 root         (0) root         (0)    20492 2023-04-05 16:00:35.000000 ucam-identitylib-1.4.0/identitylib/card_client/model/card_note.py
--rw-r--r--   0 root         (0) root         (0)    19441 2023-04-05 16:00:35.000000 ucam-identitylib-1.4.0/identitylib/card_client/model/card_note_create_request_type.py
--rw-r--r--   0 root         (0) root         (0)    19208 2023-04-05 16:00:35.000000 ucam-identitylib-1.4.0/identitylib/card_client/model/card_note_destroy_request_type.py
--rw-r--r--   0 root         (0) root         (0)    19191 2023-04-05 16:00:35.000000 ucam-identitylib-1.4.0/identitylib/card_client/model/card_note_destroy_response_type.py
--rw-r--r--   0 root         (0) root         (0)    30374 2023-04-05 16:00:35.000000 ucam-identitylib-1.4.0/identitylib/card_client/model/card_request.py
--rw-r--r--   0 root         (0) root         (0)    19640 2023-04-05 16:00:35.000000 ucam-identitylib-1.4.0/identitylib/card_client/model/card_request_bulk_update_request_type.py
--rw-r--r--   0 root         (0) root         (0)    21306 2023-04-05 16:00:35.000000 ucam-identitylib-1.4.0/identitylib/card_client/model/card_request_bulk_update_request_type_updates_inner.py
--rw-r--r--   0 root         (0) root         (0)    20037 2023-04-05 16:00:35.000000 ucam-identitylib-1.4.0/identitylib/card_client/model/card_request_bulk_update_request_type_updates_inner_fields.py
--rw-r--r--   0 root         (0) root         (0)    19489 2023-04-05 16:00:35.000000 ucam-identitylib-1.4.0/identitylib/card_client/model/card_request_bulk_update_request_type_updates_inner_identifiers_inner.py
--rw-r--r--   0 root         (0) root         (0)    19671 2023-04-05 16:00:35.000000 ucam-identitylib-1.4.0/identitylib/card_client/model/card_request_bulk_update_response_type.py
--rw-r--r--   0 root         (0) root         (0)    19284 2023-04-05 16:00:35.000000 ucam-identitylib-1.4.0/identitylib/card_client/model/card_request_create_request_type.py
--rw-r--r--   0 root         (0) root         (0)    19213 2023-04-05 16:00:35.000000 ucam-identitylib-1.4.0/identitylib/card_client/model/card_request_distinct_values.py
--rw-r--r--   0 root         (0) root         (0)    27903 2023-04-05 16:00:35.000000 ucam-identitylib-1.4.0/identitylib/card_client/model/card_request_summary.py
--rw-r--r--   0 root         (0) root         (0)    21042 2023-04-05 16:00:35.000000 ucam-identitylib-1.4.0/identitylib/card_client/model/card_request_update_request_type.py
--rw-r--r--   0 root         (0) root         (0)    19197 2023-04-05 16:00:35.000000 ucam-identitylib-1.4.0/identitylib/card_client/model/card_request_update_response_type.py
--rw-r--r--   0 root         (0) root         (0)    19721 2023-04-05 16:00:35.000000 ucam-identitylib-1.4.0/identitylib/card_client/model/card_rfid_data_config_list_response_type.py
--rw-r--r--   0 root         (0) root         (0)    19708 2023-04-05 16:00:35.000000 ucam-identitylib-1.4.0/identitylib/card_client/model/card_rfid_data_config_list_response_type_results_inner.py
--rw-r--r--   0 root         (0) root         (0)    23411 2023-04-05 16:00:35.000000 ucam-identitylib-1.4.0/identitylib/card_client/model/card_summary.py
--rw-r--r--   0 root         (0) root         (0)    19609 2023-04-05 16:00:35.000000 ucam-identitylib-1.4.0/identitylib/card_client/model/card_update_request_type.py
--rw-r--r--   0 root         (0) root         (0)    19176 2023-04-05 16:00:35.000000 ucam-identitylib-1.4.0/identitylib/card_client/model/card_update_response_type.py
--rw-r--r--   0 root         (0) root         (0)    19276 2023-04-05 16:00:35.000000 ucam-identitylib-1.4.0/identitylib/card_client/model/college_institution_ids_list_response_type.py
--rw-r--r--   0 root         (0) root         (0)    20114 2023-04-05 16:00:35.000000 ucam-identitylib-1.4.0/identitylib/card_client/model/paginated_available_barcode_type.py
--rw-r--r--   0 root         (0) root         (0)    20094 2023-04-05 16:00:35.000000 ucam-identitylib-1.4.0/identitylib/card_client/model/paginated_card_identifier_type.py
--rw-r--r--   0 root         (0) root         (0)    19851 2023-04-05 16:00:35.000000 ucam-identitylib-1.4.0/identitylib/card_client/model/paginated_card_logo_type.py
--rw-r--r--   0 root         (0) root         (0)    19851 2023-04-05 16:00:35.000000 ucam-identitylib-1.4.0/identitylib/card_client/model/paginated_card_note_type.py
--rw-r--r--   0 root         (0) root         (0)    20135 2023-04-05 16:00:35.000000 ucam-identitylib-1.4.0/identitylib/card_client/model/paginated_card_request_summary_type.py
--rw-r--r--   0 root         (0) root         (0)    20064 2023-04-05 16:00:35.000000 ucam-identitylib-1.4.0/identitylib/card_client/model/paginated_card_summary_type.py
--rw-r--r--   0 root         (0) root         (0)    19382 2023-04-05 16:00:35.000000 ucam-identitylib-1.4.0/identitylib/card_client/model/permissions_response_type.py
--rw-r--r--   0 root         (0) root         (0)    19244 2023-04-05 16:00:35.000000 ucam-identitylib-1.4.0/identitylib/card_client/model/validation_error.py
--rw-r--r--   0 root         (0) root         (0)    19608 2023-04-05 16:00:35.000000 ucam-identitylib-1.4.0/identitylib/card_client/model/version_response_type.py
--rw-r--r--   0 root         (0) root         (0)    90312 2023-04-05 16:00:36.000000 ucam-identitylib-1.4.0/identitylib/card_client/model_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 16:01:05.401023 ucam-identitylib-1.4.0/identitylib/card_client/models/
--rw-r--r--   0 root         (0) root         (0)     5469 2023-04-05 16:00:36.000000 ucam-identitylib-1.4.0/identitylib/card_client/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21989 2023-04-05 16:00:36.000000 ucam-identitylib-1.4.0/identitylib/card_client/rest.py
--rw-rw-rw-   0 root         (0) root         (0)      609 2023-03-30 12:21:35.000000 ucam-identitylib-1.4.0/identitylib/card_client_configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 16:01:05.405023 ucam-identitylib-1.4.0/identitylib/hr_client/
--rw-r--r--   0 root         (0) root         (0)     2656 2023-04-05 16:00:41.000000 ucam-identitylib-1.4.0/identitylib/hr_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 16:01:05.405023 ucam-identitylib-1.4.0/identitylib/hr_client/api/
--rw-r--r--   0 root         (0) root         (0)      230 2023-04-05 16:00:41.000000 ucam-identitylib-1.4.0/identitylib/hr_client/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15246 2023-04-05 16:00:41.000000 ucam-identitylib-1.4.0/identitylib/hr_client/api/staff_members_api.py
--rw-r--r--   0 root         (0) root         (0)    41199 2023-04-05 16:00:41.000000 ucam-identitylib-1.4.0/identitylib/hr_client/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 16:01:05.405023 ucam-identitylib-1.4.0/identitylib/hr_client/apis/
--rw-r--r--   0 root         (0) root         (0)      517 2023-04-05 16:00:41.000000 ucam-identitylib-1.4.0/identitylib/hr_client/apis/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18527 2023-04-05 16:00:41.000000 ucam-identitylib-1.4.0/identitylib/hr_client/configuration.py
--rw-r--r--   0 root         (0) root         (0)     6932 2023-04-05 16:00:41.000000 ucam-identitylib-1.4.0/identitylib/hr_client/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 16:01:05.409023 ucam-identitylib-1.4.0/identitylib/hr_client/model/
--rw-r--r--   0 root         (0) root         (0)      355 2023-04-05 16:00:41.000000 ucam-identitylib-1.4.0/identitylib/hr_client/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15386 2023-04-05 16:00:40.000000 ucam-identitylib-1.4.0/identitylib/hr_client/model/affiliation.py
--rw-r--r--   0 root         (0) root         (0)    14942 2023-04-05 16:00:40.000000 ucam-identitylib-1.4.0/identitylib/hr_client/model/affiliation_scheme.py
--rw-r--r--   0 root         (0) root         (0)    13339 2023-04-05 16:00:40.000000 ucam-identitylib-1.4.0/identitylib/hr_client/model/http_exception.py
--rw-r--r--   0 root         (0) root         (0)    13537 2023-04-05 16:00:41.000000 ucam-identitylib-1.4.0/identitylib/hr_client/model/http_validation_error.py
--rw-r--r--   0 root         (0) root         (0)    13824 2023-04-05 16:00:41.000000 ucam-identitylib-1.4.0/identitylib/hr_client/model/identifier.py
--rw-r--r--   0 root         (0) root         (0)    14333 2023-04-05 16:00:41.000000 ucam-identitylib-1.4.0/identitylib/hr_client/model/identifier_scheme.py
--rw-r--r--   0 root         (0) root         (0)    13097 2023-04-05 16:00:41.000000 ucam-identitylib-1.4.0/identitylib/hr_client/model/location_inner.py
--rw-r--r--   0 root         (0) root         (0)    14276 2023-04-05 16:00:41.000000 ucam-identitylib-1.4.0/identitylib/hr_client/model/paginated_results_staff_member.py
--rw-r--r--   0 root         (0) root         (0)    16189 2023-04-05 16:00:41.000000 ucam-identitylib-1.4.0/identitylib/hr_client/model/staff_member.py
--rw-r--r--   0 root         (0) root         (0)    13901 2023-04-05 16:00:41.000000 ucam-identitylib-1.4.0/identitylib/hr_client/model/validation_error.py
--rw-r--r--   0 root         (0) root         (0)    84466 2023-04-05 16:00:41.000000 ucam-identitylib-1.4.0/identitylib/hr_client/model_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 16:01:05.409023 ucam-identitylib-1.4.0/identitylib/hr_client/models/
--rw-r--r--   0 root         (0) root         (0)     1113 2023-04-05 16:00:41.000000 ucam-identitylib-1.4.0/identitylib/hr_client/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16143 2023-04-05 16:00:41.000000 ucam-identitylib-1.4.0/identitylib/hr_client/rest.py
--rw-rw-rw-   0 root         (0) root         (0)     9961 2023-03-30 12:21:35.000000 ucam-identitylib-1.4.0/identitylib/identifiers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 16:01:05.409023 ucam-identitylib-1.4.0/identitylib/inst_identifier_client/
--rw-r--r--   0 root         (0) root         (0)     1757 2023-04-05 16:00:53.000000 ucam-identitylib-1.4.0/identitylib/inst_identifier_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 16:01:05.409023 ucam-identitylib-1.4.0/identitylib/inst_identifier_client/api/
--rw-r--r--   0 root         (0) root         (0)      238 2023-04-05 16:00:53.000000 ucam-identitylib-1.4.0/identitylib/inst_identifier_client/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6469 2023-04-05 16:00:53.000000 ucam-identitylib-1.4.0/identitylib/inst_identifier_client/api/default_api.py
--rw-r--r--   0 root         (0) root         (0)    40103 2023-04-05 16:00:53.000000 ucam-identitylib-1.4.0/identitylib/inst_identifier_client/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 16:01:05.413023 ucam-identitylib-1.4.0/identitylib/inst_identifier_client/apis/
--rw-r--r--   0 root         (0) root         (0)      521 2023-04-05 16:00:53.000000 ucam-identitylib-1.4.0/identitylib/inst_identifier_client/apis/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17693 2023-04-05 16:00:53.000000 ucam-identitylib-1.4.0/identitylib/inst_identifier_client/configuration.py
--rw-r--r--   0 root         (0) root         (0)     5929 2023-04-05 16:00:53.000000 ucam-identitylib-1.4.0/identitylib/inst_identifier_client/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 16:01:05.413023 ucam-identitylib-1.4.0/identitylib/inst_identifier_client/model/
--rw-r--r--   0 root         (0) root         (0)      368 2023-04-05 16:00:53.000000 ucam-identitylib-1.4.0/identitylib/inst_identifier_client/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12946 2023-04-05 16:00:53.000000 ucam-identitylib-1.4.0/identitylib/inst_identifier_client/model/mapping_datum.py
--rw-r--r--   0 root         (0) root         (0)    12728 2023-04-05 16:00:53.000000 ucam-identitylib-1.4.0/identitylib/inst_identifier_client/model/mapping_response.py
--rw-r--r--   0 root         (0) root         (0)    83476 2023-04-05 16:00:53.000000 ucam-identitylib-1.4.0/identitylib/inst_identifier_client/model_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 16:01:05.413023 ucam-identitylib-1.4.0/identitylib/inst_identifier_client/models/
--rw-r--r--   0 root         (0) root         (0)      557 2023-04-05 16:00:53.000000 ucam-identitylib-1.4.0/identitylib/inst_identifier_client/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15153 2023-04-05 16:00:53.000000 ucam-identitylib-1.4.0/identitylib/inst_identifier_client/rest.py
--rw-rw-rw-   0 root         (0) root         (0)      649 2023-03-30 12:21:35.000000 ucam-identitylib-1.4.0/identitylib/inst_identifier_configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 16:01:05.413023 ucam-identitylib-1.4.0/identitylib/lookup_client/
--rw-r--r--   0 root         (0) root         (0)      872 2023-04-05 16:00:45.000000 ucam-identitylib-1.4.0/identitylib/lookup_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 16:01:05.417023 ucam-identitylib-1.4.0/identitylib/lookup_client/api/
--rw-r--r--   0 root         (0) root         (0)      227 2023-04-05 16:00:45.000000 ucam-identitylib-1.4.0/identitylib/lookup_client/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58215 2023-04-05 16:00:45.000000 ucam-identitylib-1.4.0/identitylib/lookup_client/api/group_api.py
--rw-r--r--   0 root         (0) root         (0)    10948 2023-04-05 16:00:45.000000 ucam-identitylib-1.4.0/identitylib/lookup_client/api/ibis_api.py
--rw-r--r--   0 root         (0) root         (0)    76192 2023-04-05 16:00:45.000000 ucam-identitylib-1.4.0/identitylib/lookup_client/api/institution_api.py
--rw-r--r--   0 root         (0) root         (0)   101034 2023-04-05 16:00:45.000000 ucam-identitylib-1.4.0/identitylib/lookup_client/api/person_api.py
--rw-r--r--   0 root         (0) root         (0)    39272 2023-04-05 16:00:45.000000 ucam-identitylib-1.4.0/identitylib/lookup_client/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 16:01:05.417023 ucam-identitylib-1.4.0/identitylib/lookup_client/apis/
--rw-r--r--   0 root         (0) root         (0)      690 2023-04-05 16:00:45.000000 ucam-identitylib-1.4.0/identitylib/lookup_client/apis/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16967 2023-04-05 16:00:45.000000 ucam-identitylib-1.4.0/identitylib/lookup_client/configuration.py
--rw-r--r--   0 root         (0) root         (0)     5116 2023-04-05 16:00:45.000000 ucam-identitylib-1.4.0/identitylib/lookup_client/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 16:01:05.433024 ucam-identitylib-1.4.0/identitylib/lookup_client/model/
--rw-r--r--   0 root         (0) root         (0)      359 2023-04-05 16:00:45.000000 ucam-identitylib-1.4.0/identitylib/lookup_client/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14574 2023-04-05 16:00:44.000000 ucam-identitylib-1.4.0/identitylib/lookup_client/model/attribute.py
--rw-r--r--   0 root         (0) root         (0)    14850 2023-04-05 16:00:44.000000 ucam-identitylib-1.4.0/identitylib/lookup_client/model/attribute_scheme.py
--rw-r--r--   0 root         (0) root         (0)    12076 2023-04-05 16:00:44.000000 ucam-identitylib-1.4.0/identitylib/lookup_client/model/contact_phone_number.py
--rw-r--r--   0 root         (0) root         (0)    14778 2023-04-05 16:00:44.000000 ucam-identitylib-1.4.0/identitylib/lookup_client/model/contact_row.py
--rw-r--r--   0 root         (0) root         (0)    11774 2023-04-05 16:00:44.000000 ucam-identitylib-1.4.0/identitylib/lookup_client/model/contact_web_page.py
--rw-r--r--   0 root         (0) root         (0)    12447 2023-04-05 16:00:44.000000 ucam-identitylib-1.4.0/identitylib/lookup_client/model/error.py
--rw-r--r--   0 root         (0) root         (0)    21254 2023-04-05 16:00:44.000000 ucam-identitylib-1.4.0/identitylib/lookup_client/model/group.py
--rw-r--r--   0 root         (0) root         (0)    11860 2023-04-05 16:00:44.000000 ucam-identitylib-1.4.0/identitylib/lookup_client/model/group_all_groups200_response.py
--rw-r--r--   0 root         (0) root         (0)    11698 2023-04-05 16:00:44.000000 ucam-identitylib-1.4.0/identitylib/lookup_client/model/group_all_groups200_response_result.py
--rw-r--r--   0 root         (0) root         (0)    11901 2023-04-05 16:00:44.000000 ucam-identitylib-1.4.0/identitylib/lookup_client/model/group_all_groups_default_response.py
--rw-r--r--   0 root         (0) root         (0)    11699 2023-04-05 16:00:44.000000 ucam-identitylib-1.4.0/identitylib/lookup_client/model/group_all_groups_default_response_result.py
--rw-r--r--   0 root         (0) root         (0)    11961 2023-04-05 16:00:44.000000 ucam-identitylib-1.4.0/identitylib/lookup_client/model/group_get_cancelled_members200_response.py
--rw-r--r--   0 root         (0) root         (0)    11735 2023-04-05 16:00:44.000000 ucam-identitylib-1.4.0/identitylib/lookup_client/model/group_get_cancelled_members200_response_result.py
--rw-r--r--   0 root         (0) root         (0)    11850 2023-04-05 16:00:44.000000 ucam-identitylib-1.4.0/identitylib/lookup_client/model/group_get_group200_response.py
--rw-r--r--   0 root         (0) root         (0)    11684 2023-04-05 16:00:45.000000 ucam-identitylib-1.4.0/identitylib/lookup_client/model/group_get_group200_response_result.py
--rw-r--r--   0 root         (0) root         (0)    20692 2023-04-05 16:00:45.000000 ucam-identitylib-1.4.0/identitylib/lookup_client/model/group_members_of_inst.py
--rw-r--r--   0 root         (0) root         (0)    11880 2023-04-05 16:00:45.000000 ucam-identitylib-1.4.0/identitylib/lookup_client/model/group_search_count200_response.py
--rw-r--r--   0 root         (0) root         (0)    11532 2023-04-05 16:00:45.000000 ucam-identitylib-1.4.0/identitylib/lookup_client/model/group_search_count200_response_result.py
--rw-r--r--   0 root         (0) root         (0)    11962 2023-04-05 16:00:45.000000 ucam-identitylib-1.4.0/identitylib/lookup_client/model/ibis_get_last_transaction_id200_response.py
--rw-r--r--   0 root         (0) root         (0)    11556 2023-04-05 16:00:45.000000 ucam-identitylib-1.4.0/identitylib/lookup_client/model/ibis_get_last_transaction_id200_response_result.py
--rw-r--r--   0 root         (0) root         (0)    11860 2023-04-05 16:00:45.000000 ucam-identitylib-1.4.0/identitylib/lookup_client/model/ibis_get_version200_response.py
--rw-r--r--   0 root         (0) root         (0)    11526 2023-04-05 16:00:45.000000 ucam-identitylib-1.4.0/identitylib/lookup_client/model/ibis_get_version200_response_result.py
--rw-r--r--   0 root         (0) root         (0)    11881 2023-04-05 16:00:45.000000 ucam-identitylib-1.4.0/identitylib/lookup_client/model/identifier.py
--rw-r--r--   0 root         (0) root         (0)    18567 2023-04-05 16:00:45.000000 ucam-identitylib-1.4.0/identitylib/lookup_client/model/institution.py
--rw-r--r--   0 root         (0) root         (0)    12021 2023-04-05 16:00:45.000000 ucam-identitylib-1.4.0/identitylib/lookup_client/model/institution_all_attribute_schemes200_response.py
--rw-r--r--   0 root         (0) root         (0)    11871 2023-04-05 16:00:45.000000 ucam-identitylib-1.4.0/identitylib/lookup_client/model/institution_all_attribute_schemes200_response_result.py
--rw-r--r--   0 root         (0) root         (0)    11910 2023-04-05 16:00:45.000000 ucam-identitylib-1.4.0/identitylib/lookup_client/model/institution_all_insts200_response.py
--rw-r--r--   0 root         (0) root         (0)    11785 2023-04-05 16:00:45.000000 ucam-identitylib-1.4.0/identitylib/lookup_client/model/institution_all_insts200_response_result.py
--rw-r--r--   0 root         (0) root         (0)    11950 2023-04-05 16:00:45.000000 ucam-identitylib-1.4.0/identitylib/lookup_client/model/institution_get_attribute200_response.py
--rw-r--r--   0 root         (0) root         (0)    11762 2023-04-05 16:00:45.000000 ucam-identitylib-1.4.0/identitylib/lookup_client/model/institution_get_attribute200_response_result.py
--rw-r--r--   0 root         (0) root         (0)    11960 2023-04-05 16:00:45.000000 ucam-identitylib-1.4.0/identitylib/lookup_client/model/institution_get_attributes200_response.py
--rw-r--r--   0 root         (0) root         (0)    11776 2023-04-05 16:00:45.000000 ucam-identitylib-1.4.0/identitylib/lookup_client/model/institution_get_attributes200_response_result.py
--rw-r--r--   0 root         (0) root         (0)    11971 2023-04-05 16:00:45.000000 ucam-identitylib-1.4.0/identitylib/lookup_client/model/institution_get_contact_rows200_response.py
--rw-r--r--   0 root         (0) root         (0)    11856 2023-04-05 16:00:45.000000 ucam-identitylib-1.4.0/identitylib/lookup_client/model/institution_get_contact_rows200_response_result.py
--rw-r--r--   0 root         (0) root         (0)    11900 2023-04-05 16:00:45.000000 ucam-identitylib-1.4.0/identitylib/lookup_client/model/institution_get_inst200_response.py
--rw-r--r--   0 root         (0) root         (0)    11771 2023-04-05 16:00:45.000000 ucam-identitylib-1.4.0/identitylib/lookup_client/model/institution_get_inst200_response_result.py
--rw-r--r--   0 root         (0) root         (0)    18657 2023-04-05 16:00:45.000000 ucam-identitylib-1.4.0/identitylib/lookup_client/model/person.py
--rw-r--r--   0 root         (0) root         (0)    11870 2023-04-05 16:00:45.000000 ucam-identitylib-1.4.0/identitylib/lookup_client/model/person_get_person200_response.py
--rw-r--r--   0 root         (0) root         (0)    11702 2023-04-05 16:00:45.000000 ucam-identitylib-1.4.0/identitylib/lookup_client/model/person_get_person200_response_result.py
--rw-r--r--   0 root         (0) root         (0)    14062 2023-04-05 16:00:45.000000 ucam-identitylib-1.4.0/identitylib/lookup_client/model/person_identifier.py
--rw-r--r--   0 root         (0) root         (0)    11932 2023-04-05 16:00:45.000000 ucam-identitylib-1.4.0/identitylib/lookup_client/model/person_is_member_of_group200_response.py
--rw-r--r--   0 root         (0) root         (0)    11550 2023-04-05 16:00:45.000000 ucam-identitylib-1.4.0/identitylib/lookup_client/model/person_is_member_of_group200_response_result.py
--rw-r--r--   0 root         (0) root         (0)    82654 2023-04-05 16:00:45.000000 ucam-identitylib-1.4.0/identitylib/lookup_client/model_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 16:01:05.433024 ucam-identitylib-1.4.0/identitylib/lookup_client/models/
--rw-r--r--   0 root         (0) root         (0)     4751 2023-04-05 16:00:45.000000 ucam-identitylib-1.4.0/identitylib/lookup_client/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14331 2023-04-05 16:00:45.000000 ucam-identitylib-1.4.0/identitylib/lookup_client/rest.py
--rw-rw-rw-   0 root         (0) root         (0)      618 2023-03-30 12:21:35.000000 ucam-identitylib-1.4.0/identitylib/lookup_client_configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 16:01:05.437024 ucam-identitylib-1.4.0/identitylib/photo_client/
--rw-r--r--   0 root         (0) root         (0)     5308 2023-04-05 16:00:48.000000 ucam-identitylib-1.4.0/identitylib/photo_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 16:01:05.437024 ucam-identitylib-1.4.0/identitylib/photo_client/api/
--rw-r--r--   0 root         (0) root         (0)      232 2023-04-05 16:00:48.000000 ucam-identitylib-1.4.0/identitylib/photo_client/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11772 2023-04-05 16:00:48.000000 ucam-identitylib-1.4.0/identitylib/photo_client/api/all_photos_api.py
--rw-r--r--   0 root         (0) root         (0)    10203 2023-04-05 16:00:48.000000 ucam-identitylib-1.4.0/identitylib/photo_client/api/api_versions_api.py
--rw-r--r--   0 root         (0) root         (0)    43722 2023-04-05 16:00:48.000000 ucam-identitylib-1.4.0/identitylib/photo_client/api/approved_photos_api.py
--rw-r--r--   0 root         (0) root         (0)    10164 2023-04-05 16:00:48.000000 ucam-identitylib-1.4.0/identitylib/photo_client/api/permissions_api.py
--rw-r--r--   0 root         (0) root         (0)    11335 2023-04-05 16:00:48.000000 ucam-identitylib-1.4.0/identitylib/photo_client/api/photo_identifier_api.py
--rw-r--r--   0 root         (0) root         (0)    21142 2023-04-05 16:00:48.000000 ucam-identitylib-1.4.0/identitylib/photo_client/api/photo_identifiers_api.py
--rw-r--r--   0 root         (0) root         (0)    11127 2023-04-05 16:00:48.000000 ucam-identitylib-1.4.0/identitylib/photo_client/api/photo_identifiers_including_photos_api.py
--rw-r--r--   0 root         (0) root         (0)    61774 2023-04-05 16:00:48.000000 ucam-identitylib-1.4.0/identitylib/photo_client/api/photos_including_unapproved_photos_api.py
--rw-r--r--   0 root         (0) root         (0)    11860 2023-04-05 16:00:48.000000 ucam-identitylib-1.4.0/identitylib/photo_client/api/unapproved_photos_api.py
--rw-r--r--   0 root         (0) root         (0)    43706 2023-04-05 16:00:48.000000 ucam-identitylib-1.4.0/identitylib/photo_client/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 16:01:05.437024 ucam-identitylib-1.4.0/identitylib/photo_client/apis/
--rw-r--r--   0 root         (0) root         (0)     1216 2023-04-05 16:00:48.000000 ucam-identitylib-1.4.0/identitylib/photo_client/apis/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21352 2023-04-05 16:00:48.000000 ucam-identitylib-1.4.0/identitylib/photo_client/configuration.py
--rw-r--r--   0 root         (0) root         (0)     9560 2023-04-05 16:00:48.000000 ucam-identitylib-1.4.0/identitylib/photo_client/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 16:01:05.445024 ucam-identitylib-1.4.0/identitylib/photo_client/model/
--rw-r--r--   0 root         (0) root         (0)      358 2023-04-05 16:00:48.000000 ucam-identitylib-1.4.0/identitylib/photo_client/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16212 2023-04-05 16:00:48.000000 ucam-identitylib-1.4.0/identitylib/photo_client/model/api_versions.py
--rw-r--r--   0 root         (0) root         (0)    15964 2023-04-05 16:00:48.000000 ucam-identitylib-1.4.0/identitylib/photo_client/model/bad_request.py
--rw-r--r--   0 root         (0) root         (0)    15961 2023-04-05 16:00:48.000000 ucam-identitylib-1.4.0/identitylib/photo_client/model/forbidden.py
--rw-r--r--   0 root         (0) root         (0)    15991 2023-04-05 16:00:48.000000 ucam-identitylib-1.4.0/identitylib/photo_client/model/internal_server_error.py
--rw-r--r--   0 root         (0) root         (0)    15958 2023-04-05 16:00:48.000000 ucam-identitylib-1.4.0/identitylib/photo_client/model/not_found.py
--rw-r--r--   0 root         (0) root         (0)    16791 2023-04-05 16:00:48.000000 ucam-identitylib-1.4.0/identitylib/photo_client/model/paginated_v1_beta1_photo_identifier_summary_list.py
--rw-r--r--   0 root         (0) root         (0)    16619 2023-04-05 16:00:48.000000 ucam-identitylib-1.4.0/identitylib/photo_client/model/paginated_v1_beta1_photo_list.py
--rw-r--r--   0 root         (0) root         (0)    16498 2023-04-05 16:00:48.000000 ucam-identitylib-1.4.0/identitylib/photo_client/model/patched_v1_beta1_photo_identifier_summary_request.py
--rw-r--r--   0 root         (0) root         (0)    16028 2023-04-05 16:00:48.000000 ucam-identitylib-1.4.0/identitylib/photo_client/model/permissions.py
--rw-r--r--   0 root         (0) root         (0)    18333 2023-04-05 16:00:48.000000 ucam-identitylib-1.4.0/identitylib/photo_client/model/photo_identifier.py
--rw-r--r--   0 root         (0) root         (0)    19295 2023-04-05 16:00:48.000000 ucam-identitylib-1.4.0/identitylib/photo_client/model/scheme_enum.py
--rw-r--r--   0 root         (0) root         (0)    16889 2023-04-05 16:00:48.000000 ucam-identitylib-1.4.0/identitylib/photo_client/model/status_enum.py
--rw-r--r--   0 root         (0) root         (0)    16252 2023-04-05 16:00:48.000000 ucam-identitylib-1.4.0/identitylib/photo_client/model/transient_image_url.py
--rw-r--r--   0 root         (0) root         (0)    15970 2023-04-05 16:00:48.000000 ucam-identitylib-1.4.0/identitylib/photo_client/model/unauthorized.py
--rw-r--r--   0 root         (0) root         (0)    22401 2023-04-05 16:00:48.000000 ucam-identitylib-1.4.0/identitylib/photo_client/model/v1_beta1_photo.py
--rw-r--r--   0 root         (0) root         (0)    16599 2023-04-05 16:00:48.000000 ucam-identitylib-1.4.0/identitylib/photo_client/model/v1_beta1_photo_identifier_summary.py
--rw-r--r--   0 root         (0) root         (0)    87097 2023-04-05 16:00:48.000000 ucam-identitylib-1.4.0/identitylib/photo_client/model_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 16:01:05.445024 ucam-identitylib-1.4.0/identitylib/photo_client/models/
--rw-r--r--   0 root         (0) root         (0)     1699 2023-04-05 16:00:48.000000 ucam-identitylib-1.4.0/identitylib/photo_client/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18774 2023-04-05 16:00:48.000000 ucam-identitylib-1.4.0/identitylib/photo_client/rest.py
--rw-rw-rw-   0 root         (0) root         (0)      612 2023-03-30 12:21:35.000000 ucam-identitylib-1.4.0/identitylib/photo_client_configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 16:01:05.449025 ucam-identitylib-1.4.0/identitylib/student_client/
--rw-r--r--   0 root         (0) root         (0)     2582 2023-04-05 16:00:51.000000 ucam-identitylib-1.4.0/identitylib/student_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 16:01:05.449025 ucam-identitylib-1.4.0/identitylib/student_client/api/
--rw-r--r--   0 root         (0) root         (0)      231 2023-04-05 16:00:51.000000 ucam-identitylib-1.4.0/identitylib/student_client/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21826 2023-04-05 16:00:51.000000 ucam-identitylib-1.4.0/identitylib/student_client/api/students_api.py
--rw-r--r--   0 root         (0) root         (0)    41093 2023-04-05 16:00:51.000000 ucam-identitylib-1.4.0/identitylib/student_client/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 16:01:05.449025 ucam-identitylib-1.4.0/identitylib/student_client/apis/
--rw-r--r--   0 root         (0) root         (0)      509 2023-04-05 16:00:51.000000 ucam-identitylib-1.4.0/identitylib/student_client/apis/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18407 2023-04-05 16:00:51.000000 ucam-identitylib-1.4.0/identitylib/student_client/configuration.py
--rw-r--r--   0 root         (0) root         (0)     6818 2023-04-05 16:00:51.000000 ucam-identitylib-1.4.0/identitylib/student_client/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 16:01:05.449025 ucam-identitylib-1.4.0/identitylib/student_client/model/
--rw-r--r--   0 root         (0) root         (0)      360 2023-04-05 16:00:51.000000 ucam-identitylib-1.4.0/identitylib/student_client/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15305 2023-04-05 16:00:51.000000 ucam-identitylib-1.4.0/identitylib/student_client/model/affiliation.py
--rw-r--r--   0 root         (0) root         (0)    14466 2023-04-05 16:00:51.000000 ucam-identitylib-1.4.0/identitylib/student_client/model/affiliation_scheme.py
--rw-r--r--   0 root         (0) root         (0)    13235 2023-04-05 16:00:51.000000 ucam-identitylib-1.4.0/identitylib/student_client/model/http_exception.py
--rw-r--r--   0 root         (0) root         (0)    13438 2023-04-05 16:00:51.000000 ucam-identitylib-1.4.0/identitylib/student_client/model/http_validation_error.py
--rw-r--r--   0 root         (0) root         (0)    13725 2023-04-05 16:00:51.000000 ucam-identitylib-1.4.0/identitylib/student_client/model/identifier.py
--rw-r--r--   0 root         (0) root         (0)    14035 2023-04-05 16:00:51.000000 ucam-identitylib-1.4.0/identitylib/student_client/model/identifier_scheme.py
--rw-r--r--   0 root         (0) root         (0)    12993 2023-04-05 16:00:51.000000 ucam-identitylib-1.4.0/identitylib/student_client/model/location_inner.py
--rw-r--r--   0 root         (0) root         (0)    14202 2023-04-05 16:00:51.000000 ucam-identitylib-1.4.0/identitylib/student_client/model/paginated_results_student.py
--rw-r--r--   0 root         (0) root         (0)    16439 2023-04-05 16:00:51.000000 ucam-identitylib-1.4.0/identitylib/student_client/model/student.py
--rw-r--r--   0 root         (0) root         (0)    13802 2023-04-05 16:00:51.000000 ucam-identitylib-1.4.0/identitylib/student_client/model/validation_error.py
--rw-r--r--   0 root         (0) root         (0)    84357 2023-04-05 16:00:51.000000 ucam-identitylib-1.4.0/identitylib/student_client/model_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 16:01:05.449025 ucam-identitylib-1.4.0/identitylib/student_client/models/
--rw-r--r--   0 root         (0) root         (0)     1150 2023-04-05 16:00:51.000000 ucam-identitylib-1.4.0/identitylib/student_client/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16034 2023-04-05 16:00:51.000000 ucam-identitylib-1.4.0/identitylib/student_client/rest.py
--rw-rw-rw-   0 root         (0) root         (0)      646 2023-03-30 12:21:35.000000 ucam-identitylib-1.4.0/identitylib/university_hr_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)      648 2023-03-30 12:21:35.000000 ucam-identitylib-1.4.0/identitylib/university_student_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)       56 2023-04-05 11:39:29.000000 ucam-identitylib-1.4.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-05 16:01:05.449025 ucam-identitylib-1.4.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1529 2023-04-05 15:29:30.000000 ucam-identitylib-1.4.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 16:01:05.449025 ucam-identitylib-1.4.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-05 16:00:00.000000 ucam-identitylib-1.4.0/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5517 2023-03-30 12:21:35.000000 ucam-identitylib-1.4.0/tests/test_api_client_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     3449 2023-03-30 12:21:35.000000 ucam-identitylib-1.4.0/tests/test_identifiers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 16:01:05.449025 ucam-identitylib-1.4.0/ucam_identitylib.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2699 2023-04-05 16:01:05.000000 ucam-identitylib-1.4.0/ucam_identitylib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12136 2023-04-05 16:01:05.000000 ucam-identitylib-1.4.0/ucam_identitylib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-05 16:01:05.000000 ucam-identitylib-1.4.0/ucam_identitylib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2023-04-05 16:01:05.000000 ucam-identitylib-1.4.0/ucam_identitylib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-04-05 16:01:05.000000 ucam-identitylib-1.4.0/ucam_identitylib.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.843518 ucam-identitylib-1.5.0/
+-rw-rw-rw-   0 root         (0) root         (0)       25 2023-03-30 12:19:13.000000 ucam-identitylib-1.5.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2699 2023-04-21 08:32:42.843518 ucam-identitylib-1.5.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2002 2023-03-30 12:19:13.000000 ucam-identitylib-1.5.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.795516 ucam-identitylib-1.5.0/identitylib/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 08:32:32.000000 ucam-identitylib-1.5.0/identitylib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2517 2023-04-20 19:16:44.000000 ucam-identitylib-1.5.0/identitylib/api_client_mixin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.799516 ucam-identitylib-1.5.0/identitylib/card_client/
+-rw-r--r--   0 root         (0) root         (0)     8516 2023-04-21 08:32:18.000000 ucam-identitylib-1.5.0/identitylib/card_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.799516 ucam-identitylib-1.5.0/identitylib/card_client/api/
+-rw-r--r--   0 root         (0) root         (0)      231 2023-04-21 08:32:18.000000 ucam-identitylib-1.5.0/identitylib/card_client/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13392 2023-04-21 08:32:18.000000 ucam-identitylib-1.5.0/identitylib/card_client/api/permissions_api.py
+-rw-r--r--   0 root         (0) root         (0)   217309 2023-04-21 08:32:18.000000 ucam-identitylib-1.5.0/identitylib/card_client/api/v1beta1_api.py
+-rw-r--r--   0 root         (0) root         (0)    13297 2023-04-21 08:32:18.000000 ucam-identitylib-1.5.0/identitylib/card_client/api/versions_api.py
+-rw-r--r--   0 root         (0) root         (0)    46930 2023-04-21 08:32:18.000000 ucam-identitylib-1.5.0/identitylib/card_client/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.799516 ucam-identitylib-1.5.0/identitylib/card_client/apis/
+-rw-r--r--   0 root         (0) root         (0)      643 2023-04-21 08:32:18.000000 ucam-identitylib-1.5.0/identitylib/card_client/apis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24525 2023-04-21 08:32:18.000000 ucam-identitylib-1.5.0/identitylib/card_client/configuration.py
+-rw-r--r--   0 root         (0) root         (0)    12776 2023-04-21 08:32:18.000000 ucam-identitylib-1.5.0/identitylib/card_client/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.823517 ucam-identitylib-1.5.0/identitylib/card_client/model/
+-rw-r--r--   0 root         (0) root         (0)      357 2023-04-21 08:32:18.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19212 2023-04-21 08:32:15.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/api_exception.py
+-rw-r--r--   0 root         (0) root         (0)    19855 2023-04-21 08:32:15.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/available_barcode.py
+-rw-r--r--   0 root         (0) root         (0)    19301 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/available_barcode_batch_request_type.py
+-rw-r--r--   0 root         (0) root         (0)    19607 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/available_barcode_batch_response_type.py
+-rw-r--r--   0 root         (0) root         (0)    19919 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/available_barcode_batch_response_type_details.py
+-rw-r--r--   0 root         (0) root         (0)    19449 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/available_barcode_batch_response_type_details_invalid_inner.py
+-rw-r--r--   0 root         (0) root         (0)    19216 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/available_barcode_create_request_type.py
+-rw-r--r--   0 root         (0) root         (0)    25129 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card.py
+-rw-r--r--   0 root         (0) root         (0)    22257 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card_filter_request_type.py
+-rw-r--r--   0 root         (0) root         (0)    19875 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card_filter_response_type.py
+-rw-r--r--   0 root         (0) root         (0)    21301 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card_identifier.py
+-rw-r--r--   0 root         (0) root         (0)    19670 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card_identifier_bulk_update_request_type.py
+-rw-r--r--   0 root         (0) root         (0)    19747 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card_identifier_bulk_update_request_type_updates_inner.py
+-rw-r--r--   0 root         (0) root         (0)    19680 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card_identifier_bulk_update_response_type.py
+-rw-r--r--   0 root         (0) root         (0)    19600 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card_identifier_bulk_update_response_type_details_inner.py
+-rw-r--r--   0 root         (0) root         (0)    19209 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card_identifier_destroy_response_type.py
+-rw-r--r--   0 root         (0) root         (0)    19477 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card_identifier_update_request_type.py
+-rw-r--r--   0 root         (0) root         (0)    19206 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card_identifier_update_response_type.py
+-rw-r--r--   0 root         (0) root         (0)    21069 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card_logo.py
+-rw-r--r--   0 root         (0) root         (0)    20492 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card_note.py
+-rw-r--r--   0 root         (0) root         (0)    19441 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card_note_create_request_type.py
+-rw-r--r--   0 root         (0) root         (0)    19208 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card_note_destroy_request_type.py
+-rw-r--r--   0 root         (0) root         (0)    19191 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card_note_destroy_response_type.py
+-rw-r--r--   0 root         (0) root         (0)    30374 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card_request.py
+-rw-r--r--   0 root         (0) root         (0)    19640 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card_request_bulk_update_request_type.py
+-rw-r--r--   0 root         (0) root         (0)    21306 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card_request_bulk_update_request_type_updates_inner.py
+-rw-r--r--   0 root         (0) root         (0)    20037 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card_request_bulk_update_request_type_updates_inner_fields.py
+-rw-r--r--   0 root         (0) root         (0)    19489 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card_request_bulk_update_request_type_updates_inner_identifiers_inner.py
+-rw-r--r--   0 root         (0) root         (0)    19671 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card_request_bulk_update_response_type.py
+-rw-r--r--   0 root         (0) root         (0)    19284 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card_request_create_request_type.py
+-rw-r--r--   0 root         (0) root         (0)    19213 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card_request_distinct_values.py
+-rw-r--r--   0 root         (0) root         (0)    27903 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card_request_summary.py
+-rw-r--r--   0 root         (0) root         (0)    21042 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card_request_update_request_type.py
+-rw-r--r--   0 root         (0) root         (0)    19197 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card_request_update_response_type.py
+-rw-r--r--   0 root         (0) root         (0)    19721 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card_rfid_data_config_list_response_type.py
+-rw-r--r--   0 root         (0) root         (0)    19708 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card_rfid_data_config_list_response_type_results_inner.py
+-rw-r--r--   0 root         (0) root         (0)    23411 2023-04-21 08:32:17.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card_summary.py
+-rw-r--r--   0 root         (0) root         (0)    19609 2023-04-21 08:32:17.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card_update_request_type.py
+-rw-r--r--   0 root         (0) root         (0)    19176 2023-04-21 08:32:17.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card_update_response_type.py
+-rw-r--r--   0 root         (0) root         (0)    19276 2023-04-21 08:32:17.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/college_institution_ids_list_response_type.py
+-rw-r--r--   0 root         (0) root         (0)    20114 2023-04-21 08:32:17.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/paginated_available_barcode_type.py
+-rw-r--r--   0 root         (0) root         (0)    20094 2023-04-21 08:32:17.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/paginated_card_identifier_type.py
+-rw-r--r--   0 root         (0) root         (0)    19851 2023-04-21 08:32:17.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/paginated_card_logo_type.py
+-rw-r--r--   0 root         (0) root         (0)    19851 2023-04-21 08:32:17.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/paginated_card_note_type.py
+-rw-r--r--   0 root         (0) root         (0)    20135 2023-04-21 08:32:17.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/paginated_card_request_summary_type.py
+-rw-r--r--   0 root         (0) root         (0)    20064 2023-04-21 08:32:17.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/paginated_card_summary_type.py
+-rw-r--r--   0 root         (0) root         (0)    19382 2023-04-21 08:32:17.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/permissions_response_type.py
+-rw-r--r--   0 root         (0) root         (0)    19244 2023-04-21 08:32:17.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/validation_error.py
+-rw-r--r--   0 root         (0) root         (0)    19608 2023-04-21 08:32:17.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/version_response_type.py
+-rw-r--r--   0 root         (0) root         (0)    90312 2023-04-21 08:32:18.000000 ucam-identitylib-1.5.0/identitylib/card_client/model_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.823517 ucam-identitylib-1.5.0/identitylib/card_client/models/
+-rw-r--r--   0 root         (0) root         (0)     5469 2023-04-21 08:32:18.000000 ucam-identitylib-1.5.0/identitylib/card_client/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21989 2023-04-21 08:32:18.000000 ucam-identitylib-1.5.0/identitylib/card_client/rest.py
+-rw-rw-rw-   0 root         (0) root         (0)      609 2023-03-30 12:19:13.000000 ucam-identitylib-1.5.0/identitylib/card_client_configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.823517 ucam-identitylib-1.5.0/identitylib/hr_client/
+-rw-r--r--   0 root         (0) root         (0)     2656 2023-04-21 08:32:21.000000 ucam-identitylib-1.5.0/identitylib/hr_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.823517 ucam-identitylib-1.5.0/identitylib/hr_client/api/
+-rw-r--r--   0 root         (0) root         (0)      230 2023-04-21 08:32:21.000000 ucam-identitylib-1.5.0/identitylib/hr_client/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15246 2023-04-21 08:32:21.000000 ucam-identitylib-1.5.0/identitylib/hr_client/api/staff_members_api.py
+-rw-r--r--   0 root         (0) root         (0)    41199 2023-04-21 08:32:21.000000 ucam-identitylib-1.5.0/identitylib/hr_client/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.823517 ucam-identitylib-1.5.0/identitylib/hr_client/apis/
+-rw-r--r--   0 root         (0) root         (0)      517 2023-04-21 08:32:21.000000 ucam-identitylib-1.5.0/identitylib/hr_client/apis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18527 2023-04-21 08:32:21.000000 ucam-identitylib-1.5.0/identitylib/hr_client/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     6932 2023-04-21 08:32:21.000000 ucam-identitylib-1.5.0/identitylib/hr_client/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.827517 ucam-identitylib-1.5.0/identitylib/hr_client/model/
+-rw-r--r--   0 root         (0) root         (0)      355 2023-04-21 08:32:21.000000 ucam-identitylib-1.5.0/identitylib/hr_client/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15386 2023-04-21 08:32:21.000000 ucam-identitylib-1.5.0/identitylib/hr_client/model/affiliation.py
+-rw-r--r--   0 root         (0) root         (0)    14942 2023-04-21 08:32:21.000000 ucam-identitylib-1.5.0/identitylib/hr_client/model/affiliation_scheme.py
+-rw-r--r--   0 root         (0) root         (0)    13339 2023-04-21 08:32:21.000000 ucam-identitylib-1.5.0/identitylib/hr_client/model/http_exception.py
+-rw-r--r--   0 root         (0) root         (0)    13537 2023-04-21 08:32:21.000000 ucam-identitylib-1.5.0/identitylib/hr_client/model/http_validation_error.py
+-rw-r--r--   0 root         (0) root         (0)    13824 2023-04-21 08:32:21.000000 ucam-identitylib-1.5.0/identitylib/hr_client/model/identifier.py
+-rw-r--r--   0 root         (0) root         (0)    14333 2023-04-21 08:32:21.000000 ucam-identitylib-1.5.0/identitylib/hr_client/model/identifier_scheme.py
+-rw-r--r--   0 root         (0) root         (0)    13097 2023-04-21 08:32:21.000000 ucam-identitylib-1.5.0/identitylib/hr_client/model/location_inner.py
+-rw-r--r--   0 root         (0) root         (0)    14276 2023-04-21 08:32:21.000000 ucam-identitylib-1.5.0/identitylib/hr_client/model/paginated_results_staff_member.py
+-rw-r--r--   0 root         (0) root         (0)    16189 2023-04-21 08:32:21.000000 ucam-identitylib-1.5.0/identitylib/hr_client/model/staff_member.py
+-rw-r--r--   0 root         (0) root         (0)    13901 2023-04-21 08:32:21.000000 ucam-identitylib-1.5.0/identitylib/hr_client/model/validation_error.py
+-rw-r--r--   0 root         (0) root         (0)    84466 2023-04-21 08:32:21.000000 ucam-identitylib-1.5.0/identitylib/hr_client/model_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.827517 ucam-identitylib-1.5.0/identitylib/hr_client/models/
+-rw-r--r--   0 root         (0) root         (0)     1113 2023-04-21 08:32:21.000000 ucam-identitylib-1.5.0/identitylib/hr_client/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16143 2023-04-21 08:32:21.000000 ucam-identitylib-1.5.0/identitylib/hr_client/rest.py
+-rw-rw-rw-   0 root         (0) root         (0)     9961 2023-03-30 12:19:13.000000 ucam-identitylib-1.5.0/identitylib/identifiers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.827517 ucam-identitylib-1.5.0/identitylib/inst_identifier_client/
+-rw-r--r--   0 root         (0) root         (0)     1757 2023-04-21 08:32:32.000000 ucam-identitylib-1.5.0/identitylib/inst_identifier_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.827517 ucam-identitylib-1.5.0/identitylib/inst_identifier_client/api/
+-rw-r--r--   0 root         (0) root         (0)      238 2023-04-21 08:32:32.000000 ucam-identitylib-1.5.0/identitylib/inst_identifier_client/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6469 2023-04-21 08:32:32.000000 ucam-identitylib-1.5.0/identitylib/inst_identifier_client/api/default_api.py
+-rw-r--r--   0 root         (0) root         (0)    40103 2023-04-21 08:32:32.000000 ucam-identitylib-1.5.0/identitylib/inst_identifier_client/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.827517 ucam-identitylib-1.5.0/identitylib/inst_identifier_client/apis/
+-rw-r--r--   0 root         (0) root         (0)      521 2023-04-21 08:32:32.000000 ucam-identitylib-1.5.0/identitylib/inst_identifier_client/apis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17693 2023-04-21 08:32:32.000000 ucam-identitylib-1.5.0/identitylib/inst_identifier_client/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     5929 2023-04-21 08:32:32.000000 ucam-identitylib-1.5.0/identitylib/inst_identifier_client/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.827517 ucam-identitylib-1.5.0/identitylib/inst_identifier_client/model/
+-rw-r--r--   0 root         (0) root         (0)      368 2023-04-21 08:32:32.000000 ucam-identitylib-1.5.0/identitylib/inst_identifier_client/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12946 2023-04-21 08:32:32.000000 ucam-identitylib-1.5.0/identitylib/inst_identifier_client/model/mapping_datum.py
+-rw-r--r--   0 root         (0) root         (0)    12728 2023-04-21 08:32:32.000000 ucam-identitylib-1.5.0/identitylib/inst_identifier_client/model/mapping_response.py
+-rw-r--r--   0 root         (0) root         (0)    83476 2023-04-21 08:32:32.000000 ucam-identitylib-1.5.0/identitylib/inst_identifier_client/model_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.827517 ucam-identitylib-1.5.0/identitylib/inst_identifier_client/models/
+-rw-r--r--   0 root         (0) root         (0)      557 2023-04-21 08:32:32.000000 ucam-identitylib-1.5.0/identitylib/inst_identifier_client/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15153 2023-04-21 08:32:32.000000 ucam-identitylib-1.5.0/identitylib/inst_identifier_client/rest.py
+-rw-rw-rw-   0 root         (0) root         (0)      649 2023-03-30 12:19:13.000000 ucam-identitylib-1.5.0/identitylib/inst_identifier_configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.827517 ucam-identitylib-1.5.0/identitylib/lookup_client/
+-rw-r--r--   0 root         (0) root         (0)      872 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.831518 ucam-identitylib-1.5.0/identitylib/lookup_client/api/
+-rw-r--r--   0 root         (0) root         (0)      227 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58215 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/api/group_api.py
+-rw-r--r--   0 root         (0) root         (0)    10948 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/api/ibis_api.py
+-rw-r--r--   0 root         (0) root         (0)    76192 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/api/institution_api.py
+-rw-r--r--   0 root         (0) root         (0)   101034 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/api/person_api.py
+-rw-r--r--   0 root         (0) root         (0)    39272 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.831518 ucam-identitylib-1.5.0/identitylib/lookup_client/apis/
+-rw-r--r--   0 root         (0) root         (0)      690 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/apis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16967 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     5116 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.835518 ucam-identitylib-1.5.0/identitylib/lookup_client/model/
+-rw-r--r--   0 root         (0) root         (0)      359 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14574 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/attribute.py
+-rw-r--r--   0 root         (0) root         (0)    14850 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/attribute_scheme.py
+-rw-r--r--   0 root         (0) root         (0)    12076 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/contact_phone_number.py
+-rw-r--r--   0 root         (0) root         (0)    14778 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/contact_row.py
+-rw-r--r--   0 root         (0) root         (0)    11774 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/contact_web_page.py
+-rw-r--r--   0 root         (0) root         (0)    12447 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/error.py
+-rw-r--r--   0 root         (0) root         (0)    21254 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/group.py
+-rw-r--r--   0 root         (0) root         (0)    11860 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/group_all_groups200_response.py
+-rw-r--r--   0 root         (0) root         (0)    11698 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/group_all_groups200_response_result.py
+-rw-r--r--   0 root         (0) root         (0)    11901 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/group_all_groups_default_response.py
+-rw-r--r--   0 root         (0) root         (0)    11699 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/group_all_groups_default_response_result.py
+-rw-r--r--   0 root         (0) root         (0)    11961 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/group_get_cancelled_members200_response.py
+-rw-r--r--   0 root         (0) root         (0)    11735 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/group_get_cancelled_members200_response_result.py
+-rw-r--r--   0 root         (0) root         (0)    11850 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/group_get_group200_response.py
+-rw-r--r--   0 root         (0) root         (0)    11684 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/group_get_group200_response_result.py
+-rw-r--r--   0 root         (0) root         (0)    20692 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/group_members_of_inst.py
+-rw-r--r--   0 root         (0) root         (0)    11880 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/group_search_count200_response.py
+-rw-r--r--   0 root         (0) root         (0)    11532 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/group_search_count200_response_result.py
+-rw-r--r--   0 root         (0) root         (0)    11962 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/ibis_get_last_transaction_id200_response.py
+-rw-r--r--   0 root         (0) root         (0)    11556 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/ibis_get_last_transaction_id200_response_result.py
+-rw-r--r--   0 root         (0) root         (0)    11860 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/ibis_get_version200_response.py
+-rw-r--r--   0 root         (0) root         (0)    11526 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/ibis_get_version200_response_result.py
+-rw-r--r--   0 root         (0) root         (0)    11881 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/identifier.py
+-rw-r--r--   0 root         (0) root         (0)    18567 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/institution.py
+-rw-r--r--   0 root         (0) root         (0)    12021 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/institution_all_attribute_schemes200_response.py
+-rw-r--r--   0 root         (0) root         (0)    11871 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/institution_all_attribute_schemes200_response_result.py
+-rw-r--r--   0 root         (0) root         (0)    11910 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/institution_all_insts200_response.py
+-rw-r--r--   0 root         (0) root         (0)    11785 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/institution_all_insts200_response_result.py
+-rw-r--r--   0 root         (0) root         (0)    11950 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/institution_get_attribute200_response.py
+-rw-r--r--   0 root         (0) root         (0)    11762 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/institution_get_attribute200_response_result.py
+-rw-r--r--   0 root         (0) root         (0)    11960 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/institution_get_attributes200_response.py
+-rw-r--r--   0 root         (0) root         (0)    11776 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/institution_get_attributes200_response_result.py
+-rw-r--r--   0 root         (0) root         (0)    11971 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/institution_get_contact_rows200_response.py
+-rw-r--r--   0 root         (0) root         (0)    11856 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/institution_get_contact_rows200_response_result.py
+-rw-r--r--   0 root         (0) root         (0)    11900 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/institution_get_inst200_response.py
+-rw-r--r--   0 root         (0) root         (0)    11771 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/institution_get_inst200_response_result.py
+-rw-r--r--   0 root         (0) root         (0)    18657 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/person.py
+-rw-r--r--   0 root         (0) root         (0)    11870 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/person_get_person200_response.py
+-rw-r--r--   0 root         (0) root         (0)    11702 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/person_get_person200_response_result.py
+-rw-r--r--   0 root         (0) root         (0)    14062 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/person_identifier.py
+-rw-r--r--   0 root         (0) root         (0)    11932 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/person_is_member_of_group200_response.py
+-rw-r--r--   0 root         (0) root         (0)    11550 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/person_is_member_of_group200_response_result.py
+-rw-r--r--   0 root         (0) root         (0)    82654 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.835518 ucam-identitylib-1.5.0/identitylib/lookup_client/models/
+-rw-r--r--   0 root         (0) root         (0)     4751 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14331 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/rest.py
+-rw-rw-rw-   0 root         (0) root         (0)      618 2023-03-30 12:19:13.000000 ucam-identitylib-1.5.0/identitylib/lookup_client_configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.835518 ucam-identitylib-1.5.0/identitylib/photo_client/
+-rw-r--r--   0 root         (0) root         (0)     5308 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.835518 ucam-identitylib-1.5.0/identitylib/photo_client/api/
+-rw-r--r--   0 root         (0) root         (0)      232 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11772 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/api/all_photos_api.py
+-rw-r--r--   0 root         (0) root         (0)    10203 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/api/api_versions_api.py
+-rw-r--r--   0 root         (0) root         (0)    43722 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/api/approved_photos_api.py
+-rw-r--r--   0 root         (0) root         (0)    10164 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/api/permissions_api.py
+-rw-r--r--   0 root         (0) root         (0)    11335 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/api/photo_identifier_api.py
+-rw-r--r--   0 root         (0) root         (0)    27918 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/api/photo_identifiers_api.py
+-rw-r--r--   0 root         (0) root         (0)    11127 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/api/photo_identifiers_including_photos_api.py
+-rw-r--r--   0 root         (0) root         (0)    61774 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/api/photos_including_unapproved_photos_api.py
+-rw-r--r--   0 root         (0) root         (0)    11860 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/api/unapproved_photos_api.py
+-rw-r--r--   0 root         (0) root         (0)    43706 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.839518 ucam-identitylib-1.5.0/identitylib/photo_client/apis/
+-rw-r--r--   0 root         (0) root         (0)     1216 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/apis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21352 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     9560 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.839518 ucam-identitylib-1.5.0/identitylib/photo_client/model/
+-rw-r--r--   0 root         (0) root         (0)      358 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17123 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/model/action_enum.py
+-rw-r--r--   0 root         (0) root         (0)    16212 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/model/api_versions.py
+-rw-r--r--   0 root         (0) root         (0)    15964 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/model/bad_request.py
+-rw-r--r--   0 root         (0) root         (0)    15961 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/model/forbidden.py
+-rw-r--r--   0 root         (0) root         (0)    15991 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/model/internal_server_error.py
+-rw-r--r--   0 root         (0) root         (0)    15958 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/model/not_found.py
+-rw-r--r--   0 root         (0) root         (0)    16791 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/model/paginated_v1_beta1_photo_identifier_summary_list.py
+-rw-r--r--   0 root         (0) root         (0)    16619 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/model/paginated_v1_beta1_photo_list.py
+-rw-r--r--   0 root         (0) root         (0)    16028 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/model/permissions.py
+-rw-r--r--   0 root         (0) root         (0)    18732 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/model/photo_identifier.py
+-rw-r--r--   0 root         (0) root         (0)    16464 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/model/photo_identifier_bulk_update_request_request.py
+-rw-r--r--   0 root         (0) root         (0)    16412 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/model/photo_identifier_bulk_update_update_request.py
+-rw-r--r--   0 root         (0) root         (0)    19295 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/model/scheme_enum.py
+-rw-r--r--   0 root         (0) root         (0)    16889 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/model/status_enum.py
+-rw-r--r--   0 root         (0) root         (0)    16252 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/model/transient_image_url.py
+-rw-r--r--   0 root         (0) root         (0)    15970 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/model/unauthorized.py
+-rw-r--r--   0 root         (0) root         (0)    22401 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/model/v1_beta1_photo.py
+-rw-r--r--   0 root         (0) root         (0)    16599 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/model/v1_beta1_photo_identifier_summary.py
+-rw-r--r--   0 root         (0) root         (0)    16547 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/model/v1_beta1_photo_identifier_summary_request.py
+-rw-r--r--   0 root         (0) root         (0)    87097 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/model_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.839518 ucam-identitylib-1.5.0/identitylib/photo_client/models/
+-rw-r--r--   0 root         (0) root         (0)     2004 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18774 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/rest.py
+-rw-rw-rw-   0 root         (0) root         (0)      612 2023-03-30 12:19:13.000000 ucam-identitylib-1.5.0/identitylib/photo_client_configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.839518 ucam-identitylib-1.5.0/identitylib/student_client/
+-rw-r--r--   0 root         (0) root         (0)     2582 2023-04-21 08:32:30.000000 ucam-identitylib-1.5.0/identitylib/student_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.839518 ucam-identitylib-1.5.0/identitylib/student_client/api/
+-rw-r--r--   0 root         (0) root         (0)      231 2023-04-21 08:32:30.000000 ucam-identitylib-1.5.0/identitylib/student_client/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21826 2023-04-21 08:32:30.000000 ucam-identitylib-1.5.0/identitylib/student_client/api/students_api.py
+-rw-r--r--   0 root         (0) root         (0)    41093 2023-04-21 08:32:30.000000 ucam-identitylib-1.5.0/identitylib/student_client/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.839518 ucam-identitylib-1.5.0/identitylib/student_client/apis/
+-rw-r--r--   0 root         (0) root         (0)      509 2023-04-21 08:32:30.000000 ucam-identitylib-1.5.0/identitylib/student_client/apis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18407 2023-04-21 08:32:30.000000 ucam-identitylib-1.5.0/identitylib/student_client/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     6818 2023-04-21 08:32:30.000000 ucam-identitylib-1.5.0/identitylib/student_client/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.843518 ucam-identitylib-1.5.0/identitylib/student_client/model/
+-rw-r--r--   0 root         (0) root         (0)      360 2023-04-21 08:32:30.000000 ucam-identitylib-1.5.0/identitylib/student_client/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15305 2023-04-21 08:32:30.000000 ucam-identitylib-1.5.0/identitylib/student_client/model/affiliation.py
+-rw-r--r--   0 root         (0) root         (0)    14466 2023-04-21 08:32:30.000000 ucam-identitylib-1.5.0/identitylib/student_client/model/affiliation_scheme.py
+-rw-r--r--   0 root         (0) root         (0)    13235 2023-04-21 08:32:30.000000 ucam-identitylib-1.5.0/identitylib/student_client/model/http_exception.py
+-rw-r--r--   0 root         (0) root         (0)    13438 2023-04-21 08:32:30.000000 ucam-identitylib-1.5.0/identitylib/student_client/model/http_validation_error.py
+-rw-r--r--   0 root         (0) root         (0)    13725 2023-04-21 08:32:30.000000 ucam-identitylib-1.5.0/identitylib/student_client/model/identifier.py
+-rw-r--r--   0 root         (0) root         (0)    14035 2023-04-21 08:32:30.000000 ucam-identitylib-1.5.0/identitylib/student_client/model/identifier_scheme.py
+-rw-r--r--   0 root         (0) root         (0)    12993 2023-04-21 08:32:30.000000 ucam-identitylib-1.5.0/identitylib/student_client/model/location_inner.py
+-rw-r--r--   0 root         (0) root         (0)    14202 2023-04-21 08:32:30.000000 ucam-identitylib-1.5.0/identitylib/student_client/model/paginated_results_student.py
+-rw-r--r--   0 root         (0) root         (0)    16439 2023-04-21 08:32:30.000000 ucam-identitylib-1.5.0/identitylib/student_client/model/student.py
+-rw-r--r--   0 root         (0) root         (0)    13802 2023-04-21 08:32:30.000000 ucam-identitylib-1.5.0/identitylib/student_client/model/validation_error.py
+-rw-r--r--   0 root         (0) root         (0)    84357 2023-04-21 08:32:30.000000 ucam-identitylib-1.5.0/identitylib/student_client/model_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.843518 ucam-identitylib-1.5.0/identitylib/student_client/models/
+-rw-r--r--   0 root         (0) root         (0)     1150 2023-04-21 08:32:30.000000 ucam-identitylib-1.5.0/identitylib/student_client/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16034 2023-04-21 08:32:30.000000 ucam-identitylib-1.5.0/identitylib/student_client/rest.py
+-rw-rw-rw-   0 root         (0) root         (0)      646 2023-03-30 12:19:13.000000 ucam-identitylib-1.5.0/identitylib/university_hr_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)      648 2023-03-30 12:19:13.000000 ucam-identitylib-1.5.0/identitylib/university_student_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)       56 2023-04-05 11:43:13.000000 ucam-identitylib-1.5.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-21 08:32:42.843518 ucam-identitylib-1.5.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1529 2023-04-20 15:51:40.000000 ucam-identitylib-1.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.843518 ucam-identitylib-1.5.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-21 08:31:53.000000 ucam-identitylib-1.5.0/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5517 2023-03-30 12:19:13.000000 ucam-identitylib-1.5.0/tests/test_api_client_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     3449 2023-03-30 12:19:13.000000 ucam-identitylib-1.5.0/tests/test_identifiers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.843518 ucam-identitylib-1.5.0/ucam_identitylib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2699 2023-04-21 08:32:42.000000 ucam-identitylib-1.5.0/ucam_identitylib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12331 2023-04-21 08:32:42.000000 ucam-identitylib-1.5.0/ucam_identitylib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 08:32:42.000000 ucam-identitylib-1.5.0/ucam_identitylib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2023-04-21 08:32:42.000000 ucam-identitylib-1.5.0/ucam_identitylib.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-04-21 08:32:42.000000 ucam-identitylib-1.5.0/ucam_identitylib.egg-info/top_level.txt
```

### Comparing `ucam-identitylib-1.4.0/PKG-INFO` & `ucam-identitylib-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ucam-identitylib
-Version: 1.4.0
+Version: 1.5.0
 Summary: A module containing helpers and shared code related to identity systems within UIS, University of Cambridge.
 Home-page: https://gitlab.developers.cam.ac.uk/uis/devops/iam/identity-lib
 Author: University of Cambridge Information Services
 Author-email: devops+ucam-identitylib@uis.cam.ac.uk
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ucam-identitylib-1.4.0/README.md` & `ucam-identitylib-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/api_client_mixin.py` & `ucam-identitylib-1.5.0/identitylib/api_client_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             and self._access_token_expires_at is not None
             and
             # ensure that our access token is still valid - with a leeway of 20 seconds
             now < (self._access_token_expires_at - timedelta(seconds=20))
         ):
             return self._access_token
 
-        LOG.info("Refreshing API Gateway access token")
+        LOG.debug("Refreshing API Gateway access token")
 
         auth = requests.auth.HTTPBasicAuth(self.client_key, self.client_secret)
         data = {"grant_type": "client_credentials"}
 
         response = requests.post(self.access_token_url, data=data, auth=auth)
         if (
             response.status_code >= 300
```

### Comparing `ucam-identitylib-1.4.0/identitylib/card_client/__init__.py` & `ucam-identitylib-1.5.0/identitylib/card_client/__init__.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/card_client/api/permissions_api.py` & `ucam-identitylib-1.5.0/identitylib/card_client/api/permissions_api.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/card_client/api/v1beta1_api.py` & `ucam-identitylib-1.5.0/identitylib/card_client/api/v1beta1_api.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/card_client/api/versions_api.py` & `ucam-identitylib-1.5.0/identitylib/card_client/api/versions_api.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/card_client/api_client.py` & `ucam-identitylib-1.5.0/identitylib/card_client/api_client.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/card_client/apis/__init__.py` & `ucam-identitylib-1.5.0/identitylib/card_client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/card_client/configuration.py` & `ucam-identitylib-1.5.0/identitylib/card_client/configuration.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/card_client/exceptions.py` & `ucam-identitylib-1.5.0/identitylib/card_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/card_client/model/api_exception.py` & `ucam-identitylib-1.5.0/identitylib/card_client/model/api_exception.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/card_client/model/available_barcode.py` & `ucam-identitylib-1.5.0/identitylib/card_client/model/available_barcode.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/card_client/model/available_barcode_batch_request_type.py` & `ucam-identitylib-1.5.0/identitylib/card_client/model/available_barcode_batch_request_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/card_client/model/available_barcode_batch_response_type.py` & `ucam-identitylib-1.5.0/identitylib/card_client/model/available_barcode_batch_response_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/card_client/model/available_barcode_batch_response_type_details.py` & `ucam-identitylib-1.5.0/identitylib/card_client/model/available_barcode_batch_response_type_details.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/card_client/model/available_barcode_batch_response_type_details_invalid_inner.py` & `ucam-identitylib-1.5.0/identitylib/card_client/model/available_barcode_batch_response_type_details_invalid_inner.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/card_client/model/available_barcode_create_request_type.py` & `ucam-identitylib-1.5.0/identitylib/card_client/model/available_barcode_create_request_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/card_client/model/card.py` & `ucam-identitylib-1.5.0/identitylib/card_client/model/card.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/card_client/model/card_filter_request_type.py` & `ucam-identitylib-1.5.0/identitylib/card_client/model/card_filter_request_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/card_client/model/card_filter_response_type.py` & `ucam-identitylib-1.5.0/identitylib/card_client/model/card_filter_response_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/card_client/model/card_identifier.py` & `ucam-identitylib-1.5.0/identitylib/card_client/model/card_identifier.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/card_client/model/card_identifier_bulk_update_request_type.py` & `ucam-identitylib-1.5.0/identitylib/card_client/model/card_identifier_bulk_update_request_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/card_client/model/card_identifier_bulk_update_request_type_updates_inner.py` & `ucam-identitylib-1.5.0/identitylib/card_client/model/card_identifier_bulk_update_request_type_updates_inner.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/card_client/model/card_identifier_bulk_update_response_type.py` & `ucam-identitylib-1.5.0/identitylib/card_client/model/card_identifier_bulk_update_response_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/card_client/model/card_identifier_bulk_update_response_type_details_inner.py` & `ucam-identitylib-1.5.0/identitylib/card_client/model/card_identifier_bulk_update_response_type_details_inner.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/card_client/model/card_identifier_destroy_response_type.py` & `ucam-identitylib-1.5.0/identitylib/card_client/model/card_identifier_destroy_response_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/card_client/model/card_identifier_update_request_type.py` & `ucam-identitylib-1.5.0/identitylib/card_client/model/card_identifier_update_request_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/card_client/model/card_identifier_update_response_type.py` & `ucam-identitylib-1.5.0/identitylib/card_client/model/card_identifier_update_response_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/card_client/model/card_logo.py` & `ucam-identitylib-1.5.0/identitylib/card_client/model/card_logo.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/card_client/model/card_note.py` & `ucam-identitylib-1.5.0/identitylib/card_client/model/card_note.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/card_client/model/card_note_create_request_type.py` & `ucam-identitylib-1.5.0/identitylib/card_client/model/card_note_create_request_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/card_client/model/card_note_destroy_request_type.py` & `ucam-identitylib-1.5.0/identitylib/card_client/model/card_note_destroy_request_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/card_client/model/card_note_destroy_response_type.py` & `ucam-identitylib-1.5.0/identitylib/card_client/model/card_note_destroy_response_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/card_client/model/card_request.py` & `ucam-identitylib-1.5.0/identitylib/card_client/model/card_request.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/card_client/model/card_request_bulk_update_request_type.py` & `ucam-identitylib-1.5.0/identitylib/card_client/model/card_request_bulk_update_request_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/card_client/model/card_request_bulk_update_request_type_updates_inner.py` & `ucam-identitylib-1.5.0/identitylib/card_client/model/card_request_bulk_update_request_type_updates_inner.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/card_client/model/card_request_bulk_update_request_type_updates_inner_fields.py` & `ucam-identitylib-1.5.0/identitylib/card_client/model/card_request_bulk_update_request_type_updates_inner_fields.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/card_client/model/card_request_bulk_update_request_type_updates_inner_identifiers_inner.py` & `ucam-identitylib-1.5.0/identitylib/card_client/model/card_request_bulk_update_request_type_updates_inner_identifiers_inner.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/card_client/model/card_request_bulk_update_response_type.py` & `ucam-identitylib-1.5.0/identitylib/card_client/model/card_request_bulk_update_response_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/card_client/model/card_request_create_request_type.py` & `ucam-identitylib-1.5.0/identitylib/card_client/model/card_request_create_request_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/card_client/model/card_request_distinct_values.py` & `ucam-identitylib-1.5.0/identitylib/card_client/model/card_request_distinct_values.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/card_client/model/card_request_summary.py` & `ucam-identitylib-1.5.0/identitylib/card_client/model/card_request_summary.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/card_client/model/card_request_update_request_type.py` & `ucam-identitylib-1.5.0/identitylib/card_client/model/card_request_update_request_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/card_client/model/card_request_update_response_type.py` & `ucam-identitylib-1.5.0/identitylib/card_client/model/card_request_update_response_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/card_client/model/card_rfid_data_config_list_response_type.py` & `ucam-identitylib-1.5.0/identitylib/card_client/model/card_rfid_data_config_list_response_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/card_client/model/card_rfid_data_config_list_response_type_results_inner.py` & `ucam-identitylib-1.5.0/identitylib/card_client/model/card_rfid_data_config_list_response_type_results_inner.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/card_client/model/card_summary.py` & `ucam-identitylib-1.5.0/identitylib/card_client/model/card_summary.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/card_client/model/card_update_request_type.py` & `ucam-identitylib-1.5.0/identitylib/card_client/model/card_update_request_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/card_client/model/card_update_response_type.py` & `ucam-identitylib-1.5.0/identitylib/card_client/model/card_update_response_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/card_client/model/college_institution_ids_list_response_type.py` & `ucam-identitylib-1.5.0/identitylib/card_client/model/college_institution_ids_list_response_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/card_client/model/paginated_available_barcode_type.py` & `ucam-identitylib-1.5.0/identitylib/card_client/model/paginated_available_barcode_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/card_client/model/paginated_card_identifier_type.py` & `ucam-identitylib-1.5.0/identitylib/card_client/model/paginated_card_identifier_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/card_client/model/paginated_card_logo_type.py` & `ucam-identitylib-1.5.0/identitylib/card_client/model/paginated_card_logo_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/card_client/model/paginated_card_note_type.py` & `ucam-identitylib-1.5.0/identitylib/card_client/model/paginated_card_note_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/card_client/model/paginated_card_request_summary_type.py` & `ucam-identitylib-1.5.0/identitylib/card_client/model/paginated_card_request_summary_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/card_client/model/paginated_card_summary_type.py` & `ucam-identitylib-1.5.0/identitylib/card_client/model/paginated_card_summary_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/card_client/model/permissions_response_type.py` & `ucam-identitylib-1.5.0/identitylib/card_client/model/permissions_response_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/card_client/model/validation_error.py` & `ucam-identitylib-1.5.0/identitylib/card_client/model/validation_error.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/card_client/model/version_response_type.py` & `ucam-identitylib-1.5.0/identitylib/card_client/model/version_response_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/card_client/model_utils.py` & `ucam-identitylib-1.5.0/identitylib/card_client/model_utils.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/card_client/models/__init__.py` & `ucam-identitylib-1.5.0/identitylib/card_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/card_client/rest.py` & `ucam-identitylib-1.5.0/identitylib/card_client/rest.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/card_client_configuration.py` & `ucam-identitylib-1.5.0/identitylib/card_client_configuration.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/hr_client/__init__.py` & `ucam-identitylib-1.5.0/identitylib/hr_client/__init__.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/hr_client/api/staff_members_api.py` & `ucam-identitylib-1.5.0/identitylib/hr_client/api/staff_members_api.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/hr_client/api_client.py` & `ucam-identitylib-1.5.0/identitylib/hr_client/api_client.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/hr_client/apis/__init__.py` & `ucam-identitylib-1.5.0/identitylib/hr_client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/hr_client/configuration.py` & `ucam-identitylib-1.5.0/identitylib/hr_client/configuration.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/hr_client/exceptions.py` & `ucam-identitylib-1.5.0/identitylib/hr_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/hr_client/model/affiliation.py` & `ucam-identitylib-1.5.0/identitylib/hr_client/model/affiliation.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/hr_client/model/affiliation_scheme.py` & `ucam-identitylib-1.5.0/identitylib/hr_client/model/affiliation_scheme.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/hr_client/model/http_exception.py` & `ucam-identitylib-1.5.0/identitylib/hr_client/model/http_exception.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/hr_client/model/http_validation_error.py` & `ucam-identitylib-1.5.0/identitylib/hr_client/model/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/hr_client/model/identifier.py` & `ucam-identitylib-1.5.0/identitylib/hr_client/model/identifier.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/hr_client/model/identifier_scheme.py` & `ucam-identitylib-1.5.0/identitylib/hr_client/model/identifier_scheme.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/hr_client/model/location_inner.py` & `ucam-identitylib-1.5.0/identitylib/hr_client/model/location_inner.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/hr_client/model/paginated_results_staff_member.py` & `ucam-identitylib-1.5.0/identitylib/hr_client/model/paginated_results_staff_member.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/hr_client/model/staff_member.py` & `ucam-identitylib-1.5.0/identitylib/hr_client/model/staff_member.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/hr_client/model/validation_error.py` & `ucam-identitylib-1.5.0/identitylib/hr_client/model/validation_error.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/hr_client/model_utils.py` & `ucam-identitylib-1.5.0/identitylib/hr_client/model_utils.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/hr_client/models/__init__.py` & `ucam-identitylib-1.5.0/identitylib/hr_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/hr_client/rest.py` & `ucam-identitylib-1.5.0/identitylib/hr_client/rest.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/identifiers.py` & `ucam-identitylib-1.5.0/identitylib/identifiers.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/inst_identifier_client/__init__.py` & `ucam-identitylib-1.5.0/identitylib/inst_identifier_client/__init__.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/inst_identifier_client/api/default_api.py` & `ucam-identitylib-1.5.0/identitylib/inst_identifier_client/api/default_api.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/inst_identifier_client/api_client.py` & `ucam-identitylib-1.5.0/identitylib/inst_identifier_client/api_client.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/inst_identifier_client/apis/__init__.py` & `ucam-identitylib-1.5.0/identitylib/inst_identifier_client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/inst_identifier_client/configuration.py` & `ucam-identitylib-1.5.0/identitylib/inst_identifier_client/configuration.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/inst_identifier_client/exceptions.py` & `ucam-identitylib-1.5.0/identitylib/inst_identifier_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/inst_identifier_client/model/mapping_datum.py` & `ucam-identitylib-1.5.0/identitylib/inst_identifier_client/model/mapping_datum.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/inst_identifier_client/model/mapping_response.py` & `ucam-identitylib-1.5.0/identitylib/inst_identifier_client/model/mapping_response.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/inst_identifier_client/model_utils.py` & `ucam-identitylib-1.5.0/identitylib/inst_identifier_client/model_utils.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/inst_identifier_client/models/__init__.py` & `ucam-identitylib-1.5.0/identitylib/inst_identifier_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/inst_identifier_client/rest.py` & `ucam-identitylib-1.5.0/identitylib/inst_identifier_client/rest.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/inst_identifier_configuration.py` & `ucam-identitylib-1.5.0/identitylib/inst_identifier_configuration.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/lookup_client/__init__.py` & `ucam-identitylib-1.5.0/identitylib/lookup_client/__init__.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/lookup_client/api/group_api.py` & `ucam-identitylib-1.5.0/identitylib/lookup_client/api/group_api.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/lookup_client/api/ibis_api.py` & `ucam-identitylib-1.5.0/identitylib/lookup_client/api/ibis_api.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/lookup_client/api/institution_api.py` & `ucam-identitylib-1.5.0/identitylib/lookup_client/api/institution_api.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/lookup_client/api/person_api.py` & `ucam-identitylib-1.5.0/identitylib/lookup_client/api/person_api.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/lookup_client/api_client.py` & `ucam-identitylib-1.5.0/identitylib/lookup_client/api_client.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/lookup_client/apis/__init__.py` & `ucam-identitylib-1.5.0/identitylib/lookup_client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/lookup_client/configuration.py` & `ucam-identitylib-1.5.0/identitylib/lookup_client/configuration.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/lookup_client/exceptions.py` & `ucam-identitylib-1.5.0/identitylib/lookup_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/lookup_client/model/attribute.py` & `ucam-identitylib-1.5.0/identitylib/lookup_client/model/attribute.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/lookup_client/model/attribute_scheme.py` & `ucam-identitylib-1.5.0/identitylib/lookup_client/model/attribute_scheme.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/lookup_client/model/contact_phone_number.py` & `ucam-identitylib-1.5.0/identitylib/lookup_client/model/contact_phone_number.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/lookup_client/model/contact_row.py` & `ucam-identitylib-1.5.0/identitylib/lookup_client/model/contact_row.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/lookup_client/model/contact_web_page.py` & `ucam-identitylib-1.5.0/identitylib/lookup_client/model/contact_web_page.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/lookup_client/model/error.py` & `ucam-identitylib-1.5.0/identitylib/lookup_client/model/error.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/lookup_client/model/group.py` & `ucam-identitylib-1.5.0/identitylib/lookup_client/model/group.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/lookup_client/model/group_all_groups200_response.py` & `ucam-identitylib-1.5.0/identitylib/lookup_client/model/group_all_groups200_response.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/lookup_client/model/group_all_groups200_response_result.py` & `ucam-identitylib-1.5.0/identitylib/lookup_client/model/group_all_groups200_response_result.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/lookup_client/model/group_all_groups_default_response.py` & `ucam-identitylib-1.5.0/identitylib/lookup_client/model/group_all_groups_default_response.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/lookup_client/model/group_all_groups_default_response_result.py` & `ucam-identitylib-1.5.0/identitylib/lookup_client/model/group_all_groups_default_response_result.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/lookup_client/model/group_get_cancelled_members200_response.py` & `ucam-identitylib-1.5.0/identitylib/lookup_client/model/group_get_cancelled_members200_response.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/lookup_client/model/group_get_cancelled_members200_response_result.py` & `ucam-identitylib-1.5.0/identitylib/lookup_client/model/group_get_cancelled_members200_response_result.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/lookup_client/model/group_get_group200_response.py` & `ucam-identitylib-1.5.0/identitylib/lookup_client/model/group_get_group200_response.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/lookup_client/model/group_get_group200_response_result.py` & `ucam-identitylib-1.5.0/identitylib/lookup_client/model/group_get_group200_response_result.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/lookup_client/model/group_members_of_inst.py` & `ucam-identitylib-1.5.0/identitylib/lookup_client/model/group_members_of_inst.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/lookup_client/model/group_search_count200_response.py` & `ucam-identitylib-1.5.0/identitylib/lookup_client/model/group_search_count200_response.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/lookup_client/model/group_search_count200_response_result.py` & `ucam-identitylib-1.5.0/identitylib/lookup_client/model/group_search_count200_response_result.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/lookup_client/model/ibis_get_last_transaction_id200_response.py` & `ucam-identitylib-1.5.0/identitylib/lookup_client/model/ibis_get_last_transaction_id200_response.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/lookup_client/model/ibis_get_last_transaction_id200_response_result.py` & `ucam-identitylib-1.5.0/identitylib/lookup_client/model/ibis_get_last_transaction_id200_response_result.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/lookup_client/model/ibis_get_version200_response.py` & `ucam-identitylib-1.5.0/identitylib/lookup_client/model/ibis_get_version200_response.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/lookup_client/model/ibis_get_version200_response_result.py` & `ucam-identitylib-1.5.0/identitylib/lookup_client/model/ibis_get_version200_response_result.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/lookup_client/model/identifier.py` & `ucam-identitylib-1.5.0/identitylib/lookup_client/model/identifier.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/lookup_client/model/institution.py` & `ucam-identitylib-1.5.0/identitylib/lookup_client/model/institution.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/lookup_client/model/institution_all_attribute_schemes200_response.py` & `ucam-identitylib-1.5.0/identitylib/lookup_client/model/institution_all_attribute_schemes200_response.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/lookup_client/model/institution_all_attribute_schemes200_response_result.py` & `ucam-identitylib-1.5.0/identitylib/lookup_client/model/institution_all_attribute_schemes200_response_result.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/lookup_client/model/institution_all_insts200_response.py` & `ucam-identitylib-1.5.0/identitylib/lookup_client/model/institution_all_insts200_response.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/lookup_client/model/institution_all_insts200_response_result.py` & `ucam-identitylib-1.5.0/identitylib/lookup_client/model/institution_all_insts200_response_result.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/lookup_client/model/institution_get_attribute200_response.py` & `ucam-identitylib-1.5.0/identitylib/lookup_client/model/institution_get_attribute200_response.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/lookup_client/model/institution_get_attribute200_response_result.py` & `ucam-identitylib-1.5.0/identitylib/lookup_client/model/institution_get_attribute200_response_result.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/lookup_client/model/institution_get_attributes200_response.py` & `ucam-identitylib-1.5.0/identitylib/lookup_client/model/institution_get_attributes200_response.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/lookup_client/model/institution_get_attributes200_response_result.py` & `ucam-identitylib-1.5.0/identitylib/lookup_client/model/institution_get_attributes200_response_result.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/lookup_client/model/institution_get_contact_rows200_response.py` & `ucam-identitylib-1.5.0/identitylib/lookup_client/model/institution_get_contact_rows200_response.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/lookup_client/model/institution_get_contact_rows200_response_result.py` & `ucam-identitylib-1.5.0/identitylib/lookup_client/model/institution_get_contact_rows200_response_result.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/lookup_client/model/institution_get_inst200_response.py` & `ucam-identitylib-1.5.0/identitylib/lookup_client/model/institution_get_inst200_response.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/lookup_client/model/institution_get_inst200_response_result.py` & `ucam-identitylib-1.5.0/identitylib/lookup_client/model/institution_get_inst200_response_result.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/lookup_client/model/person.py` & `ucam-identitylib-1.5.0/identitylib/lookup_client/model/person.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/lookup_client/model/person_get_person200_response.py` & `ucam-identitylib-1.5.0/identitylib/lookup_client/model/person_get_person200_response.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/lookup_client/model/person_get_person200_response_result.py` & `ucam-identitylib-1.5.0/identitylib/lookup_client/model/person_get_person200_response_result.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/lookup_client/model/person_identifier.py` & `ucam-identitylib-1.5.0/identitylib/lookup_client/model/person_identifier.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/lookup_client/model/person_is_member_of_group200_response.py` & `ucam-identitylib-1.5.0/identitylib/lookup_client/model/person_is_member_of_group200_response.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/lookup_client/model/person_is_member_of_group200_response_result.py` & `ucam-identitylib-1.5.0/identitylib/lookup_client/model/person_is_member_of_group200_response_result.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/lookup_client/model_utils.py` & `ucam-identitylib-1.5.0/identitylib/lookup_client/model_utils.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/lookup_client/models/__init__.py` & `ucam-identitylib-1.5.0/identitylib/lookup_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/lookup_client/rest.py` & `ucam-identitylib-1.5.0/identitylib/lookup_client/rest.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/lookup_client_configuration.py` & `ucam-identitylib-1.5.0/identitylib/lookup_client_configuration.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/photo_client/__init__.py` & `ucam-identitylib-1.5.0/identitylib/photo_client/__init__.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/photo_client/api/all_photos_api.py` & `ucam-identitylib-1.5.0/identitylib/photo_client/api/all_photos_api.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/photo_client/api/api_versions_api.py` & `ucam-identitylib-1.5.0/identitylib/photo_client/api/api_versions_api.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/photo_client/api/approved_photos_api.py` & `ucam-identitylib-1.5.0/identitylib/photo_client/api/approved_photos_api.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/photo_client/api/permissions_api.py` & `ucam-identitylib-1.5.0/identitylib/photo_client/api/permissions_api.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/photo_client/api/photo_identifier_api.py` & `ucam-identitylib-1.5.0/identitylib/photo_client/api/photo_identifier_api.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/photo_client/api/photo_identifiers_api.py` & `ucam-identitylib-1.5.0/identitylib/photo_client/api/photo_identifiers_api.py`

 * *Files 15% similar despite different names*

```diff
@@ -23,16 +23,17 @@
     validate_and_convert_types
 )
 from identitylib.photo_client.model.bad_request import BadRequest
 from identitylib.photo_client.model.forbidden import Forbidden
 from identitylib.photo_client.model.internal_server_error import InternalServerError
 from identitylib.photo_client.model.not_found import NotFound
 from identitylib.photo_client.model.paginated_v1_beta1_photo_identifier_summary_list import PaginatedV1Beta1PhotoIdentifierSummaryList
-from identitylib.photo_client.model.patched_v1_beta1_photo_identifier_summary_request import PatchedV1Beta1PhotoIdentifierSummaryRequest
+from identitylib.photo_client.model.photo_identifier_bulk_update_request_request import PhotoIdentifierBulkUpdateRequestRequest
 from identitylib.photo_client.model.unauthorized import Unauthorized
+from identitylib.photo_client.model.v1_beta1_photo_identifier_summary_request import V1Beta1PhotoIdentifierSummaryRequest
 
 
 class PhotoIdentifiersApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -58,14 +59,15 @@
                 'all': [
                     'cursor',
                     'deleted_at__gte',
                     'deleted_at__is_null',
                     'deleted_at__isnull',
                     'deleted_at__lte',
                     'identifier',
+                    'is_highest_primary_identifier',
                     'page_size',
                     'retain_until__gte',
                     'retain_until__is_null',
                     'retain_until__isnull',
                     'retain_until__lte',
                     'scheme',
                 ],
@@ -91,14 +93,16 @@
                         (bool,),
                     'deleted_at__isnull':
                         (bool,),
                     'deleted_at__lte':
                         (str,),
                     'identifier':
                         (str,),
+                    'is_highest_primary_identifier':
+                        (bool,),
                     'page_size':
                         (int,),
                     'retain_until__gte':
                         (str,),
                     'retain_until__is_null':
                         (bool,),
                     'retain_until__isnull':
@@ -111,28 +115,30 @@
                 'attribute_map': {
                     'cursor': 'cursor',
                     'deleted_at__gte': 'deleted_at__gte',
                     'deleted_at__is_null': 'deleted_at__isNull',
                     'deleted_at__isnull': 'deleted_at__isnull',
                     'deleted_at__lte': 'deleted_at__lte',
                     'identifier': 'identifier',
+                    'is_highest_primary_identifier': 'is_highest_primary_identifier',
                     'page_size': 'pageSize',
                     'retain_until__gte': 'retain_until__gte',
                     'retain_until__is_null': 'retain_until__isNull',
                     'retain_until__isnull': 'retain_until__isnull',
                     'retain_until__lte': 'retain_until__lte',
                     'scheme': 'scheme',
                 },
                 'location_map': {
                     'cursor': 'query',
                     'deleted_at__gte': 'query',
                     'deleted_at__is_null': 'query',
                     'deleted_at__isnull': 'query',
                     'deleted_at__lte': 'query',
                     'identifier': 'query',
+                    'is_highest_primary_identifier': 'query',
                     'page_size': 'query',
                     'retain_until__gte': 'query',
                     'retain_until__is_null': 'query',
                     'retain_until__isnull': 'query',
                     'retain_until__lte': 'query',
                     'scheme': 'query',
                 },
@@ -143,34 +149,35 @@
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.v1beta1_photo_identifiers_partial_update_endpoint = _Endpoint(
+        self.v1beta1_photo_identifiers_update_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
                     'apiGatewayAuthorizationCodeSecurityScheme',
                     'apiGatewayClientCredentialsSecurityScheme'
                 ],
                 'endpoint_path': '/v1beta1/photo-identifiers/{id}',
-                'operation_id': 'v1beta1_photo_identifiers_partial_update',
-                'http_method': 'PATCH',
+                'operation_id': 'v1beta1_photo_identifiers_update',
+                'http_method': 'PUT',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
+                    'v1_beta1_photo_identifier_summary_request',
                     'action',
-                    'patched_v1_beta1_photo_identifier_summary_request',
                 ],
                 'required': [
                     'id',
+                    'v1_beta1_photo_identifier_summary_request',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                     'action',
                 ],
                 'validation': [
@@ -180,33 +187,89 @@
                 'validations': {
                 },
                 'allowed_values': {
                     ('action',): {
 
                         "HARD_DELETE": "hard_delete",
                         "RESTORE": "restore",
-                        "SET_RETENTION": "set_retention"
+                        "SET_RETENTION": "set_retention",
+                        "SOFT_DELETE": "soft_delete"
                     },
                 },
                 'openapi_types': {
                     'id':
                         (str,),
+                    'v1_beta1_photo_identifier_summary_request':
+                        (V1Beta1PhotoIdentifierSummaryRequest,),
                     'action':
                         (str,),
-                    'patched_v1_beta1_photo_identifier_summary_request':
-                        (PatchedV1Beta1PhotoIdentifierSummaryRequest,),
                 },
                 'attribute_map': {
                     'id': 'id',
                     'action': 'action',
                 },
                 'location_map': {
                     'id': 'path',
+                    'v1_beta1_photo_identifier_summary_request': 'body',
                     'action': 'query',
-                    'patched_v1_beta1_photo_identifier_summary_request': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json',
+                    'application/x-www-form-urlencoded',
+                    'multipart/form-data'
+                ]
+            },
+            api_client=api_client
+        )
+        self.v1beta1_photo_identifiers_update_update_endpoint = _Endpoint(
+            settings={
+                'response_type': None,
+                'auth': [
+                    'apiGatewayAuthorizationCodeSecurityScheme',
+                    'apiGatewayClientCredentialsSecurityScheme'
+                ],
+                'endpoint_path': '/v1beta1/photo-identifiers/update',
+                'operation_id': 'v1beta1_photo_identifiers_update_update',
+                'http_method': 'PUT',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'photo_identifier_bulk_update_request_request',
+                ],
+                'required': [
+                    'photo_identifier_bulk_update_request_request',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'photo_identifier_bulk_update_request_request':
+                        (PhotoIdentifierBulkUpdateRequestRequest,),
+                },
+                'attribute_map': {
+                },
+                'location_map': {
+                    'photo_identifier_bulk_update_request_request': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
@@ -237,14 +300,15 @@
         Keyword Args:
             cursor (str): The pagination cursor value.. [optional]
             deleted_at__gte (str): Filter deletedAt by IsoDateTime greater than. [optional]
             deleted_at__is_null (bool): Filter deletedAt by IsoDateTime is Null. [optional]
             deleted_at__isnull (bool): [optional]
             deleted_at__lte (str): Filter deletedAt by IsoDateTime less than. [optional]
             identifier (str): PhotoIdentifier to get photos for using format `<value>@<scheme>`. [optional]
+            is_highest_primary_identifier (bool): Filter is_highest_primary_identifier. [optional]
             page_size (int): Number of results to return per page.. [optional]
             retain_until__gte (str): Filter retainUntil by IsoDateTime greater than. [optional]
             retain_until__is_null (bool): Filter retainUntil by IsoDateTime is Null. [optional]
             retain_until__isnull (bool): [optional]
             retain_until__lte (str): Filter retainUntil by IsoDateTime less than. [optional]
             scheme (str): PhotoIdentifier scheme to get photos for using format `<scheme>`. [optional]
             _return_http_data_only (bool): response data without head status
@@ -306,34 +370,35 @@
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         return self.v1beta1_photo_identifiers_list_endpoint.call_with_http_info(**kwargs)
 
-    def v1beta1_photo_identifiers_partial_update(
+    def v1beta1_photo_identifiers_update(
         self,
         id,
+        v1_beta1_photo_identifier_summary_request,
         **kwargs
     ):
         """Update a photo identifier by photo identifier UUID.  # noqa: E501
 
-         ## Update the photo identifier  This method allows a client to submit an action in the request query for a given photo identifier. The allowed actions are `set_retention`, `restore` and `hard_delete`.  ### Permissions  Principals with the `CARD_ADMIN` permission will be able to affect this endpoint.    # noqa: E501
+         ## Update the photo identifier  This method allows a client to submit an action in the request query for a given photo identifier. The allowed actions are `set_retention`, `restore`, `soft_delete` and `hard_delete`.  ### Permissions  Principals with the `CARD_ADMIN` permission will be able to affect this endpoint.    # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.v1beta1_photo_identifiers_partial_update(id, async_req=True)
+        >>> thread = api.v1beta1_photo_identifiers_update(id, v1_beta1_photo_identifier_summary_request, async_req=True)
         >>> result = thread.get()
 
         Args:
             id (str): A UUID string identifying this photo identifier.
+            v1_beta1_photo_identifier_summary_request (V1Beta1PhotoIdentifierSummaryRequest):
 
         Keyword Args:
             action (str): Action applied to the photo identifier.. [optional]
-            patched_v1_beta1_photo_identifier_summary_request (PatchedV1Beta1PhotoIdentifierSummaryRequest): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -389,9 +454,94 @@
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['id'] = \
             id
-        return self.v1beta1_photo_identifiers_partial_update_endpoint.call_with_http_info(**kwargs)
+        kwargs['v1_beta1_photo_identifier_summary_request'] = \
+            v1_beta1_photo_identifier_summary_request
+        return self.v1beta1_photo_identifiers_update_endpoint.call_with_http_info(**kwargs)
+
+    def v1beta1_photo_identifiers_update_update(
+        self,
+        photo_identifier_bulk_update_request_request,
+        **kwargs
+    ):
+        """Bulk update photo identifiers by photo identifier UUID.  # noqa: E501
+
+         ## Bulk update the photo identifier  This method allows a client to submit a list of photo identifiers and corresponding action to apply to the photo identifier. The allowed actions are `set_retention`, `restore`, `soft_delete` and `hard_delete`.  ### Permissions  Principals with the `CARD_ADMIN` permission will be able to affect this endpoint.    # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.v1beta1_photo_identifiers_update_update(photo_identifier_bulk_update_request_request, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            photo_identifier_bulk_update_request_request (PhotoIdentifierBulkUpdateRequestRequest):
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            None
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['photo_identifier_bulk_update_request_request'] = \
+            photo_identifier_bulk_update_request_request
+        return self.v1beta1_photo_identifiers_update_update_endpoint.call_with_http_info(**kwargs)
```

### Comparing `ucam-identitylib-1.4.0/identitylib/photo_client/api/photo_identifiers_including_photos_api.py` & `ucam-identitylib-1.5.0/identitylib/photo_client/api/photo_identifiers_including_photos_api.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/photo_client/api/photos_including_unapproved_photos_api.py` & `ucam-identitylib-1.5.0/identitylib/photo_client/api/photos_including_unapproved_photos_api.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/photo_client/api/unapproved_photos_api.py` & `ucam-identitylib-1.5.0/identitylib/photo_client/api/unapproved_photos_api.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/photo_client/api_client.py` & `ucam-identitylib-1.5.0/identitylib/photo_client/api_client.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/photo_client/apis/__init__.py` & `ucam-identitylib-1.5.0/identitylib/photo_client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/photo_client/configuration.py` & `ucam-identitylib-1.5.0/identitylib/photo_client/configuration.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/photo_client/exceptions.py` & `ucam-identitylib-1.5.0/identitylib/photo_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/photo_client/model/api_versions.py` & `ucam-identitylib-1.5.0/identitylib/photo_client/model/api_versions.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/photo_client/model/bad_request.py` & `ucam-identitylib-1.5.0/identitylib/photo_client/model/bad_request.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/photo_client/model/forbidden.py` & `ucam-identitylib-1.5.0/identitylib/photo_client/model/forbidden.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/photo_client/model/internal_server_error.py` & `ucam-identitylib-1.5.0/identitylib/photo_client/model/internal_server_error.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/photo_client/model/not_found.py` & `ucam-identitylib-1.5.0/identitylib/photo_client/model/not_found.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/photo_client/model/paginated_v1_beta1_photo_identifier_summary_list.py` & `ucam-identitylib-1.5.0/identitylib/photo_client/model/paginated_v1_beta1_photo_identifier_summary_list.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/photo_client/model/paginated_v1_beta1_photo_list.py` & `ucam-identitylib-1.5.0/identitylib/photo_client/model/paginated_v1_beta1_photo_list.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/photo_client/model/patched_v1_beta1_photo_identifier_summary_request.py` & `ucam-identitylib-1.5.0/identitylib/photo_client/model/v1_beta1_photo_identifier_summary.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 
 def lazy_import():
     from identitylib.photo_client.model.scheme_enum import SchemeEnum
     globals()['SchemeEnum'] = SchemeEnum
 
 
-class PatchedV1Beta1PhotoIdentifierSummaryRequest(ModelNormal):
+class V1Beta1PhotoIdentifierSummary(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -59,17 +59,14 @@
           as additional properties values.
     """
 
     allowed_values = {
     }
 
     validations = {
-        ('value',): {
-            'min_length': 1,
-        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
@@ -87,37 +84,45 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
+            'id': (str,),  # noqa: E501
             'scheme': (SchemeEnum,),  # noqa: E501
             'value': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
+        'id': 'id',  # noqa: E501
         'scheme': 'scheme',  # noqa: E501
         'value': 'value',  # noqa: E501
     }
 
     read_only_vars = {
+        'id',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """PatchedV1Beta1PhotoIdentifierSummaryRequest - a model defined in OpenAPI
+    def _from_openapi_data(cls, id, scheme, value, *args, **kwargs):  # noqa: E501
+        """V1Beta1PhotoIdentifierSummary - a model defined in OpenAPI
+
+        Args:
+            id (str):
+            scheme (SchemeEnum):
+            value (str): The identifier's value
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -142,16 +147,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            scheme (SchemeEnum): [optional]  # noqa: E501
-            value (str): The identifier's value. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -175,14 +178,17 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.id = id
+        self.scheme = scheme
+        self.value = value
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -195,16 +201,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """PatchedV1Beta1PhotoIdentifierSummaryRequest - a model defined in OpenAPI
+    def __init__(self, scheme, value, *args, **kwargs):  # noqa: E501
+        """V1Beta1PhotoIdentifierSummary - a model defined in OpenAPI
+
+            scheme (SchemeEnum):
+            value (str): The identifier's value
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -229,16 +238,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            scheme (SchemeEnum): [optional]  # noqa: E501
-            value (str): The identifier's value. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -260,14 +267,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.scheme = scheme
+        self.value = value
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `ucam-identitylib-1.4.0/identitylib/photo_client/model/permissions.py` & `ucam-identitylib-1.5.0/identitylib/photo_client/model/permissions.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/photo_client/model/photo_identifier.py` & `ucam-identitylib-1.5.0/identitylib/photo_client/model/photo_identifier.py`

 * *Files 3% similar despite different names*

```diff
@@ -93,14 +93,15 @@
             'id': (str,),  # noqa: E501
             'photos': ([str],),  # noqa: E501
             'related_identifiers': ([V1Beta1PhotoIdentifierSummary],),  # noqa: E501
             'scheme': (SchemeEnum,),  # noqa: E501
             'value': (str,),  # noqa: E501
             'deleted_at': (datetime, none_type,),  # noqa: E501
             'is_deleted': (bool,),  # noqa: E501
+            'is_highest_primary_identifier': (bool,),  # noqa: E501
             'retain_until': (datetime, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
@@ -109,14 +110,15 @@
         'id': 'id',  # noqa: E501
         'photos': 'photos',  # noqa: E501
         'related_identifiers': 'relatedIdentifiers',  # noqa: E501
         'scheme': 'scheme',  # noqa: E501
         'value': 'value',  # noqa: E501
         'deleted_at': 'deletedAt',  # noqa: E501
         'is_deleted': 'isDeleted',  # noqa: E501
+        'is_highest_primary_identifier': 'isHighestPrimaryIdentifier',  # noqa: E501
         'retain_until': 'retainUntil',  # noqa: E501
     }
 
     read_only_vars = {
         'id',  # noqa: E501
     }
 
@@ -163,14 +165,15 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             deleted_at (datetime, none_type): [optional]  # noqa: E501
             is_deleted (bool): [optional]  # noqa: E501
+            is_highest_primary_identifier (bool): Photo identifier is highest primary identifier. [optional]  # noqa: E501
             retain_until (datetime, none_type): If non-NULL, the minimum period the record should be retained. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -261,14 +264,15 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             deleted_at (datetime, none_type): [optional]  # noqa: E501
             is_deleted (bool): [optional]  # noqa: E501
+            is_highest_primary_identifier (bool): Photo identifier is highest primary identifier. [optional]  # noqa: E501
             retain_until (datetime, none_type): If non-NULL, the minimum period the record should be retained. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
```

### Comparing `ucam-identitylib-1.4.0/identitylib/photo_client/model/scheme_enum.py` & `ucam-identitylib-1.5.0/identitylib/photo_client/model/scheme_enum.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/photo_client/model/status_enum.py` & `ucam-identitylib-1.5.0/identitylib/photo_client/model/status_enum.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/photo_client/model/transient_image_url.py` & `ucam-identitylib-1.5.0/identitylib/photo_client/model/transient_image_url.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/photo_client/model/unauthorized.py` & `ucam-identitylib-1.5.0/identitylib/photo_client/model/unauthorized.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/photo_client/model/v1_beta1_photo.py` & `ucam-identitylib-1.5.0/identitylib/photo_client/model/v1_beta1_photo.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/photo_client/model/v1_beta1_photo_identifier_summary.py` & `ucam-identitylib-1.5.0/identitylib/photo_client/model/v1_beta1_photo_identifier_summary_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 
 def lazy_import():
     from identitylib.photo_client.model.scheme_enum import SchemeEnum
     globals()['SchemeEnum'] = SchemeEnum
 
 
-class V1Beta1PhotoIdentifierSummary(ModelNormal):
+class V1Beta1PhotoIdentifierSummaryRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -59,14 +59,17 @@
           as additional properties values.
     """
 
     allowed_values = {
     }
 
     validations = {
+        ('value',): {
+            'min_length': 1,
+        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
@@ -84,43 +87,39 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'id': (str,),  # noqa: E501
             'scheme': (SchemeEnum,),  # noqa: E501
             'value': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'id': 'id',  # noqa: E501
         'scheme': 'scheme',  # noqa: E501
         'value': 'value',  # noqa: E501
     }
 
     read_only_vars = {
-        'id',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, id, scheme, value, *args, **kwargs):  # noqa: E501
-        """V1Beta1PhotoIdentifierSummary - a model defined in OpenAPI
+    def _from_openapi_data(cls, scheme, value, *args, **kwargs):  # noqa: E501
+        """V1Beta1PhotoIdentifierSummaryRequest - a model defined in OpenAPI
 
         Args:
-            id (str):
             scheme (SchemeEnum):
             value (str): The identifier's value
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
@@ -178,15 +177,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.id = id
         self.scheme = scheme
         self.value = value
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
@@ -202,16 +200,17 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, scheme, value, *args, **kwargs):  # noqa: E501
-        """V1Beta1PhotoIdentifierSummary - a model defined in OpenAPI
+        """V1Beta1PhotoIdentifierSummaryRequest - a model defined in OpenAPI
 
+        Args:
             scheme (SchemeEnum):
             value (str): The identifier's value
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
```

### Comparing `ucam-identitylib-1.4.0/identitylib/photo_client/model_utils.py` & `ucam-identitylib-1.5.0/identitylib/photo_client/model_utils.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/photo_client/models/__init__.py` & `ucam-identitylib-1.5.0/identitylib/photo_client/models/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,22 +6,25 @@
 # to avoid this, import only the models that you directly need like:
 # from identitylib.photo_client.model.pet import Pet
 # or import this package, but before doing it, use:
 # import sys
 # sys.setrecursionlimit(n)
 
 from identitylib.photo_client.model.api_versions import APIVersions
+from identitylib.photo_client.model.action_enum import ActionEnum
 from identitylib.photo_client.model.bad_request import BadRequest
 from identitylib.photo_client.model.forbidden import Forbidden
 from identitylib.photo_client.model.internal_server_error import InternalServerError
 from identitylib.photo_client.model.not_found import NotFound
 from identitylib.photo_client.model.paginated_v1_beta1_photo_identifier_summary_list import PaginatedV1Beta1PhotoIdentifierSummaryList
 from identitylib.photo_client.model.paginated_v1_beta1_photo_list import PaginatedV1Beta1PhotoList
-from identitylib.photo_client.model.patched_v1_beta1_photo_identifier_summary_request import PatchedV1Beta1PhotoIdentifierSummaryRequest
 from identitylib.photo_client.model.permissions import Permissions
 from identitylib.photo_client.model.photo_identifier import PhotoIdentifier
+from identitylib.photo_client.model.photo_identifier_bulk_update_request_request import PhotoIdentifierBulkUpdateRequestRequest
+from identitylib.photo_client.model.photo_identifier_bulk_update_update_request import PhotoIdentifierBulkUpdateUpdateRequest
 from identitylib.photo_client.model.scheme_enum import SchemeEnum
 from identitylib.photo_client.model.status_enum import StatusEnum
 from identitylib.photo_client.model.transient_image_url import TransientImageUrl
 from identitylib.photo_client.model.unauthorized import Unauthorized
 from identitylib.photo_client.model.v1_beta1_photo import V1Beta1Photo
 from identitylib.photo_client.model.v1_beta1_photo_identifier_summary import V1Beta1PhotoIdentifierSummary
+from identitylib.photo_client.model.v1_beta1_photo_identifier_summary_request import V1Beta1PhotoIdentifierSummaryRequest
```

### Comparing `ucam-identitylib-1.4.0/identitylib/photo_client/rest.py` & `ucam-identitylib-1.5.0/identitylib/photo_client/rest.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/photo_client_configuration.py` & `ucam-identitylib-1.5.0/identitylib/photo_client_configuration.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/student_client/__init__.py` & `ucam-identitylib-1.5.0/identitylib/student_client/__init__.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/student_client/api/students_api.py` & `ucam-identitylib-1.5.0/identitylib/student_client/api/students_api.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/student_client/api_client.py` & `ucam-identitylib-1.5.0/identitylib/student_client/api_client.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/student_client/configuration.py` & `ucam-identitylib-1.5.0/identitylib/student_client/configuration.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/student_client/exceptions.py` & `ucam-identitylib-1.5.0/identitylib/student_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/student_client/model/affiliation.py` & `ucam-identitylib-1.5.0/identitylib/student_client/model/affiliation.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/student_client/model/affiliation_scheme.py` & `ucam-identitylib-1.5.0/identitylib/student_client/model/affiliation_scheme.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/student_client/model/http_exception.py` & `ucam-identitylib-1.5.0/identitylib/student_client/model/http_exception.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/student_client/model/http_validation_error.py` & `ucam-identitylib-1.5.0/identitylib/student_client/model/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/student_client/model/identifier.py` & `ucam-identitylib-1.5.0/identitylib/student_client/model/identifier.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/student_client/model/identifier_scheme.py` & `ucam-identitylib-1.5.0/identitylib/student_client/model/identifier_scheme.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/student_client/model/location_inner.py` & `ucam-identitylib-1.5.0/identitylib/student_client/model/location_inner.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/student_client/model/paginated_results_student.py` & `ucam-identitylib-1.5.0/identitylib/student_client/model/paginated_results_student.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/student_client/model/student.py` & `ucam-identitylib-1.5.0/identitylib/student_client/model/student.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/student_client/model/validation_error.py` & `ucam-identitylib-1.5.0/identitylib/student_client/model/validation_error.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/student_client/model_utils.py` & `ucam-identitylib-1.5.0/identitylib/student_client/model_utils.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/student_client/models/__init__.py` & `ucam-identitylib-1.5.0/identitylib/student_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/student_client/rest.py` & `ucam-identitylib-1.5.0/identitylib/student_client/rest.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/university_hr_configuration.py` & `ucam-identitylib-1.5.0/identitylib/university_hr_configuration.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/identitylib/university_student_configuration.py` & `ucam-identitylib-1.5.0/identitylib/university_student_configuration.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/setup.py` & `ucam-identitylib-1.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 PACKAGE_NAME = "ucam-identitylib"
 PACKAGE_DESCRIPTION = (
     "A module containing helpers and shared code related to identity systems within UIS, "
     "University of Cambridge."
 )
-PACKAGE_VERSION = "1.4.0"
+PACKAGE_VERSION = "1.5.0"
 PACKAGE_URL = "https://gitlab.developers.cam.ac.uk/uis/devops/iam/identity-lib"
 
 
 def load_requirements(file: str):
     """
     Load requirements file and return non-empty, non-comment lines with leading and trailing
     whitespace stripped.
```

### Comparing `ucam-identitylib-1.4.0/tests/test_api_client_mixin.py` & `ucam-identitylib-1.5.0/tests/test_api_client_mixin.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/tests/test_identifiers.py` & `ucam-identitylib-1.5.0/tests/test_identifiers.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.4.0/ucam_identitylib.egg-info/PKG-INFO` & `ucam-identitylib-1.5.0/ucam_identitylib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ucam-identitylib
-Version: 1.4.0
+Version: 1.5.0
 Summary: A module containing helpers and shared code related to identity systems within UIS, University of Cambridge.
 Home-page: https://gitlab.developers.cam.ac.uk/uis/devops/iam/identity-lib
 Author: University of Cambridge Information Services
 Author-email: devops+ucam-identitylib@uis.cam.ac.uk
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ucam-identitylib-1.4.0/ucam_identitylib.egg-info/SOURCES.txt` & `ucam-identitylib-1.5.0/ucam_identitylib.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -177,30 +177,33 @@
 identitylib/photo_client/api/photo_identifier_api.py
 identitylib/photo_client/api/photo_identifiers_api.py
 identitylib/photo_client/api/photo_identifiers_including_photos_api.py
 identitylib/photo_client/api/photos_including_unapproved_photos_api.py
 identitylib/photo_client/api/unapproved_photos_api.py
 identitylib/photo_client/apis/__init__.py
 identitylib/photo_client/model/__init__.py
+identitylib/photo_client/model/action_enum.py
 identitylib/photo_client/model/api_versions.py
 identitylib/photo_client/model/bad_request.py
 identitylib/photo_client/model/forbidden.py
 identitylib/photo_client/model/internal_server_error.py
 identitylib/photo_client/model/not_found.py
 identitylib/photo_client/model/paginated_v1_beta1_photo_identifier_summary_list.py
 identitylib/photo_client/model/paginated_v1_beta1_photo_list.py
-identitylib/photo_client/model/patched_v1_beta1_photo_identifier_summary_request.py
 identitylib/photo_client/model/permissions.py
 identitylib/photo_client/model/photo_identifier.py
+identitylib/photo_client/model/photo_identifier_bulk_update_request_request.py
+identitylib/photo_client/model/photo_identifier_bulk_update_update_request.py
 identitylib/photo_client/model/scheme_enum.py
 identitylib/photo_client/model/status_enum.py
 identitylib/photo_client/model/transient_image_url.py
 identitylib/photo_client/model/unauthorized.py
 identitylib/photo_client/model/v1_beta1_photo.py
 identitylib/photo_client/model/v1_beta1_photo_identifier_summary.py
+identitylib/photo_client/model/v1_beta1_photo_identifier_summary_request.py
 identitylib/photo_client/models/__init__.py
 identitylib/student_client/__init__.py
 identitylib/student_client/api_client.py
 identitylib/student_client/configuration.py
 identitylib/student_client/exceptions.py
 identitylib/student_client/model_utils.py
 identitylib/student_client/rest.py
```

