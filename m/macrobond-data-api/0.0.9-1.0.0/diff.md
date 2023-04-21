# Comparing `tmp/macrobond-data-api-0.0.9.tar.gz` & `tmp/macrobond-data-api-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/macrobond-data-api/macrobond-data-api/dist/.tmp-twqbz4ne/macrobond-data-api-0.0.9.tar", last modified: Wed Mar  1 14:26:43 2023, max compression
+gzip compressed data, was "/home/runner/work/macrobond-data-api/macrobond-data-api/dist/.tmp-1oq_9ln_/macrobond-data-api-1.0.0.tar", last modified: Fri Apr 21 09:00:18 2023, max compression
```

## Comparing `macrobond-data-api-0.0.9.tar` & `macrobond-data-api-1.0.0.tar`

### file list

```diff
@@ -1,142 +1,148 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:26:43.000000 macrobond-data-api-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-03-01 14:26:43.000000 macrobond-data-api-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:26:43.000000 macrobond-data-api-0.0.9/macrobond_data_api/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-03-01 14:26:43.000000 macrobond-data-api-0.0.9/macrobond_data_api/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17420 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/_generated.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/_get_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:26:43.000000 macrobond-data-api-0.0.9/macrobond_data_api/com/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/com/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/com/_com_api_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    12002 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/com/_com_api_revision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/com/_com_api_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     5942 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/com/_com_api_series.py
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/com/_fill_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/com/com_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/com/com_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:26:43.000000 macrobond-data-api-0.0.9/macrobond_data_api/com/com_types/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/com/com_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/com/com_types/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6373 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/com/com_types/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/com/com_types/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/com/com_types/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/com/com_types/metadata_information.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/com/com_types/search_query.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/com/com_types/search_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/com/com_types/series.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/com/com_types/series_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/com/com_types/series_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/com/com_types/series_with_revisions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:26:43.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20026 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:26:43.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/enums/
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/enums/calendar_date_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/enums/calendar_merge_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/enums/metadata_attribute_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/enums/series_frequency.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/enums/series_missing_value_method.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/enums/series_partial_periods_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/enums/series_to_higher_frequency_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/enums/series_to_lower_frequency_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/enums/series_weekdays.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:26:43.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/types/
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/types/_repr_html_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/types/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/types/get_all_vintage_series_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/types/get_entity_error.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/types/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/types/metadata_attribute_information.py
--rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/types/metadata_value_information.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/types/revision_history_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/types/revision_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/types/search_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/types/search_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/types/search_result_long.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/types/series.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/types/series_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/types/series_observation_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/types/series_with_vintages.py
--rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/types/start_or_end_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/types/unified_series.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/types/values_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/common/types/vintage_series.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:26:43.000000 macrobond-data-api-0.0.9/macrobond_data_api/util/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/util/save_credential_to_keyring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:26:43.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/_metadata_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/_split_in_to_chunks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/_web_api_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    10288 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/_web_api_revision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/_web_api_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/_web_api_series.py
--rw-r--r--   0 runner    (1001) docker     (123)     9272 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/_web_only_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/scope.py
--rw-r--r--   0 runner    (1001) docker     (123)     7539 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     7671 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/subscription_list_poller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:26:43.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/entity_info_for_display_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/entity_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/entity_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/feed_entities_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/http_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:26:43.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/metadata/metadata_attribute_information_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/metadata/metadata_value_information_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/metadata_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/problem_details_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/response_error_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/revision_history_request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:26:43.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/search/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/search/item_listing_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/search/search_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/search/search_for_display_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/search/search_for_display_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/search/search_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/search/search_request_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/search/search_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/search_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)    12281 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/series_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/series_observation_history_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/series_response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:26:43.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/series_tree/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/series_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/series_tree/series_tree_listing_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/series_tree/series_tree_location_part.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/series_tree/series_tree_node_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/series_tree_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/series_with_revisions_info_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/series_with_times_of_change_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/series_with_vintages_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/subscription_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/subscription_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/subscription_list_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/subscription_list_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/unified_series_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/unified_series_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/values_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/vintage_series_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/vintage_values_response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:26:43.000000 macrobond-data-api-0.0.9/macrobond_data_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-03-01 14:26:43.000000 macrobond-data-api-0.0.9/macrobond_data_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-03-01 14:26:43.000000 macrobond-data-api-0.0.9/macrobond_data_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 14:26:43.000000 macrobond-data-api-0.0.9/macrobond_data_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-03-01 14:26:43.000000 macrobond-data-api-0.0.9/macrobond_data_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-01 14:26:43.000000 macrobond-data-api-0.0.9/macrobond_data_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-03-01 14:26:43.000000 macrobond-data-api-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-03-01 14:25:23.000000 macrobond-data-api-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:00:18.000000 macrobond-data-api-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-04-21 09:00:18.000000 macrobond-data-api-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:00:18.000000 macrobond-data-api-1.0.0/macrobond_data_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-21 09:00:18.000000 macrobond-data-api-1.0.0/macrobond_data_api/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19777 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/_generated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/_get_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:00:18.000000 macrobond-data-api-1.0.0/macrobond_data_api/com/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/com/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/com/_com_api_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15973 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/com/_com_api_revision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/com/_com_api_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/com/_com_api_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/com/_error_message_to_status_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/com/_fill_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/com/_fix_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/com/com_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/com/com_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:00:18.000000 macrobond-data-api-1.0.0/macrobond_data_api/com/com_types/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/com/com_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/com/com_types/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6373 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/com/com_types/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/com/com_types/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/com/com_types/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/com/com_types/metadata_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/com/com_types/search_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/com/com_types/search_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/com/com_types/series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/com/com_types/series_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/com/com_types/series_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/com/com_types/series_with_revisions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:00:18.000000 macrobond-data-api-1.0.0/macrobond_data_api/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23175 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/common/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/common/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:00:18.000000 macrobond-data-api-1.0.0/macrobond_data_api/common/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/common/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/common/enums/calendar_date_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/common/enums/calendar_merge_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/common/enums/metadata_attribute_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/common/enums/series_frequency.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/common/enums/series_missing_value_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/common/enums/series_partial_periods_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/common/enums/series_to_higher_frequency_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/common/enums/series_to_lower_frequency_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/common/enums/series_weekdays.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/common/enums/status_code.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:00:18.000000 macrobond-data-api-1.0.0/macrobond_data_api/common/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/common/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/common/types/_parse_iso8601.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/common/types/_repr_html_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/common/types/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/common/types/format_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/common/types/get_all_vintage_series_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/common/types/get_entity_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/common/types/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/common/types/metadata_attribute_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/common/types/metadata_value_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/common/types/revision_history_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/common/types/revision_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/common/types/search_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/common/types/search_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/common/types/search_result_long.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/common/types/series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/common/types/series_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/common/types/series_observation_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/common/types/series_with_vintages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/common/types/start_or_end_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/common/types/unified_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/common/types/values_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/common/types/vintage_series.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:00:18.000000 macrobond-data-api-1.0.0/macrobond_data_api/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/util/save_credential_to_keyring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:00:18.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/_metadata_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/_split_in_to_chunks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10015 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/_subscription_list_poller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/_web_api_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11660 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/_web_api_revision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/_web_api_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/_web_api_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9824 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/_web_only_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7951 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/subscription_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/web_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/web_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:00:18.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/entity_info_for_display_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/entity_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/entity_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/feed_entities_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/http_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:00:18.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/metadata/metadata_attribute_information_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/metadata/metadata_value_information_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/metadata_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/problem_details_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/response_error_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/revision_history_request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:00:18.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/search/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/search/item_listing_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/search/search_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/search/search_for_display_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/search/search_for_display_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/search/search_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/search/search_request_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/search/search_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/search_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12235 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/series_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/series_observation_history_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/series_response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:00:18.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/series_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/series_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/series_tree/series_tree_listing_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/series_tree/series_tree_location_part.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/series_tree/series_tree_node_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/series_tree_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/series_with_revisions_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/series_with_times_of_change_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/series_with_vintages_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/subscription_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/subscription_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/subscription_list_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/subscription_list_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/unified_series_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/unified_series_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/values_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/vintage_series_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/vintage_values_response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:00:18.000000 macrobond-data-api-1.0.0/macrobond_data_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-04-21 09:00:18.000000 macrobond-data-api-1.0.0/macrobond_data_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-04-21 09:00:18.000000 macrobond-data-api-1.0.0/macrobond_data_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 09:00:18.000000 macrobond-data-api-1.0.0/macrobond_data_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-21 09:00:18.000000 macrobond-data-api-1.0.0/macrobond_data_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-21 09:00:18.000000 macrobond-data-api-1.0.0/macrobond_data_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-21 09:00:18.000000 macrobond-data-api-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-04-21 08:58:44.000000 macrobond-data-api-1.0.0/setup.py
```

### Comparing `macrobond-data-api-0.0.9/LICENSE` & `macrobond-data-api-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.9/PKG-INFO` & `macrobond-data-api-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrobond-data-api
-Version: 0.0.9
+Version: 1.0.0
 Summary: Exposes a common API in Python for the Macrobond Web and Client Data APIs
 Home-page: https://github.com/macrobond/macrobond-data-api
 Author: Macrobond Financial
 Author-email: support@macrobond.com
 Project-URL: Documentation, https://macrobond.github.io/macrobond-data-api
 Project-URL: Source, https://github.com/macrobond/macrobond-data-api
 Project-URL: Tracker, https://github.com/macrobond/macrobond-data-api/issues
@@ -24,16 +24,14 @@
     <a href="https://www.macrobond.com/">
         <img loading="lazy" aria-roledescription="brand logo" alt="Macrobond logo" src="https://macrobond.github.io/macrobond-data-api/assets/Macrobond_logo_Color.svg" width="30%">
     </a>
 </div>
 
 <h1 align="center">Macrobond Data API for Python</h1>
 
-<h1 align="center">This software is in beta !</h1>
-
 <p align="center">
     <a href="https://pypi.org/project/macrobond-data-api/">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/macrobond-data-api">
     </a>
     <a href="https://pypi.org/project/macrobond-data-api/">
         <img alt="PyPI" src="https://img.shields.io/pypi/pyversions/macrobond-data-api.svg">
     </a>
@@ -62,14 +60,16 @@
 [Macrobond Web](https://help.macrobond.com/technical-information/the-macrobond-data-web-api-feed/)
 and [Client data](https://help.macrobond.com/technical-information/the-macrobond-api-for-python/)
 APIs
 
 You have to be a licensed user and have a Data+ or data feed user account in
 order to use the API.
 
+[***Examples in Jupyter Notebooks*** to help you get started](https://github.com/macrobond/macrobond-data-api/tree/main/examples)
+
 [***API reference***](https://macrobond.github.io/macrobond-data-api/)
 
 ## Basic usage
 
 ```python
 import macrobond_data_api as mb_api
 
@@ -79,21 +79,21 @@
 ## Advanced usage
 
 ```python
 # web
 from macrobond_data_api.web import WebClient
 
 with WebClient('client id', 'client secret') as api:
-    series = api.series.get_one_series('usgdp')
+    series = api.get_one_series('usgdp')
 
 # com
 from macrobond_data_api.com import ComClient
 
 with ComClient() as api:
-    series = api.series.get_one_series('usgdp')
+    series = api.get_one_series('usgdp')
 ```
 
 ## Features
 
 The Macrobond Data API for Python uses either the
 [Macrobond Web REST API](https://help.macrobond.com/technical-information/the-macrobond-data-web-api-feed/)
 or the [Macrobond Client data API](https://help.macrobond.com/technical-information/the-macrobond-api-for-python/)
```

#### html2text {}

```diff
@@ -1,51 +1,52 @@
-Metadata-Version: 2.1 Name: macrobond-data-api Version: 0.0.9 Summary: Exposes
+Metadata-Version: 2.1 Name: macrobond-data-api Version: 1.0.0 Summary: Exposes
 a common API in Python for the Macrobond Web and Client Data APIs Home-page:
 https://github.com/macrobond/macrobond-data-api Author: Macrobond Financial
 Author-email: support@macrobond.com Project-URL: Documentation, https://
 macrobond.github.io/macrobond-data-api Project-URL: Source, https://github.com/
 macrobond/macrobond-data-api Project-URL: Tracker, https://github.com/
 macrobond/macrobond-data-api/issues Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Requires-Python: >=3.7 Description-Content-Type: text/markdown Provides-
 Extra: extra Provides-Extra: dev Provides-Extra: socks License-File: LICENSE
                                [Macrobond_logo]
                   ****** Macrobond Data API for Python ******
-                   ****** This software is in beta ! ******
   [PyPI] [PyPI] [License:_MIT] [Code_style:_black] [Continuous_Integration]
  The Macrobond Data API for Python is used to access the worldâs most
 extensive macroeconomic, aggregate financial and sector database provided by
 [Macrobond](http://www.macrobond.com). Exposes a common API in Python for the
 [Macrobond Web](https://help.macrobond.com/technical-information/the-macrobond-
 data-web-api-feed/) and [Client data](https://help.macrobond.com/technical-
 information/the-macrobond-api-for-python/) APIs You have to be a licensed user
-and have a Data+ or data feed user account in order to use the API. [***API
+and have a Data+ or data feed user account in order to use the API.
+[***Examples in Jupyter Notebooks*** to help you get started](https://
+github.com/macrobond/macrobond-data-api/tree/main/examples) [***API
 reference***](https://macrobond.github.io/macrobond-data-api/) ## Basic usage
 ```python import macrobond_data_api as mb_api usgdp = mb_api.get_one_series
 ("usgdp") ``` ## Advanced usage ```python # web from macrobond_data_api.web
 import WebClient with WebClient('client id', 'client secret') as api: series =
-api.series.get_one_series('usgdp') # com from macrobond_data_api.com import
-ComClient with ComClient() as api: series = api.series.get_one_series('usgdp')
-``` ## Features The Macrobond Data API for Python uses either the [Macrobond
-Web REST API](https://help.macrobond.com/technical-information/the-macrobond-
-data-web-api-feed/) or the [Macrobond Client data API](https://
-help.macrobond.com/technical-information/the-macrobond-api-for-python/) to
-obtain time series with values and metadata. The API consists of a set of
-functions in common between the underlying APIs as well as specialized
-functions unique to each implementation. ## Installing macrobond-data-api and
-Supported Versions Macrobond Data API for Python is available on [PyPI](https:/
-/pypi.org/project/macrobond-data-api/): ```console python -m pip install
-macrobond-data-api ``` Macrobond Data API for Python officially supports Python
-3.6+. ## Using of system keyring When using WebClient it is recommended to use
-the system keyring. This can be done easily by running the include script using
-this command: ```console python -c "from macrobond_data_api.util import *;
-save_credential_to_keyring()" ``` ### Supported keyrings * macOS [Keychain]
-(https://en.wikipedia.org/wiki/Keychain_%28software%29) * Freedesktop [Secret
-Service](http://standards.freedesktop.org/secret-service/) supports many DE
-including GNOME (requires [secretstorage](https://pypi.python.org/pypi/
-secretstorage)) * KDE4 & KDE5 [KWallet](https://en.wikipedia.org/wiki/KWallet)
-(requires [dbus](https://pypi.python.org/pypi/dbus-python)) * [Windows
-Credential Locker](https://docs.microsoft.com/en-us/windows/uwp/security/
-credential-locker) ## Contributing We welcome community pull requests for bug
-fixes, enhancements, and documentation. ## Getting support [Support options]
-(https://help.macrobond.com/support/)
+api.get_one_series('usgdp') # com from macrobond_data_api.com import ComClient
+with ComClient() as api: series = api.get_one_series('usgdp') ``` ## Features
+The Macrobond Data API for Python uses either the [Macrobond Web REST API]
+(https://help.macrobond.com/technical-information/the-macrobond-data-web-api-
+feed/) or the [Macrobond Client data API](https://help.macrobond.com/technical-
+information/the-macrobond-api-for-python/) to obtain time series with values
+and metadata. The API consists of a set of functions in common between the
+underlying APIs as well as specialized functions unique to each implementation.
+## Installing macrobond-data-api and Supported Versions Macrobond Data API for
+Python is available on [PyPI](https://pypi.org/project/macrobond-data-api/):
+```console python -m pip install macrobond-data-api ``` Macrobond Data API for
+Python officially supports Python 3.6+. ## Using of system keyring When using
+WebClient it is recommended to use the system keyring. This can be done easily
+by running the include script using this command: ```console python -c "from
+macrobond_data_api.util import *; save_credential_to_keyring()" ``` ###
+Supported keyrings * macOS [Keychain](https://en.wikipedia.org/wiki/
+Keychain_%28software%29) * Freedesktop [Secret Service](http://
+standards.freedesktop.org/secret-service/) supports many DE including GNOME
+(requires [secretstorage](https://pypi.python.org/pypi/secretstorage)) * KDE4 &
+KDE5 [KWallet](https://en.wikipedia.org/wiki/KWallet) (requires [dbus](https://
+pypi.python.org/pypi/dbus-python)) * [Windows Credential Locker](https://
+docs.microsoft.com/en-us/windows/uwp/security/credential-locker) ##
+Contributing We welcome community pull requests for bug fixes, enhancements,
+and documentation. ## Getting support [Support options](https://
+help.macrobond.com/support/)
```

### Comparing `macrobond-data-api-0.0.9/README.md` & `macrobond-data-api-1.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,14 @@
     <a href="https://www.macrobond.com/">
         <img loading="lazy" aria-roledescription="brand logo" alt="Macrobond logo" src="https://macrobond.github.io/macrobond-data-api/assets/Macrobond_logo_Color.svg" width="30%">
     </a>
 </div>
 
 <h1 align="center">Macrobond Data API for Python</h1>
 
-<h1 align="center">This software is in beta !</h1>
-
 <p align="center">
     <a href="https://pypi.org/project/macrobond-data-api/">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/macrobond-data-api">
     </a>
     <a href="https://pypi.org/project/macrobond-data-api/">
         <img alt="PyPI" src="https://img.shields.io/pypi/pyversions/macrobond-data-api.svg">
     </a>
@@ -41,14 +39,16 @@
 [Macrobond Web](https://help.macrobond.com/technical-information/the-macrobond-data-web-api-feed/)
 and [Client data](https://help.macrobond.com/technical-information/the-macrobond-api-for-python/)
 APIs
 
 You have to be a licensed user and have a Data+ or data feed user account in
 order to use the API.
 
+[***Examples in Jupyter Notebooks*** to help you get started](https://github.com/macrobond/macrobond-data-api/tree/main/examples)
+
 [***API reference***](https://macrobond.github.io/macrobond-data-api/)
 
 ## Basic usage
 
 ```python
 import macrobond_data_api as mb_api
 
@@ -58,21 +58,21 @@
 ## Advanced usage
 
 ```python
 # web
 from macrobond_data_api.web import WebClient
 
 with WebClient('client id', 'client secret') as api:
-    series = api.series.get_one_series('usgdp')
+    series = api.get_one_series('usgdp')
 
 # com
 from macrobond_data_api.com import ComClient
 
 with ComClient() as api:
-    series = api.series.get_one_series('usgdp')
+    series = api.get_one_series('usgdp')
 ```
 
 ## Features
 
 The Macrobond Data API for Python uses either the
 [Macrobond Web REST API](https://help.macrobond.com/technical-information/the-macrobond-data-web-api-feed/)
 or the [Macrobond Client data API](https://help.macrobond.com/technical-information/the-macrobond-api-for-python/)
```

#### html2text {}

```diff
@@ -1,40 +1,41 @@
                                [Macrobond_logo]
                   ****** Macrobond Data API for Python ******
-                   ****** This software is in beta ! ******
   [PyPI] [PyPI] [License:_MIT] [Code_style:_black] [Continuous_Integration]
  The Macrobond Data API for Python is used to access the worldâs most
 extensive macroeconomic, aggregate financial and sector database provided by
 [Macrobond](http://www.macrobond.com). Exposes a common API in Python for the
 [Macrobond Web](https://help.macrobond.com/technical-information/the-macrobond-
 data-web-api-feed/) and [Client data](https://help.macrobond.com/technical-
 information/the-macrobond-api-for-python/) APIs You have to be a licensed user
-and have a Data+ or data feed user account in order to use the API. [***API
+and have a Data+ or data feed user account in order to use the API.
+[***Examples in Jupyter Notebooks*** to help you get started](https://
+github.com/macrobond/macrobond-data-api/tree/main/examples) [***API
 reference***](https://macrobond.github.io/macrobond-data-api/) ## Basic usage
 ```python import macrobond_data_api as mb_api usgdp = mb_api.get_one_series
 ("usgdp") ``` ## Advanced usage ```python # web from macrobond_data_api.web
 import WebClient with WebClient('client id', 'client secret') as api: series =
-api.series.get_one_series('usgdp') # com from macrobond_data_api.com import
-ComClient with ComClient() as api: series = api.series.get_one_series('usgdp')
-``` ## Features The Macrobond Data API for Python uses either the [Macrobond
-Web REST API](https://help.macrobond.com/technical-information/the-macrobond-
-data-web-api-feed/) or the [Macrobond Client data API](https://
-help.macrobond.com/technical-information/the-macrobond-api-for-python/) to
-obtain time series with values and metadata. The API consists of a set of
-functions in common between the underlying APIs as well as specialized
-functions unique to each implementation. ## Installing macrobond-data-api and
-Supported Versions Macrobond Data API for Python is available on [PyPI](https:/
-/pypi.org/project/macrobond-data-api/): ```console python -m pip install
-macrobond-data-api ``` Macrobond Data API for Python officially supports Python
-3.6+. ## Using of system keyring When using WebClient it is recommended to use
-the system keyring. This can be done easily by running the include script using
-this command: ```console python -c "from macrobond_data_api.util import *;
-save_credential_to_keyring()" ``` ### Supported keyrings * macOS [Keychain]
-(https://en.wikipedia.org/wiki/Keychain_%28software%29) * Freedesktop [Secret
-Service](http://standards.freedesktop.org/secret-service/) supports many DE
-including GNOME (requires [secretstorage](https://pypi.python.org/pypi/
-secretstorage)) * KDE4 & KDE5 [KWallet](https://en.wikipedia.org/wiki/KWallet)
-(requires [dbus](https://pypi.python.org/pypi/dbus-python)) * [Windows
-Credential Locker](https://docs.microsoft.com/en-us/windows/uwp/security/
-credential-locker) ## Contributing We welcome community pull requests for bug
-fixes, enhancements, and documentation. ## Getting support [Support options]
-(https://help.macrobond.com/support/)
+api.get_one_series('usgdp') # com from macrobond_data_api.com import ComClient
+with ComClient() as api: series = api.get_one_series('usgdp') ``` ## Features
+The Macrobond Data API for Python uses either the [Macrobond Web REST API]
+(https://help.macrobond.com/technical-information/the-macrobond-data-web-api-
+feed/) or the [Macrobond Client data API](https://help.macrobond.com/technical-
+information/the-macrobond-api-for-python/) to obtain time series with values
+and metadata. The API consists of a set of functions in common between the
+underlying APIs as well as specialized functions unique to each implementation.
+## Installing macrobond-data-api and Supported Versions Macrobond Data API for
+Python is available on [PyPI](https://pypi.org/project/macrobond-data-api/):
+```console python -m pip install macrobond-data-api ``` Macrobond Data API for
+Python officially supports Python 3.6+. ## Using of system keyring When using
+WebClient it is recommended to use the system keyring. This can be done easily
+by running the include script using this command: ```console python -c "from
+macrobond_data_api.util import *; save_credential_to_keyring()" ``` ###
+Supported keyrings * macOS [Keychain](https://en.wikipedia.org/wiki/
+Keychain_%28software%29) * Freedesktop [Secret Service](http://
+standards.freedesktop.org/secret-service/) supports many DE including GNOME
+(requires [secretstorage](https://pypi.python.org/pypi/secretstorage)) * KDE4 &
+KDE5 [KWallet](https://en.wikipedia.org/wiki/KWallet) (requires [dbus](https://
+pypi.python.org/pypi/dbus-python)) * [Windows Credential Locker](https://
+docs.microsoft.com/en-us/windows/uwp/security/credential-locker) ##
+Contributing We welcome community pull requests for bug fixes, enhancements,
+and documentation. ## Getting support [Support options](https://
+help.macrobond.com/support/)
```

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/_generated.py` & `macrobond-data-api-1.0.0/macrobond_data_api/_generated.py`

 * *Files 18% similar despite different names*

```diff
@@ -114,51 +114,55 @@
     Returns
     -------
     `macrobond_data_api.common.types.get_all_vintage_series_result.GetAllVintageSeriesResult`
     """
     return _get_api().get_all_vintage_series(series_name)
 
 
-def get_entities(*entity_names: str, raise_error: bool = None) -> Sequence[Entity]:
+def get_entities(entity_names: Sequence[str], raise_error: bool = None) -> Sequence[Entity]:
     """
     Download one or more entities.
 
     .. Important:: It is much more efficient to download more than one entity at a time.
        However, downloading too many at a time is less efficient and can exhaust memory.
        A good habit is to download entities in batches of around 200.
 
     Parameters
     ----------
-    *entity_names : str
-        One or more names of entities.
+    entity_names : Sequence[str]
+        The names of the entities.
     raise_error : bool
         If True, accessing the resulting entities raises a GetEntitiesError.
         If False you should inspect the is_error property of the result instead.
         If None, it will use the global value `macrobond_data_api.common.api.Api.raise_error`
 
     Returns
     -------
     `Sequence[macrobond_data_api.common.types.entity.Entity]`
     The result is in the same order as in the request.
     """
-    return _get_api().get_entities(*entity_names, raise_error=raise_error)
+    return _get_api().get_entities(entity_names, raise_error)
 
 
-def get_many_series(*series: Tuple[str, datetime]) -> Generator[Optional[Series], None, None]:
+def get_many_series(
+    series: Sequence[Union[str, Tuple[str, Optional[datetime]]]], include_not_modified: bool = False
+) -> Generator[Series, None, None]:
     """
     Parameters
     ----------
-    *series: `Tuple[str, datetime.datetime]`
-        A sequence of series requests.
+    series: `Sequence[Union[str, Tuple[str, Optional[datetime]]]]`
+        A sequence of series names or a sequence of name plus a timestamp for the last modification.
+    include_not_modified: `bool`
+        Set this value to True in order to include NotNodified series.
 
     Returns
     -------
     `Generator[Optional[macrobond_data_api.common.types.series.Series]]`
     """
-    return _get_api().get_many_series(*series)
+    return _get_api().get_many_series(series, include_not_modified)
 
 
 def get_many_series_with_revisions(
     requests: Sequence[RevisionHistoryRequest], include_not_modified: bool = False
 ) -> Generator[SeriesWithVintages, None, None]:
     """
     Download all revisions for one or more series.
@@ -183,38 +187,38 @@
     -------
     `Generator[macrobond_data_api.common.types.series_with_vintages.SeriesWithVintages]`
     """
     return _get_api().get_many_series_with_revisions(requests, include_not_modified)
 
 
 def get_nth_release(
-    nth: int, *series_names: str, include_times_of_change: bool = False, raise_error: bool = None
+    nth: int, series_names: Sequence[str], include_times_of_change: bool = False, raise_error: bool = None
 ) -> Sequence[Series]:
     """
-    Fetcha series where each value is the nth change of the value.
+    Get one or more series where each value is the nth change of the value.
 
     Parameters
     ----------
     time : nth
         The nth change of each value.
     series_names : str
-        One or more names of series.
+        The names of the series.
+    include_times_of_change : bool
+        Include information of the time each values was last changed.
     raise_error : bool
         If True, accessing the resulting series raises a GetEntitiesError.
         If False you should inspect the is_error property of the result instead.
         If None, it will use the global value `macrobond_data_api.common.api.Api.raise_error`
 
     Returns
     -------
     `Sequence[macrobond_data_api.common.types.series.Series]`
     The result is in the same order as in the request.
     """
-    return _get_api().get_nth_release(
-        nth, *series_names, include_times_of_change=include_times_of_change, raise_error=raise_error
-    )
+    return _get_api().get_nth_release(nth, series_names, include_times_of_change, raise_error)
 
 
 def get_observation_history(series_name: str, *times: datetime) -> Sequence[SeriesObservationHistory]:
     """
     Get the revision of an observation.
 
     Parameters
@@ -250,14 +254,40 @@
     Returns
     -------
     `macrobond_data_api.common.types.entity.Entity`
     """
     return _get_api().get_one_entity(entity_name, raise_error)
 
 
+def get_one_nth_release(
+    nth: int, series_name: str, include_times_of_change: bool = False, raise_error: bool = None
+) -> Series:
+    """
+    Get a series where each value is the nth change of the value.
+
+    Parameters
+    ----------
+    time : nth
+        The nth change of each value.
+    series_name : str
+        The name of the series.
+    include_times_of_change : bool
+        Include information of the time each values was last changed.
+    raise_error : bool
+        If True, accessing the resulting series raises a GetEntitiesError.
+        If False you should inspect the is_error property of the result instead.
+        If None, it will use the global value `macrobond_data_api.common.api.Api.raise_error`
+
+    Returns
+    -------
+    `macrobond_data_api.common.types.series.Series`
+    """
+    return _get_api().get_one_nth_release(nth, series_name, include_times_of_change, raise_error)
+
+
 def get_one_series(series_name: str, raise_error: bool = None) -> Series:
     """
     Download one series.
 
     .. important:: It is much more efficient to download more than one series at a time.
        See `Api.get_series`.
 
@@ -273,14 +303,40 @@
     Returns
     -------
     `macrobond_data_api.common.types.series.Series`
     """
     return _get_api().get_one_series(series_name, raise_error)
 
 
+def get_one_vintage_series(
+    time: datetime, series_name: str, include_times_of_change: bool = False, raise_error: bool = None
+) -> VintageSeries:
+    """
+    Get one vintage series.
+
+    Parameters
+    ----------
+    time : datetime
+        The time of the vintage to return.
+    series_name : str
+        The name of the series.
+    include_times_of_change : bool
+        Include information of the time each values was last changed.
+    raise_error : bool
+        If True, accessing the resulting series raises a GetEntitiesError.
+        If False you should inspect the is_error property of the result instead.
+        If None, it will use the global value `macrobond_data_api.common.api.Api.raise_error`
+
+    Returns
+    -------
+    `macrobond_data_api.common.types.vintage_series.VintageSeries`
+    """
+    return _get_api().get_one_vintage_series(time, series_name, include_times_of_change, raise_error)
+
+
 def get_revision_info(*series_names: str, raise_error: bool = None) -> Sequence[RevisionInfo]:
     """
     Get information about if revision history is available for a series
     and a list of revision timestamps.
 
     Parameters
     ----------
@@ -295,37 +351,37 @@
     -------
     `Sequence[macrobond_data_api.common.types.revision_info.RevisionInfo]`
     The result is in the sane order as in the request.
     """
     return _get_api().get_revision_info(*series_names, raise_error=raise_error)
 
 
-def get_series(*series_names: str, raise_error: bool = None) -> Sequence[Series]:
+def get_series(series_names: Sequence[str], raise_error: bool = None) -> Sequence[Series]:
     """
     Download one or more series.
 
     .. Important:: It is much more efficient to download more than one series at a time.
        However, downloading too many at a time is less efficient and can exhaust memory.
        A good habit is to download series in batches of around 200.
 
     Parameters
     ----------
-    *series_names : str
-        One or more names of series.
+    series_names : Sequence[str]
+        The names of the series.
     raise_error : bool
         If True, accessing the resulting series raises a GetEntitiesError.
         If False you should inspect the is_error property of the result instead.
         If None, it will use the global value `macrobond_data_api.common.api.Api.raise_error`
 
     Returns
     -------
     `Sequence[macrobond_data_api.common.types.series.Series]`
     The result is in the same order as in the request.
     """
-    return _get_api().get_series(*series_names, raise_error=raise_error)
+    return _get_api().get_series(series_names, raise_error)
 
 
 def get_unified_series(
     *series_entries: Union[SeriesEntry, str],
     frequency: SeriesFrequency = SeriesFrequency.HIGHEST,
     weekdays: SeriesWeekdays = SeriesWeekdays.MONDAY_TO_FRIDAY,
     calendar_merge_mode: CalendarMergeMode = CalendarMergeMode.AVAILABLE_IN_ANY,
@@ -374,35 +430,42 @@
         currency=currency,
         start_point=start_point,
         end_point=end_point,
         raise_error=raise_error
     )
 
 
-def get_vintage_series(time: datetime, *series_names: str, raise_error: bool = None) -> Sequence[VintageSeries]:
+def get_vintage_series(
+    time: datetime,
+    series_names: Sequence[str],
+    include_times_of_change: bool = False,
+    raise_error: bool = None,
+) -> Sequence[VintageSeries]:
     """
-    Fetch vintage series.
+    Get one or more vintage series.
 
     Parameters
     ----------
     time : datetime
         The time of the vintage to return.
     series_names : str
-        One or more names of series.
+        The names of the series.
+    include_times_of_change : bool
+        Include information of the time each values was last changed.
     raise_error : bool
         If True, accessing the resulting series raises a GetEntitiesError.
         If False you should inspect the is_error property of the result instead.
         If None, it will use the global value `macrobond_data_api.common.api.Api.raise_error`
 
     Returns
     -------
     `Sequence[macrobond_data_api.common.types.vintage_series.VintageSeries]`
     The result is in the same order as in the request.
     """
-    return _get_api().get_vintage_series(time, *series_names, raise_error=raise_error)
+    return _get_api().get_vintage_series(time, series_names, include_times_of_change, raise_error)
 
 
 def metadata_get_attribute_information(*names: str) -> Sequence[MetadataAttributeInformation]:
     """
     Get information about metadata attributes.
 
     Parameters
```

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/com/_com_api_metadata.py` & `macrobond-data-api-1.0.0/macrobond_data_api/com/_com_api_metadata.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/com/_com_api_revision.py` & `macrobond-data-api-1.0.0/macrobond_data_api/com/_com_api_revision.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 from math import isnan
 from typing import Generator, Optional, Tuple, List, TYPE_CHECKING, Sequence, cast
 
 from datetime import datetime, timezone
-from dateutil.tz import tzutc
 
 from macrobond_data_api.common.types import (
     RevisionInfo,
     GetEntitiesError,
     VintageSeries,
     Series,
     GetAllVintageSeriesResult,
     SeriesObservationHistory,
     SeriesWithVintages,
-    SeriesWithVintagesErrorCode,
     RevisionHistoryRequest,
     VintageValues,
 )
+from macrobond_data_api.common.enums import StatusCode
 
 from macrobond_data_api.common.types._repr_html_sequence import _ReprHtmlSequence
 
 from ._fill_metadata import _fill_metadata_from_entity, _fill_values_metadata_from_series
+from ._error_message_to_status_code import _error_message_to_status_code
+from ._fix_datetime import _fix_datetime, _fix_optional_datetime
 
 if TYPE_CHECKING:  # pragma: no cover
     from .com_api import ComApi
 
     from .com_types import SeriesWithRevisions
 
     from .com_types import Series as ComSeries, Entity as ComEntity
@@ -33,34 +34,45 @@
     return [datetime(x.year, x.month, x.day, x.hour, x.minute, x.second, x.microsecond, timezone.utc) for x in dates]
 
 
 def _datetime_to_datetime_timezone(dates: Sequence[datetime]) -> List[datetime]:
     return [datetime(x.year, x.month, x.day, x.hour, x.minute, x.second, x.microsecond) for x in dates]
 
 
+def _datetime_to_datetime_timezone_and_skip_com_datetime_min(dates: Sequence[datetime]) -> List[Optional[datetime]]:
+    return [_skip_com_datetime_min(x) for x in dates]
+
+
+def _skip_com_datetime_min(d: datetime) -> Optional[datetime]:
+    return None if d.year == 1899 and d.month == 12 and d.day == 30 else datetime(d.year, d.month, d.day)
+
+
 def _remove_padding(
     series: "ComSeries",
 ) -> Tuple[List[Optional[float]], Tuple[datetime, ...]]:
     series_values = series.Values
 
     padding_front = 0
     for value in series_values:
         if value is None or not isnan(value):
             break
-        padding_front = padding_front + 1
+        padding_front += 1
 
     padding_back = 0
     for value in series_values[::-1]:
         if value is None or not isnan(value):
             break
-        padding_back = padding_back + 1
+        padding_back += 1
 
     padding_back = len(series_values) - padding_back
 
-    return (list(series_values[padding_front:padding_back]), series.DatesAtStartOfPeriod[padding_front:padding_back])
+    values = [None if isnan(x) else x for x in series_values[padding_front:padding_back]]  # type: ignore
+    dates = series.DatesAtStartOfPeriod[padding_front:padding_back]
+
+    return (values, dates)
 
 
 def get_revision_info(self: "ComApi", *series_names: str, raise_error: bool = None) -> Sequence[RevisionInfo]:
     def to_obj(name: str, serie: "SeriesWithRevisions") -> RevisionInfo:
         if serie.IsError:
             return RevisionInfo(name, serie.ErrorMessage, False, False, None, None, [])
 
@@ -83,125 +95,224 @@
 
     if self.raise_error if raise_error is None else raise_error:
         GetEntitiesError._raise_if([(x, y.ErrorMessage) for x, y in zip(series_names, series)])
 
     return _ReprHtmlSequence([to_obj(x, y) for x, y in zip(series_names, series)])
 
 
+def get_one_vintage_series(
+    self: "ComApi", time: datetime, series_name: str, include_times_of_change: bool = False, raise_error: bool = None
+) -> VintageSeries:
+    return self.get_vintage_series(
+        time, [series_name], include_times_of_change=include_times_of_change, raise_error=raise_error
+    )[0]
+
+
 def get_vintage_series(
-    self: "ComApi", time: datetime, *series_names: str, raise_error: bool = None
+    self: "ComApi",
+    time: datetime,
+    series_names: Sequence[str],
+    include_times_of_change: bool = False,
+    raise_error: bool = None,
 ) -> Sequence[VintageSeries]:
+    time = _fix_datetime(time)
+
     def to_obj(series_name: str) -> VintageSeries:
         series_with_revisions = self.database.FetchOneSeriesWithRevisions(series_name)
 
         if series_with_revisions.IsError:
-            return VintageSeries(series_name, series_with_revisions.ErrorMessage, None, None, None, None, None)
+            return VintageSeries(
+                series_name,
+                series_with_revisions.ErrorMessage,
+                _error_message_to_status_code(series_with_revisions),
+                None,
+                None,
+                None,
+                None,
+                None,
+            )
 
         try:
             series = series_with_revisions.GetVintage(time)
         except OSError as os_error:
             if os_error.errno == 22 and os_error.strerror == "Invalid argument":
                 raise ValueError("Invalid time") from os_error
             raise os_error
 
         if series.IsError:
-            return VintageSeries(series_name, series.ErrorMessage, None, None, None, None, None)
+            return VintageSeries(
+                series_name,
+                series.ErrorMessage,
+                _error_message_to_status_code(series),
+                None,
+                None,
+                None,
+                None,
+                None,
+            )
 
         values, dates = _remove_padding(series)
 
+        if include_times_of_change:
+            if series_with_revisions.HasRevisions:
+                values_metadata = _fill_values_metadata_from_series(series, True)
+            else:
+                values_metadata = [{}] * len(values)
+        else:
+            values_metadata = None
+
         return VintageSeries(
             series_name,
             "",
+            StatusCode.OK,
             _fill_metadata_from_entity(series),
-            None,
+            values_metadata,
             values,
             _datetime_to_datetime_timezone(dates),
             None,
         )
 
     series = [to_obj(x) for x in series_names]
 
     if self.raise_error if raise_error is None else raise_error:
         GetEntitiesError._raise_if([(x, y.error_message) for x, y in zip(series_names, series)])
 
     return _ReprHtmlSequence(series)
 
 
+def get_one_nth_release(
+    self: "ComApi", nth: int, series_name: str, include_times_of_change: bool = False, raise_error: bool = None
+) -> Series:
+    return self.get_nth_release(
+        nth, [series_name], include_times_of_change=include_times_of_change, raise_error=raise_error
+    )[0]
+
+
 def get_nth_release(
-    self: "ComApi", nth: int, *series_names: str, include_times_of_change: bool = False, raise_error: bool = None
+    self: "ComApi",
+    nth: int,
+    series_names: Sequence[str],
+    include_times_of_change: bool = False,
+    raise_error: bool = None,
 ) -> Sequence[Series]:
     if len(series_names) == 0:
         raise ValueError("No series names")
 
     def to_obj(series_name: str) -> Series:
         series_with_revisions = self.database.FetchOneSeriesWithRevisions(series_name)
 
         if series_with_revisions.IsError:
-            return Series(series_name, series_with_revisions.ErrorMessage, None, None, None, None)
+            return Series(
+                series_name,
+                series_with_revisions.ErrorMessage,
+                _error_message_to_status_code(series_with_revisions),
+                None,
+                None,
+                None,
+                None,
+            )
 
         series = series_with_revisions.GetNthRelease(nth)
         if series.IsError:
-            return Series(series_name, series.ErrorMessage, None, None, None, None)
+            return Series(
+                series_name, series.ErrorMessage, _error_message_to_status_code(series), None, None, None, None
+            )
 
         values = [None if isnan(x) else x for x in series.Values]  # type: ignore
         dates = _datetime_to_datetime_timezone(series.DatesAtStartOfPeriod)
-        values_metadata = _fill_values_metadata_from_series(series) if include_times_of_change else None
 
-        return Series(series_name, None, _fill_metadata_from_entity(series), values_metadata, values, dates)
+        if include_times_of_change:
+            if series_with_revisions.HasRevisions:
+                values_metadata = _fill_values_metadata_from_series(series)
+            else:
+                values_metadata = [{}] * len(values)
+        else:
+            values_metadata = None
+
+        return Series(
+            series_name, None, StatusCode.OK, _fill_metadata_from_entity(series), values_metadata, values, dates
+        )
 
     series = [to_obj(x) for x in series_names]
 
     if self.raise_error if raise_error is None else raise_error:
         GetEntitiesError._raise_if([(x, y.error_message) for x, y in zip(series_names, series)])
 
     return _ReprHtmlSequence(series)
 
 
 def get_all_vintage_series(self: "ComApi", series_name: str) -> GetAllVintageSeriesResult:
     def to_obj(com_series: "ComSeries", name: str) -> VintageSeries:
         if com_series.IsError:
-            return VintageSeries(name, com_series.ErrorMessage, None, None, None, None, None)
+            return VintageSeries(
+                name, com_series.ErrorMessage, _error_message_to_status_code(series), None, None, None, None, None
+            )
 
         values, dates = _remove_padding(com_series)
 
         return VintageSeries(
             name,
             None,
+            StatusCode.OK,
             _fill_metadata_from_entity(com_series),
             None,
             values,
             _datetime_to_datetime_timezone(dates),
             None,
         )
 
     series_with_revisions = self.database.FetchOneSeriesWithRevisions(series_name)
 
     if series_with_revisions.IsError:
         if series_with_revisions.ErrorMessage == "Not found":
             raise ValueError("Series not found: " + series_name)
         raise Exception(series_with_revisions.ErrorMessage)
 
-    return GetAllVintageSeriesResult(
-        [to_obj(x, series_name) for x in series_with_revisions.GetCompleteHistory()],
-        series_name,
-    )
+    complete_history = series_with_revisions.GetCompleteHistory()
+
+    if not series_with_revisions.HasRevisions:
+        series = complete_history[0]
+        values = [None if isnan(x) else x for x in series.Values]  # type: ignore
+        dates = _datetime_to_datetime_timezone(series.DatesAtStartOfPeriod)
+        return GetAllVintageSeriesResult(
+            [
+                VintageSeries(
+                    series_name, None, StatusCode.OK, _fill_metadata_from_entity(series), None, values, dates, None
+                )
+            ],
+            series_name,
+        )
+
+    return GetAllVintageSeriesResult([to_obj(x, series_name) for x in complete_history], series_name)
 
 
 def get_observation_history(self: "ComApi", series_name: str, *times: datetime) -> Sequence[SeriesObservationHistory]:
+    times = tuple(_fix_datetime(x) for x in times)
     series_with_revisions = self.database.FetchOneSeriesWithRevisions(series_name)
 
     if series_with_revisions.IsError:
         if series_with_revisions.ErrorMessage == "Not found":
             raise ValueError("Not found " + series_name)
         raise Exception(series_with_revisions.ErrorMessage)
 
     def to_obj(time: datetime) -> SeriesObservationHistory:
         series = series_with_revisions.GetObservationHistory(time)
-        dates = _datetime_to_datetime_timezone(series.DatesAtStartOfPeriod)
-        return SeriesObservationHistory(time, series.Values, dates)
+        observation_date = cast(datetime, series.Metadata.GetFirstValue("ObservationDate"))
+
+        # todo (2023-04-18) remove in the future, when the version is no longer supported by macrobond_data_api
+        if observation_date is None:
+            raise Exception(
+                "Your version of the Macrobond application does not support get_observation_history. "
+                + "Please upgrade to a later version."
+            )
+
+        observation_date = datetime(observation_date.year, observation_date.month, observation_date.day)
+        values = [None if isnan(x) else x for x in series.Values]
+        dates = _datetime_to_datetime_timezone_and_skip_com_datetime_min(series.DatesAtStartOfPeriod)
+        return SeriesObservationHistory(observation_date, values, dates)
 
     return _ReprHtmlSequence([to_obj(x) for x in times])
 
 
 def _create_vintage_values(
     start_index: int, vintage_dates: List[datetime], com_series: List["ComSeries"]
 ) -> Generator[VintageValues, None, None]:
@@ -214,15 +325,15 @@
             vintage_date.year,
             vintage_date.month,
             vintage_date.day,
             vintage_date.hour,
             vintage_date.minute,
             vintage_date.second,
             vintage_date.microsecond,
-            tzutc(),
+            timezone.utc,
         )
         values, dates = _remove_padding(series)
         yield VintageValues(vintage_date, _datetime_to_datetime_timezone(dates), values)
 
 
 def _equal_with_margin(d1: Optional[datetime], d2: Optional[datetime]) -> bool:
     if not d1 and not d2:
@@ -247,42 +358,46 @@
 def get_many_series_with_revisions(
     self: "ComApi", requests: Sequence[RevisionHistoryRequest], include_not_modified: bool = False
 ) -> Generator[SeriesWithVintages, None, None]:
     if len(requests) == 0:
         yield from ()
 
     for request in requests:
+        request.if_modified_since = _fix_optional_datetime(request.if_modified_since)
+        request.last_revision = _fix_optional_datetime(request.last_revision)
+        request.last_revision_adjustment = _fix_optional_datetime(request.last_revision_adjustment)
+
         series_with_revisions = self.database.FetchOneSeriesWithRevisions(request.name)
 
         if series_with_revisions.IsError:
             if series_with_revisions.ErrorMessage == "Not found":
-                yield SeriesWithVintages("Not found", SeriesWithVintagesErrorCode.NOT_FOUND, None, [])
+                yield SeriesWithVintages("Not found", StatusCode.NOT_FOUND, None, [])
                 continue
             raise Exception(series_with_revisions.ErrorMessage)
 
         head = series_with_revisions.Head
         metadata = _fill_metadata_from_entity(head)
         last_modified_time = metadata["LastModifiedTimeStamp"]
 
         if (
             request.if_modified_since
             and last_modified_time
             and _less_than_or_equal_with_margin(last_modified_time, request.if_modified_since)
         ):
             if not include_not_modified:
                 continue
-            yield SeriesWithVintages("Not modified", SeriesWithVintagesErrorCode.NOT_MODIFIED, None, [])
+            yield SeriesWithVintages("Not modified", StatusCode.NOT_MODIFIED, None, [])
             continue
 
         can_do_incremental_response = request.last_revision is not None
 
         if can_do_incremental_response and not request.if_modified_since:
             yield SeriesWithVintages(
                 "If lastRevision is specified, then ifModifiedSince must also be included",
-                SeriesWithVintagesErrorCode.OTHER,
+                StatusCode.OTHER,
                 None,
                 [],
             )
             continue
 
         last_revision_adjustment = metadata.get("LastRevisionAdjustmentTimeStamp")
 
@@ -309,18 +424,18 @@
                 ):
                     index = i + 1
                     break
 
             if index != -1:
                 yield SeriesWithVintages(
                     "Incremental update",
-                    SeriesWithVintagesErrorCode.PARTIAL_CONTENT,
+                    StatusCode.PARTIAL_CONTENT,
                     metadata,
                     list(_create_vintage_values(index, vintage_dates, complete_history)),
                 )
                 continue
         yield SeriesWithVintages(
             None,
-            None,
+            StatusCode.OK,
             metadata,
             list(_create_vintage_values(0, vintage_dates, complete_history)),
         )
```

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/com/_com_api_search.py` & `macrobond-data-api-1.0.0/macrobond_data_api/com/_com_api_search.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+from datetime import datetime
 from typing import List, TYPE_CHECKING
 
 from macrobond_data_api.common.types import SearchResult
 from ._fill_metadata import _fill_metadata_from_entity
+from ._fix_datetime import _fix_datetime
 
 
 if TYPE_CHECKING:  # pragma: no cover
     from .com_api import ComApi
 
     from macrobond_data_api.common.types import SearchFilter
 
@@ -27,17 +29,23 @@
         for entity_type in _filter.entity_types:
             query.SetEntityTypeFilter(entity_type)
 
         if _filter.text:
             query.Text = _filter.text
 
         for key in _filter.must_have_values:
-            query.AddAttributeValueFilter(key, _filter.must_have_values[key])
+            val = _filter.must_have_values[key]
+            if isinstance(val, datetime):
+                val = _fix_datetime(val)
+            query.AddAttributeValueFilter(key, val)
 
         for key in _filter.must_not_have_values:
+            val = _filter.must_not_have_values[key]
+            if isinstance(val, datetime):
+                val = _fix_datetime(val)
             query.AddAttributeValueFilter(key, _filter.must_not_have_values[key], False)
 
         for attribute in _filter.must_have_attributes:
             query.AddAttributeFilter(attribute)
 
         for attribute in _filter.must_not_have_attributes:
             query.AddAttributeFilter(attribute, False)
```

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/com/_com_api_series.py` & `macrobond-data-api-1.0.0/macrobond_data_api/com/_com_api_series.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from math import isnan
 from typing import Generator, List, Optional, Tuple, Union, TYPE_CHECKING, Sequence
 
 from datetime import datetime
 
 
-from macrobond_data_api.common.enums import SeriesWeekdays, SeriesFrequency, CalendarMergeMode
+from macrobond_data_api.common.enums import SeriesWeekdays, SeriesFrequency, CalendarMergeMode, StatusCode
 
 from macrobond_data_api.common.types import (
     SeriesEntry,
     GetEntitiesError,
     EntityErrorInfo,
     Series,
     Entity,
     UnifiedSeriesList,
     UnifiedSeries,
 )
-
 from macrobond_data_api.common.types._repr_html_sequence import _ReprHtmlSequence
 
 from ._fill_metadata import _fill_metadata_from_entity
+from ._error_message_to_status_code import _error_message_to_status_code
 
 if TYPE_CHECKING:  # pragma: no cover
     from .com_api import ComApi
 
     from macrobond_data_api.common.types import StartOrEndPoint
 
     from .com_types import Series as ComSeries, Entity as ComEntity
@@ -30,73 +30,82 @@
 
 def _datetime_to_datetime(dates: Sequence[datetime]) -> List[datetime]:
     return [datetime(x.year, x.month, x.day, x.hour, x.minute, x.second, x.microsecond) for x in dates]
 
 
 def _create_entity(com_entity: "ComEntity", name: str) -> Entity:
     if com_entity.IsError:
-        return Entity(name, com_entity.ErrorMessage, None)
-    return Entity(name, None, _fill_metadata_from_entity(com_entity))
+        return Entity(name, com_entity.ErrorMessage, _error_message_to_status_code(com_entity), None)
+    return Entity(name, None, StatusCode.OK, _fill_metadata_from_entity(com_entity))
 
 
 def _create_series(com_series: "ComSeries", name: str) -> Series:
     if com_series.IsError:
-        return Series(name, com_series.ErrorMessage, None, None, None, None)
+        return Series(name, com_series.ErrorMessage, _error_message_to_status_code(com_series), None, None, None, None)
     return Series(
         name,
         None,
+        StatusCode.OK,
         _fill_metadata_from_entity(com_series),
         None,
-        list(com_series.Values),
+        [None if isnan(x) else x for x in com_series.Values],
         _datetime_to_datetime(com_series.DatesAtStartOfPeriod),
     )
 
 
 def get_one_series(self: "ComApi", series_name: str, raise_error: bool = None) -> Series:
-    return self.get_series(series_name, raise_error=raise_error)[0]
+    return self.get_series([series_name], raise_error=raise_error)[0]
 
 
-def get_series(self: "ComApi", *series_names: str, raise_error: Optional[bool] = None) -> Sequence[Series]:
+def get_series(self: "ComApi", series_names: Sequence[str], raise_error: Optional[bool] = None) -> Sequence[Series]:
+    series_names = tuple(series_names)
     com_series = self.database.FetchSeries(series_names)
     series = [_create_series(x, y) for x, y in zip(com_series, series_names)]
     if self.raise_error if raise_error is None else raise_error:
         GetEntitiesError._raise_if([(x, y.error_message) for x, y in zip(series_names, series)])
     return _ReprHtmlSequence(series)
 
 
 def get_one_entity(self: "ComApi", entity_name: str, raise_error: bool = None) -> Entity:
-    return self.get_entities(entity_name, raise_error=raise_error)[0]
+    return self.get_entities([entity_name], raise_error=raise_error)[0]
 
 
-def get_entities(self: "ComApi", *entity_names: str, raise_error: bool = None) -> Sequence[Entity]:
+def get_entities(self: "ComApi", entity_names: Sequence[str], raise_error: bool = None) -> Sequence[Entity]:
+    entity_names = tuple(entity_names)
     com_entitys = self.database.FetchEntities(entity_names)
     entitys = [_create_entity(x, y) for x, y in zip(com_entitys, entity_names)]
     if self.raise_error if raise_error is None else raise_error:
         GetEntitiesError._raise_if([(x, y.error_message) for x, y in zip(entity_names, entitys)])
     return _ReprHtmlSequence(entitys)
 
 
-def get_many_series(self: "ComApi", *series: Tuple[str, datetime]) -> Generator[Optional[Series], None, None]:
+def get_many_series(
+    self: "ComApi", series: Sequence[Union[str, Tuple[str, Optional[datetime]]]], include_not_modified: bool = False
+) -> Generator[Series, None, None]:
     if len(series) == 0:
         yield from ()
 
-    names = {x[0] for x in series}
+    series_as_tuple: List[Tuple[str, Optional[datetime]]] = [(x, None) if isinstance(x, str) else x for x in series]
+
+    names = {x[0] for x in series_as_tuple}
 
-    if len(names) != len(series):
+    if len(names) != len(series_as_tuple):
         raise ValueError("duplicate of series")
 
-    for serie, serie_info in zip(self.get_series(*[x[0] for x in series], raise_error=False), series):
+    for serie, serie_info in zip(self.get_series([x[0] for x in series_as_tuple], raise_error=False), series_as_tuple):
         if serie.is_error:
             yield serie
             continue
 
-        last_modified_time = serie.metadata["LastModifiedTimeStamp"]
-        if last_modified_time <= serie_info[1]:
-            yield Series(serie_info[0], "Not modified", None, None, None, None)
-            continue
+        if serie_info[1]:
+            last_modified_time = serie.metadata["LastModifiedTimeStamp"]
+            if last_modified_time <= serie_info[1]:
+                if include_not_modified:
+                    yield Series(serie_info[0], "Not modified", StatusCode.NOT_MODIFIED, None, None, None, None)
+                continue
 
         yield serie
 
 
 def get_unified_series(
     self: "ComApi",
     *series_entries: Union[SeriesEntry, str],
@@ -152,15 +161,15 @@
         if com_one_series.IsError:
             return UnifiedSeries(name, com_one_series.ErrorMessage, {}, [])
 
         return UnifiedSeries(
             name,
             "",
             _fill_metadata_from_entity(com_one_series),
-            [None if x is not None and isnan(x) else x for x in com_one_series.Values],
+            [None if isnan(x) else x for x in com_one_series.Values],
         )
 
     ret = UnifiedSeriesList([to_obj(request.AddedSeries[x].Name, y) for x, y in enumerate(com_series)], dates)
 
     if self.raise_error if raise_error is None else raise_error:
         errors = [EntityErrorInfo(x, y) for x, y in ret.get_errors().items()]
         if errors:
```

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/com/_fill_metadata.py` & `macrobond-data-api-1.0.0/macrobond_data_api/com/_fill_metadata.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,26 @@
     from .com_types import Metadata as ComMetadata
     from macrobond_data_api.common.types.metadata import Metadata
     from macrobond_data_api.common.types.values_metadata import ValuesMetadata
 
 
 def _get_val(name: str, values: Sequence[Any]) -> Any:
     if isinstance(values[0], TimeType):
-        if name == "LastModifiedTimeStamp":
+        if name in ("OriginalStartDate", "OriginalEndDate"):
+            datetime_ = values[0]
+            return datetime(
+                datetime_.year,
+                datetime_.month,
+                datetime_.day,
+                datetime_.hour,
+                datetime_.minute,
+                datetime_.second,
+                datetime_.microsecond,
+            )
+        if name in ("LastModifiedTimeStamp"):
             datetime_ = values[0]
             return datetime(
                 datetime_.year,
                 datetime_.month,
                 datetime_.day,
                 datetime_.hour,
                 datetime_.minute,
@@ -43,19 +54,24 @@
         values = [
             datetime(x.year, x.month, x.day, x.hour, x.minute, x.second, x.microsecond, timezone.utc) for x in values
         ]
         return values[0] if len(values) == 1 else values
     return values[0] if len(values) == 1 else list(values)
 
 
-def _fill_metadata_from_metadata(com_metadata: "ComMetadata") -> Dict:
-    return {x: _get_val(x, com_metadata.GetValues(x)) for x, _ in com_metadata.ListNames()}
+def _fill_metadata_from_metadata(com_metadata: "ComMetadata", add_empty_revision_time_stamp: bool = False) -> Dict:
+    metadata = {x: _get_val(x, com_metadata.GetValues(x)) for x, _ in com_metadata.ListNames()}
+    if add_empty_revision_time_stamp and "RevisionTimeStamp" not in metadata:
+        metadata["RevisionTimeStamp"] = None
+    return metadata
 
 
 def _fill_metadata_from_entity(com_entity: "ComEntity") -> "Metadata":
     ret = _fill_metadata_from_metadata(com_entity.Metadata)
     ret.setdefault("FullDescription", com_entity.Title)
     return ret
 
 
-def _fill_values_metadata_from_series(com_series: "ComSeries") -> "ValuesMetadata":
-    return [_fill_metadata_from_metadata(x) for x in com_series.ValuesMetadata]
+def _fill_values_metadata_from_series(
+    com_series: "ComSeries", add_empty_revision_time_stamp: bool = False
+) -> "ValuesMetadata":
+    return [_fill_metadata_from_metadata(x, add_empty_revision_time_stamp) for x in com_series.ValuesMetadata]
```

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/com/com_api.py` & `macrobond-data-api-1.0.0/macrobond_data_api/com/com_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Optional
 
 from macrobond_data_api.common import Api
 
 from ._com_api_metadata import (
     metadata_get_attribute_information,
     metadata_get_value_information,
     metadata_list_values,
 )
 
 from ._com_api_revision import (
     get_all_vintage_series,
+    get_one_nth_release,
     get_nth_release,
     get_observation_history,
     get_revision_info,
+    get_one_vintage_series,
     get_vintage_series,
     get_many_series_with_revisions,
 )
 
 from ._com_api_search import entity_search_multi_filter
 
 from ._com_api_series import (
@@ -35,36 +37,42 @@
 
 __pdoc__ = {
     "ComApi.__init__": False,
 }
 
 
 class ComApi(Api):
+    _connection: Optional["Connection"]
+
     def __init__(self, connection: "Connection") -> None:
         super().__init__()
-        self.__connection = connection
+        self._connection = connection
 
     @property
     def connection(self) -> "Connection":
-        return self.__connection
+        if self._connection is None:
+            raise ValueError("ComApi is not open")
+        return self._connection
 
     @property
     def database(self) -> "Database":
-        return self.__connection.Database
+        return self.connection.Database
 
     # metadata
 
     metadata_list_values = metadata_list_values
     metadata_get_attribute_information = metadata_get_attribute_information
     metadata_get_value_information = metadata_get_value_information
 
     # revision
 
     get_revision_info = get_revision_info
+    get_one_vintage_series = get_one_vintage_series
     get_vintage_series = get_vintage_series
+    get_one_nth_release = get_one_nth_release
     get_nth_release = get_nth_release
     get_all_vintage_series = get_all_vintage_series
     get_observation_history = get_observation_history
     get_many_series_with_revisions = get_many_series_with_revisions
 
     # Search
```

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/com/com_client.py` & `macrobond-data-api-1.0.0/macrobond_data_api/com/com_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,14 +24,45 @@
 try:
     # winreg is not available on linux so mypy will fail on build server as it is runiong on linux
     from winreg import OpenKey, QueryValueEx, HKEY_CLASSES_ROOT, HKEY_CURRENT_USER  # type: ignore
 except ImportError:
     ...
 
 
+def _test_regedit_assembly() -> Optional[str]:
+    sub_key = "CLSID\\{F22A9A5C-E6F2-4FA8-8D1B-E928AB5DDF9B}\\InprocServer32"
+    try:
+        with OpenKey(HKEY_CLASSES_ROOT, sub_key) as regkey:
+            QueryValueEx(regkey, "Assembly")
+    except OSError:
+        return (
+            "The Macrobond application is probably not installed.\n"
+            + '(Could not find the registry key "HKEY_CLASSES_ROOT\\'
+            + sub_key
+            + '\\Assembly")\n'
+        )
+    return None
+
+
+def _test_regedit_username() -> Optional[str]:
+    sub_key = "Software\\Macrobond Financial\\Communication\\Connector"
+    try:
+        with OpenKey(HKEY_CURRENT_USER, sub_key) as regkey:
+            QueryValueEx(regkey, "UserName")
+    except OSError:
+        return (
+            "The Macrobond application does not seem to be logged in. Please start the application and verify that "
+            + "it works properly.\n"
+            + '(Could not find the registry key "HKEY_CURRENT_USER\\'
+            + sub_key
+            + '\\UserName")\n'
+        )
+    return None
+
+
 class ComClientVersionException(Exception):
     pass
 
 
 class ComClient(Client["ComApi"]):
     """
     ComClient to get data via the Macrobond desktop API
@@ -47,93 +78,79 @@
     with ComClient() as api:
         # use the api here
     ```
     """
 
     def __init__(self) -> None:
         super().__init__()
+        self.has_closed = False
         self.__api: Optional["ComApi"] = None
 
     @property
     def is_open(self) -> bool:
         return bool(self.__api)
 
     def open(self) -> "ComApi":
+        error_hints: List[str] = []
+        try:
+            return self.open_and_hint(error_hints)
+        except Exception:
+            if len(error_hints) != 0:
+                print("\n\nERROR in ComClient.open()", file=sys.stderr)
+
+            for hint in error_hints:
+                print("\n" + hint, file=sys.stderr)
+
+            if len(error_hints) != 0:
+                print("", file=sys.stderr)
+
+            raise
+
+    def open_and_hint(self, hints: List[str]) -> "ComApi":
+        if self.has_closed:
+            raise ValueError("ComClient cannot be reopend")
+
         if _win32com_import_error:
             raise _win32com_import_error
 
         if _pywintypes_import_error:
             raise _pywintypes_import_error
 
         if self.__api is None:
             try:
                 connection: "Connection" = cast("Connection", _client.Dispatch("Macrobond.Connection"))
             except com_error:
-                hints: List[str] = []
-
-                sub_key = "CLSID\\{F22A9A5C-E6F2-4FA8-8D1B-E928AB5DDF9B}\\InprocServer32"
-                try:
-                    with OpenKey(HKEY_CLASSES_ROOT, sub_key) as regkey:
-                        QueryValueEx(regkey, "Assembly")
-                except OSError:
-                    hints.append(
-                        (
-                            'Could not find the registration key "HKEY_CLASSES_ROOT\\'
-                            + sub_key
-                            + '\\Assembly",\nThis indicates that Macrobond is not installed.'
-                        )
-                    )
-
-                sub_key = "Software\\Macrobond Financial\\Communication\\Connector"
-                try:
-                    with OpenKey(HKEY_CURRENT_USER, sub_key) as regkey:
-                        QueryValueEx(regkey, "UserName")
-                except OSError:
-                    hints.append(
-                        (
-                            'Could not find the registration key "HKEY_CURRENT_USER\\'
-                            + sub_key
-                            + '\\UserName",\nThis indicates that Macrobond is not logged in.'
-                        )
-                    )
-
-                if len(hints) != 0:
-                    print("\n\nERROR in ComClient.open()", file=sys.stderr)
-
-                for hint in hints:
-                    print("\n" + hint, file=sys.stderr)
-
-                if len(hints) != 0:
-                    print("", file=sys.stderr)
-
+                new_hint = _test_regedit_assembly()
+                if new_hint:
+                    hints.append(new_hint)
+
+                new_hint = _test_regedit_username()
+                if new_hint:
+                    hints.append(new_hint)
                 raise
 
             ComClient._test_version(connection.Version)
 
             self.__api = ComApi(connection)
         return self.__api
 
     @staticmethod
     def _test_version(version: Tuple[int, int, int]) -> None:
         if version == (0, 0, 0):
             return
 
-        major, minor, _ = version
-
-        if major > 1:
+        if version >= (1, 25, 0):
             return
 
-        if major == 0:
-            raise ComClientVersionException("Unsupported version " + (".".join([str(x) for x in version])))
-
-        if minor < 25:
-            raise ComClientVersionException("Unsupported version " + (".".join([str(x) for x in version])))
+        raise ComClientVersionException("Unsupported version " + (".".join([str(x) for x in version])))
 
     def close(self) -> None:
         """
         free all resources used by the Macrobond API.
         Opening and closing sessions can be slow,
         so it is usually not a good idea to open and close them for each request
         """
+        self.has_closed = True
         if self.__api:
             self.__api.connection.Close()
+            self.__api._connection = None
             self.__api = None
```

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/com/com_types/connection.py` & `macrobond-data-api-1.0.0/macrobond_data_api/com/com_types/connection.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/com/com_types/database.py` & `macrobond-data-api-1.0.0/macrobond_data_api/com/com_types/database.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/com/com_types/entity.py` & `macrobond-data-api-1.0.0/macrobond_data_api/com/com_types/entity.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/com/com_types/metadata.py` & `macrobond-data-api-1.0.0/macrobond_data_api/com/com_types/metadata.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/com/com_types/metadata_information.py` & `macrobond-data-api-1.0.0/macrobond_data_api/com/com_types/metadata_information.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/com/com_types/search_query.py` & `macrobond-data-api-1.0.0/macrobond_data_api/com/com_types/search_query.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/com/com_types/series.py` & `macrobond-data-api-1.0.0/macrobond_data_api/com/com_types/series.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # pylint: disable = invalid-name , missing-module-docstring
 # mypy: disable_error_code = empty-body
 
-from typing import List, Tuple, Optional
+from typing import List, Tuple
 from datetime import datetime
 
 from .entity import Entity
 from .metadata import Metadata
 
 
 class Series(Entity):
     """Interface for a Macrobond time series."""
 
     @property
-    def Values(self) -> Tuple[Optional[float], ...]:
+    def Values(self) -> Tuple[float, ...]:
         """The values of the series."""
 
     @property
     def DatesAtStartOfPeriod(self) -> Tuple[datetime, ...]:
         """The dates of of the observations at the start of each period."""
 
     @property
```

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/com/com_types/series_expression.py` & `macrobond-data-api-1.0.0/macrobond_data_api/com/com_types/series_expression.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/com/com_types/series_request.py` & `macrobond-data-api-1.0.0/macrobond_data_api/com/com_types/series_request.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/com/com_types/series_with_revisions.py` & `macrobond-data-api-1.0.0/macrobond_data_api/com/com_types/series_with_revisions.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/common/api.py` & `macrobond-data-api-1.0.0/macrobond_data_api/common/api.py`

 * *Files 7% similar despite different names*

```diff
@@ -53,15 +53,17 @@
         `macrobond_data_api.common.api.Api.get_series`  
         `macrobond_data_api.common.api.Api.get_one_entity`  
         `macrobond_data_api.common.api.Api.get_entities`  
         `macrobond_data_api.common.api.Api.get_unified_series`  
 
     Series revision methods:  
         `macrobond_data_api.common.api.Api.get_revision_info`  
+        `macrobond_data_api.common.api.Api.get_one_vintage_series`  
         `macrobond_data_api.common.api.Api.get_vintage_series`  
+        `macrobond_data_api.common.api.Api.get_one_nth_release`  
         `macrobond_data_api.common.api.Api.get_nth_release`  
         `macrobond_data_api.common.api.Api.get_all_vintage_series`  
         `macrobond_data_api.common.api.Api.get_observation_history`  
 
     Search methods:  
         `macrobond_data_api.common.api.Api.entity_search`  
         `macrobond_data_api.common.api.Api.entity_search_multi_filter`  
@@ -77,14 +79,15 @@
         API calls. The default value is "True".
         """
 
     # metadata
 
     @abstractmethod
     def metadata_list_values(self, name: str) -> MetadataValueInformation:
+        # fmt: off
         """
         List all metadata attribute values of an attribute that uses a value list.
 
         Parameters
         ----------
         name : str
             The name of the metadata attribute
@@ -104,18 +107,18 @@
             # as dict
             print(api.metadata_list_values('RateType').to_dict())
 
             # as data_frame
             print(metadata_list_values("RateType").to_pd_data_frame())
         ```
         """
+        # fmt: on
 
     @abstractmethod
     def metadata_get_attribute_information(self, *names: str) -> Sequence[MetadataAttributeInformation]:
-        # pylint: disable=line-too-long
         # fmt: off
         """
         Get information about metadata attributes.
 
         Parameters
         ----------
         *names : str
@@ -141,15 +144,14 @@
             print(api.metadata_get_attribute_information("Region")[0].to_pd_data_frame())
         ```
         """
         # fmt: on
 
     @abstractmethod
     def metadata_get_value_information(self, *name_val: Tuple[str, str]) -> Sequence[MetadataValueInformationItem]:
-        # pylint: disable=line-too-long
         # fmt: off
         """
         Get information about metadata values.
 
         Parameters
         ----------
         *name_val : Tuple[str, str]
@@ -177,14 +179,15 @@
         """
         # fmt: on
 
     # revision
 
     @abstractmethod
     def get_revision_info(self, *series_names: str, raise_error: bool = None) -> Sequence[RevisionInfo]:
+        # fmt: off
         """
         Get information about if revision history is available for a series
         and a list of revision timestamps.
 
         Parameters
         ----------
         *series_names : str
@@ -195,99 +198,171 @@
             If None, it will use the global value `macrobond_data_api.common.api.Api.raise_error`
 
         Returns
         -------
         `Sequence[macrobond_data_api.common.types.revision_info.RevisionInfo]`
         The result is in the sane order as in the request.
         """
+        # fmt: on
+
+    @abstractmethod
+    def get_one_vintage_series(
+        self, time: datetime, series_name: str, include_times_of_change: bool = False, raise_error: bool = None
+    ) -> VintageSeries:
+        # fmt: off
+        """
+        Get one vintage series.
+
+        Parameters
+        ----------
+        time : datetime
+            The time of the vintage to return.
+        series_name : str
+            The name of the series.
+        include_times_of_change : bool
+            Include information of the time each values was last changed.
+        raise_error : bool
+            If True, accessing the resulting series raises a GetEntitiesError.
+            If False you should inspect the is_error property of the result instead.
+            If None, it will use the global value `macrobond_data_api.common.api.Api.raise_error`
+
+        Returns
+        -------
+        `macrobond_data_api.common.types.vintage_series.VintageSeries`
+        """
+        # fmt: on
 
     @abstractmethod
     def get_vintage_series(
-        self, time: datetime, *series_names: str, raise_error: bool = None
+        self,
+        time: datetime,
+        series_names: Sequence[str],
+        include_times_of_change: bool = False,
+        raise_error: bool = None,
     ) -> Sequence[VintageSeries]:
+        # fmt: off
         """
-        Fetch vintage series.
+        Get one or more vintage series.
 
         Parameters
         ----------
         time : datetime
             The time of the vintage to return.
         series_names : str
-            One or more names of series.
+            The names of the series.
+        include_times_of_change : bool
+            Include information of the time each values was last changed.
         raise_error : bool
             If True, accessing the resulting series raises a GetEntitiesError.
             If False you should inspect the is_error property of the result instead.
             If None, it will use the global value `macrobond_data_api.common.api.Api.raise_error`
 
         Returns
         -------
         `Sequence[macrobond_data_api.common.types.vintage_series.VintageSeries]`
         The result is in the same order as in the request.
         """
+        # fmt: on
+
+    @abstractmethod
+    def get_one_nth_release(
+        self, nth: int, series_name: str, include_times_of_change: bool = False, raise_error: bool = None
+    ) -> Series:
+        # fmt: off
+        """
+        Get a series where each value is the nth change of the value.
+
+        Parameters
+        ----------
+        time : nth
+            The nth change of each value.
+        series_name : str
+            The name of the series.
+        include_times_of_change : bool
+            Include information of the time each values was last changed.
+        raise_error : bool
+            If True, accessing the resulting series raises a GetEntitiesError.
+            If False you should inspect the is_error property of the result instead.
+            If None, it will use the global value `macrobond_data_api.common.api.Api.raise_error`
+
+        Returns
+        -------
+        `macrobond_data_api.common.types.series.Series`
+        """
+        # fmt: on
 
     @abstractmethod
     def get_nth_release(
-        self, nth: int, *series_names: str, include_times_of_change: bool = False, raise_error: bool = None
+        self, nth: int, series_names: Sequence[str], include_times_of_change: bool = False, raise_error: bool = None
     ) -> Sequence[Series]:
+        # fmt: off
         """
-        Fetcha series where each value is the nth change of the value.
+        Get one or more series where each value is the nth change of the value.
 
         Parameters
         ----------
         time : nth
             The nth change of each value.
         series_names : str
-            One or more names of series.
+            The names of the series.
+        include_times_of_change : bool
+            Include information of the time each values was last changed.
         raise_error : bool
             If True, accessing the resulting series raises a GetEntitiesError.
             If False you should inspect the is_error property of the result instead.
             If None, it will use the global value `macrobond_data_api.common.api.Api.raise_error`
 
         Returns
         -------
         `Sequence[macrobond_data_api.common.types.series.Series]`
         The result is in the same order as in the request.
         """
+        # fmt: on
 
     @abstractmethod
     def get_all_vintage_series(self, series_name: str) -> GetAllVintageSeriesResult:
+        # fmt: off
         """
         Get all vintages of a series.
 
         Parameters
         ----------
         series_name : str
             The name of the series.
 
         Returns
         -------
         `macrobond_data_api.common.types.get_all_vintage_series_result.GetAllVintageSeriesResult`
         """
+        # fmt: on
 
     @abstractmethod
     def get_observation_history(self, series_name: str, *times: datetime) -> Sequence[SeriesObservationHistory]:
+        # fmt: off
         """
         Get the revision of an observation.
 
         Parameters
         ----------
         series_name : str
             The name of the series.
         times : datetime
             One or more timestamps.
 
         Returns
         -------
         `Sequence[macrobond_data_api.common.types.series_observation_history.SeriesObservationHistory]`
         """
+        # fmt: on
 
     @abstractmethod
     def get_many_series_with_revisions(
         self, requests: Sequence[RevisionHistoryRequest], include_not_modified: bool = False
     ) -> Generator[SeriesWithVintages, None, None]:
+        # fmt: off
         """
         Download all revisions for one or more series.
         Specify a callback to receive the response series by series.
         This method is primarily intended for syncronizing a local database with updates.
 
         You are expected to retain the LastModifiedTimeStamp, LastRevisionTimeStamp and LastRevisionAdjustmentTimeStamp
         for each series and use them in the next request. The attributes LastRevisionTimeStamp and
@@ -303,28 +378,30 @@
         include_not_modified: `bool`
             Set this value to True in order to include NotNodified series.
 
         Returns
         -------
         `Generator[macrobond_data_api.common.types.series_with_vintages.SeriesWithVintages]`
         """
+        # fmt: on
 
     # Search
 
     def entity_search(
         self,
         text: str = None,
         entity_types: Union[Sequence[str], str] = None,
         must_have_values: Dict[str, object] = None,
         must_not_have_values: Dict[str, object] = None,
         must_have_attributes: Union[Sequence[str], str] = None,
         must_not_have_attributes: Union[Sequence[str], str] = None,
         include_discontinued: bool = False,
         no_metadata: bool = False,
     ) -> SearchResult:
+        # fmt: off
         """
         Search for time series and other entitites.
 
         Parameters
         ----------
         text: str
             Optional set of keywords separated by space.
@@ -344,14 +421,15 @@
         include_discontinued: bool
             Set this value to True in order to include discontinued entities in the search.
 
         Returns
         -------
         `macrobond_data_api.common.types.search_result.SearchResult`
         """
+        # fmt: on
         return self.entity_search_multi_filter(
             SearchFilter(
                 text=text,
                 entity_types=entity_types,
                 must_have_values=must_have_values,
                 must_not_have_values=must_not_have_values,
                 must_have_attributes=must_have_attributes,
@@ -361,14 +439,15 @@
             no_metadata=no_metadata,
         )
 
     @abstractmethod
     def entity_search_multi_filter(
         self, *filters: SearchFilter, include_discontinued: bool = False, no_metadata: bool = False
     ) -> SearchResult:
+        # fmt: off
         """
         Search for time series and other entitites.
         You can pass more than one search filter. In this case the filters have to use different
         entity types and searches will be nested so that the result of the previous filter will be
         used as a condition in the subsequent filter linked by the entity type.
 
         Parameters
@@ -380,19 +459,21 @@
         no_metadata : bool
             Set this value to True in order only return the entity names and no metadata, which is faster.
 
         Returns
         -------
         `macrobond_data_api.common.types.search_result.SearchResult`
         """
+        # fmt: on
 
     # Series
 
     @abstractmethod
     def get_one_series(self, series_name: str, raise_error: bool = None) -> Series:
+        # fmt: off
         """
         Download one series.
 
         .. important:: It is much more efficient to download more than one series at a time.
            See `Api.get_series`.
 
         Parameters
@@ -404,41 +485,45 @@
             If False you should inspect the is_error property of the result instead.
             If None, it will use the global value `macrobond_data_api.common.api.Api.raise_error`
 
         Returns
         -------
         `macrobond_data_api.common.types.series.Series`
         """
+        # fmt: on
 
     @abstractmethod
-    def get_series(self, *series_names: str, raise_error: bool = None) -> Sequence[Series]:
+    def get_series(self, series_names: Sequence[str], raise_error: bool = None) -> Sequence[Series]:
+        # fmt: off
         """
         Download one or more series.
 
         .. Important:: It is much more efficient to download more than one series at a time.
            However, downloading too many at a time is less efficient and can exhaust memory.
            A good habit is to download series in batches of around 200.
 
         Parameters
         ----------
-        *series_names : str
-            One or more names of series.
+        series_names : Sequence[str]
+            The names of the series.
         raise_error : bool
             If True, accessing the resulting series raises a GetEntitiesError.
             If False you should inspect the is_error property of the result instead.
             If None, it will use the global value `macrobond_data_api.common.api.Api.raise_error`
 
         Returns
         -------
         `Sequence[macrobond_data_api.common.types.series.Series]`
         The result is in the same order as in the request.
         """
+        # fmt: on
 
     @abstractmethod
     def get_one_entity(self, entity_name: str, raise_error: bool = None) -> Entity:
+        # fmt: off
         """
         Download one entity.
 
         .. important:: It is much more efficient to download more than one entity at a time.
            See `Api.get_entities`.
 
         Parameters
@@ -450,65 +535,75 @@
             If False you should inspect the is_error property of the result instead.
             If None, it will use the global value `macrobond_data_api.common.api.Api.raise_error`
 
         Returns
         -------
         `macrobond_data_api.common.types.entity.Entity`
         """
+        # fmt: on
 
     @abstractmethod
-    def get_entities(self, *entity_names: str, raise_error: bool = None) -> Sequence[Entity]:
+    def get_entities(self, entity_names: Sequence[str], raise_error: bool = None) -> Sequence[Entity]:
+        # fmt: off
         """
         Download one or more entities.
 
         .. Important:: It is much more efficient to download more than one entity at a time.
            However, downloading too many at a time is less efficient and can exhaust memory.
            A good habit is to download entities in batches of around 200.
 
         Parameters
         ----------
-        *entity_names : str
-            One or more names of entities.
+        entity_names : Sequence[str]
+            The names of the entities.
         raise_error : bool
             If True, accessing the resulting entities raises a GetEntitiesError.
             If False you should inspect the is_error property of the result instead.
             If None, it will use the global value `macrobond_data_api.common.api.Api.raise_error`
 
         Returns
         -------
         `Sequence[macrobond_data_api.common.types.entity.Entity]`
         The result is in the same order as in the request.
         """
+        # fmt: on
 
     @abstractmethod
-    def get_many_series(self, *series: Tuple[str, datetime]) -> Generator[Optional[Series], None, None]:
+    def get_many_series(
+        self, series: Sequence[Union[str, Tuple[str, Optional[datetime]]]], include_not_modified: bool = False
+    ) -> Generator[Series, None, None]:
+        # fmt: off
         """
 
         Parameters
         ----------
-        *series: `Tuple[str, datetime.datetime]`
-            A sequence of series requests.
+        series: `Sequence[Union[str, Tuple[str, Optional[datetime]]]]`
+            A sequence of series names or a sequence of name plus a timestamp for the last modification.
+        include_not_modified: `bool`
+            Set this value to True in order to include NotNodified series.
 
         Returns
         -------
         `Generator[Optional[macrobond_data_api.common.types.series.Series]]`
         """
+        # fmt: on
 
     @abstractmethod
     def get_unified_series(
         self,
         *series_entries: Union[SeriesEntry, str],
         frequency: SeriesFrequency = SeriesFrequency.HIGHEST,
         weekdays: SeriesWeekdays = SeriesWeekdays.MONDAY_TO_FRIDAY,
         calendar_merge_mode: CalendarMergeMode = CalendarMergeMode.AVAILABLE_IN_ANY,
         currency: str = "",
         start_point: StartOrEndPoint = None,
         end_point: StartOrEndPoint = None,
         raise_error: bool = None
     ) -> UnifiedSeriesList:
+        # fmt: off
         """
         Get one or more series and convert them to a common frequency and calendar.
 
         Parameters
         ----------
         *series_entries : Union[macrobond_data_api.common.types.series_entry.SeriesEntry, str]
             One or more names of series or
@@ -533,7 +628,8 @@
             If None, it will use the global value `macrobond_data_api.common.api.Api.raise_error`
 
         Returns
         -------
         `macrobond_data_api.common.types.unified_series.UnifiedSeries`
         The result is in the same order as in the request.
         """
+        # fmt: on
```

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/common/client.py` & `macrobond-data-api-1.0.0/macrobond_data_api/common/client.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/common/enums/series_frequency.py` & `macrobond-data-api-1.0.0/macrobond_data_api/common/enums/series_frequency.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/common/enums/series_partial_periods_method.py` & `macrobond-data-api-1.0.0/macrobond_data_api/common/enums/series_partial_periods_method.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/common/enums/series_to_higher_frequency_method.py` & `macrobond-data-api-1.0.0/macrobond_data_api/common/enums/series_to_higher_frequency_method.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/common/enums/series_to_lower_frequency_method.py` & `macrobond-data-api-1.0.0/macrobond_data_api/common/enums/series_to_lower_frequency_method.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/common/enums/series_weekdays.py` & `macrobond-data-api-1.0.0/macrobond_data_api/common/enums/series_weekdays.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/common/types/__init__.py` & `macrobond-data-api-1.0.0/macrobond_data_api/common/types/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,10 +31,14 @@
 
 from .revision_info import RevisionInfo, RevisionInfoDict
 
 from .get_all_vintage_series_result import GetAllVintageSeriesResult
 
 from .metadata import Metadata
 
-from .series_with_vintages import SeriesWithVintages, VintageValues, SeriesWithVintagesErrorCode
+from .series_with_vintages import SeriesWithVintages, VintageValues
 
 from .revision_history_request import RevisionHistoryRequest
+
+from .values_metadata import ValuesMetadata
+
+from .format_exception import FormatException
```

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/common/types/_repr_html_sequence.py` & `macrobond-data-api-1.0.0/macrobond_data_api/common/types/_repr_html_sequence.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,14 @@
-from typing import Generic, Sequence, TypeVar, overload
+from typing import Generic, Sequence, TypeVar, overload, cast, List
 
+from macrobond_data_api.common.types import (
+    MetadataAttributeInformation,
+    MetadataValueInformationItem,
+    RevisionInfo,
+)
 
 _TypeVar = TypeVar("_TypeVar")
 
 
 class _ReprHtmlSequence(Sequence[_TypeVar], Generic[_TypeVar]):
     __slots__ = ("items",)
 
@@ -23,9 +28,24 @@
 
     def __getitem__(self, key):  # type: ignore
         return _ReprHtmlSequence(self.items[key]) if isinstance(key, slice) else self.items[key]
 
     def __len__(self) -> int:
         return len(self.items)
 
-    def _repr_html_(self) -> str:
-        return "".join(x._repr_html_() for x in self)  # type: ignore
+    def _ipython_display_(self) -> None:
+        # pylint: disable=import-outside-toplevel
+        from IPython.display import display  # type: ignore
+        import pandas  # type: ignore
+
+        # pylint: enable=import-outside-toplevel
+
+        if len(self.items) > 1 and len(set((type(x) for x in self.items))) == 1:
+            t = type(self.items[0])
+            if t in (MetadataAttributeInformation, MetadataValueInformationItem, RevisionInfo):
+                display(
+                    pandas.concat([x.to_pd_data_frame() for x in cast(List[MetadataAttributeInformation], self.items)])
+                )
+                return
+
+        for x in self.items:
+            display(x)
```

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/common/types/entity.py` & `macrobond-data-api-1.0.0/macrobond_data_api/common/types/entity.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from dataclasses import dataclass
+from datetime import datetime
 from typing import Any, Dict, List, Optional, TYPE_CHECKING
 from typing_extensions import Literal
 
+from macrobond_data_api.common.enums import StatusCode
+
 if TYPE_CHECKING:  # pragma: no cover
-    from pandas import Series, DataFrame  # type: ignore
+    from pandas import Series  # type: ignore
     from .metadata import Metadata
 
 
 EntityColumnsLiterals = Literal["ErrorMessage", "Name", "PrimName", "FullDescription", "EntityType"]
 
 EntityColumns = List[EntityColumnsLiterals]
 
@@ -18,18 +21,19 @@
 
 @dataclass(init=False)
 class Entity:
     """
     Represents a Macrobond entity.
     """
 
-    __slots__ = ("name", "error_message", "metadata")
+    __slots__ = ("name", "error_message", "status_code", "metadata")
 
     name: str
     error_message: str
+    status_code: StatusCode
     metadata: "Metadata"
 
     @property
     def is_error(self) -> bool:
         """
         True if there was an error downloading this entity. `Entity.error_message` will
         contain any error message.
@@ -63,31 +67,40 @@
         """
         entity_type = self.metadata["EntityType"]
         if isinstance(entity_type, list):
             entity_type = entity_type[0]
         return entity_type
 
     @property
+    def last_modified(self) -> datetime:
+        """The time of the last modification of the entity."""
+        return self.metadata["LastModifiedTimeStamp"]
+
+    @property
     def is_discontinued(self) -> bool:
         """Returns True if the entity is discontinued and no longer updated."""
         entity_state = self.metadata.get("EntityState")
         return entity_state is not None and entity_state != 0
 
     def __init__(
         self,
         name: str,
         error_message: Optional[str],
+        status_code: StatusCode,
         metadata: Optional["Metadata"],
     ) -> None:
         self.name = name
         """The name of the entity."""
 
         self.error_message = error_message if error_message else ""
         """Contains an error message if `Entity.is_error` is True."""
 
+        self.status_code = status_code
+        """The status code of the Entity"""
+
         self.metadata = metadata if metadata else {}
         """The metadata of the entity."""
 
     def _add_metadata(self, destination: Dict[str, Any]) -> None:
         for key in self.metadata.keys():
             destination["metadata." + key] = self.metadata[key]
 
@@ -104,14 +117,14 @@
         return ret
 
     def metadata_to_pd_series(self, name: str = None) -> "Series":
         """Returns a Pandas series containing all the metadata."""
         import pandas  # pylint: disable=import-outside-toplevel
 
         name = name if name else self.name
-        return pandas.Series(self.metadata.values(), self.metadata.keys(), name=name)
+        return pandas.Series(self.metadata.values(), self.metadata.keys(), name=name, dtype="object")
 
     def _repr_html_(self) -> str:
         return self.metadata_to_pd_series().to_frame()._repr_html_()
 
     def __bool__(self) -> bool:
         return not self.is_error
```

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/common/types/get_all_vintage_series_result.py` & `macrobond-data-api-1.0.0/macrobond_data_api/common/types/get_all_vintage_series_result.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from dataclasses import dataclass
 
-from typing import TYPE_CHECKING, Any, Dict, Sequence, overload
+from typing import TYPE_CHECKING, Any, Dict, Sequence, overload, List
 
 from macrobond_data_api.common.types.vintage_series import VintageSeries
 
 if TYPE_CHECKING:  # pragma: no cover
     from pandas import DataFrame  # type: ignore
 
 __pdoc__ = {
@@ -19,40 +19,46 @@
     """
 
     __slots__ = ("series", "series_name")
 
     series: Sequence[VintageSeries]
     series_name: str
 
-    def __init__(self, series: Sequence[VintageSeries], series_name: str) -> None:
+    def __init__(self, series: List[VintageSeries], series_name: str) -> None:
         super().__init__()
         self.series = series
         """A sequence of time series corresponding to the vintages."""
         self.series_name = series_name
         """The name of the requested series."""
 
     def to_pd_data_frame(self) -> "DataFrame":
         """
         Return the result as a Pandas DataFrame.
         """
         import pandas  # pylint: disable=import-outside-toplevel
 
-        data = [x.values_to_pd_series() for x in self]
-        data_frame = pandas.concat(data, axis=1, keys=[s.revision_time_stamp for s in self])
-        data_frame = data_frame.sort_index()
-        return data_frame
+        return pandas.DataFrame(
+            {
+                **{"date": self.series[len(self.series) - 1].dates},
+                **{
+                    x.revision_time_stamp: pandas.Series(data=x.values, name="Value", dtype="float64")  # type: ignore
+                    for x in self.series
+                },
+            }
+        )
 
     def to_dict(self) -> Dict[str, Any]:
         """
         Return the result as a dictionary.
         """
         return {"series_name": self.series_name, "series": [x.to_dict() for x in self]}
 
     def _repr_html_(self) -> str:
-        return self.to_pd_data_frame()._repr_html_()
+        html = self.to_pd_data_frame()._repr_html_()
+        return f"<p>{self.series_name}</p>{html}"
 
     @overload
     def __getitem__(self, i: int) -> VintageSeries:
         ...
 
     @overload
     def __getitem__(self, s: slice) -> Sequence[VintageSeries]:
```

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/common/types/get_entity_error.py` & `macrobond-data-api-1.0.0/macrobond_data_api/common/types/get_entity_error.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/common/types/metadata_attribute_information.py` & `macrobond-data-api-1.0.0/macrobond_data_api/common/types/metadata_attribute_information.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,11 +147,11 @@
             "is_database_entity": self.is_database_entity,
         }
 
     def to_pd_data_frame(self) -> "DataFrame":
         """The information represented as a Pandas DataFrame"""
         import pandas  # pylint: disable=import-outside-toplevel
 
-        return pandas.DataFrame([self.to_dict()])
+        return pandas.DataFrame([self.to_dict()], dtype="object")
 
     def _repr_html_(self) -> str:
         return self.to_pd_data_frame()._repr_html_()
```

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/common/types/metadata_value_information.py` & `macrobond-data-api-1.0.0/macrobond_data_api/common/types/metadata_value_information.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,42 +75,40 @@
 
     def _repr_html_(self) -> str:
         return self.to_pd_data_frame()._repr_html_()
 
 
 @dataclass(init=False)
 class MetadataValueInformation(Sequence[MetadataValueInformationItem]):
-    # fmt: off
     """
-    The result of a call to `macrobond_data_api.common.api.Api.metadata_get_value_information`.  
+    The result of a call to `macrobond_data_api.common.api.Api.metadata_get_value_information`.
     Contains information about the requested metadata attribute values.
     """
-    # fmt: on
 
     __slots__ = ("attribute_name", "entities")
 
     entities: Sequence[MetadataValueInformationItem]
     attribute_name: str
 
     def __init__(
         self,
-        entities: Sequence[MetadataValueInformationItem],
+        entities: List[MetadataValueInformationItem],
         attribute_name: str,
     ) -> None:
         super().__init__()
         self.entities = entities
         """entities"""
         self.attribute_name = attribute_name
         """The name of the metadata attribute"""
 
     def to_pd_data_frame(self) -> "DataFrame":
         """The information represented as a Pandas DataFrame"""
         import pandas  # pylint: disable=import-outside-toplevel
 
-        return pandas.DataFrame(self.to_dict())
+        return pandas.DataFrame(self.to_dict(), dtype="object")
 
     def to_dict(self) -> List[TypedDictMetadataValueInformationItem]:
         """The information represented as a dictionary"""
         return [x.to_dict() for x in self]
 
     @overload
     def __getitem__(self, i: int) -> MetadataValueInformationItem:
@@ -125,8 +123,8 @@
 
     def __len__(self) -> int:
         return len(self.entities)
 
     def _repr_html_(self) -> str:
         frame = self.to_pd_data_frame()
         del frame["attribute_name"]
-        return f"<h1>{self.attribute_name}</h1>" + frame._repr_html_()
+        return f"<p>{self.attribute_name}</p>" + frame._repr_html_()
```

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/common/types/revision_history_request.py` & `macrobond-data-api-1.0.0/macrobond_data_api/common/types/revision_history_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# pylint: disable = missing-module-docstring
-
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Optional
 
 
 @dataclass(init=False)
 class RevisionHistoryRequest:
```

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/common/types/revision_info.py` & `macrobond-data-api-1.0.0/macrobond_data_api/common/types/revision_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from dataclasses import dataclass
 from datetime import datetime
-from typing import TYPE_CHECKING, Optional, Sequence
+from typing import TYPE_CHECKING, Optional, Sequence, List
 
 from typing_extensions import TypedDict
 
 if TYPE_CHECKING:  # pragma: no cover
     from pandas import DataFrame  # type: ignore
 
 __pdoc__ = {
@@ -49,15 +49,15 @@
         self,
         name: str,
         error_message: str,
         stores_revisions: bool,
         has_revisions: bool,
         time_stamp_of_first_revision: Optional[datetime],
         time_stamp_of_last_revision: Optional[datetime],
-        vintage_time_stamps: Sequence[datetime],
+        vintage_time_stamps: List[datetime],
     ) -> None:
         self.name = name
         """The name of the series"""
 
         self.error_message = error_message
         """Contains an error message in case of an error."""
 
@@ -90,11 +90,11 @@
             "vintage_time_stamps": self.vintage_time_stamps,
         }
 
     def to_pd_data_frame(self) -> "DataFrame":
         """Returns a Pandas dataframe with the information about the series revisions."""
         import pandas  # pylint: disable=import-outside-toplevel
 
-        return pandas.DataFrame(self.to_dict())
+        return pandas.DataFrame(self.to_dict(), dtype="object")
 
     def _repr_html_(self) -> str:
         return self.to_pd_data_frame()._repr_html_()
```

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/common/types/search_filter.py` & `macrobond-data-api-1.0.0/macrobond_data_api/common/types/search_filter.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/common/types/search_result.py` & `macrobond-data-api-1.0.0/macrobond_data_api/common/types/search_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     """
 
     __slots__ = ("entities", "is_truncated")
 
     entities: Sequence["Metadata"]
     is_truncated: bool
 
-    def __init__(self, entities: Sequence["Metadata"], is_truncated: bool) -> None:
+    def __init__(self, entities: List["Metadata"], is_truncated: bool) -> None:
         super().__init__()
         self.entities = entities
         """
         A sequence of the metadata of the entities found.
         """
         self.is_truncated = is_truncated
         """
```

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/common/types/search_result_long.py` & `macrobond-data-api-1.0.0/macrobond_data_api/common/types/search_result_long.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     """
 
     __slots__ = ("entities", "is_truncated")
 
     entities: Sequence[str]
     is_truncated: bool
 
-    def __init__(self, entities: Sequence[str], is_truncated: bool) -> None:
+    def __init__(self, entities: List[str], is_truncated: bool) -> None:
         super().__init__()
         self.entities = entities
         self.is_truncated = is_truncated
         """
         Indicates whether the search result was too long and truncated.
         """
 
@@ -37,15 +37,15 @@
 
     def to_pd_data_frame(self) -> "DataFrame":
         """
         Return the result as a `DataFrame`.
         """
         import pandas  # pylint: disable=import-outside-toplevel
 
-        return pandas.DataFrame(self.entities)
+        return pandas.DataFrame(self.entities, dtype="string")
 
     def _repr_html_(self) -> str:
         return self.to_pd_data_frame()._repr_html_()
 
     @overload
     def __getitem__(self, i: int) -> str:
         ...
```

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/common/types/series.py` & `macrobond-data-api-1.0.0/macrobond_data_api/common/types/series.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,52 @@
 from dataclasses import dataclass
 from datetime import datetime
 
 from typing import Any, Dict, Optional, List, Sequence, TYPE_CHECKING, cast
 from typing_extensions import Literal
 
-from .entity import Entity, EntityColumnsLiterals
+from macrobond_data_api.common.enums import StatusCode
 
+from .entity import Entity, EntityColumnsLiterals
 
 SeriesColumnsLiterals = Literal[EntityColumnsLiterals, "Values", "Dates"]
 
 SeriesColumns = List[SeriesColumnsLiterals]
 
 if TYPE_CHECKING:  # pragma: no cover
-    from pandas import Series as PdSeries  # type: ignore
+    from pandas import DataFrame  # type: ignore
     from .metadata import Metadata
     from .values_metadata import ValuesMetadata
 
 __pdoc__ = {
     "Series.__init__": False,
 }
 
 
 @dataclass(init=False)
 class Series(Entity):
     """Represents a Macrobond time series."""
 
     __slots__ = ("values_metadata", "values", "dates")
 
+    values_metadata: Optional["ValuesMetadata"]
     values: Sequence[Optional[float]]
     dates: Sequence[datetime]
 
     def __init__(
         self,
         name: str,
         error_message: Optional[str],
+        status_code: StatusCode,
         metadata: Optional["Metadata"],
         values_metadata: Optional["ValuesMetadata"],
         values: Optional[List[Optional[float]]],
         dates: Optional[List[datetime]],
     ) -> None:
-        super().__init__(name, error_message, metadata)
+        super().__init__(name, error_message, status_code, metadata)
 
         self.values_metadata = values_metadata
         """
         The meta data for the values.
         """
 
         self.values = ...  # type: ignore
@@ -61,28 +64,43 @@
             self.values = []
             self.dates = []
         else:
             self.values = values
             self.dates = cast(Sequence[datetime], dates)
 
     def to_dict(self) -> Dict[str, Any]:
+        """
+        The series content as a dictionary of "Name", "Values" and "Dates".
+        """
         if self.is_error:
             return {
                 "Name": self.name,
                 "ErrorMessage": self.error_message,
             }
         ret = {
             "Name": self.name,
             "Values": self.values,
             "Dates": self.dates,
         }
         self._add_metadata(ret)
         return ret
 
-    def values_to_pd_series(self, name: str = None) -> "PdSeries":
+    def values_to_pd_data_frame(self) -> "DataFrame":
+        """
+        A Pandas DataFrame with the with a series called "date" and one called "value"
+        """
         import pandas  # pylint: disable=import-outside-toplevel
 
-        name = name if name else self.name
-        return pandas.Series(self.values, self.dates, name=name)
+        if self.is_error:
+            ...
+        return pandas.DataFrame(
+            {
+                "date": self.dates,
+                "value": self.values,
+            }
+        )
 
     def _repr_html_(self) -> str:
-        return self.metadata_to_pd_series().to_frame()._repr_html_()
+        if self.is_error:
+            return f"<p>{self.name}</p><p>error_message: {self.error_message}</p>"
+        html = self.values_to_pd_data_frame()._repr_html_()
+        return f"<p>{self.name}</p>{html}"
```

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/common/types/series_entry.py` & `macrobond-data-api-1.0.0/macrobond_data_api/common/types/series_entry.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/common/types/series_observation_history.py` & `macrobond-data-api-1.0.0/macrobond_data_api/common/types/series_observation_history.py`

 * *Files 20% similar despite different names*

```diff
@@ -29,16 +29,16 @@
     observation_date: datetime
     values: Sequence[Optional[float]]
     time_stamps: Sequence[Optional[datetime]]
 
     def __init__(
         self,
         observation_date: datetime,
-        values: Sequence[Optional[float]],
-        time_stamps: Sequence[Optional[datetime]],
+        values: List[Optional[float]],
+        time_stamps: List[Optional[datetime]],
     ) -> None:
         self.observation_date = observation_date
         """The date of the observation"""
 
         self.values = values
         """
         The historical values of the observation or an empty tuple if
@@ -50,24 +50,24 @@
         A tuple of timestamps of when the historical values were recorded.
         The first timestamp may be null if the time of the original is unknown.
         """
 
     def to_dict(self) -> Dict[str, Any]:
         return {
             "ObservationDate": self.observation_date,
-            "Values": self.values,
+            "Value": self.values,
             "TimeStamps": self.time_stamps,
         }
 
     def to_pd_data_frame(self) -> "DataFrame":
         import pandas  # pylint: disable=import-outside-toplevel
 
-        return pandas.DataFrame({"values": self.values}, self.time_stamps)
+        return pandas.DataFrame({"values": self.values}, self.time_stamps, dtype="float64")
 
     def to_pd_series(self, name: str = None) -> "Series":
         import pandas  # pylint: disable=import-outside-toplevel
 
         name = name if name else str(self.observation_date)
-        return pandas.Series(self.values, self.time_stamps, name=name)
+        return pandas.Series(self.values, self.time_stamps, name=name, dtype="float64")
 
     def _repr_html_(self) -> str:
         return self.to_pd_data_frame()._repr_html_()
```

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/common/types/series_with_vintages.py` & `macrobond-data-api-1.0.0/macrobond_data_api/common/types/series_with_vintages.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Optional, List
 
-from enum import IntEnum
+from macrobond_data_api.common.enums import StatusCode
 
 from .metadata import Metadata
 
 __pdoc__ = {
     "VintageValues.__init__": False,
     "SeriesWithVintages.__init__": False,
 }
@@ -31,49 +31,26 @@
         self, vintage_time_stamp: Optional[datetime], dates: List[datetime], values: List[Optional[float]]
     ) -> None:
         self.vintage_time_stamp = vintage_time_stamp
         self.dates = dates
         self.values = values
 
 
-class SeriesWithVintagesErrorCode(IntEnum):
-    PARTIAL_CONTENT = 206
-    """The item was not modified and is not included in the response"""
-
-    NOT_MODIFIED = 304
-    """The item was not modified and is not included in the response"""
-
-    FORBIDDEN = 403
-    """Access to the item was denied"""
-
-    NOT_FOUND = 404
-    """The item was not found"""
-
-    OTHER = 500
-    """There was an error and it is described in the error text"""
-
-
 @dataclass(init=False)
 class SeriesWithVintages:
     """A time series with times of change"""
 
-    __slots__ = ("error_text", "error_code", "metadata", "vintages")
+    __slots__ = ("error_text", "status_code", "metadata", "vintages")
 
     error_text: Optional[str]
     """The error text if there was an error or not specified if there was no error"""
 
-    error_code: Optional[SeriesWithVintagesErrorCode]
+    status_code: StatusCode
     """
     Set if there was an error and not specified if there was no error
-
-    206 = PartialContent (The item was not modified and is not included in the response)
-    304 = NotModified (The item was not modified and is not included in the response)
-    403 = Forbidden (Access to the item was denied)
-    404 = NotFound (The item was not found)
-    500 = Other (There was an error and it is described in the error text)
     """
 
     metadata: Optional[Metadata]
     """
     The time when this version of the series was recorded
     """
 
@@ -129,15 +106,15 @@
             if self.metadata and "LastModifiedTimeStamp" in self.metadata
             else None
         )
 
     def __init__(
         self,
         error_text: Optional[str],
-        error_code: Optional[SeriesWithVintagesErrorCode],
+        status_code: StatusCode,
         metadata: Optional[Metadata],
         vintages: List[VintageValues],
     ) -> None:
         self.error_text = error_text
-        self.error_code = error_code
+        self.status_code = status_code
         self.metadata = metadata
         self.vintages = vintages
```

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/common/types/start_or_end_point.py` & `macrobond-data-api-1.0.0/macrobond_data_api/common/types/start_or_end_point.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/common/types/unified_series.py` & `macrobond-data-api-1.0.0/macrobond_data_api/common/types/unified_series.py`

 * *Files 7% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         return self.error_message != ""
 
     def __init__(
         self,
         name: str,
         error_message: str,
         metadata: "Metadata",
-        values: Sequence[Optional[float]],
+        values: List[Optional[float]],
     ) -> None:
         self.name = name
         """The name of the requested series."""
 
         self.error_message = error_message
         """Contains an error message if `UnifiedSerie.is_error` is True."""
 
@@ -104,16 +104,16 @@
         """
         True if any of the series has an error.
         """
         return any(self)
 
     def __init__(
         self,
-        series: Sequence[UnifiedSeries],
-        dates: Sequence[datetime],
+        series: List[UnifiedSeries],
+        dates: List[datetime],
     ) -> None:
         super().__init__()
         self.series = series
         """The list of series"""
         self.dates = dates
         """The dates of the observations"""
 
@@ -125,15 +125,27 @@
 
     def get_errors(self) -> Dict[str, str]:
         return {e.name: e.error_message for e in self if e.is_error}
 
     def to_pd_data_frame(self) -> "DataFrame":
         import pandas  # pylint: disable=import-outside-toplevel
 
-        return pandas.DataFrame({kv.name: kv.values for kv in self}, self.dates)
+        return pandas.DataFrame(
+            {
+                **{"date": self.dates},
+                **{
+                    "Error: " + kv.error_message
+                    if kv.is_error
+                    else kv.name: [None] * len(self.dates)  # type: ignore
+                    if kv.is_error
+                    else kv.values
+                    for kv in self
+                },
+            }
+        )
 
     def _repr_html_(self) -> str:
         return self.to_pd_data_frame()._repr_html_()
 
     @overload
     def __getitem__(self, i: int) -> UnifiedSeries:
         ...
```

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/common/types/vintage_series.py` & `macrobond-data-api-1.0.0/macrobond_data_api/common/types/vintage_series.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from dataclasses import dataclass
 from datetime import datetime
 
 from typing import List, Optional, TYPE_CHECKING
 from typing_extensions import Literal
-from dateutil import parser
 
+from macrobond_data_api.common.enums import StatusCode
 from .series import Series, SeriesColumnsLiterals
 
+from ._parse_iso8601 import _parse_iso8601
+
 if TYPE_CHECKING:  # pragma: no cover
     from .metadata import Metadata
     from .values_metadata import ValuesMetadata
 
 
 VintageSeriesColumns = List[Literal[SeriesColumnsLiterals, "VintageTimeStamp", "TimesOfChange"]]
 
@@ -26,21 +28,22 @@
 
     __slots__ = ("_revision_time_stamp",)
 
     def __init__(
         self,
         name: str,
         error_message: Optional[str],
+        status_code: StatusCode,
         metadata: Optional["Metadata"],
         values_metadata: Optional["ValuesMetadata"],
         values: Optional[List[Optional[float]]],
         dates: Optional[List[datetime]],
         _revision_time_stamp: Optional[datetime],
     ) -> None:
-        super().__init__(name, error_message, metadata, values_metadata, values, dates)
+        super().__init__(name, error_message, status_code, metadata, values_metadata, values, dates)
         self._revision_time_stamp = _revision_time_stamp
 
     @property
     def revision_time_stamp(self) -> Optional[datetime]:
         """The vintage of the series."""
         if self._revision_time_stamp:
             return self._revision_time_stamp
@@ -48,8 +51,8 @@
         if "RevisionTimeStamp" not in self.metadata:
             return None
 
         revision_time_stamp = self.metadata["RevisionTimeStamp"]
         if isinstance(revision_time_stamp, list):
             revision_time_stamp = revision_time_stamp[0]
 
-        return parser.parse(revision_time_stamp) if isinstance(revision_time_stamp, str) else revision_time_stamp
+        return _parse_iso8601(revision_time_stamp) if isinstance(revision_time_stamp, str) else revision_time_stamp
```

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/util/save_credential_to_keyring.py` & `macrobond-data-api-1.0.0/macrobond_data_api/util/save_credential_to_keyring.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/env python3
 import sys
 import json
+import traceback
 from getpass import getpass
 
 import keyring
-from macrobond_data_api.web.web_client import (
-    DEFAULT_SERVICE_NAME,
-    DARWIN_USERNAME,
-)
+from keyring.backends.fail import Keyring as fail_keyring_backend
+from keyring.backends.null import Keyring as null_keyring_backend
+from macrobond_data_api.web.web_client import DEFAULT_SERVICE_NAME, DARWIN_USERNAME, WebClient
 
 
 def _inquiry(question: str, default: str = "yes") -> bool:
     valid = {"yes": True, "y": True, "no": False, "n": False}
     if default is None:
         prompt = " [y/n] "
     elif default == "yes":
@@ -39,14 +39,33 @@
         ):
             return False
         keyring.delete_password(service_name, old_credential.username)
         old_credential = keyring.get_credential(service_name, username)
     return True
 
 
+def _test_keyring_backend() -> bool:
+    try:
+        keyring_backend = keyring.get_keyring()
+    except Exception:  # pylint: disable=broad-exception-caught
+        print(traceback.format_exc())
+        print("Error: failed to get keyring")
+        return False
+
+    if isinstance(keyring_backend, null_keyring_backend):
+        print("Error: keyring_backend is null_keyring_backend")
+        return False
+
+    if isinstance(keyring_backend, fail_keyring_backend):
+        print("Error: keyring_backend is fail_keyring_backend")
+        return False
+
+    return True
+
+
 def save_credential_to_keyring(warn_before_removing: bool = True, ask_for_service_name: bool = False) -> bool:
     # fmt: off
     # pylint: disable=line-too-long
     """
     Create or update a key in the system's keyring interactively via terminal.
 
     By defult the method will ask interactively for:
@@ -87,14 +106,18 @@
     * Freedesktop [Secret Service](http://standards.freedesktop.org/secret-service/) supports many DE including GNOME (requires [secretstorage](https://pypi.python.org/pypi/secretstorage))
     * KDE4 & KDE5 [KWallet](https://en.wikipedia.org/wiki/KWallet) (requires [dbus](https://pypi.python.org/pypi/dbus-python))
     * [Windows Credential Locker](https://docs.microsoft.com/en-us/windows/uwp/security/credential-locker)
 
     """
     # pylint: enable=line-too-long
     # fmt: on
+
+    if not _test_keyring_backend():
+        return False
+
     is_darwin = sys.platform.startswith("darwin")
     keyring_name = keyring.get_keyring().name
 
     print("Saving secret to " + keyring_name + "\n")
 
     service_name = (
         input(
@@ -108,22 +131,39 @@
     if service_name == "":
         service_name = DEFAULT_SERVICE_NAME
 
     if not _remove_duplicates(service_name, DARWIN_USERNAME if is_darwin else "", warn_before_removing):
         return False
 
     username = input("Please enter Macrobond Web Api username: ")
-
     password = getpass("Please enter Macrobond Web Api password: ")
 
+    print("Testing username and password")
+    try:
+        with WebClient(username=username, password=password) as api:
+            api.metadata_get_attribute_information("PrimName")
+    except Exception:  # pylint: disable=broad-exception-caught
+        print(traceback.format_exc())
+        print("Error: failed testing username and password")
+        return False
+
     if is_darwin:
         keyring.set_password(service_name, DARWIN_USERNAME, json.dumps({"username": username, "password": password}))
     else:
         keyring.set_password(service_name, username, password)
 
-    print(f'successfully saved to the keyring with the service name: "{ service_name }" in {keyring_name}')
+    print("Testing keyring")
+    try:
+        with WebClient() as api:
+            api.metadata_get_attribute_information("PrimName")
+    except Exception:  # pylint: disable=broad-exception-caught
+        print(traceback.format_exc())
+        print("Error: failed testing keyring")
+        return False
+
+    print(f'Successfully saved to the keyring with the service name: "{ service_name }" in {keyring_name}')
 
     return True
 
 
 if __name__ == "__main__":
     save_credential_to_keyring()
```

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/web/_metadata.py` & `macrobond-data-api-1.0.0/macrobond_data_api/web/_metadata.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/web/_metadata_directory.py` & `macrobond-data-api-1.0.0/macrobond_data_api/web/_metadata_directory.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from datetime import datetime, timezone
 from typing import TYPE_CHECKING, Any, Dict, Optional
 
 from json import load as json_load
-from dateutil import parser, tz
+
+from macrobond_data_api.common.types._parse_iso8601 import _parse_iso8601
 
 from ..common.enums import MetadataAttributeType
 from .web_types.metadata import MetadataAttributeTypeRestriction
 
 from .session import ProblemDetailsException
 
 if TYPE_CHECKING:  # pragma: no cover
@@ -56,16 +57,16 @@
             if type_info.value_type == MetadataAttributeType.INT:
                 return int(obj)
             if type_info.value_type == MetadataAttributeType.DOUBLE:
                 return float(obj)
             if type_info.value_type == MetadataAttributeType.TIME_STAMP:
                 if type_info.value_restriction == MetadataAttributeTypeRestriction.DATE:
                     return datetime(int(obj[0:4]), int(obj[5:7]), int(obj[8:10]))
-                time = parser.parse(obj)
-                if time.tzinfo == tz.tzutc():
+                time = _parse_iso8601(obj)
+                if time.tzinfo == timezone.utc:
                     time = datetime(
                         time.year,
                         time.month,
                         time.day,
                         time.hour,
                         time.minute,
                         time.second,
```

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/web/_web_api_metadata.py` & `macrobond-data-api-1.0.0/macrobond_data_api/web/_web_api_metadata.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/web/_web_api_revision.py` & `macrobond-data-api-1.0.0/macrobond_data_api/web/_web_api_revision.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,61 +1,48 @@
 from datetime import datetime
 from typing import TYPE_CHECKING, Any, Dict, Generator, List, Optional, Sequence, cast
 
-from dateutil import parser
-
 import ijson  # type: ignore
 
 from macrobond_data_api.common.types import (
     RevisionInfo,
     GetEntitiesError,
     VintageSeries,
     Series,
     SeriesObservationHistory,
     GetAllVintageSeriesResult,
     SeriesWithVintages,
     VintageValues,
-    SeriesWithVintagesErrorCode,
     RevisionHistoryRequest,
+    ValuesMetadata,
 )
+from macrobond_data_api.common.enums import StatusCode
+from macrobond_data_api.common.types._parse_iso8601 import _parse_iso8601
 from macrobond_data_api.common.types._repr_html_sequence import _ReprHtmlSequence
 from ._split_in_to_chunks import split_in_to_chunks
 
 from .session import ProblemDetailsException, Session, _raise_on_error
 
 # from .series_with_vintages import SeriesWithVintages
 
 
 if TYPE_CHECKING:  # pragma: no cover
     from .web_api import WebApi
-
     from .web_types import (
         SeriesWithRevisionsInfoResponse,
         VintageSeriesResponse,
         SeriesWithVintagesResponse,
         RevisionHistoryRequest as WebRevisionHistoryRequest,
         SeriesWithTimesOfChangeResponse,
         VintageValuesResponse,
     )
 
 
 def _optional_str_to_datetime(datetime_str: Optional[str]) -> Optional[datetime]:
-    return parser.parse(datetime_str) if datetime_str else None
-
-
-def _str_to_datetime_ignoretz(datetime_str: str) -> datetime:
-    return parser.parse(datetime_str, ignoretz=True)
-
-
-def _str_to_datetime(datetime_str: str) -> datetime:
-    return parser.parse(datetime_str)
-
-
-def _optional_str_to_datetime_ignoretz(datetime_str: Optional[str]) -> Optional[datetime]:
-    return parser.parse(datetime_str, ignoretz=True) if datetime_str else None
+    return _parse_iso8601(datetime_str) if datetime_str else None
 
 
 def int_to_float_or_none(int_: Optional[int]) -> Optional[float]:
     return float(int_) if int_ else None
 
 
 def get_revision_info(self: "WebApi", *series_names: str, raise_error: Optional[bool] = None) -> Sequence[RevisionInfo]:
@@ -66,15 +53,15 @@
 
         time_stamp_of_first_revision = _optional_str_to_datetime(serie.get("timeStampOfFirstRevision"))
 
         time_stamp_of_last_revision = _optional_str_to_datetime(serie.get("timeStampOfLastRevision"))
 
         stores_revisions = serie["storesRevisions"]
 
-        vintage_time_stamps = [parser.parse(x) for x in serie["vintageTimeStamps"]] if stores_revisions else []
+        vintage_time_stamps = [_parse_iso8601(x) for x in serie["vintageTimeStamps"]] if stores_revisions else []
 
         return RevisionInfo(
             name,
             "",
             stores_revisions,
             serie["hasRevisions"],
             time_stamp_of_first_revision,
@@ -86,71 +73,121 @@
 
     if self.raise_error if raise_error is None else raise_error:
         GetEntitiesError._raise_if([(x, y.get("errorText")) for x, y in zip(series_names, response)])
 
     return _ReprHtmlSequence([to_obj(x, y) for x, y in zip(series_names, response)])
 
 
+def get_one_vintage_series(
+    self: "WebApi",
+    time: datetime,
+    series_name: str,
+    include_times_of_change: bool = False,
+    raise_error: Optional[bool] = None,
+) -> VintageSeries:
+    return self.get_vintage_series(
+        time, [series_name], include_times_of_change=include_times_of_change, raise_error=raise_error
+    )[0]
+
+
 def get_vintage_series(
-    self: "WebApi", time: datetime, *series_names: str, raise_error: Optional[bool] = None
+    self: "WebApi",
+    time: datetime,
+    series_names: Sequence[str],
+    include_times_of_change: bool = False,
+    raise_error: Optional[bool] = None,
 ) -> Sequence[VintageSeries]:
     def to_obj(response: "VintageSeriesResponse", series_name: str) -> VintageSeries:
         error_message = response.get("errorText")
         if error_message:
-            return VintageSeries(series_name, error_message, None, None, None, None, None)
+            return VintageSeries(
+                series_name, error_message, StatusCode(cast(int, response["errorCode"])), None, None, None, None, None
+            )
 
         metadata = self.session._create_metadata(response["metadata"])
 
         revision_time_stamp = cast(str, metadata.get("RevisionTimeStamp"))
 
         if not revision_time_stamp or time != revision_time_stamp:
             raise ValueError("Invalid time")
 
         values = [float(x) if x else None for x in cast(List[Optional[int]], response["values"])]
-        dates = [_str_to_datetime_ignoretz(x) for x in cast(List[str], response["dates"])]
+        dates = [_parse_iso8601(x) for x in cast(List[str], response["dates"])]
+
+        if include_times_of_change:
+            timesOfChange = response.get("timesOfChange")
+            if timesOfChange:
+                values_metadata = [
+                    {"RevisionTimeStamp": _optional_str_to_datetime(x)} for x in cast(List[str], timesOfChange)
+                ]
+            else:
+                values_metadata = [{}] * len(values)
+        else:
+            values_metadata = None
 
         vintage_time_stamp = (
-            _str_to_datetime(cast(str, response["vintageTimeStamp"])) if "vintageTimeStamp" in response else None
+            _parse_iso8601(cast(str, response["vintageTimeStamp"])) if "vintageTimeStamp" in response else None
         )
 
-        return VintageSeries(series_name, None, metadata, None, values, dates, vintage_time_stamp)
+        return VintageSeries(
+            series_name, None, StatusCode.OK, metadata, values_metadata, values, dates, vintage_time_stamp
+        )
 
-    response = self.session.series.fetch_vintage_series(time, *series_names, get_times_of_change=False)
+    response = self.session.series.fetch_vintage_series(
+        time, *series_names, get_times_of_change=include_times_of_change
+    )
 
     series = [to_obj(x, y) for x, y in zip(response, series_names)]
 
     if self.raise_error if raise_error is None else raise_error:
         GetEntitiesError._raise_if([(x, y.error_message) for x, y in zip(series_names, series)])
 
     return _ReprHtmlSequence(series)
 
 
+def get_one_nth_release(
+    self: "WebApi",
+    nth: int,
+    series_name: str,
+    include_times_of_change: bool = False,
+    raise_error: Optional[bool] = None,
+) -> Series:
+    return self.get_nth_release(
+        nth, [series_name], include_times_of_change=include_times_of_change, raise_error=raise_error
+    )[0]
+
+
 def get_nth_release(
     self: "WebApi",
     nth: int,
-    *series_names: str,
+    series_names: Sequence[str],
     include_times_of_change: bool = False,
-    raise_error: Optional[bool] = None
+    raise_error: Optional[bool] = None,
 ) -> Sequence[Series]:
     def to_obj(response: "SeriesWithTimesOfChangeResponse", name: str, session: Session) -> Series:
         error_text = response.get("errorText")
 
         if error_text:
-            return Series(name, error_text, None, None, None, None)
+            return Series(name, error_text, StatusCode(cast(int, response["errorCode"])), None, None, None, None)
 
-        dates = [_str_to_datetime_ignoretz(x) for x in cast(List[str], response["dates"])]
+        dates = [_parse_iso8601(x) for x in cast(List[str], response["dates"])]
         values = [float(x) if x else None for x in cast(List[Optional[int]], response["values"])]
         metadata = session._create_metadata(response["metadata"])
-        values_metadata = (
-            [{"timesOfChange": _optional_str_to_datetime(x)} for x in cast(List[str], response["timesOfChange"])]
-            if include_times_of_change and "timesOfChange" in response
-            else None
-        )
+        if include_times_of_change:
+            timesOfChange = response.get("timesOfChange")
+            if not timesOfChange or (len(values) != 0 and _optional_str_to_datetime(timesOfChange[0]) is None):
+                values_metadata: Optional[ValuesMetadata] = [{}] * len(values)
+            else:
+                values_metadata = [
+                    {"RevisionTimeStamp": _optional_str_to_datetime(x)} for x in cast(List[str], timesOfChange)
+                ]
+        else:
+            values_metadata = None
 
-        return Series(name, "", cast(Dict[str, Any], metadata), values_metadata, values, dates)
+        return Series(name, "", StatusCode.OK, cast(Dict[str, Any], metadata), values_metadata, values, dates)
 
     if len(series_names) == 0:
         raise ValueError("No series names")
 
     response = self.session.series.fetch_nth_release_series(
         nth, *series_names, get_times_of_change=include_times_of_change
     )
@@ -163,25 +200,27 @@
     return _ReprHtmlSequence(series)
 
 
 def get_all_vintage_series(self: "WebApi", series_name: str) -> GetAllVintageSeriesResult:
     def to_obj(response: "VintageSeriesResponse", series_name: str) -> VintageSeries:
         error_message = response.get("errorText")
         if error_message:
-            return VintageSeries(series_name, error_message, None, None, None, None, None)
+            return VintageSeries(
+                series_name, error_message, StatusCode(cast(int, response["errorCode"])), None, None, None, None, None
+            )
 
         metadata = self.session._create_metadata(response["metadata"])
         values = [float(x) if x else None for x in cast(List[Optional[int]], response["values"])]
-        dates = [_str_to_datetime_ignoretz(x) for x in cast(List[str], response["dates"])]
+        dates = [_parse_iso8601(x) for x in cast(List[str], response["dates"])]
 
         vintage_time_stamp = (
-            _str_to_datetime(cast(str, response["vintageTimeStamp"])) if "vintageTimeStamp" in response else None
+            _parse_iso8601(cast(str, response["vintageTimeStamp"])) if "vintageTimeStamp" in response else None
         )
 
-        return VintageSeries(series_name, None, metadata, None, values, dates, vintage_time_stamp)
+        return VintageSeries(series_name, None, StatusCode.OK, metadata, None, values, dates, vintage_time_stamp)
 
     try:
         response = self.session.series.get_fetch_all_vintage_series(series_name)
     except ProblemDetailsException as ex:
         if ex.status == 404:
             raise ValueError("Series not found: " + series_name) from ex
         raise ex
@@ -196,26 +235,26 @@
         if ex.status == 404:
             raise Exception(ex.detail) from ex
         raise ex
 
     return _ReprHtmlSequence(
         [
             SeriesObservationHistory(
-                parser.parse(x["observationDate"]),
+                _parse_iso8601(x["observationDate"]),
                 [float(y) if y else None for y in x["values"]],
-                [_optional_str_to_datetime_ignoretz(y) for y in x["timeStamps"]],
+                [_optional_str_to_datetime(y) for y in x["timeStamps"]],
             )
             for x in response
         ]
     )
 
 
 def _create_vintage_values(vintage_values: "VintageValuesResponse") -> VintageValues:
     _vintage_time_stamp = vintage_values.get("vintageTimeStamp")
-    vintage_time_stamp = parser.parse(_vintage_time_stamp) if _vintage_time_stamp else None
+    vintage_time_stamp = _parse_iso8601(_vintage_time_stamp) if _vintage_time_stamp else None
 
     dates = [datetime(int(x[0:4]), int(x[5:7]), int(x[8:10])) for x in vintage_values["dates"]]
 
     values = [float(x) if x else None for x in vintage_values["values"]]
 
     return VintageValues(vintage_time_stamp, dates, values)
 
@@ -243,20 +282,20 @@
         with self.session.series.post_fetch_all_vintage_series(
             _create_web_revision_h_request(requests_chunkd), stream=True
         ) as response:
             _raise_on_error(response)
             ijson_items = ijson.items(response.raw, "item")
             item: "SeriesWithVintagesResponse"
             for item in ijson_items:
-                _error_code = item.get("errorCode")
-                error_code = SeriesWithVintagesErrorCode(_error_code) if _error_code else None
+                error_code = item.get("errorCode")
+                status_code = StatusCode(error_code) if error_code else StatusCode.OK
 
-                if not include_not_modified and error_code == SeriesWithVintagesErrorCode.NOT_MODIFIED:
+                if not include_not_modified and status_code == StatusCode.NOT_MODIFIED:
                     continue
 
                 _metadata = item.get("metadata")
                 metadata = self.session._create_metadata(_metadata) if _metadata else None
 
                 _vintages = item.get("vintages")
                 vintages = [_create_vintage_values(x) for x in _vintages] if _vintages else []
 
-                yield SeriesWithVintages(item.get("errorText"), error_code, metadata, vintages)
+                yield SeriesWithVintages(item.get("errorText"), status_code, metadata, vintages)
```

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/web/_web_api_search.py` & `macrobond-data-api-1.0.0/macrobond_data_api/web/_web_api_search.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/web/_web_api_series.py` & `macrobond-data-api-1.0.0/macrobond_data_api/web/_web_api_series.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 from datetime import datetime
 from typing import TYPE_CHECKING, Any, Dict, Generator, List, Optional, Sequence, Tuple, Union, cast
 
-from dateutil import parser
-
 from macrobond_data_api.common.types._repr_html_sequence import _ReprHtmlSequence
+from macrobond_data_api.common.types._parse_iso8601 import _parse_iso8601
 
-from macrobond_data_api.common.types import SeriesEntry
-
-from macrobond_data_api.common.enums import SeriesWeekdays, SeriesFrequency, CalendarMergeMode
-
+from macrobond_data_api.common.enums import SeriesWeekdays, SeriesFrequency, CalendarMergeMode, StatusCode
 from macrobond_data_api.common.types import (
     GetEntitiesError,
     EntityErrorInfo,
     Series,
     Entity,
     UnifiedSeries,
     UnifiedSeriesList,
+    SeriesEntry,
 )
 
 from .session import Session
 from ._split_in_to_chunks import split_in_to_chunks
 
 if TYPE_CHECKING:  # pragma: no cover
     from .web_api import WebApi
@@ -32,91 +29,88 @@
 
 
 __pdoc__ = {
     "WebApi.__init__": False,
 }
 
 
-def _optional_str_to_datetime(datetime_str: Optional[str]) -> Optional[datetime]:
-    return parser.parse(datetime_str) if datetime_str else None
-
-
-def _optional_str_to_datetime_no_utc(datetime_str: str) -> Optional[datetime]:
-    return parser.parse(datetime_str, ignoretz=True) if datetime_str else None
-
-
-def _str_to_datetime_no_utc(datetime_str: str) -> datetime:
-    return parser.parse(datetime_str, ignoretz=True)
-
-
 def _create_entity(response: "EntityResponse", name: str, session: Session) -> Entity:
     error_text = response.get("errorText")
 
     if error_text:
-        return Entity(name, error_text, None)
+        return Entity(name, error_text, StatusCode(cast(int, response["errorCode"])), None)
 
     metadata = session._create_metadata(response["metadata"])
 
-    return Entity(name, None, cast(Dict[str, Any], metadata))
+    return Entity(name, None, StatusCode.OK, cast(Dict[str, Any], metadata))
 
 
 def _create_series(response: "SeriesResponse", name: str, session: Session) -> Series:
     error_text = response.get("errorText")
 
     if error_text:
-        return Series(name, error_text, None, None, None, None)
+        return Series(name, error_text, StatusCode(cast(int, response["errorCode"])), None, None, None, None)
 
-    dates = [_str_to_datetime_no_utc(x) for x in cast(List[str], response["dates"])]
+    dates = [_parse_iso8601(x) for x in cast(List[str], response["dates"])]
 
     values = [float(x) if x else None for x in cast(List[Optional[float]], response["values"])]
 
     metadata = session._create_metadata(response["metadata"])
 
     # values = cast(Tuple[Optional[float]], response["values"])
-    return Series(name, "", metadata, None, values, dates)
+    return Series(name, "", StatusCode.OK, metadata, None, values, dates)
 
 
 def get_one_series(self: "WebApi", series_name: str, raise_error: Optional[bool] = None) -> Series:
-    return self.get_series(series_name, raise_error=raise_error)[0]
+    return self.get_series([series_name], raise_error=raise_error)[0]
 
 
-def get_series(self: "WebApi", *series_names: str, raise_error: Optional[bool] = None) -> Sequence[Series]:
+def get_series(self: "WebApi", series_names: Sequence[str], raise_error: Optional[bool] = None) -> Sequence[Series]:
     response = self.session.series.get_fetch_series(*series_names)
     series = [_create_series(x, y, self.session) for x, y in zip(response, series_names)]
     if self.raise_error if raise_error is None else raise_error:
         GetEntitiesError._raise_if([(x, y.error_message) for x, y in zip(series_names, series)])
     return _ReprHtmlSequence(series)
 
 
 def get_one_entity(self: "WebApi", entity_name: str, raise_error: Optional[bool] = None) -> Entity:
-    return self.get_entities(entity_name, raise_error=raise_error)[0]
+    return self.get_entities([entity_name], raise_error=raise_error)[0]
 
 
-def get_entities(self: "WebApi", *entity_names: str, raise_error: Optional[bool] = None) -> Sequence[Entity]:
+def get_entities(self: "WebApi", entity_names: Sequence[str], raise_error: Optional[bool] = None) -> Sequence[Entity]:
     response = self.session.series.fetch_entities(*entity_names)
     entitys = [_create_entity(x, y, self.session) for x, y in zip(response, entity_names)]
     if self.raise_error if raise_error is None else raise_error:
         GetEntitiesError._raise_if([(x, y.error_message) for x, y in zip(entity_names, entitys)])
     return _ReprHtmlSequence(entitys)
 
 
-def get_many_series(self: "WebApi", *series: Tuple[str, datetime]) -> Generator[Optional[Series], None, None]:
+def get_many_series(
+    self: "WebApi", series: Sequence[Union[str, Tuple[str, Optional[datetime]]]], include_not_modified: bool = False
+) -> Generator[Series, None, None]:
     if len(series) == 0:
         yield from ()
 
-    names = {x[0] for x in series}
+    series_as_tuple: List[Tuple[str, Optional[datetime]]] = [(x, None) if isinstance(x, str) else x for x in series]
+
+    names = {x[0] for x in series_as_tuple}
 
-    if len(names) != len(series):
+    if len(names) != len(series_as_tuple):
         raise ValueError("duplicate of series")
 
-    for chunk in split_in_to_chunks(series, 200):
-        requests: List["EntityRequest"] = [{"name": x[0], "ifModifiedSince": x[1].isoformat()} for x in chunk]
+    for chunk in split_in_to_chunks(series_as_tuple, 200):
+        requests: List["EntityRequest"] = [
+            {"name": x[0], "ifModifiedSince": x[1].isoformat() if x[1] else None} for x in chunk
+        ]
         response_list = self.session.series.post_fetch_series(*requests)
         for response, request in zip(response_list, requests):
-            yield _create_series(response, request["name"], self.session)
+            ret = _create_series(response, request["name"], self.session)
+            if ret.status_code == StatusCode.NOT_MODIFIED and not include_not_modified:
+                continue
+            yield ret
 
 
 def get_unified_series(
     self: "WebApi",
     *series_entries: Union[SeriesEntry, str],
     frequency: SeriesFrequency = SeriesFrequency.HIGHEST,
     weekdays: SeriesWeekdays = SeriesWeekdays.FULL_WEEK,
@@ -157,15 +151,15 @@
         request["endPoint"] = end_point.time
         request["endDateMode"] = end_point.mode
 
     response = self.session.series.fetch_unified_series(request)
 
     str_dates = response.get("dates")
 
-    dates = [_str_to_datetime_no_utc(x) for x in str_dates] if str_dates else []
+    dates = [_parse_iso8601(x) for x in str_dates] if str_dates else []
 
     series: List[UnifiedSeries] = []
     for i, one_series in enumerate(response["series"]):
         name = request["seriesEntries"][i]["name"]
         error_text = one_series.get("errorText")
 
         if error_text:
```

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/web/_web_only_api.py` & `macrobond-data-api-1.0.0/macrobond_data_api/web/_web_only_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 from datetime import datetime
 from typing import TYPE_CHECKING, Any, List, Optional, Callable, Tuple
 
 import ijson  # type: ignore
-from dateutil import parser
-
 
 from macrobond_data_api.common.types import SearchResultLong
-
+from macrobond_data_api.common.types._parse_iso8601 import _parse_iso8601
 
 from .web_types.subscription_list_state import SubscriptionListState
 from .web_types.subscription_list_item import SubscriptionListItem
-from .web_types.subscription_list import SubscriptionList
+from .web_types.subscription_list import SubscriptionList as OldSubscriptionList
 from .web_types.subscription_body import SubscriptionBody
 
-
 from .session import _raise_on_error
+from .subscription_list import SubscriptionList
 
 if TYPE_CHECKING:  # pragma: no cover
     from macrobond_data_api.common.types import SearchFilter
 
     from .web_api import WebApi
     from .web_types.search import SearchRequest, SearchFilter as WebSearchFilter
 
@@ -34,19 +32,19 @@
     time_stamp_for_if_modified_since: Optional[datetime] = None
     download_full_list_on_or_after: Optional[datetime] = None
     state: Optional[SubscriptionListState] = None
     for prefix, event, value in ijson_parse:
         if prefix == "timeStampForIfModifiedSince":
             if event != "string":
                 raise Exception("bad format: timeStampForIfModifiedSince is not a string")
-            time_stamp_for_if_modified_since = parser.parse(value)
+            time_stamp_for_if_modified_since = _parse_iso8601(value)
         elif prefix == "downloadFullListOnOrAfter":
             if event != "string":
                 raise Exception("bad format: downloadFullListOnOrAfter is not a string")
-            download_full_list_on_or_after = parser.parse(value)
+            download_full_list_on_or_after = _parse_iso8601(value)
         elif prefix == "state":
             if event != "number":
                 raise Exception("bad format: state is not a number")
             state = SubscriptionListState(value)
         elif event == "start_array":
             if prefix != "entities":
                 raise Exception("bad format: event start_array do not have a prefix of entities")
@@ -82,22 +80,22 @@
         elif prefix == "entities.item.name":
             if event != "string":
                 raise Exception("bad format: entities.item.name is not a string")
             name = value
         elif prefix == "entities.item.modified":
             if event != "string":
                 raise Exception("bad format: entities.item.modified is not a string")
-            modified = parser.parse(value)
+            modified = _parse_iso8601(value)
 
     if len(items) != 0:
         return items_callback(body, items) is not False
     return True
 
 
-def get_subscription_list(self: "WebApi", if_modified_since: datetime = None) -> SubscriptionList:
+def get_subscription_list(self: "WebApi", if_modified_since: datetime = None) -> OldSubscriptionList:
     # pylint: disable=line-too-long
     """
     Get the items in the subscription list.
     .. Important:: For large lists you might want to use `macrobond_data_api.web.web_api.WebApi.get_subscription_list_iterative`.
 
     Typically you want to pass the date of time_stamp_for_if_modified_since from response of the previous call
     to get incremental updates.
@@ -109,31 +107,34 @@
         If not specified, all items will be returned.
 
     Returns
     -------
     `macrobond_data_api.web.web_types.subscription_list.SubscriptionList`
     """
     # pylint: enable=line-too-long
-    return SubscriptionList(self.session.series.get_subscription_list(if_modified_since))
+    return OldSubscriptionList(self.session.series.get_subscription_list(if_modified_since))
+
+
+# TODO: @mb-jp ree add cooment to get_subscription_list_iterative , when SubscriptionListPoller is done
+# .. Note:: For for continous polling you might
+# want to use `macrobond_data_api.web.subscription_list_poller.SubscriptionListPoller`.
 
 
 def get_subscription_list_iterative(
     self: "WebApi",
     body_callback: Callable[[SubscriptionBody], Optional[bool]],
     items_callback: Callable[[SubscriptionBody, List[SubscriptionListItem]], Optional[bool]],
     if_modified_since: datetime = None,
     buffer_size: int = 200,
 ) -> Optional[SubscriptionBody]:
     # pylint: disable=line-too-long
     """
     Process the subscription list in batches.
     This is more efficient since the complete list does not have to be in memory.
 
-    .. Note:: For for continous polling you might want to use `macrobond_data_api.web.subscription_list_poller.SubscriptionListPoller`.
-
     Typically you want to pass the date of time_stamp_for_if_modified_since from response of the previous call
     to get incremental updates.
 
     Parameters
     ----------
     body_callback : `Callable[[macrobond_data_api.web.web_types.subscription_body.SubscriptionBody], Optional[bool]]`
         The callback for the body. This call comes first. Return True to continue processing.
@@ -154,15 +155,15 @@
     # pylint: enable=line-too-long
     params = {}
     body: Optional[SubscriptionBody] = None
 
     if if_modified_since:
         params["ifModifiedSince"] = if_modified_since.isoformat()
 
-    with self.__session.get("v1/series/getsubscriptionlist", params=params, stream=True) as response:
+    with self._session.get("v1/series/getsubscriptionlist", params=params, stream=True) as response:
         _raise_on_error(response)
         ijson_parse = ijson.parse(response.raw)
 
         (
             time_stamp_for_if_modified_since,
             download_full_list_on_or_after,
             state,
@@ -227,7 +228,17 @@
         "noMetadata": True,
         "allowLongResult": True,
     }
 
     response = self.session.search.post_entities(request)
 
     return SearchResultLong([x["Name"] for x in response["results"]], response.get("isTruncated") is True)
+
+
+def subscription_list(self: "WebApi", last_modified: datetime) -> SubscriptionList:
+    """
+    Retrieves the subscription list with the specified date since last update.
+    """
+    if not self._session._is_open:
+        raise ValueError("WebApi is not open")
+
+    return SubscriptionList(self._session, last_modified)
```

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/web/session.py` & `macrobond-data-api-1.0.0/macrobond_data_api/web/session.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         non_error_status = [200]
 
     if response.status_code in non_error_status:
         return
 
     content_type = response.headers.get("Content-Type")
 
-    if not content_type or ["application/json; charset=utf-8", "application/json"].count(content_type) != 0:
+    if content_type in ["application/json; charset=utf-8", "application/json"]:
         raise ProblemDetailsException.create_from_response(response)
 
     macrobond_status = response.headers.get("X-Macrobond-Status")
     if macrobond_status:
         raise ProblemDetailsException(response, detail=macrobond_status)
 
     raise HttpException(response)
@@ -130,27 +130,38 @@
         self.__metadata = MetadataMethods(self)
         self.__search = SearchMethods(self)
         self.__series = SeriesMethods(self)
         self.__series_tree = SeriesTreeMethods(self)
 
         self._metadata_type_directory = _MetadataTypeDirectory(self)
 
+        self._is_open = True
+
     def _is_https_url(self, url: str) -> bool:
         return url.lower().startswith("https://")
 
     def close(self) -> None:
+        if not self._is_open:
+            return
         self.auth2_session.close()
         self._metadata_type_directory.close()
+        self._is_open = False
 
     def fetch_token(self) -> None:
+        if not self._is_open:
+            raise ValueError("Session is not open")
+
         if self.token_endpoint is None:
             self.__token_endpoint = self.discovery(self.authorization_url)
         self.auth2_session.fetch_token(self.token_endpoint, proxies=self.__proxies)
 
     def get(self, url: str, params: dict = None, stream: bool = False) -> "Response":
+        if not self._is_open:
+            raise ValueError("Session is not open")
+
         def http() -> "Response":
             return self.auth2_session.get(
                 url=self.api_url + url,
                 params=params,
                 stream=stream,
                 proxies=self.__proxies,
                 headers={"Accept": "application/json"},
@@ -166,14 +177,17 @@
         stream: bool = False,
     ) -> "Response":
         response = self.get(url, params, stream=stream)
         _raise_on_error(response, non_error_status)
         return response
 
     def post(self, url: str, params: dict = None, json: object = None, stream: bool = False) -> "Response":
+        if not self._is_open:
+            raise ValueError("Session is not open")
+
         def http() -> "Response":
             return self.auth2_session.post(
                 url=self.api_url + url,
                 params=params,
                 json=json,
                 stream=stream,
                 proxies=self.__proxies,
@@ -191,14 +205,17 @@
         stream: bool = False,
     ) -> "Response":
         response = self.post(url, params, json, stream=stream)
         _raise_on_error(response, non_error_status)
         return response
 
     def discovery(self, url: str) -> str:
+        if not self._is_open:
+            raise ValueError("Session is not open")
+
         response = self.auth2_session.request(
             "get", url + ".well-known/openid-configuration", True, proxies=self.__proxies
         )
         if response.status_code != 200:
             raise Exception("discovery Exception, status code is not 200")
 
         try:
```

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/web/subscription_list_poller.py` & `macrobond-data-api-1.0.0/macrobond_data_api/web/_subscription_list_poller.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,44 +11,72 @@
     from .web_types import SubscriptionBody, SubscriptionListItem
 
 
 class _AbortException(Exception):
     ...
 
 
-class SubscriptionListPoller(ABC):
+class _SubscriptionListPoller(ABC):
+    """
+    This is work in progress and might change soon.
+    Run a loop polling for changed series in the subscription list.
+    Derive from this class and override `on_full_listing_start`, `on_full_listing_items`, `on_full_listing_stop`,
+    `on_incremental_start`, `on_incremental_items` and `on_incremental_stop`.
+
+    Parameters
+    ----------
+    api : WebApi
+        The API instance to use.
+    download_full_list_on_or_after : datetime
+        The saved value of `download_full_list_on_or_after` from the previous run. `None` on first run.
+    time_stamp_for_if_modified_since: datetime
+        The saved value of `time_stamp_for_if_modified_since` from the previous run. `None`on first run.
+    """
+
     def __init__(
         self,
         api: WebApi,
         download_full_list_on_or_after: Optional[datetime] = None,
         time_stamp_for_if_modified_since: Optional[datetime] = None,
         _sleep: Callable[[int], None] = time.sleep,
     ) -> None:
+        self.up_to_date_delay = 15 * 60
+        """ The time to wait, in seconds, between polls. """
+        self.incomplete_delay = 15
+        """ The time to wait, in seconds, between continuing partial updates. """
+        self.on_error_delay = 30
+        """ The time to wait, in seconds, before retrying after an error. """
         self._api = api
         self._sleep = _sleep
         self._abort = False
-        self.up_to_date_delay = 15 * 60
-        self.incomplete_delay = 60
-        self.on_error_delay = 10
         self._download_full_list_on_or_after = download_full_list_on_or_after
         self._time_stamp_for_if_modified_since = time_stamp_for_if_modified_since
 
     @property
     def api(self) -> WebApi:
         return self._api
 
     @property
     def download_full_list_on_or_after(self) -> Optional[datetime]:
+        """
+        The time of the scheduled next full listing. Save this value after processing and pass in constructor for
+        the next run.
+        """
         return self._download_full_list_on_or_after
 
     @property
     def time_stamp_for_if_modified_since(self) -> Optional[datetime]:
+        """
+        This value is used internall to keep track of the the time of the last detected modification.
+        Save this value after processing and pass in constructor for the next run.
+        """
         return self._time_stamp_for_if_modified_since
 
     def start(self) -> None:
+        """Start processing. It will continue to run until `abort` is called."""
         self._abort = False
         while not self._abort:
             if not self._time_stamp_for_if_modified_since or (
                 self._download_full_list_on_or_after
                 and datetime.now(timezone.utc) > self._download_full_list_on_or_after
             ):
                 sub = self._run_full_listing()
@@ -73,15 +101,15 @@
             self.on_full_listing_start(body)
 
         try:
             for attempt in range(1, max_attempts):
                 try:
                     sub = self._api.get_subscription_list_iterative(
                         _body_callback,
-                        self.on_full_listing_itmes,
+                        self.on_full_listing_items,
                         None,
                     )
                     if not sub:
                         raise ValueError("subscription is None")
 
                     self.on_full_listing_stop(False, None)
                     return sub
@@ -89,121 +117,138 @@
                     if self._abort:
                         raise _AbortException() from ex
                     if attempt > max_attempts:
                         raise ex
                     self._sleep(self.on_error_delay)
         except _AbortException as ex:
             if is_stated:
-                self.on_listing_stop(True, cast(Exception, ex.__cause__))
+                self.on_full_listing_stop(True, cast(Exception, ex.__cause__))
         except Exception as ex:  # pylint: disable=broad-except
             if is_stated:
-                self.on_listing_stop(False, ex)
+                self.on_full_listing_stop(False, ex)
         return None
 
     def _run_listing(self, if_modified_since: datetime, max_attempts: int = 3) -> Optional["SubscriptionBody"]:
         is_stated = False
 
         def _body_callback(body: "SubscriptionBody") -> None:
             is_stated = True  # pylint: disable=unused-variable
-            self.on_listing_start(body)
+            self.on_incremental_start(body)
 
         try:
             for attempt in range(1, max_attempts):
                 try:
                     sub = self._api.get_subscription_list_iterative(
                         _body_callback,
-                        self.on_listing_items,
+                        self.on_incremental_items,
                         if_modified_since,
                     )
                     break
                 except Exception as ex:  # pylint: disable=broad-except
                     if self._abort:
                         raise _AbortException() from ex
                     if attempt > max_attempts:
                         raise
                     self._sleep(self.on_error_delay)
 
             if not sub:
                 raise ValueError("subscription is None")
 
             if sub.state == SubscriptionListState.UP_TO_DATE:
-                self.on_listing_stop(False, None)
+                self.on_incremental_stop(False, None)
                 return sub
 
             self._sleep(self.incomplete_delay)
 
             return self._run_listing_incomplete(sub.time_stamp_for_if_modified_since, is_stated, max_attempts)
         except _AbortException as ex:
             if is_stated:
-                self.on_listing_stop(True, cast(Exception, ex.__cause__))
+                self.on_incremental_stop(True, cast(Exception, ex.__cause__))
         except Exception as ex:  # pylint: disable=broad-except
             if is_stated:
-                self.on_listing_stop(False, ex)
+                self.on_incremental_stop(False, ex)
         return None
 
     def _run_listing_incomplete(
         self, if_modified_since: datetime, is_stated: bool, max_attempts: int = 3
     ) -> Optional["SubscriptionBody"]:
         try:
             while True:
                 for attempt in range(1, max_attempts):
                     try:
                         sub = self._api.get_subscription_list_iterative(
                             lambda _: None,
-                            self.on_listing_items,
+                            self.on_incremental_items,
                             if_modified_since,
                         )
 
                         if not sub:
                             raise ValueError("subscription is None")
 
                         if sub.state == SubscriptionListState.UP_TO_DATE:
-                            self.on_listing_stop(False, None)
+                            self.on_incremental_stop(False, None)
                             return sub
 
                         self._sleep(self.incomplete_delay)
 
                         if_modified_since = sub.time_stamp_for_if_modified_since
                     except Exception as ex2:  # pylint: disable=broad-except
                         if self._abort:
                             raise _AbortException() from ex2
                         if attempt > max_attempts:
                             raise
                         self._sleep(self.on_error_delay)
         except _AbortException as ex:
             if is_stated:
-                self.on_listing_stop(True, cast(Exception, ex.__cause__))
+                self.on_incremental_stop(True, cast(Exception, ex.__cause__))
         except Exception as ex:  # pylint: disable=broad-except
             if is_stated:
-                self.on_listing_stop(False, ex)
+                self.on_incremental_stop(False, ex)
         return None
 
     # full_listing
 
     @abstractmethod
     def on_full_listing_start(self, subscription: "SubscriptionBody") -> None:
-        ...
+        """This override is called when a full listing starts."""
 
     @abstractmethod
-    def on_full_listing_itmes(self, subscription: "SubscriptionBody", items: List["SubscriptionListItem"]) -> None:
-        ...
+    def on_full_listing_items(self, subscription: "SubscriptionBody", items: List["SubscriptionListItem"]) -> None:
+        """This override is called repeatedly with one or more items until all items are listed."""
 
     @abstractmethod
-    def on_full_listing_stop(self, is_abortd: bool, exception: Optional[Exception]) -> None:
-        ...
+    def on_full_listing_stop(self, is_aborted: bool, exception: Optional[Exception]) -> None:
+        """
+        This override is called when the full listing is stopped.
+        Parameters
+        ----------
+        is_aborted : bool
+            The processing was aborted.
+        exception : Optional[Exception]
+            If not None, there was an exception.
+        """
 
     # listing
 
     @abstractmethod
-    def on_listing_start(self, subscription: "SubscriptionBody") -> None:
-        ...
+    def on_incremental_start(self, subscription: "SubscriptionBody") -> None:
+        """This override is called when an incremental listing starts."""
 
     @abstractmethod
-    def on_listing_items(self, subscription: "SubscriptionBody", items: List["SubscriptionListItem"]) -> None:
-        ...
+    def on_incremental_items(self, subscription: "SubscriptionBody", items: List["SubscriptionListItem"]) -> None:
+        """This override is called repeatedly with one or more items until all updated items are listed."""
 
     @abstractmethod
-    def on_listing_stop(self, is_abortd: bool, exception: Optional[Exception]) -> None:
-        ...
+    def on_incremental_stop(self, is_aborted: bool, exception: Optional[Exception]) -> None:
+        """
+        This override is called when the incremental listing is stopped.
+        Parameters
+        ----------
+        is_aborted : bool
+            The processing was aborted.
+        exception : Optional[Exception]
+            If not None, there was an exception.
+        """
 
     def abort(self) -> None:
+        """Call this method to stop processing."""
         self._abort = True
```

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/web/web_api.py` & `macrobond-data-api-1.0.0/macrobond_data_api/web/web_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 from macrobond_data_api.common import Api
 
-from ._web_only_api import entity_search_multi_filter_long, get_subscription_list, get_subscription_list_iterative
-
+from ._web_only_api import (
+    entity_search_multi_filter_long,
+    get_subscription_list,
+    get_subscription_list_iterative,
+    subscription_list,
+)
 from ._web_api_metadata import metadata_list_values, metadata_get_attribute_information, metadata_get_value_information
 
 from ._web_api_revision import (
     get_all_vintage_series,
+    get_one_nth_release,
     get_nth_release,
     get_revision_info,
+    get_one_vintage_series,
     get_vintage_series,
     get_observation_history,
     get_many_series_with_revisions,
 )
 
 from ._web_api_series import (
     get_one_series,
@@ -19,52 +25,56 @@
     get_one_entity,
     get_entities,
     get_many_series,
     get_unified_series,
 )
 
 from ._web_api_search import entity_search_multi_filter
-
 from .session import Session
 
 
 __pdoc__ = {
     "WebApi.__init__": False,
 }
 
 
 class WebApi(Api):
     def __init__(self, session: Session) -> None:
         super().__init__()
-        self.__session = session
+        self._session = session
 
     @property
     def session(self) -> Session:
-        return self.__session
+        if not self._session._is_open:
+            raise ValueError("WebApi is not open")
+        return self._session
 
     # metadata
 
     metadata_list_values = metadata_list_values
     metadata_get_attribute_information = metadata_get_attribute_information
     metadata_get_value_information = metadata_get_value_information
 
     # revision
 
     get_revision_info = get_revision_info
+    get_one_vintage_series = get_one_vintage_series
     get_vintage_series = get_vintage_series
+    get_one_nth_release = get_one_nth_release
     get_nth_release = get_nth_release
     get_all_vintage_series = get_all_vintage_series
     get_observation_history = get_observation_history
     get_many_series_with_revisions = get_many_series_with_revisions
 
     # web only
 
     get_subscription_list = get_subscription_list
     get_subscription_list_iterative = get_subscription_list_iterative
     entity_search_multi_filter_long = entity_search_multi_filter_long
+    subscription_list = subscription_list
 
     # Search
 
     entity_search_multi_filter = entity_search_multi_filter
 
     # Series
```

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/web/web_client.py` & `macrobond-data-api-1.0.0/macrobond_data_api/web/web_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,79 @@
 _keyring_import_error: Optional[ImportError] = None
 try:
     import keyring as _keyring
 except ImportError as ex:
     _keyring_import_error = ex
 
 
+class KeyringException(Exception):
+    pass
+
+
+def _get_credentials_from_keyring(  # pylint: disable=too-many-branches
+    service_name: str, username: Optional[str]
+) -> Tuple[str, str]:
+    if username == "":
+        raise ValueError('username is set to ""')
+
+    if _keyring_import_error:
+        raise _keyring_import_error
+
+    keyring_name = _keyring.get_keyring().name
+
+    if sys.platform.startswith("darwin"):
+        credentials = _keyring.get_credential(service_name, DARWIN_USERNAME)
+        if not credentials:
+            raise KeyringException(f"Can not find the key in keyring {keyring_name}")
+
+        json_obj = json.loads(credentials.password)
+
+        if not isinstance(dict, json_obj):
+            raise KeyringException(f"Bad format, password is not a json objekt in keyring {keyring_name}")
+
+        if "username" not in json_obj:
+            raise KeyringException(f"Bad format, the json objekt is missing username in keyring {keyring_name}")
+
+        if "password" not in json_obj:
+            raise KeyringException(f"Bad format, the json objekt is missing password in keyring  {keyring_name}")
+
+        if username is None:
+            username = json_obj["username"]
+
+        password = json_obj["password"]
+    else:
+        credentials = _keyring.get_credential(service_name, None)
+
+        if credentials is None:
+            raise KeyringException(f"Can not find the key in keyring {_keyring.get_keyring()}")
+
+        if username is None:
+            username = credentials.username
+
+        password = credentials.password
+
+    if username == "":
+        raise KeyringException(f'Username is set to "" in keyring {keyring_name}')
+
+    if password == "":
+        raise KeyringException(f'Password is set to "" in keyring {keyring_name}')
+
+    return username, password
+
+
+def _has_credentials_in_keyring(service_name: Optional[str] = None) -> bool:
+    if not service_name:
+        service_name = DEFAULT_SERVICE_NAME
+    try:
+        _get_credentials_from_keyring(service_name, None)
+        return True
+    except KeyringException:
+        return False
+
+
 class WebClient(Client["WebApi"]):
     """
     WebClient to get data from the web
 
     Parameters
     ----------
     username : str, optional
@@ -76,76 +141,39 @@
         authorization_url: str = AUTHORIZATION_URL_DEFAULT,
         service_name: str = DEFAULT_SERVICE_NAME,
         proxy: str = None,
     ) -> None:
         super().__init__()
 
         if password is None:
-            credentials = self.__get_credentials_from_keyring(service_name, username)
+            credentials = _get_credentials_from_keyring(service_name, username)
             username = credentials[0]
             password = credentials[1]
         else:
             if username is None:
                 raise ValueError("username is None")
 
         if scopes is None:
             scopes = []
 
+        self.has_closed = False
         self.__api: Optional["WebApi"] = None
         self.__session = _Session(
             username, password, *scopes, api_url=api_url, authorization_url=authorization_url, proxy=proxy
         )
 
     @property
     def is_open(self) -> bool:
         return bool(self.__api)
 
     def open(self) -> "WebApi":
+        if self.has_closed:
+            raise ValueError("WebClient can not be reopend")
         if self.__api is None:
             self.__session.fetch_token()
             self.__api = WebApi(self.__session)
         return self.__api
 
     def close(self) -> None:
         self.__session.close()
-
-    def __get_credentials_from_keyring(self, service_name: str, username: Optional[str]) -> Tuple[str, str]:
-        if _keyring_import_error:
-            raise _keyring_import_error
-
-        keyring_name = _keyring.get_keyring().name
-
-        if sys.platform.startswith("darwin"):
-            credentials = _keyring.get_credential(service_name, DARWIN_USERNAME)
-            if not credentials:
-                raise ValueError(f"can not find the key in keyring {keyring_name}")
-
-            if credentials.password == "":
-                raise ValueError(f"can not find the key in keyring {keyring_name}")
-
-            json_obj = json.loads(credentials.password)
-
-            if not isinstance(dict, json_obj):
-                raise ValueError(f"can not find the key in keyring {keyring_name}")
-
-            if "username" not in json_obj:
-                raise ValueError(f"can not find the key in keyring {keyring_name}")
-
-            if "password" not in json_obj:
-                raise ValueError(f"can not find the key in keyring {keyring_name}")
-
-            if username is None:
-                username = json_obj["username"]
-
-            password = json_obj["password"]
-        else:
-            credentials = _keyring.get_credential(service_name, "")
-
-            if credentials is None:
-                raise ValueError(f"can not find the key in keyring {_keyring.get_keyring()}")
-
-            if username is None:
-                username = credentials.username
-
-            password = credentials.password
-
-        return username, password
+        self.__api = None
+        self.has_closed = True
```

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/__init__.py` & `macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 from .series_methods import SeriesMethods
 
 from .series_tree_methods import SeriesTreeMethods
 
 from .http_exception import HttpException
 from .problem_details_exception import ProblemDetailsException
 
-from .status_response import ResponseErrorCode
-
 from .entity_info_for_display_response import (
     EntityInfoForDisplayItem,
     EntityInfoForDisplayGroup,
     EntityInfoForDisplayResponse,
 )
 
 from .entity_request import EntityRequest
```

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/entity_info_for_display_response.py` & `macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/entity_info_for_display_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# pylint: disable = missing-module-docstring
-
 from typing import List, Optional
 from typing_extensions import TypedDict
 
 
 from .metadata import MetadataAttributeTypeRestriction
 
 from ...common.enums import MetadataAttributeType
```

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/feed_entities_response.py` & `macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/feed_entities_response.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# pylint: disable = missing-module-docstring
-
 from typing import List
 from typing_extensions import TypedDict
 
 
 class EntityNameWithTimeStamp(TypedDict):
     """Name and timestamp of an entity"""
```

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/http_exception.py` & `macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/http_exception.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/metadata/metadata_attribute_information_response.py` & `macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/metadata/metadata_attribute_information_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# pylint: disable = missing-module-docstring
-
 from typing import Optional, List
 from enum import IntEnum
 from typing_extensions import TypedDict
 
 from ....common.enums import MetadataAttributeType
```

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/metadata_methods.py` & `macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/metadata_methods.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/problem_details_exception.py` & `macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/problem_details_exception.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/response_error_code.py` & `macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/response_error_code.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/revision_history_request.py` & `macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/revision_history_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# pylint: disable = missing-module-docstring
-
 from typing import Optional
 from typing_extensions import TypedDict
 
 
 class RevisionHistoryRequest(TypedDict, total=False):
     """Request of new revisions of a time series"""
```

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/search/item_listing_response.py` & `macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/search/item_listing_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# pylint: disable = missing-module-docstring
-
 from typing import Optional, List
 from typing_extensions import TypedDict
 
 
 class ItemInformation(TypedDict):
     # pylint: disable = missing-class-docstring
```

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/search/search_filter.py` & `macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/search/search_filter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# pylint: disable = missing-module-docstring
-
 from typing import Optional, List, Dict
 from typing_extensions import TypedDict
 
 
 class SearchFilter(TypedDict, total=False):
     """A filter in a search request"""
```

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/search_methods.py` & `macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/search_methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# pylint: disable = missing-module-docstring
-
 from typing import cast, List, Dict, TYPE_CHECKING
 
 if TYPE_CHECKING:  # pragma: no cover
     from ..session import Session
     from .search import (
         SearchResponse,
         SearchRequest,
```

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/series_methods.py` & `macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/series_methods.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# pylint: disable = missing-module-docstring
-
 from typing import List, Sequence, cast, TYPE_CHECKING
 
 from datetime import datetime
 
 if TYPE_CHECKING:  # pragma: no cover
     from requests import Response
     from ..session import Session
```

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/series_observation_history_response.py` & `macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/series_observation_history_response.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# pylint: disable = missing-module-docstring
-
 from typing import List, Optional
 from typing_extensions import TypedDict
 
 
 class SeriesObservationHistoryResponse(TypedDict):
     """The history of changes of an observation"""
```

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/series_tree/series_tree_listing_response.py` & `macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/series_tree/series_tree_listing_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# pylint: disable = missing-module-docstring
-
 from typing import Optional, List, Dict
 from typing_extensions import TypedDict
 
 
 class SeriesTreeListingSeries(TypedDict):
     """Defines an aspect in a structured series list"""
```

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/series_tree/series_tree_node_response.py` & `macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/series_tree/series_tree_node_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# pylint: disable = missing-module-docstring
-
 from typing import Union, List
 
 from typing_extensions import TypedDict
 
 
 class SeriesTreeNodeResponse(TypedDict):
     nodeType: str
```

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/series_tree_methods.py` & `macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/series_tree_methods.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# pylint: disable = missing-module-docstring
-
 from typing import List, Union, cast, TYPE_CHECKING
 
 if TYPE_CHECKING:  # pragma: no cover
     from ..session import Session
     from .series_tree import (
         SeriesTreeNodeLeaf,
         SeriesTreeNodeBranchRef,
```

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/series_with_revisions_info_response.py` & `macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/series_with_revisions_info_response.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# pylint: disable = missing-module-docstring
-
 from typing import List, Optional
 
 from .status_response import StatusResponse
 
 
 class SeriesWithRevisionsInfoResponse(StatusResponse):
     """Information about a series related to storage of updates"""
```

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/series_with_vintages_response.py` & `macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/series_with_vintages_response.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# pylint: disable = missing-module-docstring
-
 from typing import Optional, Dict, Any, List
 from typing_extensions import TypedDict
 
 from .vintage_values_response import VintageValuesResponse
 
 
 class SeriesWithVintagesResponse(TypedDict, total=False):
```

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/status_response.py` & `macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/status_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,19 @@
-# pylint: disable = missing-module-docstring
-
 from typing import Optional
-from enum import IntEnum
 from typing_extensions import TypedDict
 
 
-class ResponseErrorCode(IntEnum):
-    """Response Error Codes"""
-
-    NOT_MODIFIED = 304
-    """The item was not modified and is not included in the response"""
-
-    NOT_FOUND = 404
-    """The item was not found"""
-
-    FORBIDDEN = 403
-    """Access to the item was denied"""
-
-    OTHER = 500
-    """There was an error and it is described in the error text"""
-
-
 class StatusResponse(TypedDict):
     """A status response"""
 
     errorText: Optional[str]
     """The error text if there was an error or not specified if there was no error"""
 
-    errorCode: Optional[ResponseErrorCode]
-    """Set if there was an error and not specified if there was no error"""
+    errorCode: Optional[int]
+    """
+    Set if there was an error and not specified if there was no error
+
+    304 - The item was not modified and is not included in the response.
+    404 - The item was not found.
+    403 - Access to the item was denied.
+    500 - There was an error and it is described in the error text.
+    """
```

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/subscription_body.py` & `macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/subscription_body.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/subscription_list.py` & `macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/subscription_list.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import dataclass
 
 from typing import List, Sequence, TYPE_CHECKING, overload
 
-from dateutil import parser
+from macrobond_data_api.common.types._parse_iso8601 import _parse_iso8601
 
 from .subscription_list_state import SubscriptionListState
 from .subscription_list_item import SubscriptionListItem
 from .subscription_body import SubscriptionBody
 
 if TYPE_CHECKING:  # pragma: no cover
     from .feed_entities_response import FeedEntitiesResponse
@@ -18,19 +18,19 @@
 
     items: Sequence[SubscriptionListItem]
 
     def __init__(self, response: "FeedEntitiesResponse") -> None:
         download_full = response.get("downloadFullListOnOrAfter")
         SubscriptionBody.__init__(
             self,
-            parser.parse(response["timeStampForIfModifiedSince"]),
-            parser.parse(download_full) if download_full is not None else None,
+            _parse_iso8601(response["timeStampForIfModifiedSince"]),
+            _parse_iso8601(download_full) if download_full is not None else None,
             SubscriptionListState(response["state"]),
         )
-        self.items = [SubscriptionListItem(x["name"], parser.parse(x["modified"])) for x in response["entities"]]
+        self.items = [SubscriptionListItem(x["name"], _parse_iso8601(x["modified"])) for x in response["entities"]]
 
     @overload
     def __getitem__(self, i: int) -> SubscriptionListItem:
         ...
 
     @overload
     def __getitem__(self, s: slice) -> List[SubscriptionListItem]:
```

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/subscription_list_state.py` & `macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/subscription_list_state.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api/web/web_types/unified_series_request.py` & `macrobond-data-api-1.0.0/macrobond_data_api/web/web_types/unified_series_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# pylint: disable = missing-module-docstring
-
 from typing import List, Optional
 from typing_extensions import TypedDict
 
 from macrobond_data_api.common.enums import (
     SeriesWeekdays,
     SeriesFrequency,
     CalendarDateMode,
```

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api.egg-info/PKG-INFO` & `macrobond-data-api-1.0.0/macrobond_data_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrobond-data-api
-Version: 0.0.9
+Version: 1.0.0
 Summary: Exposes a common API in Python for the Macrobond Web and Client Data APIs
 Home-page: https://github.com/macrobond/macrobond-data-api
 Author: Macrobond Financial
 Author-email: support@macrobond.com
 Project-URL: Documentation, https://macrobond.github.io/macrobond-data-api
 Project-URL: Source, https://github.com/macrobond/macrobond-data-api
 Project-URL: Tracker, https://github.com/macrobond/macrobond-data-api/issues
@@ -24,16 +24,14 @@
     <a href="https://www.macrobond.com/">
         <img loading="lazy" aria-roledescription="brand logo" alt="Macrobond logo" src="https://macrobond.github.io/macrobond-data-api/assets/Macrobond_logo_Color.svg" width="30%">
     </a>
 </div>
 
 <h1 align="center">Macrobond Data API for Python</h1>
 
-<h1 align="center">This software is in beta !</h1>
-
 <p align="center">
     <a href="https://pypi.org/project/macrobond-data-api/">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/macrobond-data-api">
     </a>
     <a href="https://pypi.org/project/macrobond-data-api/">
         <img alt="PyPI" src="https://img.shields.io/pypi/pyversions/macrobond-data-api.svg">
     </a>
@@ -62,14 +60,16 @@
 [Macrobond Web](https://help.macrobond.com/technical-information/the-macrobond-data-web-api-feed/)
 and [Client data](https://help.macrobond.com/technical-information/the-macrobond-api-for-python/)
 APIs
 
 You have to be a licensed user and have a Data+ or data feed user account in
 order to use the API.
 
+[***Examples in Jupyter Notebooks*** to help you get started](https://github.com/macrobond/macrobond-data-api/tree/main/examples)
+
 [***API reference***](https://macrobond.github.io/macrobond-data-api/)
 
 ## Basic usage
 
 ```python
 import macrobond_data_api as mb_api
 
@@ -79,21 +79,21 @@
 ## Advanced usage
 
 ```python
 # web
 from macrobond_data_api.web import WebClient
 
 with WebClient('client id', 'client secret') as api:
-    series = api.series.get_one_series('usgdp')
+    series = api.get_one_series('usgdp')
 
 # com
 from macrobond_data_api.com import ComClient
 
 with ComClient() as api:
-    series = api.series.get_one_series('usgdp')
+    series = api.get_one_series('usgdp')
 ```
 
 ## Features
 
 The Macrobond Data API for Python uses either the
 [Macrobond Web REST API](https://help.macrobond.com/technical-information/the-macrobond-data-web-api-feed/)
 or the [Macrobond Client data API](https://help.macrobond.com/technical-information/the-macrobond-api-for-python/)
```

#### html2text {}

```diff
@@ -1,51 +1,52 @@
-Metadata-Version: 2.1 Name: macrobond-data-api Version: 0.0.9 Summary: Exposes
+Metadata-Version: 2.1 Name: macrobond-data-api Version: 1.0.0 Summary: Exposes
 a common API in Python for the Macrobond Web and Client Data APIs Home-page:
 https://github.com/macrobond/macrobond-data-api Author: Macrobond Financial
 Author-email: support@macrobond.com Project-URL: Documentation, https://
 macrobond.github.io/macrobond-data-api Project-URL: Source, https://github.com/
 macrobond/macrobond-data-api Project-URL: Tracker, https://github.com/
 macrobond/macrobond-data-api/issues Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Requires-Python: >=3.7 Description-Content-Type: text/markdown Provides-
 Extra: extra Provides-Extra: dev Provides-Extra: socks License-File: LICENSE
                                [Macrobond_logo]
                   ****** Macrobond Data API for Python ******
-                   ****** This software is in beta ! ******
   [PyPI] [PyPI] [License:_MIT] [Code_style:_black] [Continuous_Integration]
  The Macrobond Data API for Python is used to access the worldâs most
 extensive macroeconomic, aggregate financial and sector database provided by
 [Macrobond](http://www.macrobond.com). Exposes a common API in Python for the
 [Macrobond Web](https://help.macrobond.com/technical-information/the-macrobond-
 data-web-api-feed/) and [Client data](https://help.macrobond.com/technical-
 information/the-macrobond-api-for-python/) APIs You have to be a licensed user
-and have a Data+ or data feed user account in order to use the API. [***API
+and have a Data+ or data feed user account in order to use the API.
+[***Examples in Jupyter Notebooks*** to help you get started](https://
+github.com/macrobond/macrobond-data-api/tree/main/examples) [***API
 reference***](https://macrobond.github.io/macrobond-data-api/) ## Basic usage
 ```python import macrobond_data_api as mb_api usgdp = mb_api.get_one_series
 ("usgdp") ``` ## Advanced usage ```python # web from macrobond_data_api.web
 import WebClient with WebClient('client id', 'client secret') as api: series =
-api.series.get_one_series('usgdp') # com from macrobond_data_api.com import
-ComClient with ComClient() as api: series = api.series.get_one_series('usgdp')
-``` ## Features The Macrobond Data API for Python uses either the [Macrobond
-Web REST API](https://help.macrobond.com/technical-information/the-macrobond-
-data-web-api-feed/) or the [Macrobond Client data API](https://
-help.macrobond.com/technical-information/the-macrobond-api-for-python/) to
-obtain time series with values and metadata. The API consists of a set of
-functions in common between the underlying APIs as well as specialized
-functions unique to each implementation. ## Installing macrobond-data-api and
-Supported Versions Macrobond Data API for Python is available on [PyPI](https:/
-/pypi.org/project/macrobond-data-api/): ```console python -m pip install
-macrobond-data-api ``` Macrobond Data API for Python officially supports Python
-3.6+. ## Using of system keyring When using WebClient it is recommended to use
-the system keyring. This can be done easily by running the include script using
-this command: ```console python -c "from macrobond_data_api.util import *;
-save_credential_to_keyring()" ``` ### Supported keyrings * macOS [Keychain]
-(https://en.wikipedia.org/wiki/Keychain_%28software%29) * Freedesktop [Secret
-Service](http://standards.freedesktop.org/secret-service/) supports many DE
-including GNOME (requires [secretstorage](https://pypi.python.org/pypi/
-secretstorage)) * KDE4 & KDE5 [KWallet](https://en.wikipedia.org/wiki/KWallet)
-(requires [dbus](https://pypi.python.org/pypi/dbus-python)) * [Windows
-Credential Locker](https://docs.microsoft.com/en-us/windows/uwp/security/
-credential-locker) ## Contributing We welcome community pull requests for bug
-fixes, enhancements, and documentation. ## Getting support [Support options]
-(https://help.macrobond.com/support/)
+api.get_one_series('usgdp') # com from macrobond_data_api.com import ComClient
+with ComClient() as api: series = api.get_one_series('usgdp') ``` ## Features
+The Macrobond Data API for Python uses either the [Macrobond Web REST API]
+(https://help.macrobond.com/technical-information/the-macrobond-data-web-api-
+feed/) or the [Macrobond Client data API](https://help.macrobond.com/technical-
+information/the-macrobond-api-for-python/) to obtain time series with values
+and metadata. The API consists of a set of functions in common between the
+underlying APIs as well as specialized functions unique to each implementation.
+## Installing macrobond-data-api and Supported Versions Macrobond Data API for
+Python is available on [PyPI](https://pypi.org/project/macrobond-data-api/):
+```console python -m pip install macrobond-data-api ``` Macrobond Data API for
+Python officially supports Python 3.6+. ## Using of system keyring When using
+WebClient it is recommended to use the system keyring. This can be done easily
+by running the include script using this command: ```console python -c "from
+macrobond_data_api.util import *; save_credential_to_keyring()" ``` ###
+Supported keyrings * macOS [Keychain](https://en.wikipedia.org/wiki/
+Keychain_%28software%29) * Freedesktop [Secret Service](http://
+standards.freedesktop.org/secret-service/) supports many DE including GNOME
+(requires [secretstorage](https://pypi.python.org/pypi/secretstorage)) * KDE4 &
+KDE5 [KWallet](https://en.wikipedia.org/wiki/KWallet) (requires [dbus](https://
+pypi.python.org/pypi/dbus-python)) * [Windows Credential Locker](https://
+docs.microsoft.com/en-us/windows/uwp/security/credential-locker) ##
+Contributing We welcome community pull requests for bug fixes, enhancements,
+and documentation. ## Getting support [Support options](https://
+help.macrobond.com/support/)
```

### Comparing `macrobond-data-api-0.0.9/macrobond_data_api.egg-info/SOURCES.txt` & `macrobond-data-api-1.0.0/macrobond_data_api.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,17 @@
 macrobond_data_api.egg-info/requires.txt
 macrobond_data_api.egg-info/top_level.txt
 macrobond_data_api/com/__init__.py
 macrobond_data_api/com/_com_api_metadata.py
 macrobond_data_api/com/_com_api_revision.py
 macrobond_data_api/com/_com_api_search.py
 macrobond_data_api/com/_com_api_series.py
+macrobond_data_api/com/_error_message_to_status_code.py
 macrobond_data_api/com/_fill_metadata.py
+macrobond_data_api/com/_fix_datetime.py
 macrobond_data_api/com/com_api.py
 macrobond_data_api/com/com_client.py
 macrobond_data_api/com/com_types/__init__.py
 macrobond_data_api/com/com_types/connection.py
 macrobond_data_api/com/com_types/database.py
 macrobond_data_api/com/com_types/entity.py
 macrobond_data_api/com/com_types/metadata.py
@@ -41,17 +43,20 @@
 macrobond_data_api/common/enums/metadata_attribute_type.py
 macrobond_data_api/common/enums/series_frequency.py
 macrobond_data_api/common/enums/series_missing_value_method.py
 macrobond_data_api/common/enums/series_partial_periods_method.py
 macrobond_data_api/common/enums/series_to_higher_frequency_method.py
 macrobond_data_api/common/enums/series_to_lower_frequency_method.py
 macrobond_data_api/common/enums/series_weekdays.py
+macrobond_data_api/common/enums/status_code.py
 macrobond_data_api/common/types/__init__.py
+macrobond_data_api/common/types/_parse_iso8601.py
 macrobond_data_api/common/types/_repr_html_sequence.py
 macrobond_data_api/common/types/entity.py
+macrobond_data_api/common/types/format_exception.py
 macrobond_data_api/common/types/get_all_vintage_series_result.py
 macrobond_data_api/common/types/get_entity_error.py
 macrobond_data_api/common/types/metadata.py
 macrobond_data_api/common/types/metadata_attribute_information.py
 macrobond_data_api/common/types/metadata_value_information.py
 macrobond_data_api/common/types/revision_history_request.py
 macrobond_data_api/common/types/revision_info.py
@@ -68,22 +73,23 @@
 macrobond_data_api/common/types/vintage_series.py
 macrobond_data_api/util/__init__.py
 macrobond_data_api/util/save_credential_to_keyring.py
 macrobond_data_api/web/__init__.py
 macrobond_data_api/web/_metadata.py
 macrobond_data_api/web/_metadata_directory.py
 macrobond_data_api/web/_split_in_to_chunks.py
+macrobond_data_api/web/_subscription_list_poller.py
 macrobond_data_api/web/_web_api_metadata.py
 macrobond_data_api/web/_web_api_revision.py
 macrobond_data_api/web/_web_api_search.py
 macrobond_data_api/web/_web_api_series.py
 macrobond_data_api/web/_web_only_api.py
 macrobond_data_api/web/scope.py
 macrobond_data_api/web/session.py
-macrobond_data_api/web/subscription_list_poller.py
+macrobond_data_api/web/subscription_list.py
 macrobond_data_api/web/web_api.py
 macrobond_data_api/web/web_client.py
 macrobond_data_api/web/web_types/__init__.py
 macrobond_data_api/web/web_types/entity_info_for_display_response.py
 macrobond_data_api/web/web_types/entity_request.py
 macrobond_data_api/web/web_types/entity_response.py
 macrobond_data_api/web/web_types/feed_entities_response.py
```

### Comparing `macrobond-data-api-0.0.9/setup.cfg` & `macrobond-data-api-1.0.0/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -22,14 +22,20 @@
 	duplicate-code,
 	protected-access,
 	
 	signature-differs,
 	
 	multiple-statements,
 	invalid-name,
+	
+	line-too-long,
+	
+	W0511,
+	
+	W0719,
 
 [metadata]
 description_file = README.md
 license_files = LICENSE
 
 [egg_info]
 tag_build =
```

### Comparing `macrobond-data-api-0.0.9/setup.py` & `macrobond-data-api-1.0.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -51,16 +51,14 @@
 __url__ = "''' + URL + '''"
 '''
 # fmt: on
 
 with open(version_info_path, "w+", encoding="utf-8") as fh:
     fh.write(PACKAGE_INFO)
 
-REQUESTS_VERSION = "2.28.1"
-
 setuptools.setup(
     name="macrobond-data-api",
     packages=setuptools.find_packages(include=["macrobond_data_api", "macrobond_data_api.*"]),
     version=version,
     author=AUTHOR,
     author_email=AUTHOR_EMAIL,
     description=DESCRIPTION,
@@ -76,40 +74,39 @@
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
     ],
     python_requires=">=3.7",
     install_requires=[
         "keyring>=23.11.0",
         "Authlib>=1.2.0",
-        "requests>=" + REQUESTS_VERSION,
-        "python-dateutil>=2.8.2",
+        "requests>=2.28.2",
         "ijson>=3.1.4",
-        "typing_extensions>=4.4.0",
+        "typing_extensions>=4.5.0",
         "pywin32>=305; os_name=='nt'",
     ],
     extras_require={
         "extra": ["matplotlib", "statsmodels", "scikit-learn", "pandas"],
         "dev": [
-            "mypy==1.0.0",
-            "pylint==2.15.8",
+            "mypy==1.2.0",
+            "pylint==2.17.2",
             "pycodestyle==2.10.0",
             "pdoc3==0.10.0",
             "build>=0.10.0",
-            "pytest==7.2.1",
+            "pytest==7.2.2",
             "pytest-xdist==3.2.0",
-            "coverage>=7.1.0",
-            "black[jupyter]==23.1.0",
-            "requests[socks]>=" + REQUESTS_VERSION,
-            # types
-            "types-pywin32==305.0.0.7",
-            "types-python-dateutil==2.8.19.6",
-            "types-requests==2.28.11.8",
-            "types-setuptools==67.2.0.1",
+            "coverage>=7.2.1",
+            "black[jupyter]==23.3.0",
+            "requests[socks]>=2.28.2",
+            "nbconvert==7.3.0",
+            "ipython>=7.34.0",
+            "types-pywin32==305.0.0.10",
+            "types-requests==2.28.11.15",
+            "types-setuptools==67.6.0.0",
         ],
-        "socks": ["requests[socks]>=" + REQUESTS_VERSION],
+        "socks": ["requests[socks]>=2.28.2"],
     },
     project_urls={
         "Documentation": "https://macrobond.github.io/macrobond-data-api",
         "Source": "https://github.com/macrobond/macrobond-data-api",
         "Tracker": "https://github.com/macrobond/macrobond-data-api/issues",
     },
 )
```

