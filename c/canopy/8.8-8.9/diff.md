# Comparing `tmp/canopy-8.8.tar.gz` & `tmp/canopy-8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/canopy-8.8.tar", last modified: Wed Mar 11 10:29:31 2020, max compression
+gzip compressed data, was "dist/canopy-8.9.tar", last modified: Wed Mar 11 12:22:12 2020, max compression
```

## Comparing `canopy-8.8.tar` & `canopy-8.9.tar`

### file list

```diff
@@ -1,264 +1,264 @@
-drwxr-xr-x   0 vsts      (1001) docker     (115)        0 2020-03-11 10:29:31.000000 canopy-8.8/
--rw-r--r--   0 vsts      (1001) docker     (115)     9324 2020-03-11 10:29:31.000000 canopy-8.8/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (115)     7156 2020-03-11 10:29:10.000000 canopy-8.8/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (115)        0 2020-03-11 10:29:31.000000 canopy-8.8/canopy/
--rw-r--r--   0 vsts      (1001) docker     (115)     2858 2020-03-11 10:29:10.000000 canopy-8.8/canopy/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (115)     3754 2020-03-11 10:29:10.000000 canopy-8.8/canopy/authentication.py
--rw-r--r--   0 vsts      (1001) docker     (115)      966 2020-03-11 10:29:10.000000 canopy-8.8/canopy/authentication_data.py
--rw-r--r--   0 vsts      (1001) docker     (115)     2214 2020-03-11 10:29:10.000000 canopy-8.8/canopy/config_result.py
--rw-r--r--   0 vsts      (1001) docker     (115)      115 2020-03-11 10:29:10.000000 canopy-8.8/canopy/constants.py
--rw-r--r--   0 vsts      (1001) docker     (115)     1051 2020-03-11 10:29:10.000000 canopy-8.8/canopy/create_config.py
--rw-r--r--   0 vsts      (1001) docker     (115)     2204 2020-03-11 10:29:10.000000 canopy-8.8/canopy/create_list_filter.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4619 2020-03-11 10:29:10.000000 canopy-8.8/canopy/create_study.py
--rw-r--r--   0 vsts      (1001) docker     (115)       92 2020-03-11 10:29:10.000000 canopy-8.8/canopy/defined_kwargs.py
--rw-r--r--   0 vsts      (1001) docker     (115)      553 2020-03-11 10:29:10.000000 canopy-8.8/canopy/delete_config.py
--rw-r--r--   0 vsts      (1001) docker     (115)      545 2020-03-11 10:29:10.000000 canopy-8.8/canopy/delete_study.py
--rw-r--r--   0 vsts      (1001) docker     (115)      188 2020-03-11 10:29:10.000000 canopy-8.8/canopy/dict_to_object.py
--rw-r--r--   0 vsts      (1001) docker     (115)      778 2020-03-11 10:29:10.000000 canopy-8.8/canopy/dict_to_object_test.py
--rw-r--r--   0 vsts      (1001) docker     (115)      383 2020-03-11 10:29:10.000000 canopy-8.8/canopy/dynamic_dict_to_object.py
--rw-r--r--   0 vsts      (1001) docker     (115)      237 2020-03-11 10:29:10.000000 canopy-8.8/canopy/ensure_dict.py
--rw-r--r--   0 vsts      (1001) docker     (115)      222 2020-03-11 10:29:10.000000 canopy-8.8/canopy/ensure_sim_type_string.py
--rw-r--r--   0 vsts      (1001) docker     (115)      681 2020-03-11 10:29:10.000000 canopy-8.8/canopy/ensure_sim_type_string_test.py
--rw-r--r--   0 vsts      (1001) docker     (115)      223 2020-03-11 10:29:10.000000 canopy-8.8/canopy/ensure_study_type_string.py
--rw-r--r--   0 vsts      (1001) docker     (115)      695 2020-03-11 10:29:10.000000 canopy-8.8/canopy/ensure_study_type_string_test.py
--rw-r--r--   0 vsts      (1001) docker     (115)     1639 2020-03-11 10:29:10.000000 canopy-8.8/canopy/find_config.py
--rw-r--r--   0 vsts      (1001) docker     (115)     1339 2020-03-11 10:29:10.000000 canopy-8.8/canopy/find_study.py
--rw-r--r--   0 vsts      (1001) docker     (115)      299 2020-03-11 10:29:10.000000 canopy-8.8/canopy/get_default_config_path.py
--rw-r--r--   0 vsts      (1001) docker     (115)      330 2020-03-11 10:29:10.000000 canopy-8.8/canopy/get_study_document.py
--rw-r--r--   0 vsts      (1001) docker     (115)      678 2020-03-11 10:29:10.000000 canopy-8.8/canopy/get_study_type_definition_for_sim_version.py
--rw-r--r--   0 vsts      (1001) docker     (115)     1982 2020-03-11 10:29:10.000000 canopy-8.8/canopy/get_study_type_definition_for_sim_version_test.py
--rw-r--r--   0 vsts      (1001) docker     (115)      131 2020-03-11 10:29:10.000000 canopy-8.8/canopy/job_count_to_simulation_count.py
--rw-r--r--   0 vsts      (1001) docker     (115)     2246 2020-03-11 10:29:10.000000 canopy-8.8/canopy/load_channel.py
--rw-r--r--   0 vsts      (1001) docker     (115)      795 2020-03-11 10:29:10.000000 canopy-8.8/canopy/load_config.py
--rw-r--r--   0 vsts      (1001) docker     (115)      787 2020-03-11 10:29:10.000000 canopy-8.8/canopy/load_default_config.py
--rw-r--r--   0 vsts      (1001) docker     (115)     3454 2020-03-11 10:29:10.000000 canopy-8.8/canopy/load_study.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4943 2020-03-11 10:29:10.000000 canopy-8.8/canopy/load_study_job.py
--rw-r--r--   0 vsts      (1001) docker     (115)      752 2020-03-11 10:29:10.000000 canopy-8.8/canopy/load_study_job_scalar_results.py
--rw-r--r--   0 vsts      (1001) docker     (115)     2393 2020-03-11 10:29:10.000000 canopy-8.8/canopy/load_study_scalar_results.py
--rw-r--r--   0 vsts      (1001) docker     (115)      716 2020-03-11 10:29:10.000000 canopy-8.8/canopy/load_vector_metadata.py
--rw-r--r--   0 vsts      (1001) docker     (115)      396 2020-03-11 10:29:10.000000 canopy-8.8/canopy/loaded_channel.py
--rw-r--r--   0 vsts      (1001) docker     (115)     2423 2020-03-11 10:29:10.000000 canopy-8.8/canopy/local_config.py
--rw-r--r--   0 vsts      (1001) docker     (115)       41 2020-03-11 10:29:10.000000 canopy-8.8/canopy/not_found_error.py
-drwxr-xr-x   0 vsts      (1001) docker     (115)        0 2020-03-11 10:29:31.000000 canopy-8.8/canopy/openapi/
--rw-r--r--   0 vsts      (1001) docker     (115)    14635 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (115)        0 2020-03-11 10:29:31.000000 canopy-8.8/canopy/openapi/api/
--rw-r--r--   0 vsts      (1001) docker     (115)      947 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/api/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (115)    13001 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/api/account_settings_api.py
--rw-r--r--   0 vsts      (1001) docker     (115)     9687 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/api/availability_api.py
--rw-r--r--   0 vsts      (1001) docker     (115)   129759 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/api/config_api.py
--rw-r--r--   0 vsts      (1001) docker     (115)     6148 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/api/end_to_end_test_inbox_api.py
--rw-r--r--   0 vsts      (1001) docker     (115)     5382 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/api/list_filter_api.py
--rw-r--r--   0 vsts      (1001) docker     (115)    50216 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/api/membership_api.py
--rw-r--r--   0 vsts      (1001) docker     (115)    16259 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/api/pool_api.py
--rw-r--r--   0 vsts      (1001) docker     (115)    33249 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/api/sim_version_api.py
--rw-r--r--   0 vsts      (1001) docker     (115)   223359 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/api/study_api.py
--rw-r--r--   0 vsts      (1001) docker     (115)    31393 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/api/support_session_api.py
--rw-r--r--   0 vsts      (1001) docker     (115)    25266 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/api/tenancy_api.py
--rw-r--r--   0 vsts      (1001) docker     (115)    57156 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/api/tenant_settings_api.py
--rw-r--r--   0 vsts      (1001) docker     (115)    13118 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/api/user_settings_api.py
--rw-r--r--   0 vsts      (1001) docker     (115)    26249 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/api/worksheet_api.py
--rw-r--r--   0 vsts      (1001) docker     (115)    25538 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/api_client.py
--rw-r--r--   0 vsts      (1001) docker     (115)    10570 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/configuration.py
--rw-r--r--   0 vsts      (1001) docker     (115)     3784 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/exceptions.py
-drwxr-xr-x   0 vsts      (1001) docker     (115)        0 2020-03-11 10:29:31.000000 canopy-8.8/canopy/openapi/models/
--rw-r--r--   0 vsts      (1001) docker     (115)    13339 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4963 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/additional_tests.py
--rw-r--r--   0 vsts      (1001) docker     (115)     9396 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/admin_tenant_settings.py
--rw-r--r--   0 vsts      (1001) docker     (115)     9620 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/admin_tenant_settings_builder.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4646 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/auto_scale_run.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4637 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/auto_scale_run_error.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4846 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/availability_result.py
--rw-r--r--   0 vsts      (1001) docker     (115)     3488 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/batch_create_configs_result.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4159 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/blob_access_information.py
--rw-r--r--   0 vsts      (1001) docker     (115)    13754 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/canopy_document.py
--rw-r--r--   0 vsts      (1001) docker     (115)     3907 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/channel_import_mapping.py
--rw-r--r--   0 vsts      (1001) docker     (115)     3888 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/channel_settings.py
--rw-r--r--   0 vsts      (1001) docker     (115)     5859 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/chart_settings.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4858 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/collated_label_definitions.py
--rw-r--r--   0 vsts      (1001) docker     (115)     5162 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/collated_worksheet_labels.py
--rw-r--r--   0 vsts      (1001) docker     (115)     6164 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/compute_node_result.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4257 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/config_column_label_definitions.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4084 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/config_hash.py
--rw-r--r--   0 vsts      (1001) docker     (115)     3338 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/config_owner_data.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4079 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/config_reference.py
--rw-r--r--   0 vsts      (1001) docker     (115)     5019 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/config_resolved_labels.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4813 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/config_resolved_reference.py
--rw-r--r--   0 vsts      (1001) docker     (115)     7411 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/config_resolved_reference_data.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4436 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/config_type_definition.py
--rw-r--r--   0 vsts      (1001) docker     (115)     6104 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/config_type_metadata.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4007 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/default_config_id.py
--rw-r--r--   0 vsts      (1001) docker     (115)     3335 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/default_config_reference.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4751 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/default_custom_property_names.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4020 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/document_custom_property_data.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4118 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/document_custom_property_group.py
--rw-r--r--   0 vsts      (1001) docker     (115)     3916 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/document_group_result.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4663 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/document_name_result.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4995 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/document_type_custom_property_groups.py
--rw-r--r--   0 vsts      (1001) docker     (115)     3463 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/document_user_information.py
--rw-r--r--   0 vsts      (1001) docker     (115)     5352 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/documents_and_continuation_token.py
--rw-r--r--   0 vsts      (1001) docker     (115)     6429 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/duplicate_configs_data.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4663 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/duplicate_configs_result.py
--rw-r--r--   0 vsts      (1001) docker     (115)     3908 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/file_download_metadata.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4823 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/get_account_settings_result.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4231 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/get_admin_tenant_settings_query_result.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4522 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/get_all_support_sessions_query_result.py
--rw-r--r--   0 vsts      (1001) docker     (115)     3588 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/get_all_tenants_study_statistics_query_result.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4422 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/get_config_names_query_result.py
--rw-r--r--   0 vsts      (1001) docker     (115)     5247 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/get_config_query_result.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4487 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/get_config_versions_query_result.py
--rw-r--r--   0 vsts      (1001) docker     (115)     5378 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/get_configs_query_result.py
--rw-r--r--   0 vsts      (1001) docker     (115)    13094 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/get_pool_status_query_result.py
--rw-r--r--   0 vsts      (1001) docker     (115)     7482 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/get_pools_item.py
--rw-r--r--   0 vsts      (1001) docker     (115)     5287 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/get_pools_item_interval.py
--rw-r--r--   0 vsts      (1001) docker     (115)     3376 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/get_pools_query_result.py
--rw-r--r--   0 vsts      (1001) docker     (115)     3522 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/get_sim_version_document_query_result.py
--rw-r--r--   0 vsts      (1001) docker     (115)     5127 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/get_sim_version_documents_query_result.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4392 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/get_sim_version_downloads_query_result.py
--rw-r--r--   0 vsts      (1001) docker     (115)     5393 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/get_studies_query_result.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4327 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/get_study_download_url_query_result.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4513 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/get_study_job_metadata_query_result.py
--rw-r--r--   0 vsts      (1001) docker     (115)     7910 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/get_study_job_query_result.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4514 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/get_study_jobs_query_result.py
--rw-r--r--   0 vsts      (1001) docker     (115)     7846 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/get_study_query_result.py
--rw-r--r--   0 vsts      (1001) docker     (115)     6199 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/get_study_types_query_result.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4416 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/get_support_session_query_result.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4490 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/get_tenant_access_information_query_result.py
--rw-r--r--   0 vsts      (1001) docker     (115)     5033 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/get_tenant_billable_stored_simulation_count_query_result.py
--rw-r--r--   0 vsts      (1001) docker     (115)     3934 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/get_tenant_channel_import_mappings_query_result.py
--rw-r--r--   0 vsts      (1001) docker     (115)     7638 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/get_tenant_default_custom_property_names_query_result.py
--rw-r--r--   0 vsts      (1001) docker     (115)     6329 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/get_tenant_query_result.py
--rw-r--r--   0 vsts      (1001) docker     (115)     3602 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/get_tenant_settings_sim_version_query_result.py
--rw-r--r--   0 vsts      (1001) docker     (115)     3568 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/get_tenant_study_statistics_query_result.py
--rw-r--r--   0 vsts      (1001) docker     (115)     3487 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/get_tenant_users_query_result.py
--rw-r--r--   0 vsts      (1001) docker     (115)     6386 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/get_tenant_users_query_result_user_item.py
--rw-r--r--   0 vsts      (1001) docker     (115)     3817 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/get_tenant_worksheet_label_definitions_query_result.py
--rw-r--r--   0 vsts      (1001) docker     (115)     3489 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/get_tenants_query_result.py
--rw-r--r--   0 vsts      (1001) docker     (115)     8038 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/get_tenants_query_result_tenant_item.py
--rw-r--r--   0 vsts      (1001) docker     (115)     3381 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/get_user_roles_query_result.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4126 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/get_user_settings_query_result.py
--rw-r--r--   0 vsts      (1001) docker     (115)     3474 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/get_wiki_document_query_result.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4381 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/get_worksheet_query_result.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4421 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/i_previous_definition_sim_type_definition.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4451 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/i_previous_definition_study_type_definition.py
--rw-r--r--   0 vsts      (1001) docker     (115)     5348 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/identified_user_data.py
--rw-r--r--   0 vsts      (1001) docker     (115)     3908 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/label_definition.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4954 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/label_definitions.py
--rw-r--r--   0 vsts      (1001) docker     (115)    10838 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/list_filter.py
--rw-r--r--   0 vsts      (1001) docker     (115)     5717 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/list_filter_condition.py
--rw-r--r--   0 vsts      (1001) docker     (115)     5165 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/list_filter_group.py
--rw-r--r--   0 vsts      (1001) docker     (115)     3864 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/name_value_pair.py
--rw-r--r--   0 vsts      (1001) docker     (115)     3371 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/new_batch_config_data.py
--rw-r--r--   0 vsts      (1001) docker     (115)     7601 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/new_config_data.py
--rw-r--r--   0 vsts      (1001) docker     (115)     3434 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/new_sim_version_data.py
--rw-r--r--   0 vsts      (1001) docker     (115)     8948 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/new_study_data.py
--rw-r--r--   0 vsts      (1001) docker     (115)     6106 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/new_study_data_source.py
--rw-r--r--   0 vsts      (1001) docker     (115)     5304 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/new_tenant_data.py
--rw-r--r--   0 vsts      (1001) docker     (115)     5392 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/new_worksheet_data.py
--rw-r--r--   0 vsts      (1001) docker     (115)     5074 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/password_reset_confirmation_data.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4741 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/password_reset_request_data.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4169 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/pool_settings.py
--rw-r--r--   0 vsts      (1001) docker     (115)     3358 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/post_study_result.py
--rw-r--r--   0 vsts      (1001) docker     (115)     5345 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/registration_data.py
--rw-r--r--   0 vsts      (1001) docker     (115)     6908 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/resolved_label.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4707 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/resolved_statistic_label.py
--rw-r--r--   0 vsts      (1001) docker     (115)     8743 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/sim_type_definition.py
--rw-r--r--   0 vsts      (1001) docker     (115)     5248 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/sim_type_input_telemetry_channel.py
--rw-r--r--   0 vsts      (1001) docker     (115)     5583 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/sim_type_input_telemetry_channels.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4410 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/sim_type_input_telemetry_evaluated_channel.py
--rw-r--r--   0 vsts      (1001) docker     (115)     5461 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/sim_type_input_telemetry_evaluated_channel_suffix.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4024 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/sim_version_document_name_result.py
--rw-r--r--   0 vsts      (1001) docker     (115)     5052 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/simulation_column_label_definitions.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4149 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/simulation_input.py
--rw-r--r--   0 vsts      (1001) docker     (115)     5129 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/simulation_resolved_labels.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4924 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/study_blob_access_information.py
--rw-r--r--   0 vsts      (1001) docker     (115)    23710 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/study_document.py
--rw-r--r--   0 vsts      (1001) docker     (115)     6538 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/study_document_study_document_data_source.py
--rw-r--r--   0 vsts      (1001) docker     (115)     5432 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/study_documents_and_continuation_token.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4132 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/study_input_hash.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4110 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/study_input_hashes.py
--rw-r--r--   0 vsts      (1001) docker     (115)     5480 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/study_job_documents_and_continuation_token.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4054 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/study_reference.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4389 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/study_resolved_labels.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4791 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/study_resolved_reference.py
--rw-r--r--   0 vsts      (1001) docker     (115)    10919 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/study_resolved_reference_data.py
--rw-r--r--   0 vsts      (1001) docker     (115)    15251 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/study_type_definition.py
--rw-r--r--   0 vsts      (1001) docker     (115)     6558 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/support_session.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4066 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/support_session_data.py
--rw-r--r--   0 vsts      (1001) docker     (115)     5598 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/support_session_response.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4850 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/tenant_config_reference.py
--rw-r--r--   0 vsts      (1001) docker     (115)     3999 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/tenant_default_custom_property_names.py
--rw-r--r--   0 vsts      (1001) docker     (115)     5378 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/tenant_information.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4108 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/tenant_statistics.py
--rw-r--r--   0 vsts      (1001) docker     (115)     3632 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/test_auto_scale_formula_query_result.py
--rw-r--r--   0 vsts      (1001) docker     (115)     3892 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/text_document.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4072 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/text_document_optional_content.py
--rw-r--r--   0 vsts      (1001) docker     (115)     5725 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/updated_account_settings.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4168 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/updated_admin_tenant_settings.py
--rw-r--r--   0 vsts      (1001) docker     (115)     3830 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/updated_channel_import_mappings.py
--rw-r--r--   0 vsts      (1001) docker     (115)     6834 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/updated_config_data.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4700 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/updated_study_data.py
--rw-r--r--   0 vsts      (1001) docker     (115)     5466 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/updated_tenant_data.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4055 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/updated_tenant_default_custom_property_names.py
--rw-r--r--   0 vsts      (1001) docker     (115)     3546 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/updated_tenant_settings_sim_version.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4063 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/updated_user_settings.py
--rw-r--r--   0 vsts      (1001) docker     (115)     5472 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/updated_worksheet_data.py
--rw-r--r--   0 vsts      (1001) docker     (115)     3713 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/updated_worksheet_label_definitions.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4816 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/upgrade_config_data.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4363 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/upgrade_config_query_result.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4616 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/user_information.py
--rw-r--r--   0 vsts      (1001) docker     (115)     3954 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/user_role_data.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4929 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/user_settings.py
--rw-r--r--   0 vsts      (1001) docker     (115)     5041 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/user_settings_builder.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4890 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/versioned_document_metadata.py
--rw-r--r--   0 vsts      (1001) docker     (115)     9783 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/worksheet.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4994 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/worksheet_config.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4223 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/worksheet_outline.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4285 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/worksheet_resolved_references.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4576 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/worksheet_row.py
--rw-r--r--   0 vsts      (1001) docker     (115)     3404 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/models/worksheet_study.py
--rw-r--r--   0 vsts      (1001) docker     (115)    12493 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi/rest.py
-drwxr-xr-x   0 vsts      (1001) docker     (115)        0 2020-03-11 10:29:31.000000 canopy-8.8/canopy/openapi_asyncio/
--rw-r--r--   0 vsts      (1001) docker     (115)      399 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi_asyncio/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (115)    25558 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi_asyncio/api_client.py
--rw-r--r--   0 vsts      (1001) docker     (115)    10192 2020-03-11 10:29:10.000000 canopy-8.8/canopy/openapi_asyncio/rest.py
--rw-r--r--   0 vsts      (1001) docker     (115)     1223 2020-03-11 10:29:10.000000 canopy-8.8/canopy/process_data_frame.py
--rw-r--r--   0 vsts      (1001) docker     (115)     1732 2020-03-11 10:29:10.000000 canopy-8.8/canopy/process_data_frame_test.py
--rw-r--r--   0 vsts      (1001) docker     (115)      889 2020-03-11 10:29:10.000000 canopy-8.8/canopy/prompt_for_authentication.py
--rw-r--r--   0 vsts      (1001) docker     (115)      564 2020-03-11 10:29:10.000000 canopy-8.8/canopy/properties_dict_to_list.py
--rw-r--r--   0 vsts      (1001) docker     (115)     1221 2020-03-11 10:29:10.000000 canopy-8.8/canopy/proxy_configuration.py
--rw-r--r--   0 vsts      (1001) docker     (115)     1015 2020-03-11 10:29:10.000000 canopy-8.8/canopy/proxy_configuration_test.py
--rw-r--r--   0 vsts      (1001) docker     (115)      143 2020-03-11 10:29:10.000000 canopy-8.8/canopy/run.py
--rw-r--r--   0 vsts      (1001) docker     (115)      400 2020-03-11 10:29:10.000000 canopy-8.8/canopy/serializable_value.py
--rw-r--r--   0 vsts      (1001) docker     (115)     3792 2020-03-11 10:29:10.000000 canopy-8.8/canopy/session.py
--rw-r--r--   0 vsts      (1001) docker     (115)      133 2020-03-11 10:29:10.000000 canopy-8.8/canopy/sim_version_to_number.py
--rw-r--r--   0 vsts      (1001) docker     (115)      766 2020-03-11 10:29:10.000000 canopy-8.8/canopy/sim_version_to_number_test.py
--rw-r--r--   0 vsts      (1001) docker     (115)     3741 2020-03-11 10:29:10.000000 canopy-8.8/canopy/study_job_result.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4316 2020-03-11 10:29:10.000000 canopy-8.8/canopy/study_result.py
--rw-r--r--   0 vsts      (1001) docker     (115)      994 2020-03-11 10:29:10.000000 canopy-8.8/canopy/study_scalar_results.py
--rw-r--r--   0 vsts      (1001) docker     (115)     3318 2020-03-11 10:29:10.000000 canopy-8.8/canopy/study_types_cache.py
--rw-r--r--   0 vsts      (1001) docker     (115)      986 2020-03-11 10:29:10.000000 canopy-8.8/canopy/tenant_sim_version_cache.py
--rw-r--r--   0 vsts      (1001) docker     (115)     1036 2020-03-11 10:29:10.000000 canopy-8.8/canopy/tenant_users.py
--rw-r--r--   0 vsts      (1001) docker     (115)     1046 2020-03-11 10:29:10.000000 canopy-8.8/canopy/tenant_users_cache.py
--rw-r--r--   0 vsts      (1001) docker     (115)     1234 2020-03-11 10:29:10.000000 canopy-8.8/canopy/tenant_users_test.py
--rw-r--r--   0 vsts      (1001) docker     (115)     1071 2020-03-11 10:29:10.000000 canopy-8.8/canopy/try_load_csv_from_url.py
--rw-r--r--   0 vsts      (1001) docker     (115)    12387 2020-03-11 10:29:10.000000 canopy-8.8/canopy/units.py
--rw-r--r--   0 vsts      (1001) docker     (115)    12842 2020-03-11 10:29:10.000000 canopy-8.8/canopy/units_test.py
--rw-r--r--   0 vsts      (1001) docker     (115)      862 2020-03-11 10:29:10.000000 canopy-8.8/canopy/update_config.py
--rw-r--r--   0 vsts      (1001) docker     (115)     1619 2020-03-11 10:29:10.000000 canopy-8.8/canopy/user_settings_cache.py
--rw-r--r--   0 vsts      (1001) docker     (115)     1554 2020-03-11 10:29:10.000000 canopy-8.8/canopy/wait_for_study.py
-drwxr-xr-x   0 vsts      (1001) docker     (115)        0 2020-03-11 10:29:31.000000 canopy-8.8/canopy.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (115)     9324 2020-03-11 10:29:30.000000 canopy-8.8/canopy.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (115)    10983 2020-03-11 10:29:31.000000 canopy-8.8/canopy.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (115)        1 2020-03-11 10:29:30.000000 canopy-8.8/canopy.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (115)       99 2020-03-11 10:29:30.000000 canopy-8.8/canopy.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (115)       25 2020-03-11 10:29:30.000000 canopy-8.8/canopy.egg-info/top_level.txt
-drwxr-xr-x   0 vsts      (1001) docker     (115)        0 2020-03-11 10:29:31.000000 canopy-8.8/integration_tests/
--rw-r--r--   0 vsts      (1001) docker     (115)      185 2020-03-11 10:29:10.000000 canopy-8.8/integration_tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (115)     1141 2020-03-11 10:29:10.000000 canopy-8.8/integration_tests/environment.py
--rw-r--r--   0 vsts      (1001) docker     (115)      518 2020-03-11 10:29:10.000000 canopy-8.8/integration_tests/environment_data.py
--rw-r--r--   0 vsts      (1001) docker     (115)     2819 2020-03-11 10:29:10.000000 canopy-8.8/integration_tests/environment_loader.py
--rw-r--r--   0 vsts      (1001) docker     (115)     5338 2020-03-11 10:29:10.000000 canopy-8.8/integration_tests/test_config.py
--rw-r--r--   0 vsts      (1001) docker     (115)    13267 2020-03-11 10:29:10.000000 canopy-8.8/integration_tests/test_study.py
--rw-r--r--   0 vsts      (1001) docker     (115)      464 2020-03-11 10:29:10.000000 canopy-8.8/integration_tests/test_synchronous.py
--rw-r--r--   0 vsts      (1001) docker     (115)      125 2020-03-11 10:29:31.000000 canopy-8.8/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (115)     1537 2020-03-11 10:29:29.000000 canopy-8.8/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (115)        0 2020-03-11 12:22:12.000000 canopy-8.9/
+-rw-r--r--   0 vsts      (1001) docker     (115)     9509 2020-03-11 12:22:12.000000 canopy-8.9/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (115)     7325 2020-03-11 12:21:51.000000 canopy-8.9/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (115)        0 2020-03-11 12:22:12.000000 canopy-8.9/canopy/
+-rw-r--r--   0 vsts      (1001) docker     (115)     2858 2020-03-11 12:21:51.000000 canopy-8.9/canopy/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     3754 2020-03-11 12:21:51.000000 canopy-8.9/canopy/authentication.py
+-rw-r--r--   0 vsts      (1001) docker     (115)      966 2020-03-11 12:21:51.000000 canopy-8.9/canopy/authentication_data.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     2214 2020-03-11 12:21:51.000000 canopy-8.9/canopy/config_result.py
+-rw-r--r--   0 vsts      (1001) docker     (115)      115 2020-03-11 12:21:51.000000 canopy-8.9/canopy/constants.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     1051 2020-03-11 12:21:51.000000 canopy-8.9/canopy/create_config.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     2204 2020-03-11 12:21:51.000000 canopy-8.9/canopy/create_list_filter.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4619 2020-03-11 12:21:51.000000 canopy-8.9/canopy/create_study.py
+-rw-r--r--   0 vsts      (1001) docker     (115)       92 2020-03-11 12:21:51.000000 canopy-8.9/canopy/defined_kwargs.py
+-rw-r--r--   0 vsts      (1001) docker     (115)      553 2020-03-11 12:21:51.000000 canopy-8.9/canopy/delete_config.py
+-rw-r--r--   0 vsts      (1001) docker     (115)      545 2020-03-11 12:21:51.000000 canopy-8.9/canopy/delete_study.py
+-rw-r--r--   0 vsts      (1001) docker     (115)      188 2020-03-11 12:21:51.000000 canopy-8.9/canopy/dict_to_object.py
+-rw-r--r--   0 vsts      (1001) docker     (115)      778 2020-03-11 12:21:51.000000 canopy-8.9/canopy/dict_to_object_test.py
+-rw-r--r--   0 vsts      (1001) docker     (115)      383 2020-03-11 12:21:51.000000 canopy-8.9/canopy/dynamic_dict_to_object.py
+-rw-r--r--   0 vsts      (1001) docker     (115)      237 2020-03-11 12:21:51.000000 canopy-8.9/canopy/ensure_dict.py
+-rw-r--r--   0 vsts      (1001) docker     (115)      222 2020-03-11 12:21:51.000000 canopy-8.9/canopy/ensure_sim_type_string.py
+-rw-r--r--   0 vsts      (1001) docker     (115)      681 2020-03-11 12:21:51.000000 canopy-8.9/canopy/ensure_sim_type_string_test.py
+-rw-r--r--   0 vsts      (1001) docker     (115)      223 2020-03-11 12:21:51.000000 canopy-8.9/canopy/ensure_study_type_string.py
+-rw-r--r--   0 vsts      (1001) docker     (115)      695 2020-03-11 12:21:51.000000 canopy-8.9/canopy/ensure_study_type_string_test.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     1639 2020-03-11 12:21:51.000000 canopy-8.9/canopy/find_config.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     1339 2020-03-11 12:21:51.000000 canopy-8.9/canopy/find_study.py
+-rw-r--r--   0 vsts      (1001) docker     (115)      299 2020-03-11 12:21:51.000000 canopy-8.9/canopy/get_default_config_path.py
+-rw-r--r--   0 vsts      (1001) docker     (115)      330 2020-03-11 12:21:51.000000 canopy-8.9/canopy/get_study_document.py
+-rw-r--r--   0 vsts      (1001) docker     (115)      678 2020-03-11 12:21:51.000000 canopy-8.9/canopy/get_study_type_definition_for_sim_version.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     1982 2020-03-11 12:21:51.000000 canopy-8.9/canopy/get_study_type_definition_for_sim_version_test.py
+-rw-r--r--   0 vsts      (1001) docker     (115)      131 2020-03-11 12:21:51.000000 canopy-8.9/canopy/job_count_to_simulation_count.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     2246 2020-03-11 12:21:51.000000 canopy-8.9/canopy/load_channel.py
+-rw-r--r--   0 vsts      (1001) docker     (115)      795 2020-03-11 12:21:51.000000 canopy-8.9/canopy/load_config.py
+-rw-r--r--   0 vsts      (1001) docker     (115)      787 2020-03-11 12:21:51.000000 canopy-8.9/canopy/load_default_config.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     3454 2020-03-11 12:21:51.000000 canopy-8.9/canopy/load_study.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4943 2020-03-11 12:21:51.000000 canopy-8.9/canopy/load_study_job.py
+-rw-r--r--   0 vsts      (1001) docker     (115)      752 2020-03-11 12:21:51.000000 canopy-8.9/canopy/load_study_job_scalar_results.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     2393 2020-03-11 12:21:51.000000 canopy-8.9/canopy/load_study_scalar_results.py
+-rw-r--r--   0 vsts      (1001) docker     (115)      716 2020-03-11 12:21:51.000000 canopy-8.9/canopy/load_vector_metadata.py
+-rw-r--r--   0 vsts      (1001) docker     (115)      396 2020-03-11 12:21:51.000000 canopy-8.9/canopy/loaded_channel.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     2423 2020-03-11 12:21:51.000000 canopy-8.9/canopy/local_config.py
+-rw-r--r--   0 vsts      (1001) docker     (115)       41 2020-03-11 12:21:51.000000 canopy-8.9/canopy/not_found_error.py
+drwxr-xr-x   0 vsts      (1001) docker     (115)        0 2020-03-11 12:22:12.000000 canopy-8.9/canopy/openapi/
+-rw-r--r--   0 vsts      (1001) docker     (115)    14635 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (115)        0 2020-03-11 12:22:12.000000 canopy-8.9/canopy/openapi/api/
+-rw-r--r--   0 vsts      (1001) docker     (115)      947 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/api/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (115)    13001 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/api/account_settings_api.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     9687 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/api/availability_api.py
+-rw-r--r--   0 vsts      (1001) docker     (115)   129759 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/api/config_api.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     6148 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/api/end_to_end_test_inbox_api.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     5382 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/api/list_filter_api.py
+-rw-r--r--   0 vsts      (1001) docker     (115)    50216 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/api/membership_api.py
+-rw-r--r--   0 vsts      (1001) docker     (115)    16259 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/api/pool_api.py
+-rw-r--r--   0 vsts      (1001) docker     (115)    33249 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/api/sim_version_api.py
+-rw-r--r--   0 vsts      (1001) docker     (115)   223359 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/api/study_api.py
+-rw-r--r--   0 vsts      (1001) docker     (115)    31393 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/api/support_session_api.py
+-rw-r--r--   0 vsts      (1001) docker     (115)    25266 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/api/tenancy_api.py
+-rw-r--r--   0 vsts      (1001) docker     (115)    57156 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/api/tenant_settings_api.py
+-rw-r--r--   0 vsts      (1001) docker     (115)    13118 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/api/user_settings_api.py
+-rw-r--r--   0 vsts      (1001) docker     (115)    26249 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/api/worksheet_api.py
+-rw-r--r--   0 vsts      (1001) docker     (115)    25571 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/api_client.py
+-rw-r--r--   0 vsts      (1001) docker     (115)    10570 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/configuration.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     3784 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/exceptions.py
+drwxr-xr-x   0 vsts      (1001) docker     (115)        0 2020-03-11 12:22:12.000000 canopy-8.9/canopy/openapi/models/
+-rw-r--r--   0 vsts      (1001) docker     (115)    13339 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4963 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/additional_tests.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     9396 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/admin_tenant_settings.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     9620 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/admin_tenant_settings_builder.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4646 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/auto_scale_run.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4637 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/auto_scale_run_error.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4846 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/availability_result.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     3488 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/batch_create_configs_result.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4159 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/blob_access_information.py
+-rw-r--r--   0 vsts      (1001) docker     (115)    13754 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/canopy_document.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     3907 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/channel_import_mapping.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     3888 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/channel_settings.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     5859 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/chart_settings.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4858 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/collated_label_definitions.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     5162 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/collated_worksheet_labels.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     6164 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/compute_node_result.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4257 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/config_column_label_definitions.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4084 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/config_hash.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     3338 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/config_owner_data.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4079 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/config_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     5019 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/config_resolved_labels.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4813 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/config_resolved_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     7411 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/config_resolved_reference_data.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4436 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/config_type_definition.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     6104 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/config_type_metadata.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4007 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/default_config_id.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     3335 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/default_config_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4751 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/default_custom_property_names.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4020 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/document_custom_property_data.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4118 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/document_custom_property_group.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     3916 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/document_group_result.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4663 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/document_name_result.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4995 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/document_type_custom_property_groups.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     3463 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/document_user_information.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     5352 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/documents_and_continuation_token.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     6429 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/duplicate_configs_data.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4663 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/duplicate_configs_result.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     3908 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/file_download_metadata.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4823 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/get_account_settings_result.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4231 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/get_admin_tenant_settings_query_result.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4522 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/get_all_support_sessions_query_result.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     3588 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/get_all_tenants_study_statistics_query_result.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4422 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/get_config_names_query_result.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     5247 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/get_config_query_result.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4487 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/get_config_versions_query_result.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     5378 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/get_configs_query_result.py
+-rw-r--r--   0 vsts      (1001) docker     (115)    13094 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/get_pool_status_query_result.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     7482 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/get_pools_item.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     5287 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/get_pools_item_interval.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     3376 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/get_pools_query_result.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     3522 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/get_sim_version_document_query_result.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     5127 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/get_sim_version_documents_query_result.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4392 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/get_sim_version_downloads_query_result.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     5393 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/get_studies_query_result.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4327 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/get_study_download_url_query_result.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4513 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/get_study_job_metadata_query_result.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     7910 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/get_study_job_query_result.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4514 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/get_study_jobs_query_result.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     7846 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/get_study_query_result.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     6199 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/get_study_types_query_result.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4416 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/get_support_session_query_result.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4490 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/get_tenant_access_information_query_result.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     5033 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/get_tenant_billable_stored_simulation_count_query_result.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     3934 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/get_tenant_channel_import_mappings_query_result.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     7638 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/get_tenant_default_custom_property_names_query_result.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     6329 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/get_tenant_query_result.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     3602 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/get_tenant_settings_sim_version_query_result.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     3568 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/get_tenant_study_statistics_query_result.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     3487 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/get_tenant_users_query_result.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     6386 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/get_tenant_users_query_result_user_item.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     3817 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/get_tenant_worksheet_label_definitions_query_result.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     3489 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/get_tenants_query_result.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     8038 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/get_tenants_query_result_tenant_item.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     3381 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/get_user_roles_query_result.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4126 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/get_user_settings_query_result.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     3474 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/get_wiki_document_query_result.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4381 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/get_worksheet_query_result.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4421 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/i_previous_definition_sim_type_definition.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4451 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/i_previous_definition_study_type_definition.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     5348 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/identified_user_data.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     3908 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/label_definition.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4954 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/label_definitions.py
+-rw-r--r--   0 vsts      (1001) docker     (115)    10838 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/list_filter.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     5717 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/list_filter_condition.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     5165 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/list_filter_group.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     3864 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/name_value_pair.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     3371 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/new_batch_config_data.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     7601 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/new_config_data.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     3434 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/new_sim_version_data.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     8948 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/new_study_data.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     6106 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/new_study_data_source.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     5304 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/new_tenant_data.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     5392 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/new_worksheet_data.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     5074 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/password_reset_confirmation_data.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4741 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/password_reset_request_data.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4169 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/pool_settings.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     3358 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/post_study_result.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     5345 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/registration_data.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     6908 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/resolved_label.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4707 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/resolved_statistic_label.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     8743 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/sim_type_definition.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     5248 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/sim_type_input_telemetry_channel.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     5583 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/sim_type_input_telemetry_channels.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4410 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/sim_type_input_telemetry_evaluated_channel.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     5461 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/sim_type_input_telemetry_evaluated_channel_suffix.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4024 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/sim_version_document_name_result.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     5052 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/simulation_column_label_definitions.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4149 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/simulation_input.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     5129 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/simulation_resolved_labels.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4924 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/study_blob_access_information.py
+-rw-r--r--   0 vsts      (1001) docker     (115)    23710 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/study_document.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     6538 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/study_document_study_document_data_source.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     5432 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/study_documents_and_continuation_token.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4132 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/study_input_hash.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4110 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/study_input_hashes.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     5480 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/study_job_documents_and_continuation_token.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4054 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/study_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4389 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/study_resolved_labels.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4791 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/study_resolved_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (115)    10919 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/study_resolved_reference_data.py
+-rw-r--r--   0 vsts      (1001) docker     (115)    15251 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/study_type_definition.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     6558 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/support_session.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4066 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/support_session_data.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     5598 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/support_session_response.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4850 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/tenant_config_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     3999 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/tenant_default_custom_property_names.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     5378 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/tenant_information.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4108 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/tenant_statistics.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     3632 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/test_auto_scale_formula_query_result.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     3892 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/text_document.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4072 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/text_document_optional_content.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     5725 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/updated_account_settings.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4168 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/updated_admin_tenant_settings.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     3830 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/updated_channel_import_mappings.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     6834 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/updated_config_data.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4700 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/updated_study_data.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     5466 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/updated_tenant_data.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4055 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/updated_tenant_default_custom_property_names.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     3546 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/updated_tenant_settings_sim_version.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4063 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/updated_user_settings.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     5472 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/updated_worksheet_data.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     3713 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/updated_worksheet_label_definitions.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4816 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/upgrade_config_data.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4363 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/upgrade_config_query_result.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4616 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/user_information.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     3954 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/user_role_data.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4929 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/user_settings.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     5041 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/user_settings_builder.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4890 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/versioned_document_metadata.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     9783 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/worksheet.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4994 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/worksheet_config.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4223 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/worksheet_outline.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4285 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/worksheet_resolved_references.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4576 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/worksheet_row.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     3404 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/models/worksheet_study.py
+-rw-r--r--   0 vsts      (1001) docker     (115)    12493 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi/rest.py
+drwxr-xr-x   0 vsts      (1001) docker     (115)        0 2020-03-11 12:22:12.000000 canopy-8.9/canopy/openapi_asyncio/
+-rw-r--r--   0 vsts      (1001) docker     (115)      399 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi_asyncio/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (115)    25591 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi_asyncio/api_client.py
+-rw-r--r--   0 vsts      (1001) docker     (115)    10192 2020-03-11 12:21:51.000000 canopy-8.9/canopy/openapi_asyncio/rest.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     1223 2020-03-11 12:21:51.000000 canopy-8.9/canopy/process_data_frame.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     1732 2020-03-11 12:21:51.000000 canopy-8.9/canopy/process_data_frame_test.py
+-rw-r--r--   0 vsts      (1001) docker     (115)      889 2020-03-11 12:21:51.000000 canopy-8.9/canopy/prompt_for_authentication.py
+-rw-r--r--   0 vsts      (1001) docker     (115)      564 2020-03-11 12:21:51.000000 canopy-8.9/canopy/properties_dict_to_list.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     1221 2020-03-11 12:21:51.000000 canopy-8.9/canopy/proxy_configuration.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     1015 2020-03-11 12:21:51.000000 canopy-8.9/canopy/proxy_configuration_test.py
+-rw-r--r--   0 vsts      (1001) docker     (115)      143 2020-03-11 12:21:51.000000 canopy-8.9/canopy/run.py
+-rw-r--r--   0 vsts      (1001) docker     (115)      400 2020-03-11 12:21:51.000000 canopy-8.9/canopy/serializable_value.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     3792 2020-03-11 12:21:51.000000 canopy-8.9/canopy/session.py
+-rw-r--r--   0 vsts      (1001) docker     (115)      133 2020-03-11 12:21:51.000000 canopy-8.9/canopy/sim_version_to_number.py
+-rw-r--r--   0 vsts      (1001) docker     (115)      766 2020-03-11 12:21:51.000000 canopy-8.9/canopy/sim_version_to_number_test.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     3741 2020-03-11 12:21:51.000000 canopy-8.9/canopy/study_job_result.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4316 2020-03-11 12:21:51.000000 canopy-8.9/canopy/study_result.py
+-rw-r--r--   0 vsts      (1001) docker     (115)      994 2020-03-11 12:21:51.000000 canopy-8.9/canopy/study_scalar_results.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     3318 2020-03-11 12:21:51.000000 canopy-8.9/canopy/study_types_cache.py
+-rw-r--r--   0 vsts      (1001) docker     (115)      986 2020-03-11 12:21:51.000000 canopy-8.9/canopy/tenant_sim_version_cache.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     1036 2020-03-11 12:21:51.000000 canopy-8.9/canopy/tenant_users.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     1046 2020-03-11 12:21:51.000000 canopy-8.9/canopy/tenant_users_cache.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     1234 2020-03-11 12:21:51.000000 canopy-8.9/canopy/tenant_users_test.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     1071 2020-03-11 12:21:51.000000 canopy-8.9/canopy/try_load_csv_from_url.py
+-rw-r--r--   0 vsts      (1001) docker     (115)    12387 2020-03-11 12:21:51.000000 canopy-8.9/canopy/units.py
+-rw-r--r--   0 vsts      (1001) docker     (115)    12842 2020-03-11 12:21:51.000000 canopy-8.9/canopy/units_test.py
+-rw-r--r--   0 vsts      (1001) docker     (115)      862 2020-03-11 12:21:51.000000 canopy-8.9/canopy/update_config.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     1619 2020-03-11 12:21:51.000000 canopy-8.9/canopy/user_settings_cache.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     1554 2020-03-11 12:21:51.000000 canopy-8.9/canopy/wait_for_study.py
+drwxr-xr-x   0 vsts      (1001) docker     (115)        0 2020-03-11 12:22:12.000000 canopy-8.9/canopy.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (115)     9509 2020-03-11 12:22:12.000000 canopy-8.9/canopy.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (115)    10983 2020-03-11 12:22:12.000000 canopy-8.9/canopy.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (115)        1 2020-03-11 12:22:12.000000 canopy-8.9/canopy.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (115)       99 2020-03-11 12:22:12.000000 canopy-8.9/canopy.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (115)       25 2020-03-11 12:22:12.000000 canopy-8.9/canopy.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (115)        0 2020-03-11 12:22:12.000000 canopy-8.9/integration_tests/
+-rw-r--r--   0 vsts      (1001) docker     (115)      185 2020-03-11 12:21:51.000000 canopy-8.9/integration_tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     1141 2020-03-11 12:21:51.000000 canopy-8.9/integration_tests/environment.py
+-rw-r--r--   0 vsts      (1001) docker     (115)      518 2020-03-11 12:21:51.000000 canopy-8.9/integration_tests/environment_data.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     2819 2020-03-11 12:21:51.000000 canopy-8.9/integration_tests/environment_loader.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     6012 2020-03-11 12:21:51.000000 canopy-8.9/integration_tests/test_config.py
+-rw-r--r--   0 vsts      (1001) docker     (115)    13267 2020-03-11 12:21:51.000000 canopy-8.9/integration_tests/test_study.py
+-rw-r--r--   0 vsts      (1001) docker     (115)      464 2020-03-11 12:21:51.000000 canopy-8.9/integration_tests/test_synchronous.py
+-rw-r--r--   0 vsts      (1001) docker     (115)      125 2020-03-11 12:22:12.000000 canopy-8.9/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (115)     1537 2020-03-11 12:22:11.000000 canopy-8.9/setup.py
```

### Comparing `canopy-8.8/PKG-INFO` & `canopy-8.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canopy
-Version: 8.8
+Version: 8.9
 Summary: Python Client for the Canopy Simulation API
 Home-page: https://github.com/canopysimulations/canopy-python/
 Author: James Thurley
 Author-email: james.thurley@canopysimulations.com
 License: MIT
 Description: # Installation
         
@@ -179,15 +179,17 @@
         sed -i 's/from canopy\.openapi import rest/from canopy.openapi_asyncio import rest/g' gen/canopy/openapi_asyncio/api_client.py
         sed -i '/from canopy.*/d' gen/canopy/openapi_asyncio/__init__.py
         sed -i '/# import /d' gen/canopy/openapi_asyncio/__init__.py
         echo 'from canopy.openapi_asyncio.api_client import ApiClient' >> gen/canopy/openapi_asyncio/__init__.py
         cp -r gen/canopy/openapi_asyncio repo/canopy
         ```
         
-        Note: The openapi_asyncio/rest.py file will need to be manually modified to support proxy servers after generation. 
+        Note: The `openapi_asyncio/rest.py` file will need to be manually modified to support proxy servers after generation. 
+        Note: The `openapi_asyncio/client_api.py` and `openapi/client_api.py` files will need to be manually modified to 
+        support numpy array serialization after generation. 
         
         ## Documentation for OpenAPI Generated Client
         
         OpenAPI generated documentation can be found [here](OPENAPI_README.md).
         
 Keywords: Canopy API,Canopy Simulations,Canopy Client
 Platform: UNKNOWN
```

### Comparing `canopy-8.8/README.md` & `canopy-8.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -171,12 +171,14 @@
 sed -i 's/from canopy\.openapi import rest/from canopy.openapi_asyncio import rest/g' gen/canopy/openapi_asyncio/api_client.py
 sed -i '/from canopy.*/d' gen/canopy/openapi_asyncio/__init__.py
 sed -i '/# import /d' gen/canopy/openapi_asyncio/__init__.py
 echo 'from canopy.openapi_asyncio.api_client import ApiClient' >> gen/canopy/openapi_asyncio/__init__.py
 cp -r gen/canopy/openapi_asyncio repo/canopy
 ```
 
-Note: The openapi_asyncio/rest.py file will need to be manually modified to support proxy servers after generation. 
+Note: The `openapi_asyncio/rest.py` file will need to be manually modified to support proxy servers after generation. 
+Note: The `openapi_asyncio/client_api.py` and `openapi/client_api.py` files will need to be manually modified to 
+support numpy array serialization after generation. 
 
 ## Documentation for OpenAPI Generated Client
 
 OpenAPI generated documentation can be found [here](OPENAPI_README.md).
```

### Comparing `canopy-8.8/canopy/__init__.py` & `canopy-8.9/canopy/__init__.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/authentication.py` & `canopy-8.9/canopy/authentication.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/authentication_data.py` & `canopy-8.9/canopy/authentication_data.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/config_result.py` & `canopy-8.9/canopy/config_result.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/create_config.py` & `canopy-8.9/canopy/create_config.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/create_list_filter.py` & `canopy-8.9/canopy/create_list_filter.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/create_study.py` & `canopy-8.9/canopy/create_study.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/delete_config.py` & `canopy-8.9/canopy/delete_config.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/delete_study.py` & `canopy-8.9/canopy/delete_study.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/dict_to_object_test.py` & `canopy-8.9/canopy/dict_to_object_test.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/ensure_sim_type_string_test.py` & `canopy-8.9/canopy/ensure_sim_type_string_test.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/ensure_study_type_string_test.py` & `canopy-8.9/canopy/ensure_study_type_string_test.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/find_config.py` & `canopy-8.9/canopy/find_config.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/find_study.py` & `canopy-8.9/canopy/find_study.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/get_study_type_definition_for_sim_version.py` & `canopy-8.9/canopy/get_study_type_definition_for_sim_version.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/get_study_type_definition_for_sim_version_test.py` & `canopy-8.9/canopy/get_study_type_definition_for_sim_version_test.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/load_channel.py` & `canopy-8.9/canopy/load_channel.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/load_config.py` & `canopy-8.9/canopy/load_config.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/load_default_config.py` & `canopy-8.9/canopy/load_default_config.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/load_study.py` & `canopy-8.9/canopy/load_study.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/load_study_job.py` & `canopy-8.9/canopy/load_study_job.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/load_study_job_scalar_results.py` & `canopy-8.9/canopy/load_study_job_scalar_results.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/load_study_scalar_results.py` & `canopy-8.9/canopy/load_study_scalar_results.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/load_vector_metadata.py` & `canopy-8.9/canopy/load_vector_metadata.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/local_config.py` & `canopy-8.9/canopy/local_config.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/__init__.py` & `canopy-8.9/canopy/openapi/__init__.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/api/__init__.py` & `canopy-8.9/canopy/openapi/api/__init__.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/api/account_settings_api.py` & `canopy-8.9/canopy/openapi/api/account_settings_api.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/api/availability_api.py` & `canopy-8.9/canopy/openapi/api/availability_api.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/api/config_api.py` & `canopy-8.9/canopy/openapi/api/config_api.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/api/end_to_end_test_inbox_api.py` & `canopy-8.9/canopy/openapi/api/end_to_end_test_inbox_api.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/api/list_filter_api.py` & `canopy-8.9/canopy/openapi/api/list_filter_api.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/api/membership_api.py` & `canopy-8.9/canopy/openapi/api/membership_api.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/api/pool_api.py` & `canopy-8.9/canopy/openapi/api/pool_api.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/api/sim_version_api.py` & `canopy-8.9/canopy/openapi/api/sim_version_api.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/api/study_api.py` & `canopy-8.9/canopy/openapi/api/study_api.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/api/support_session_api.py` & `canopy-8.9/canopy/openapi/api/support_session_api.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/api/tenancy_api.py` & `canopy-8.9/canopy/openapi/api/tenancy_api.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/api/tenant_settings_api.py` & `canopy-8.9/canopy/openapi/api/tenant_settings_api.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/api/user_settings_api.py` & `canopy-8.9/canopy/openapi/api/user_settings_api.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/api/worksheet_api.py` & `canopy-8.9/canopy/openapi/api/worksheet_api.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/api_client.py` & `canopy-8.9/canopy/openapi/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from dateutil.parser import parse
 import json
 import mimetypes
 from multiprocessing.pool import ThreadPool
 import os
 import re
 import tempfile
+import numpy as np
 
 # python 2 and python 3 compatibility library
 import six
 from six.moves.urllib.parse import quote
 
 from canopy.openapi.configuration import Configuration
 import canopy.openapi.models
@@ -213,15 +214,15 @@
         :param obj: The data to serialize.
         :return: The serialized form of data.
         """
         if obj is None:
             return None
         elif isinstance(obj, self.PRIMITIVE_TYPES):
             return obj
-        elif isinstance(obj, list):
+        elif isinstance(obj, (list, np.ndarray)):
             return [self.sanitize_for_serialization(sub_obj)
                     for sub_obj in obj]
         elif isinstance(obj, tuple):
             return tuple(self.sanitize_for_serialization(sub_obj)
                          for sub_obj in obj)
         elif isinstance(obj, (datetime.datetime, datetime.date)):
             return obj.isoformat()
```

### Comparing `canopy-8.8/canopy/openapi/configuration.py` & `canopy-8.9/canopy/openapi/configuration.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/exceptions.py` & `canopy-8.9/canopy/openapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/__init__.py` & `canopy-8.9/canopy/openapi/models/__init__.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/additional_tests.py` & `canopy-8.9/canopy/openapi/models/additional_tests.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/admin_tenant_settings.py` & `canopy-8.9/canopy/openapi/models/admin_tenant_settings.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/admin_tenant_settings_builder.py` & `canopy-8.9/canopy/openapi/models/admin_tenant_settings_builder.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/auto_scale_run.py` & `canopy-8.9/canopy/openapi/models/auto_scale_run.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/auto_scale_run_error.py` & `canopy-8.9/canopy/openapi/models/auto_scale_run_error.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/availability_result.py` & `canopy-8.9/canopy/openapi/models/availability_result.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/batch_create_configs_result.py` & `canopy-8.9/canopy/openapi/models/batch_create_configs_result.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/blob_access_information.py` & `canopy-8.9/canopy/openapi/models/blob_access_information.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/canopy_document.py` & `canopy-8.9/canopy/openapi/models/canopy_document.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/channel_import_mapping.py` & `canopy-8.9/canopy/openapi/models/channel_import_mapping.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/channel_settings.py` & `canopy-8.9/canopy/openapi/models/channel_settings.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/chart_settings.py` & `canopy-8.9/canopy/openapi/models/chart_settings.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/collated_label_definitions.py` & `canopy-8.9/canopy/openapi/models/collated_label_definitions.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/collated_worksheet_labels.py` & `canopy-8.9/canopy/openapi/models/collated_worksheet_labels.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/compute_node_result.py` & `canopy-8.9/canopy/openapi/models/compute_node_result.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/config_column_label_definitions.py` & `canopy-8.9/canopy/openapi/models/config_column_label_definitions.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/config_hash.py` & `canopy-8.9/canopy/openapi/models/config_hash.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/config_owner_data.py` & `canopy-8.9/canopy/openapi/models/config_owner_data.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/config_reference.py` & `canopy-8.9/canopy/openapi/models/config_reference.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/config_resolved_labels.py` & `canopy-8.9/canopy/openapi/models/config_resolved_labels.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/config_resolved_reference.py` & `canopy-8.9/canopy/openapi/models/config_resolved_reference.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/config_resolved_reference_data.py` & `canopy-8.9/canopy/openapi/models/config_resolved_reference_data.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/config_type_definition.py` & `canopy-8.9/canopy/openapi/models/config_type_definition.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/config_type_metadata.py` & `canopy-8.9/canopy/openapi/models/config_type_metadata.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/default_config_id.py` & `canopy-8.9/canopy/openapi/models/default_config_id.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/default_config_reference.py` & `canopy-8.9/canopy/openapi/models/default_config_reference.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/default_custom_property_names.py` & `canopy-8.9/canopy/openapi/models/default_custom_property_names.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/document_custom_property_data.py` & `canopy-8.9/canopy/openapi/models/document_custom_property_data.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/document_custom_property_group.py` & `canopy-8.9/canopy/openapi/models/document_custom_property_group.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/document_group_result.py` & `canopy-8.9/canopy/openapi/models/document_group_result.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/document_name_result.py` & `canopy-8.9/canopy/openapi/models/document_name_result.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/document_type_custom_property_groups.py` & `canopy-8.9/canopy/openapi/models/document_type_custom_property_groups.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/document_user_information.py` & `canopy-8.9/canopy/openapi/models/document_user_information.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/documents_and_continuation_token.py` & `canopy-8.9/canopy/openapi/models/documents_and_continuation_token.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/duplicate_configs_data.py` & `canopy-8.9/canopy/openapi/models/duplicate_configs_data.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/duplicate_configs_result.py` & `canopy-8.9/canopy/openapi/models/duplicate_configs_result.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/file_download_metadata.py` & `canopy-8.9/canopy/openapi/models/file_download_metadata.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/get_account_settings_result.py` & `canopy-8.9/canopy/openapi/models/get_account_settings_result.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/get_admin_tenant_settings_query_result.py` & `canopy-8.9/canopy/openapi/models/get_admin_tenant_settings_query_result.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/get_all_support_sessions_query_result.py` & `canopy-8.9/canopy/openapi/models/get_all_support_sessions_query_result.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/get_all_tenants_study_statistics_query_result.py` & `canopy-8.9/canopy/openapi/models/get_all_tenants_study_statistics_query_result.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/get_config_names_query_result.py` & `canopy-8.9/canopy/openapi/models/get_config_names_query_result.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/get_config_query_result.py` & `canopy-8.9/canopy/openapi/models/get_config_query_result.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/get_config_versions_query_result.py` & `canopy-8.9/canopy/openapi/models/get_config_versions_query_result.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/get_configs_query_result.py` & `canopy-8.9/canopy/openapi/models/get_configs_query_result.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/get_pool_status_query_result.py` & `canopy-8.9/canopy/openapi/models/get_pool_status_query_result.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/get_pools_item.py` & `canopy-8.9/canopy/openapi/models/get_pools_item.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/get_pools_item_interval.py` & `canopy-8.9/canopy/openapi/models/get_pools_item_interval.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/get_pools_query_result.py` & `canopy-8.9/canopy/openapi/models/get_pools_query_result.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/get_sim_version_document_query_result.py` & `canopy-8.9/canopy/openapi/models/get_sim_version_document_query_result.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/get_sim_version_documents_query_result.py` & `canopy-8.9/canopy/openapi/models/get_sim_version_documents_query_result.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/get_sim_version_downloads_query_result.py` & `canopy-8.9/canopy/openapi/models/get_sim_version_downloads_query_result.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/get_studies_query_result.py` & `canopy-8.9/canopy/openapi/models/get_studies_query_result.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/get_study_download_url_query_result.py` & `canopy-8.9/canopy/openapi/models/get_study_download_url_query_result.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/get_study_job_metadata_query_result.py` & `canopy-8.9/canopy/openapi/models/get_study_job_metadata_query_result.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/get_study_job_query_result.py` & `canopy-8.9/canopy/openapi/models/get_study_job_query_result.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/get_study_jobs_query_result.py` & `canopy-8.9/canopy/openapi/models/get_study_jobs_query_result.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/get_study_query_result.py` & `canopy-8.9/canopy/openapi/models/get_study_query_result.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/get_study_types_query_result.py` & `canopy-8.9/canopy/openapi/models/get_study_types_query_result.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/get_support_session_query_result.py` & `canopy-8.9/canopy/openapi/models/get_support_session_query_result.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/get_tenant_access_information_query_result.py` & `canopy-8.9/canopy/openapi/models/get_tenant_access_information_query_result.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/get_tenant_billable_stored_simulation_count_query_result.py` & `canopy-8.9/canopy/openapi/models/get_tenant_billable_stored_simulation_count_query_result.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/get_tenant_channel_import_mappings_query_result.py` & `canopy-8.9/canopy/openapi/models/get_tenant_channel_import_mappings_query_result.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/get_tenant_default_custom_property_names_query_result.py` & `canopy-8.9/canopy/openapi/models/get_tenant_default_custom_property_names_query_result.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/get_tenant_query_result.py` & `canopy-8.9/canopy/openapi/models/get_tenant_query_result.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/get_tenant_settings_sim_version_query_result.py` & `canopy-8.9/canopy/openapi/models/get_tenant_settings_sim_version_query_result.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/get_tenant_study_statistics_query_result.py` & `canopy-8.9/canopy/openapi/models/get_tenant_study_statistics_query_result.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/get_tenant_users_query_result.py` & `canopy-8.9/canopy/openapi/models/get_tenant_users_query_result.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/get_tenant_users_query_result_user_item.py` & `canopy-8.9/canopy/openapi/models/get_tenant_users_query_result_user_item.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/get_tenant_worksheet_label_definitions_query_result.py` & `canopy-8.9/canopy/openapi/models/get_tenant_worksheet_label_definitions_query_result.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/get_tenants_query_result.py` & `canopy-8.9/canopy/openapi/models/get_tenants_query_result.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/get_tenants_query_result_tenant_item.py` & `canopy-8.9/canopy/openapi/models/get_tenants_query_result_tenant_item.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/get_user_roles_query_result.py` & `canopy-8.9/canopy/openapi/models/get_user_roles_query_result.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/get_user_settings_query_result.py` & `canopy-8.9/canopy/openapi/models/get_user_settings_query_result.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/get_wiki_document_query_result.py` & `canopy-8.9/canopy/openapi/models/get_wiki_document_query_result.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/get_worksheet_query_result.py` & `canopy-8.9/canopy/openapi/models/get_worksheet_query_result.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/i_previous_definition_sim_type_definition.py` & `canopy-8.9/canopy/openapi/models/i_previous_definition_sim_type_definition.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/i_previous_definition_study_type_definition.py` & `canopy-8.9/canopy/openapi/models/i_previous_definition_study_type_definition.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/identified_user_data.py` & `canopy-8.9/canopy/openapi/models/identified_user_data.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/label_definition.py` & `canopy-8.9/canopy/openapi/models/label_definition.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/label_definitions.py` & `canopy-8.9/canopy/openapi/models/label_definitions.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/list_filter.py` & `canopy-8.9/canopy/openapi/models/list_filter.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/list_filter_condition.py` & `canopy-8.9/canopy/openapi/models/list_filter_condition.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/list_filter_group.py` & `canopy-8.9/canopy/openapi/models/list_filter_group.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/name_value_pair.py` & `canopy-8.9/canopy/openapi/models/name_value_pair.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/new_batch_config_data.py` & `canopy-8.9/canopy/openapi/models/new_batch_config_data.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/new_config_data.py` & `canopy-8.9/canopy/openapi/models/new_config_data.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/new_sim_version_data.py` & `canopy-8.9/canopy/openapi/models/new_sim_version_data.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/new_study_data.py` & `canopy-8.9/canopy/openapi/models/new_study_data.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/new_study_data_source.py` & `canopy-8.9/canopy/openapi/models/new_study_data_source.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/new_tenant_data.py` & `canopy-8.9/canopy/openapi/models/new_tenant_data.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/new_worksheet_data.py` & `canopy-8.9/canopy/openapi/models/new_worksheet_data.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/password_reset_confirmation_data.py` & `canopy-8.9/canopy/openapi/models/password_reset_confirmation_data.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/password_reset_request_data.py` & `canopy-8.9/canopy/openapi/models/password_reset_request_data.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/pool_settings.py` & `canopy-8.9/canopy/openapi/models/pool_settings.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/post_study_result.py` & `canopy-8.9/canopy/openapi/models/post_study_result.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/registration_data.py` & `canopy-8.9/canopy/openapi/models/registration_data.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/resolved_label.py` & `canopy-8.9/canopy/openapi/models/resolved_label.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/resolved_statistic_label.py` & `canopy-8.9/canopy/openapi/models/resolved_statistic_label.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/sim_type_definition.py` & `canopy-8.9/canopy/openapi/models/sim_type_definition.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/sim_type_input_telemetry_channel.py` & `canopy-8.9/canopy/openapi/models/sim_type_input_telemetry_channel.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/sim_type_input_telemetry_channels.py` & `canopy-8.9/canopy/openapi/models/sim_type_input_telemetry_channels.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/sim_type_input_telemetry_evaluated_channel.py` & `canopy-8.9/canopy/openapi/models/sim_type_input_telemetry_evaluated_channel.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/sim_type_input_telemetry_evaluated_channel_suffix.py` & `canopy-8.9/canopy/openapi/models/sim_type_input_telemetry_evaluated_channel_suffix.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/sim_version_document_name_result.py` & `canopy-8.9/canopy/openapi/models/sim_version_document_name_result.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/simulation_column_label_definitions.py` & `canopy-8.9/canopy/openapi/models/simulation_column_label_definitions.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/simulation_input.py` & `canopy-8.9/canopy/openapi/models/simulation_input.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/simulation_resolved_labels.py` & `canopy-8.9/canopy/openapi/models/simulation_resolved_labels.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/study_blob_access_information.py` & `canopy-8.9/canopy/openapi/models/study_blob_access_information.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/study_document.py` & `canopy-8.9/canopy/openapi/models/study_document.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/study_document_study_document_data_source.py` & `canopy-8.9/canopy/openapi/models/study_document_study_document_data_source.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/study_documents_and_continuation_token.py` & `canopy-8.9/canopy/openapi/models/study_documents_and_continuation_token.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/study_input_hash.py` & `canopy-8.9/canopy/openapi/models/study_input_hash.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/study_input_hashes.py` & `canopy-8.9/canopy/openapi/models/study_input_hashes.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/study_job_documents_and_continuation_token.py` & `canopy-8.9/canopy/openapi/models/study_job_documents_and_continuation_token.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/study_reference.py` & `canopy-8.9/canopy/openapi/models/study_reference.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/study_resolved_labels.py` & `canopy-8.9/canopy/openapi/models/study_resolved_labels.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/study_resolved_reference.py` & `canopy-8.9/canopy/openapi/models/study_resolved_reference.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/study_resolved_reference_data.py` & `canopy-8.9/canopy/openapi/models/study_resolved_reference_data.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/study_type_definition.py` & `canopy-8.9/canopy/openapi/models/study_type_definition.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/support_session.py` & `canopy-8.9/canopy/openapi/models/support_session.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/support_session_data.py` & `canopy-8.9/canopy/openapi/models/support_session_data.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/support_session_response.py` & `canopy-8.9/canopy/openapi/models/support_session_response.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/tenant_config_reference.py` & `canopy-8.9/canopy/openapi/models/tenant_config_reference.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/tenant_default_custom_property_names.py` & `canopy-8.9/canopy/openapi/models/tenant_default_custom_property_names.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/tenant_information.py` & `canopy-8.9/canopy/openapi/models/tenant_information.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/tenant_statistics.py` & `canopy-8.9/canopy/openapi/models/tenant_statistics.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/test_auto_scale_formula_query_result.py` & `canopy-8.9/canopy/openapi/models/test_auto_scale_formula_query_result.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/text_document.py` & `canopy-8.9/canopy/openapi/models/text_document.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/text_document_optional_content.py` & `canopy-8.9/canopy/openapi/models/text_document_optional_content.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/updated_account_settings.py` & `canopy-8.9/canopy/openapi/models/updated_account_settings.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/updated_admin_tenant_settings.py` & `canopy-8.9/canopy/openapi/models/updated_admin_tenant_settings.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/updated_channel_import_mappings.py` & `canopy-8.9/canopy/openapi/models/updated_channel_import_mappings.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/updated_config_data.py` & `canopy-8.9/canopy/openapi/models/updated_config_data.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/updated_study_data.py` & `canopy-8.9/canopy/openapi/models/updated_study_data.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/updated_tenant_data.py` & `canopy-8.9/canopy/openapi/models/updated_tenant_data.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/updated_tenant_default_custom_property_names.py` & `canopy-8.9/canopy/openapi/models/updated_tenant_default_custom_property_names.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/updated_tenant_settings_sim_version.py` & `canopy-8.9/canopy/openapi/models/updated_tenant_settings_sim_version.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/updated_user_settings.py` & `canopy-8.9/canopy/openapi/models/updated_user_settings.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/updated_worksheet_data.py` & `canopy-8.9/canopy/openapi/models/updated_worksheet_data.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/updated_worksheet_label_definitions.py` & `canopy-8.9/canopy/openapi/models/updated_worksheet_label_definitions.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/upgrade_config_data.py` & `canopy-8.9/canopy/openapi/models/upgrade_config_data.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/upgrade_config_query_result.py` & `canopy-8.9/canopy/openapi/models/upgrade_config_query_result.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/user_information.py` & `canopy-8.9/canopy/openapi/models/user_information.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/user_role_data.py` & `canopy-8.9/canopy/openapi/models/user_role_data.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/user_settings.py` & `canopy-8.9/canopy/openapi/models/user_settings.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/user_settings_builder.py` & `canopy-8.9/canopy/openapi/models/user_settings_builder.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/versioned_document_metadata.py` & `canopy-8.9/canopy/openapi/models/versioned_document_metadata.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/worksheet.py` & `canopy-8.9/canopy/openapi/models/worksheet.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/worksheet_config.py` & `canopy-8.9/canopy/openapi/models/worksheet_config.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/worksheet_outline.py` & `canopy-8.9/canopy/openapi/models/worksheet_outline.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/worksheet_resolved_references.py` & `canopy-8.9/canopy/openapi/models/worksheet_resolved_references.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/worksheet_row.py` & `canopy-8.9/canopy/openapi/models/worksheet_row.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/models/worksheet_study.py` & `canopy-8.9/canopy/openapi/models/worksheet_study.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi/rest.py` & `canopy-8.9/canopy/openapi/rest.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/openapi_asyncio/api_client.py` & `canopy-8.9/canopy/openapi_asyncio/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from dateutil.parser import parse
 import json
 import mimetypes
 from multiprocessing.pool import ThreadPool
 import os
 import re
 import tempfile
+import numpy as np
 
 # python 2 and python 3 compatibility library
 import six
 from six.moves.urllib.parse import quote
 
 from canopy.openapi.configuration import Configuration
 import canopy.openapi.models
@@ -213,15 +214,15 @@
         :param obj: The data to serialize.
         :return: The serialized form of data.
         """
         if obj is None:
             return None
         elif isinstance(obj, self.PRIMITIVE_TYPES):
             return obj
-        elif isinstance(obj, list):
+        elif isinstance(obj, (list, np.ndarray)):
             return [self.sanitize_for_serialization(sub_obj)
                     for sub_obj in obj]
         elif isinstance(obj, tuple):
             return tuple(self.sanitize_for_serialization(sub_obj)
                          for sub_obj in obj)
         elif isinstance(obj, (datetime.datetime, datetime.date)):
             return obj.isoformat()
```

### Comparing `canopy-8.8/canopy/openapi_asyncio/rest.py` & `canopy-8.9/canopy/openapi_asyncio/rest.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/process_data_frame.py` & `canopy-8.9/canopy/process_data_frame.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/process_data_frame_test.py` & `canopy-8.9/canopy/process_data_frame_test.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/prompt_for_authentication.py` & `canopy-8.9/canopy/prompt_for_authentication.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/properties_dict_to_list.py` & `canopy-8.9/canopy/properties_dict_to_list.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/proxy_configuration.py` & `canopy-8.9/canopy/proxy_configuration.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/proxy_configuration_test.py` & `canopy-8.9/canopy/proxy_configuration_test.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/session.py` & `canopy-8.9/canopy/session.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/sim_version_to_number_test.py` & `canopy-8.9/canopy/sim_version_to_number_test.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/study_job_result.py` & `canopy-8.9/canopy/study_job_result.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/study_result.py` & `canopy-8.9/canopy/study_result.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/study_scalar_results.py` & `canopy-8.9/canopy/study_scalar_results.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/study_types_cache.py` & `canopy-8.9/canopy/study_types_cache.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/tenant_sim_version_cache.py` & `canopy-8.9/canopy/tenant_sim_version_cache.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/tenant_users.py` & `canopy-8.9/canopy/tenant_users.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/tenant_users_cache.py` & `canopy-8.9/canopy/tenant_users_cache.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/tenant_users_test.py` & `canopy-8.9/canopy/tenant_users_test.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/try_load_csv_from_url.py` & `canopy-8.9/canopy/try_load_csv_from_url.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/units.py` & `canopy-8.9/canopy/units.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/units_test.py` & `canopy-8.9/canopy/units_test.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/update_config.py` & `canopy-8.9/canopy/update_config.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/user_settings_cache.py` & `canopy-8.9/canopy/user_settings_cache.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy/wait_for_study.py` & `canopy-8.9/canopy/wait_for_study.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/canopy.egg-info/PKG-INFO` & `canopy-8.9/canopy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canopy
-Version: 8.8
+Version: 8.9
 Summary: Python Client for the Canopy Simulation API
 Home-page: https://github.com/canopysimulations/canopy-python/
 Author: James Thurley
 Author-email: james.thurley@canopysimulations.com
 License: MIT
 Description: # Installation
         
@@ -179,15 +179,17 @@
         sed -i 's/from canopy\.openapi import rest/from canopy.openapi_asyncio import rest/g' gen/canopy/openapi_asyncio/api_client.py
         sed -i '/from canopy.*/d' gen/canopy/openapi_asyncio/__init__.py
         sed -i '/# import /d' gen/canopy/openapi_asyncio/__init__.py
         echo 'from canopy.openapi_asyncio.api_client import ApiClient' >> gen/canopy/openapi_asyncio/__init__.py
         cp -r gen/canopy/openapi_asyncio repo/canopy
         ```
         
-        Note: The openapi_asyncio/rest.py file will need to be manually modified to support proxy servers after generation. 
+        Note: The `openapi_asyncio/rest.py` file will need to be manually modified to support proxy servers after generation. 
+        Note: The `openapi_asyncio/client_api.py` and `openapi/client_api.py` files will need to be manually modified to 
+        support numpy array serialization after generation. 
         
         ## Documentation for OpenAPI Generated Client
         
         OpenAPI generated documentation can be found [here](OPENAPI_README.md).
         
 Keywords: Canopy API,Canopy Simulations,Canopy Client
 Platform: UNKNOWN
```

### Comparing `canopy-8.8/canopy.egg-info/SOURCES.txt` & `canopy-8.9/canopy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `canopy-8.8/integration_tests/environment.py` & `canopy-8.9/integration_tests/environment.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/integration_tests/environment_data.py` & `canopy-8.9/integration_tests/environment_data.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/integration_tests/environment_loader.py` & `canopy-8.9/integration_tests/environment_loader.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/integration_tests/test_config.py` & `canopy-8.9/integration_tests/test_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from asyncio import Future
 from typing import List, Optional
 
 import asyncio
 import pytest
+import numpy as np
 
 import canopy
 import integration_tests
 
 default_car_name = 'Canopy F1 Car 2019'
 test_car_name = 'Python Automated Test Car'
 test_car_name_2 = 'Python Automated Test Car 2'
@@ -64,14 +65,29 @@
                 test_car_name_2,
                 state.default_car.raw_data)
 
             assert state.test_car_config_id_2 is not None
 
             state.configs_to_remove.append(state.test_car_config_id_2)
 
+    async def test_0220_it_should_create_a_config_containing_numpy_arrays(self, state: State):
+        async with integration_tests.Environment() as environment:
+            state.default_car.data.chassis.rUndertrayFront = np.array(state.default_car.data.chassis.rUndertrayFront)
+
+            state.test_car_config_id = await canopy.create_config(
+                environment.session,
+                'car',
+                test_car_name,
+                state.default_car.raw_data,
+                test_car_custom_properties)
+
+            assert state.test_car_config_id is not None
+
+            state.configs_to_remove.append(state.test_car_config_id)
+
     async def test_0300_it_should_find_a_config_by_name(self, state: State):
         async with integration_tests.Environment() as environment:
             car = await canopy.find_config(
                 environment.session,
                 'car',
                 owner_username=environment.data.authentication.username,
                 name=test_car_name)
```

### Comparing `canopy-8.8/integration_tests/test_study.py` & `canopy-8.9/integration_tests/test_study.py`

 * *Files identical despite different names*

### Comparing `canopy-8.8/setup.py` & `canopy-8.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from setuptools import setup, find_packages  # noqa: H301
 
 with open('README.md') as f:
     long_description = f.read()
 
 NAME = "canopy"
-VERSION = "8.8"
+VERSION = "8.9"
 
 REQUIRES = [
     "numpy",
     "certifi>=2017.4.17",
     "six>=1.10",
     "python-dateutil>=2.1",
     "urllib3>=1.23",
```

