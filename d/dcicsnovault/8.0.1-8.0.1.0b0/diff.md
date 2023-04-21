# Comparing `tmp/dcicsnovault-8.0.1.tar.gz` & `tmp/dcicsnovault-8.0.1.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcicsnovault-8.0.1.tar", max compression
+gzip compressed data, was "dcicsnovault-8.0.1.0b0.tar", max compression
```

## Comparing `dcicsnovault-8.0.1.tar` & `dcicsnovault-8.0.1.0b0.tar`

### file list

```diff
@@ -1,123 +1,154 @@
--rw-r--r--   0        0        0     1135 2023-04-10 18:53:44.992983 dcicsnovault-8.0.1/LICENSE.txt
--rw-r--r--   0        0        0     6407 2023-04-10 18:53:44.992983 dcicsnovault-8.0.1/README.rst
--rw-r--r--   0        0        0     5556 2023-04-10 18:53:44.996983 dcicsnovault-8.0.1/pyproject.toml
--rw-r--r--   0        0        0     4460 2023-04-10 18:53:44.996983 dcicsnovault-8.0.1/snovault/__init__.py
--rw-r--r--   0        0        0     1942 2023-04-10 18:53:44.996983 dcicsnovault-8.0.1/snovault/aggregated_items.py
--rw-r--r--   0        0        0     8799 2023-04-10 18:53:44.996983 dcicsnovault-8.0.1/snovault/app.py
--rw-r--r--   0        0        0    11879 2023-04-10 18:53:44.996983 dcicsnovault-8.0.1/snovault/attachment.py
--rw-r--r--   0        0        0     6670 2023-04-10 18:53:44.996983 dcicsnovault-8.0.1/snovault/batchupgrade.py
--rw-r--r--   0        0        0     1902 2023-04-10 18:53:44.996983 dcicsnovault-8.0.1/snovault/cache.py
--rw-r--r--   0        0        0     6461 2023-04-10 18:53:44.996983 dcicsnovault-8.0.1/snovault/calculated.py
--rw-r--r--   0        0        0       10 2023-04-10 18:53:44.996983 dcicsnovault-8.0.1/snovault/commands/__init__.py
--rw-r--r--   0        0        0     3416 2023-04-10 18:53:44.996983 dcicsnovault-8.0.1/snovault/commands/check_rendering.py
--rw-r--r--   0        0        0     1608 2023-04-10 18:53:44.996983 dcicsnovault-8.0.1/snovault/commands/es_index_data.py
--rw-r--r--   0        0        0     1644 2023-04-10 18:53:44.996983 dcicsnovault-8.0.1/snovault/commands/jsonld_rdf.py
--rw-r--r--   0        0        0     4350 2023-04-10 18:53:44.996983 dcicsnovault-8.0.1/snovault/commands/profile.py
--rw-r--r--   0        0        0      909 2023-04-10 18:53:44.996983 dcicsnovault-8.0.1/snovault/commands/wipe_test_indices.py
--rw-r--r--   0        0        0     4183 2023-04-10 18:53:44.996983 dcicsnovault-8.0.1/snovault/config.py
--rw-r--r--   0        0        0     6352 2023-04-10 18:53:44.996983 dcicsnovault-8.0.1/snovault/connection.py
--rw-r--r--   0        0        0    14815 2023-04-10 18:53:44.996983 dcicsnovault-8.0.1/snovault/crud_views.py
--rw-r--r--   0        0        0     4282 2023-04-10 18:53:44.996983 dcicsnovault-8.0.1/snovault/elasticsearch/__init__.py
--rw-r--r--   0        0        0     4727 2023-04-10 18:53:44.996983 dcicsnovault-8.0.1/snovault/elasticsearch/cached_views.py
--rw-r--r--   0        0        0    61320 2023-04-10 18:53:44.996983 dcicsnovault-8.0.1/snovault/elasticsearch/create_mapping.py
--rw-r--r--   0        0        0     7939 2023-04-10 18:53:44.996983 dcicsnovault-8.0.1/snovault/elasticsearch/es_index_listener.py
--rw-r--r--   0        0        0    18572 2023-04-10 18:53:44.996983 dcicsnovault-8.0.1/snovault/elasticsearch/esstorage.py
--rw-r--r--   0        0        0    24405 2023-04-10 18:53:44.996983 dcicsnovault-8.0.1/snovault/elasticsearch/indexer.py
--rw-r--r--   0        0        0    31356 2023-04-10 18:53:44.996983 dcicsnovault-8.0.1/snovault/elasticsearch/indexer_queue.py
--rw-r--r--   0        0        0    20947 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/elasticsearch/indexer_utils.py
--rw-r--r--   0        0        0      349 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/elasticsearch/interfaces.py
--rw-r--r--   0        0        0    10190 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/elasticsearch/mpindexer.py
--rw-r--r--   0        0        0     8249 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/embed.py
--rw-r--r--   0        0        0     1061 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/etag.py
--rw-r--r--   0        0        0    10835 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/indexing_views.py
--rw-r--r--   0        0        0      774 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/interfaces.py
--rw-r--r--   0        0        0     2229 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/invalidation.py
--rw-r--r--   0        0        0     1639 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/json_renderer.py
--rw-r--r--   0        0        0     2292 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/jsongraph.py
--rw-r--r--   0        0        0     9713 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/jsonld_context.py
--rw-r--r--   0        0        0      846 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/predicates.py
--rw-r--r--   0        0        0       95 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/redis/README.rst
--rw-r--r--   0        0        0       90 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/redis/__init__.py
--rw-r--r--   0        0        0       16 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/redis/interfaces.py
--rw-r--r--   0        0        0     4106 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/redis/redis_connection.py
--rw-r--r--   0        0        0     6495 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/renderers.py
--rw-r--r--   0        0        0    11201 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/resource_views.py
--rw-r--r--   0        0        0    21863 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/resources.py
--rw-r--r--   0        0        0     3450 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/schema_graph.py
--rw-r--r--   0        0        0    16947 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/schema_utils.py
--rw-r--r--   0        0        0     4359 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/schema_views.py
--rw-r--r--   0        0        0      522 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/settings.py
--rw-r--r--   0        0        0     1498 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/standalone_dev.py
--rw-r--r--   0        0        0     4383 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/stats.py
--rw-r--r--   0        0        0    34834 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/storage.py
--rw-r--r--   0        0        0      330 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/test_schemas/AbstractItemTestSecondSubItem.json
--rw-r--r--   0        0        0      300 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/test_schemas/AbstractItemTestSubItem.json
--rw-r--r--   0        0        0     2467 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/test_schemas/EmbeddingTest.json
--rw-r--r--   0        0        0      446 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/test_schemas/NestedEmbeddingContainer.json
--rw-r--r--   0        0        0      883 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/test_schemas/NestedObjectLinkTarget.json
--rw-r--r--   0        0        0      473 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/test_schemas/TestingBiogroupSno.json
--rw-r--r--   0        0        0      968 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/test_schemas/TestingBiosampleSno.json
--rw-r--r--   0        0        0     1082 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/test_schemas/TestingBiosourceSno.json
--rw-r--r--   0        0        0      894 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/test_schemas/TestingCalculatedProperties.json
--rw-r--r--   0        0        0      276 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/test_schemas/TestingDependencies.json
--rw-r--r--   0        0        0      577 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/test_schemas/TestingDownload.json
--rw-r--r--   0        0        0      555 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/test_schemas/TestingIndividualSno.json
--rw-r--r--   0        0        0      730 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/test_schemas/TestingLinkAggregateSno.json
--rw-r--r--   0        0        0      697 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/test_schemas/TestingLinkSourceSno.json
--rw-r--r--   0        0        0      472 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/test_schemas/TestingLinkTargetElasticSearch.json
--rw-r--r--   0        0        0      292 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/test_schemas/TestingLinkTargetSno.json
--rw-r--r--   0        0        0      311 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/test_schemas/TestingMixins.json
--rw-r--r--   0        0        0      845 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/test_schemas/TestingNestedEnabled.json
--rw-r--r--   0        0        0     3721 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/test_schemas/TestingNoteSno.json
--rw-r--r--   0        0        0     1622 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/test_schemas/TestingPostPutPatchSno.json
--rw-r--r--   0        0        0      576 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/test_schemas/TestingServerDefault.json
--rw-r--r--   0        0        0      417 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/test_schemas/mixins.json
--rw-r--r--   0        0        0        0 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/tests/__init__.py
--rw-r--r--   0        0        0     9899 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/tests/authentication.py
--rw-r--r--   0        0        0     2068 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/tests/authorization.py
--rw-r--r--   0        0        0     2210 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/tests/conftest.py
--rw-r--r--   0        0        0      100 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/tests/conftest_settings.py
--rw-r--r--   0        0        0     3086 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/tests/elasticsearch_fixture.py
--rw-r--r--   0        0        0     3921 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/tests/postgresql_fixture.py
--rw-r--r--   0        0        0      852 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/tests/pyramidfixtures.py
--rw-r--r--   0        0        0     3007 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/tests/root.py
--rw-r--r--   0        0        0    59212 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/tests/search.py
--rw-r--r--   0        0        0    17312 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/tests/serverfixtures.py
--rw-r--r--   0        0        0     1857 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/tests/snowflake_hash.py
--rw-r--r--   0        0        0    20332 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/tests/test_attachment.py
--rw-r--r--   0        0        0     3932 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/tests/test_authentication.py
--rw-r--r--   0        0        0     1370 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/tests/test_calculated.py
--rw-r--r--   0        0        0     8984 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/tests/test_create_mapping.py
--rw-r--r--   0        0        0     7458 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/tests/test_embed_utils.py
--rw-r--r--   0        0        0     8823 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/tests/test_embedding.py
--rw-r--r--   0        0        0    10024 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/tests/test_es_permissions.py
--rw-r--r--   0        0        0    97622 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/tests/test_indexing.py
--rw-r--r--   0        0        0    28258 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/tests/test_invalidation_scope.py
--rw-r--r--   0        0        0     2147 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/tests/test_key.py
--rw-r--r--   0        0        0     2458 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/tests/test_link.py
--rw-r--r--   0        0        0     5316 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/tests/test_logging.py
--rw-r--r--   0        0        0     1134 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/tests/test_misc.py
--rw-r--r--   0        0        0      373 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/tests/test_mixins.py
--rw-r--r--   0        0        0    13660 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/tests/test_post_put_patch.py
--rw-r--r--   0        0        0     1570 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/tests/test_postgresql_fixture.py
--rw-r--r--   0        0        0     1194 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/tests/test_schemas.py
--rw-r--r--   0        0        0      952 2023-04-10 18:53:45.004983 dcicsnovault-8.0.1/snovault/tests/test_serverfixtures.py
--rw-r--r--   0        0        0      484 2023-04-10 18:53:45.004983 dcicsnovault-8.0.1/snovault/tests/test_snowflake_hash.py
--rw-r--r--   0        0        0     4267 2023-04-10 18:53:45.004983 dcicsnovault-8.0.1/snovault/tests/test_standalone_dev.py
--rw-r--r--   0        0        0     2211 2023-04-10 18:53:45.004983 dcicsnovault-8.0.1/snovault/tests/test_stats.py
--rw-r--r--   0        0        0    13182 2023-04-10 18:53:45.004983 dcicsnovault-8.0.1/snovault/tests/test_storage.py
--rw-r--r--   0        0        0     1291 2023-04-10 18:53:45.004983 dcicsnovault-8.0.1/snovault/tests/test_upgrader.py
--rw-r--r--   0        0        0     6635 2023-04-10 18:53:45.004983 dcicsnovault-8.0.1/snovault/tests/test_util.py
--rw-r--r--   0        0        0    18612 2023-04-10 18:53:45.004983 dcicsnovault-8.0.1/snovault/tests/test_views.py
--rw-r--r--   0        0        0     4621 2023-04-10 18:53:45.004983 dcicsnovault-8.0.1/snovault/tests/testappfixtures.py
--rw-r--r--   0        0        0      688 2023-04-10 18:53:45.004983 dcicsnovault-8.0.1/snovault/tests/testing_key.py
--rw-r--r--   0        0        0      677 2023-04-10 18:53:45.004983 dcicsnovault-8.0.1/snovault/tests/testing_upgrader.py
--rw-r--r--   0        0        0    26232 2023-04-10 18:53:45.004983 dcicsnovault-8.0.1/snovault/tests/testing_views.py
--rw-r--r--   0        0        0     1342 2023-04-10 18:53:45.004983 dcicsnovault-8.0.1/snovault/tests/toolfixtures.py
--rw-r--r--   0        0        0     4031 2023-04-10 18:53:45.004983 dcicsnovault-8.0.1/snovault/tools.py
--rw-r--r--   0        0        0     7605 2023-04-10 18:53:45.004983 dcicsnovault-8.0.1/snovault/typeinfo.py
--rw-r--r--   0        0        0     8124 2023-04-10 18:53:45.004983 dcicsnovault-8.0.1/snovault/upgrader.py
--rw-r--r--   0        0        0    45963 2023-04-10 18:53:45.004983 dcicsnovault-8.0.1/snovault/util.py
--rw-r--r--   0        0        0     5460 2023-04-10 18:53:45.004983 dcicsnovault-8.0.1/snovault/validation.py
--rw-r--r--   0        0        0     5718 2023-04-10 18:53:45.004983 dcicsnovault-8.0.1/snovault/validators.py
--rw-r--r--   0        0        0     9042 1970-01-01 00:00:00.000000 dcicsnovault-8.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1135 2020-04-22 15:19:59.681690 dcicsnovault-8.0.1.0b0/LICENSE.txt
+-rw-r--r--   0        0        0     6407 2023-02-08 18:10:49.791837 dcicsnovault-8.0.1.0b0/README.rst
+-rw-r--r--   0        0        0     5597 2023-04-21 16:49:59.844602 dcicsnovault-8.0.1.0b0/pyproject.toml
+-rw-r--r--   0        0        0     4586 2023-04-10 19:15:18.757135 dcicsnovault-8.0.1.0b0/snovault/__init__.py
+-rw-r--r--   0        0        0     1942 2023-02-08 18:10:49.809612 dcicsnovault-8.0.1.0b0/snovault/aggregated_items.py
+-rw-r--r--   0        0        0     8799 2023-04-10 19:15:16.606539 dcicsnovault-8.0.1.0b0/snovault/app.py
+-rw-r--r--   0        0        0    11879 2023-02-08 18:10:49.815230 dcicsnovault-8.0.1.0b0/snovault/attachment.py
+-rw-r--r--   0        0        0    25327 2023-04-10 19:15:18.762744 dcicsnovault-8.0.1.0b0/snovault/authentication.py
+-rw-r--r--   0        0        0     4467 2023-04-10 19:15:18.769224 dcicsnovault-8.0.1.0b0/snovault/authorization.py
+-rw-r--r--   0        0        0     6670 2023-02-08 18:10:49.815747 dcicsnovault-8.0.1.0b0/snovault/batchupgrade.py
+-rw-r--r--   0        0        0     1902 2020-04-22 15:19:59.997364 dcicsnovault-8.0.1.0b0/snovault/cache.py
+-rw-r--r--   0        0        0     6461 2020-10-21 18:02:06.878589 dcicsnovault-8.0.1.0b0/snovault/calculated.py
+-rw-r--r--   0        0        0       10 2020-04-22 15:19:59.995285 dcicsnovault-8.0.1.0b0/snovault/commands/__init__.py
+-rw-r--r--   0        0        0     3416 2020-09-15 14:05:58.054812 dcicsnovault-8.0.1.0b0/snovault/commands/check_rendering.py
+-rw-r--r--   0        0        0     6813 2023-04-10 19:15:18.770085 dcicsnovault-8.0.1.0b0/snovault/commands/clear_db_es_contents.py
+-rw-r--r--   0        0        0     3928 2023-04-12 19:00:53.363747 dcicsnovault-8.0.1.0b0/snovault/commands/create_mapping_on_deploy.py
+-rw-r--r--   0        0        0     1608 2023-02-08 18:10:49.821555 dcicsnovault-8.0.1.0b0/snovault/commands/es_index_data.py
+-rw-r--r--   0        0        0     1644 2020-04-22 15:19:59.991754 dcicsnovault-8.0.1.0b0/snovault/commands/jsonld_rdf.py
+-rw-r--r--   0        0        0     6212 2023-04-10 19:15:18.783044 dcicsnovault-8.0.1.0b0/snovault/commands/load_access_keys.py
+-rw-r--r--   0        0        0     2402 2023-04-12 18:12:36.164770 dcicsnovault-8.0.1.0b0/snovault/commands/load_data.py
+-rw-r--r--   0        0        0     2188 2023-04-10 19:15:18.794707 dcicsnovault-8.0.1.0b0/snovault/commands/load_data_by_type.py
+-rw-r--r--   0        0        0     4350 2023-02-08 18:10:49.822376 dcicsnovault-8.0.1.0b0/snovault/commands/profile.py
+-rw-r--r--   0        0        0     3236 2023-04-10 19:15:18.800917 dcicsnovault-8.0.1.0b0/snovault/commands/purge_item_type.py
+-rw-r--r--   0        0        0     1868 2023-04-10 19:15:18.806775 dcicsnovault-8.0.1.0b0/snovault/commands/run_upgrader_on_inserts.py
+-rw-r--r--   0        0        0     8533 2023-04-10 19:15:18.813142 dcicsnovault-8.0.1.0b0/snovault/commands/update_inserts_from_server.py
+-rw-r--r--   0        0        0      909 2023-02-08 18:10:49.823005 dcicsnovault-8.0.1.0b0/snovault/commands/wipe_test_indices.py
+-rw-r--r--   0        0        0     4183 2023-02-08 18:10:49.823623 dcicsnovault-8.0.1.0b0/snovault/config.py
+-rw-r--r--   0        0        0     6352 2023-02-08 18:10:49.824292 dcicsnovault-8.0.1.0b0/snovault/connection.py
+-rw-r--r--   0        0        0    14798 2023-04-12 18:07:32.110006 dcicsnovault-8.0.1.0b0/snovault/crud_views.py
+-rw-r--r--   0        0        0    15301 2023-04-10 19:15:18.825267 dcicsnovault-8.0.1.0b0/snovault/custom_embed.py
+-rw-r--r--   0        0        0     7216 2023-04-10 19:15:18.827085 dcicsnovault-8.0.1.0b0/snovault/dev_servers.py
+-rw-r--r--   0        0        0     4340 2023-04-13 14:12:36.718529 dcicsnovault-8.0.1.0b0/snovault/drs.py
+-rw-r--r--   0        0        0     1829 2023-04-10 19:15:18.836570 dcicsnovault-8.0.1.0b0/snovault/edw_hash.py
+-rw-r--r--   0        0        0     4282 2023-02-08 18:10:49.830617 dcicsnovault-8.0.1.0b0/snovault/elasticsearch/__init__.py
+-rw-r--r--   0        0        0     4727 2023-02-08 18:10:49.835624 dcicsnovault-8.0.1.0b0/snovault/elasticsearch/cached_views.py
+-rw-r--r--   0        0        0    61320 2023-04-07 15:35:45.681095 dcicsnovault-8.0.1.0b0/snovault/elasticsearch/create_mapping.py
+-rw-r--r--   0        0        0     7939 2023-02-08 18:10:49.846547 dcicsnovault-8.0.1.0b0/snovault/elasticsearch/es_index_listener.py
+-rw-r--r--   0        0        0    18572 2023-02-08 18:10:49.851730 dcicsnovault-8.0.1.0b0/snovault/elasticsearch/esstorage.py
+-rw-r--r--   0        0        0    24405 2023-04-10 19:15:16.612559 dcicsnovault-8.0.1.0b0/snovault/elasticsearch/indexer.py
+-rw-r--r--   0        0        0    31356 2023-02-08 18:10:49.863845 dcicsnovault-8.0.1.0b0/snovault/elasticsearch/indexer_queue.py
+-rw-r--r--   0        0        0    20947 2023-02-08 18:10:49.871835 dcicsnovault-8.0.1.0b0/snovault/elasticsearch/indexer_utils.py
+-rw-r--r--   0        0        0      349 2021-08-12 19:39:17.751212 dcicsnovault-8.0.1.0b0/snovault/elasticsearch/interfaces.py
+-rw-r--r--   0        0        0    10190 2023-04-10 19:15:16.619476 dcicsnovault-8.0.1.0b0/snovault/elasticsearch/mpindexer.py
+-rw-r--r--   0        0        0     8249 2021-08-12 19:39:17.757097 dcicsnovault-8.0.1.0b0/snovault/embed.py
+-rw-r--r--   0        0        0     1061 2023-02-08 18:10:49.878124 dcicsnovault-8.0.1.0b0/snovault/etag.py
+-rw-r--r--   0        0        0    10835 2023-02-08 18:10:49.886932 dcicsnovault-8.0.1.0b0/snovault/indexing_views.py
+-rw-r--r--   0        0        0      774 2020-04-22 15:19:59.962133 dcicsnovault-8.0.1.0b0/snovault/interfaces.py
+-rw-r--r--   0        0        0     2229 2023-02-08 18:10:49.892547 dcicsnovault-8.0.1.0b0/snovault/invalidation.py
+-rw-r--r--   0        0        0     1639 2023-02-08 18:10:49.897621 dcicsnovault-8.0.1.0b0/snovault/json_renderer.py
+-rw-r--r--   0        0        0     2292 2020-09-15 14:05:58.093412 dcicsnovault-8.0.1.0b0/snovault/jsongraph.py
+-rw-r--r--   0        0        0     9713 2023-02-08 18:10:49.904627 dcicsnovault-8.0.1.0b0/snovault/jsonld_context.py
+-rw-r--r--   0        0        0    30294 2023-04-10 19:15:18.843268 dcicsnovault-8.0.1.0b0/snovault/loadxl.py
+-rw-r--r--   0        0        0     2425 2023-04-10 19:15:18.848768 dcicsnovault-8.0.1.0b0/snovault/memlimit.py
+-rw-r--r--   0        0        0     1165 2023-04-10 19:15:18.854745 dcicsnovault-8.0.1.0b0/snovault/parallel.py
+-rw-r--r--   0        0        0      846 2020-04-22 15:19:59.956023 dcicsnovault-8.0.1.0b0/snovault/predicates.py
+-rw-r--r--   0        0        0       95 2023-04-10 19:15:16.625324 dcicsnovault-8.0.1.0b0/snovault/redis/README.rst
+-rw-r--r--   0        0        0       90 2023-04-10 19:15:16.630313 dcicsnovault-8.0.1.0b0/snovault/redis/__init__.py
+-rw-r--r--   0        0        0       16 2023-04-10 19:15:16.635178 dcicsnovault-8.0.1.0b0/snovault/redis/interfaces.py
+-rw-r--r--   0        0        0     4106 2023-04-10 19:15:16.640462 dcicsnovault-8.0.1.0b0/snovault/redis/redis_connection.py
+-rw-r--r--   0        0        0    22128 2023-04-10 19:15:18.861451 dcicsnovault-8.0.1.0b0/snovault/renderers.py
+-rw-r--r--   0        0        0    11201 2023-02-08 18:10:49.914597 dcicsnovault-8.0.1.0b0/snovault/resource_views.py
+-rw-r--r--   0        0        0    21863 2023-04-10 19:15:16.646344 dcicsnovault-8.0.1.0b0/snovault/resources.py
+-rw-r--r--   0        0        0     3450 2023-02-08 18:10:49.920477 dcicsnovault-8.0.1.0b0/snovault/schema_graph.py
+-rw-r--r--   0        0        0    14162 2023-04-10 19:15:18.867518 dcicsnovault-8.0.1.0b0/snovault/schema_utils.py
+-rw-r--r--   0        0        0     4358 2023-04-10 19:15:18.873112 dcicsnovault-8.0.1.0b0/snovault/schema_views.py
+-rw-r--r--   0        0        0     1855 2023-04-12 15:13:35.702783 dcicsnovault-8.0.1.0b0/snovault/schemas/access_key.json
+-rw-r--r--   0        0        0     5098 2023-04-10 19:15:18.881989 dcicsnovault-8.0.1.0b0/snovault/schemas/filter_set.json
+-rw-r--r--   0        0        0    18744 2023-04-10 19:15:18.887742 dcicsnovault-8.0.1.0b0/snovault/schemas/mixins.json
+-rw-r--r--   0        0        0    19600 2023-04-10 19:15:18.893767 dcicsnovault-8.0.1.0b0/snovault/schemas/user.json
+-rw-r--r--   0        0        0    20952 2023-04-10 19:15:18.900179 dcicsnovault-8.0.1.0b0/snovault/search/compound_search.py
+-rw-r--r--   0        0        0    58595 2023-04-10 19:15:18.906948 dcicsnovault-8.0.1.0b0/snovault/search/lucene_builder.py
+-rw-r--r--   0        0        0    62789 2023-04-10 19:15:18.913908 dcicsnovault-8.0.1.0b0/snovault/search/search.py
+-rw-r--r--   0        0        0    17901 2023-04-10 19:15:18.923487 dcicsnovault-8.0.1.0b0/snovault/search/search_utils.py
+-rw-r--r--   0        0        0     4541 2023-04-10 19:15:18.929481 dcicsnovault-8.0.1.0b0/snovault/server_defaults.py
+-rw-r--r--   0        0        0      522 2023-02-08 18:10:49.926443 dcicsnovault-8.0.1.0b0/snovault/settings.py
+-rw-r--r--   0        0        0     1498 2021-08-12 19:39:17.787731 dcicsnovault-8.0.1.0b0/snovault/standalone_dev.py
+-rw-r--r--   0        0        0     4383 2023-02-08 18:10:49.931408 dcicsnovault-8.0.1.0b0/snovault/stats.py
+-rw-r--r--   0        0        0    34834 2023-04-10 19:15:20.635570 dcicsnovault-8.0.1.0b0/snovault/storage.py
+-rw-r--r--   0        0        0      330 2020-04-22 15:19:59.941685 dcicsnovault-8.0.1.0b0/snovault/test_schemas/AbstractItemTestSecondSubItem.json
+-rw-r--r--   0        0        0      300 2020-04-22 15:19:59.940748 dcicsnovault-8.0.1.0b0/snovault/test_schemas/AbstractItemTestSubItem.json
+-rw-r--r--   0        0        0     2467 2023-02-08 18:10:49.937350 dcicsnovault-8.0.1.0b0/snovault/test_schemas/EmbeddingTest.json
+-rw-r--r--   0        0        0      446 2021-08-12 19:39:17.798764 dcicsnovault-8.0.1.0b0/snovault/test_schemas/NestedEmbeddingContainer.json
+-rw-r--r--   0        0        0      883 2021-08-12 19:39:17.803883 dcicsnovault-8.0.1.0b0/snovault/test_schemas/NestedObjectLinkTarget.json
+-rw-r--r--   0        0        0      473 2021-08-12 19:39:17.810025 dcicsnovault-8.0.1.0b0/snovault/test_schemas/TestingBiogroupSno.json
+-rw-r--r--   0        0        0      968 2023-02-08 18:10:49.943722 dcicsnovault-8.0.1.0b0/snovault/test_schemas/TestingBiosampleSno.json
+-rw-r--r--   0        0        0     1082 2021-08-12 19:39:17.820805 dcicsnovault-8.0.1.0b0/snovault/test_schemas/TestingBiosourceSno.json
+-rw-r--r--   0        0        0      894 2020-09-25 18:48:35.851983 dcicsnovault-8.0.1.0b0/snovault/test_schemas/TestingCalculatedProperties.json
+-rw-r--r--   0        0        0      276 2020-04-22 15:19:59.938605 dcicsnovault-8.0.1.0b0/snovault/test_schemas/TestingDependencies.json
+-rw-r--r--   0        0        0      697 2023-04-10 19:15:18.936475 dcicsnovault-8.0.1.0b0/snovault/test_schemas/TestingDownload.json
+-rw-r--r--   0        0        0      555 2021-08-12 19:39:17.826025 dcicsnovault-8.0.1.0b0/snovault/test_schemas/TestingIndividualSno.json
+-rw-r--r--   0        0        0      730 2020-04-22 15:19:59.936694 dcicsnovault-8.0.1.0b0/snovault/test_schemas/TestingLinkAggregateSno.json
+-rw-r--r--   0        0        0      697 2021-08-12 19:39:17.831918 dcicsnovault-8.0.1.0b0/snovault/test_schemas/TestingLinkSourceSno.json
+-rw-r--r--   0        0        0      472 2021-08-12 19:39:17.838406 dcicsnovault-8.0.1.0b0/snovault/test_schemas/TestingLinkTargetElasticSearch.json
+-rw-r--r--   0        0        0      292 2020-04-22 15:19:59.934939 dcicsnovault-8.0.1.0b0/snovault/test_schemas/TestingLinkTargetSno.json
+-rw-r--r--   0        0        0      311 2023-04-10 18:54:40.455623 dcicsnovault-8.0.1.0b0/snovault/test_schemas/TestingMixins.json
+-rw-r--r--   0        0        0      845 2021-08-12 19:39:18.009063 dcicsnovault-8.0.1.0b0/snovault/test_schemas/TestingNestedEnabled.json
+-rw-r--r--   0        0        0     3721 2023-02-08 18:10:49.949847 dcicsnovault-8.0.1.0b0/snovault/test_schemas/TestingNoteSno.json
+-rw-r--r--   0        0        0     1622 2021-08-12 19:39:17.850333 dcicsnovault-8.0.1.0b0/snovault/test_schemas/TestingPostPutPatchSno.json
+-rw-r--r--   0        0        0      576 2020-04-22 15:19:59.932932 dcicsnovault-8.0.1.0b0/snovault/test_schemas/TestingServerDefault.json
+-rw-r--r--   0        0        0     1215 2023-04-10 19:15:18.938054 dcicsnovault-8.0.1.0b0/snovault/test_schemas/mixins.json
+-rw-r--r--   0        0        0        0 2023-03-31 18:39:46.436489 dcicsnovault-8.0.1.0b0/snovault/tests/__init__.py
+-rw-r--r--   0        0        0     2210 2023-04-10 19:15:16.653133 dcicsnovault-8.0.1.0b0/snovault/tests/conftest.py
+-rw-r--r--   0        0        0      100 2023-02-08 18:10:49.952678 dcicsnovault-8.0.1.0b0/snovault/tests/conftest_settings.py
+-rw-r--r--   0        0        0     3086 2023-02-08 18:10:49.957620 dcicsnovault-8.0.1.0b0/snovault/tests/elasticsearch_fixture.py
+-rw-r--r--   0        0        0     3921 2020-09-15 14:05:58.160270 dcicsnovault-8.0.1.0b0/snovault/tests/postgresql_fixture.py
+-rw-r--r--   0        0        0      852 2023-04-10 19:15:16.658135 dcicsnovault-8.0.1.0b0/snovault/tests/pyramidfixtures.py
+-rw-r--r--   0        0        0     3007 2020-09-15 14:05:58.161510 dcicsnovault-8.0.1.0b0/snovault/tests/root.py
+-rw-r--r--   0        0        0    17313 2023-04-10 19:15:18.943657 dcicsnovault-8.0.1.0b0/snovault/tests/serverfixtures.py
+-rw-r--r--   0        0        0    20332 2023-04-10 19:15:20.636889 dcicsnovault-8.0.1.0b0/snovault/tests/test_attachment.py
+-rw-r--r--   0        0        0     3937 2023-04-12 18:08:29.011696 dcicsnovault-8.0.1.0b0/snovault/tests/test_authentication.py
+-rw-r--r--   0        0        0     1370 2021-08-12 19:39:17.883512 dcicsnovault-8.0.1.0b0/snovault/tests/test_calculated.py
+-rw-r--r--   0        0        0    15979 2023-04-10 19:15:18.956210 dcicsnovault-8.0.1.0b0/snovault/tests/test_clear_db_es_contents.py
+-rw-r--r--   0        0        0     8984 2023-02-08 18:10:49.975775 dcicsnovault-8.0.1.0b0/snovault/tests/test_create_mapping.py
+-rw-r--r--   0        0        0     3173 2023-04-13 14:15:18.241821 dcicsnovault-8.0.1.0b0/snovault/tests/test_drs.py
+-rw-r--r--   0        0        0      528 2023-04-10 19:15:18.963682 dcicsnovault-8.0.1.0b0/snovault/tests/test_edw_hash.py
+-rw-r--r--   0        0        0     7493 2023-04-10 19:17:54.481828 dcicsnovault-8.0.1.0b0/snovault/tests/test_embed_utils.py
+-rw-r--r--   0        0        0     8823 2023-03-13 18:29:27.181151 dcicsnovault-8.0.1.0b0/snovault/tests/test_embedding.py
+-rw-r--r--   0        0        0    10024 2020-04-22 15:19:59.916562 dcicsnovault-8.0.1.0b0/snovault/tests/test_es_permissions.py
+-rw-r--r--   0        0        0   115140 2023-04-10 19:18:26.571266 dcicsnovault-8.0.1.0b0/snovault/tests/test_indexing.py
+-rw-r--r--   0        0        0    28258 2023-02-08 18:10:49.984723 dcicsnovault-8.0.1.0b0/snovault/tests/test_invalidation_scope.py
+-rw-r--r--   0        0        0     1808 2023-04-10 19:15:18.977778 dcicsnovault-8.0.1.0b0/snovault/tests/test_key.py
+-rw-r--r--   0        0        0     2458 2020-04-22 15:19:59.908101 dcicsnovault-8.0.1.0b0/snovault/tests/test_link.py
+-rw-r--r--   0        0        0     5316 2023-02-08 18:10:49.991255 dcicsnovault-8.0.1.0b0/snovault/tests/test_logging.py
+-rw-r--r--   0        0        0     1134 2023-03-13 18:29:27.182699 dcicsnovault-8.0.1.0b0/snovault/tests/test_misc.py
+-rw-r--r--   0        0        0      373 2020-09-25 18:48:35.895147 dcicsnovault-8.0.1.0b0/snovault/tests/test_mixins.py
+-rw-r--r--   0        0        0    13660 2023-02-08 18:10:49.997635 dcicsnovault-8.0.1.0b0/snovault/tests/test_post_put_patch.py
+-rw-r--r--   0        0        0     1570 2023-02-08 18:10:50.005697 dcicsnovault-8.0.1.0b0/snovault/tests/test_postgresql_fixture.py
+-rw-r--r--   0        0        0     1194 2021-08-12 19:39:17.921857 dcicsnovault-8.0.1.0b0/snovault/tests/test_schemas.py
+-rw-r--r--   0        0        0      952 2023-02-08 18:10:50.011548 dcicsnovault-8.0.1.0b0/snovault/tests/test_serverfixtures.py
+-rw-r--r--   0        0        0     4267 2021-08-12 19:39:17.928403 dcicsnovault-8.0.1.0b0/snovault/tests/test_standalone_dev.py
+-rw-r--r--   0        0        0     2211 2023-02-08 18:10:50.016544 dcicsnovault-8.0.1.0b0/snovault/tests/test_stats.py
+-rw-r--r--   0        0        0    13182 2023-04-10 19:15:20.639545 dcicsnovault-8.0.1.0b0/snovault/tests/test_storage.py
+-rw-r--r--   0        0        0     6782 2023-04-10 19:15:18.984951 dcicsnovault-8.0.1.0b0/snovault/tests/test_types_access_key.py
+-rw-r--r--   0        0        0     1291 2020-04-22 15:19:59.901514 dcicsnovault-8.0.1.0b0/snovault/tests/test_upgrader.py
+-rw-r--r--   0        0        0     6635 2023-02-08 18:10:50.017803 dcicsnovault-8.0.1.0b0/snovault/tests/test_util.py
+-rw-r--r--   0        0        0    18612 2023-02-08 18:10:50.023759 dcicsnovault-8.0.1.0b0/snovault/tests/test_views.py
+-rw-r--r--   0        0        0     4578 2023-04-10 19:15:18.986928 dcicsnovault-8.0.1.0b0/snovault/tests/testappfixtures.py
+-rw-r--r--   0        0        0      677 2020-09-15 14:05:58.215585 dcicsnovault-8.0.1.0b0/snovault/tests/testing_upgrader.py
+-rw-r--r--   0        0        0    34107 2023-04-13 14:14:38.777790 dcicsnovault-8.0.1.0b0/snovault/tests/testing_views.py
+-rw-r--r--   0        0        0     1342 2020-09-15 14:05:58.228484 dcicsnovault-8.0.1.0b0/snovault/tests/toolfixtures.py
+-rw-r--r--   0        0        0     4031 2023-04-07 15:35:45.690459 dcicsnovault-8.0.1.0b0/snovault/tools.py
+-rw-r--r--   0        0        0     1807 2023-04-10 19:15:19.001310 dcicsnovault-8.0.1.0b0/snovault/typedsheets.py
+-rw-r--r--   0        0        0     7605 2021-08-12 19:39:17.963916 dcicsnovault-8.0.1.0b0/snovault/typeinfo.py
+-rw-r--r--   0        0        0       70 2023-04-10 19:15:19.007462 dcicsnovault-8.0.1.0b0/snovault/types/__init__.py
+-rw-r--r--   0        0        0     5101 2023-04-10 19:15:19.012443 dcicsnovault-8.0.1.0b0/snovault/types/access_key.py
+-rw-r--r--   0        0        0    16288 2023-04-10 19:15:19.017711 dcicsnovault-8.0.1.0b0/snovault/types/base.py
+-rw-r--r--   0        0        0      738 2023-04-10 19:15:19.023321 dcicsnovault-8.0.1.0b0/snovault/types/filter_set.py
+-rw-r--r--   0        0        0     5536 2023-04-10 19:15:19.028682 dcicsnovault-8.0.1.0b0/snovault/types/user.py
+-rw-r--r--   0        0        0     8124 2023-02-08 18:10:50.037173 dcicsnovault-8.0.1.0b0/snovault/upgrader.py
+-rw-r--r--   0        0        0    50126 2023-04-10 19:15:19.035305 dcicsnovault-8.0.1.0b0/snovault/util.py
+-rw-r--r--   0        0        0     5460 2023-02-08 18:10:50.039101 dcicsnovault-8.0.1.0b0/snovault/validation.py
+-rw-r--r--   0        0        0     5718 2023-02-08 18:10:50.044485 dcicsnovault-8.0.1.0b0/snovault/validators.py
+-rw-r--r--   0        0        0     8848 1970-01-01 00:00:00.000000 dcicsnovault-8.0.1.0b0/setup.py
+-rw-r--r--   0        0        0     9135 1970-01-01 00:00:00.000000 dcicsnovault-8.0.1.0b0/PKG-INFO
```

### Comparing `dcicsnovault-8.0.1/LICENSE.txt` & `dcicsnovault-8.0.1.0b0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/README.rst` & `dcicsnovault-8.0.1.0b0/README.rst`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/pyproject.toml` & `dcicsnovault-8.0.1.0b0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dcicsnovault"
-version = "8.0.1"
+version = "8.0.1.0b0"  # to become 8.1.0
 description = "Storage support for 4DN Data Portals."
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/4dn-dcic/snovault"
 repository = "https://github.com/4dn-dcic/snovault"
 documentation = "https://github.com/4dn-dcic/snovault"
@@ -31,15 +31,15 @@
     # Specify the Python versions you support here. In particular, ensure
     # that you indicate whether you support Python 2, Python 3 or both.
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3.8',
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.8.1,<3.9"
+python = ">=3.8.1,<3.10"
 aws_requests_auth = "^0.4.1"
 # TODO: This is a backport of Python's statistics library for versions earlier than Python 3.4,
 #       so may no longer be needed. Something to investigate later. -kmp 20-Feb-2020
 # "backports.statistics" = "0.1.0"
 botocore = ">=1.27.36"  # no particular version required, but this speeds up search
 boto3 = ">=1.24.36"  # no particular version required, but this speeds up search
 elasticsearch = "7.13.4"  # versions >= 7.14.0 lock out AWS ES
@@ -79,14 +79,15 @@
 WebOb = "^1.8.7"
 WebTest = "^2.0.35"
 WSGIProxy2 = "0.4.2"
 xlrd = "^1.0.0"
 "zope.deprecation" = "^4.4.0"
 "zope.interface" = ">=4.7.2,<6"
 "zope.sqlalchemy" = "1.6"
+pyjwt = "^2.6.0"
 pytest-redis = "^2.0.0"
 redis = "^4.5.1"
 
 [tool.poetry.dev-dependencies]
 botocore-stubs = ">=1.27.36"  # no particular version required, but this speeds up search
 boto3-stubs = ">=1.24.36"  # no particular version required, but this speeds up search
 coverage = ">=6.2"
```

### Comparing `dcicsnovault-8.0.1/snovault/__init__.py` & `dcicsnovault-8.0.1.0b0/snovault/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,29 +17,33 @@
 from .schema_utils import load_schema  # noqa
 from .upgrader import upgrade_step  # noqa
 
 
 def includeme(config):
     config.include('pyramid_retry')
     config.include('pyramid_tm')
+    config.include('.authentication')
     config.include('.util')
+    config.include('.drs')
     config.include('.stats')
     config.include('.batchupgrade')
     config.include('.calculated')
     config.include('.config')
     config.include('.connection')
+    config.include('.custom_embed')
     config.include('.embed')
     config.include('.json_renderer')
     config.include('.validation')
     config.include('.predicates')
     config.include('.invalidation')
     config.include('.upgrader')
     config.include('.aggregated_items')
     config.include('.storage')
     config.include('.typeinfo')
+    config.include('.types')
     config.include('.resources')
     config.include('.attachment')
     config.include('.schema_graph')
     config.include('.jsonld_context')
     config.include('.schema_views')
     config.include('.crud_views')
     config.include('.indexing_views')
@@ -79,21 +83,22 @@
 
     config.include(configure_dbsession)
     config.include('snovault')
     config.commit()  # commit so search can override listing
 
     config.include('.renderers')
 
+    if settings.get('elasticsearch.server'):
+        config.include('snovault.search.search')
+        config.include('snovault.search.compound_search')
+
     # only include this stuff if we're testing
     if asbool(settings.get('testing', False)):
         config.include('snovault.tests.testing_views')
-        config.include('snovault.tests.authentication')
         config.include('snovault.tests.root')
-        if settings.get('elasticsearch.server'):
-            config.include('snovault.tests.search')
 
         # in addition, enable invalidation scope for testing - but NOT by default
         settings[INVALIDATION_SCOPE_ENABLED] = True
 
     if 'elasticsearch.server' in config.registry.settings:
         config.include('snovault.elasticsearch')
```

### Comparing `dcicsnovault-8.0.1/snovault/aggregated_items.py` & `dcicsnovault-8.0.1.0b0/snovault/aggregated_items.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/app.py` & `dcicsnovault-8.0.1.0b0/snovault/app.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/attachment.py` & `dcicsnovault-8.0.1.0b0/snovault/attachment.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/batchupgrade.py` & `dcicsnovault-8.0.1.0b0/snovault/batchupgrade.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/cache.py` & `dcicsnovault-8.0.1.0b0/snovault/cache.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/calculated.py` & `dcicsnovault-8.0.1.0b0/snovault/calculated.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/commands/check_rendering.py` & `dcicsnovault-8.0.1.0b0/snovault/commands/check_rendering.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/commands/es_index_data.py` & `dcicsnovault-8.0.1.0b0/snovault/commands/es_index_data.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/commands/jsonld_rdf.py` & `dcicsnovault-8.0.1.0b0/snovault/commands/jsonld_rdf.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/commands/profile.py` & `dcicsnovault-8.0.1.0b0/snovault/commands/profile.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/commands/wipe_test_indices.py` & `dcicsnovault-8.0.1.0b0/snovault/commands/wipe_test_indices.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/config.py` & `dcicsnovault-8.0.1.0b0/snovault/config.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/connection.py` & `dcicsnovault-8.0.1.0b0/snovault/connection.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/crud_views.py` & `dcicsnovault-8.0.1.0b0/snovault/crud_views.py`

 * *Files 2% similar despite different names*

```diff
@@ -263,16 +263,16 @@
     """
     item_uuid = str(context.uuid)
     links = request.registry[STORAGE].find_uuids_linked_to_item(item_uuid)
     request.response.status = 200
     result = {
         'status': 'success',
         '@type': ['result'],
-        'display_title': 'Links to %s' % item_uuid,
-        'notification' : '%s has %s items linking to it. This may include rev_links if status != deleted' % (item_uuid, len(links)),
+        'display_title': f'Links to {item_uuid}',
+        'notification': f'{item_uuid} has {len(links)} items linking to it. This may include rev_links if status != deleted',
         'uuids_linking_to': links
     }
     return result
 
 
 @view_config(context=Item, permission='edit', request_method='DELETE')
 @debug_log
@@ -285,49 +285,48 @@
     To purge, use ?purge=true query string
     For example: DELETE `/<item-type>/<uuid>?purge=true`
     """
     # possibly temporary fix to check if user is admin
     if hasattr(request, 'user_info'):
         user_details = request.user_info.get('details', {})
     else:
-        if 'group.admin' in request.effective_principals:
-            user_details = {'groups': 'admin'}  # you can do it
-        else:
-            user_details = {}  # you cannot
+        # used to check for admin here, now done in user_info above
+        # note that hasattr() results in a function call when referring to an @property
+        user_details = {}
     if 'admin' not in user_details.get('groups', []):
         msg = u'Must be admin to fully delete items.'
         raise ValidationFailure('body', ['userid'], msg)
 
     purge_from_database = asbool(request.GET and request.GET.get('purge'))
     uuid = str(context.uuid)
     if purge_from_database:
         # Delete entirely - WARNING USE WITH CAUTION - DELETES PERMANENTLY
         # checking of item status and links is done within purge_item()
         result = purge_item(context, request)
         if result:
             return {
                 'status': 'success',
                 '@type': ['result'],
-                'notification' : 'Permanently deleted ' + uuid,
+                'notification': f'Permanently deleted {uuid}',
                 '@graph': [uuid]
             }
     else:
         result = delete_item(context, request)
         if result:
             return {
                 'status': 'success',
                 '@type': ['result'],
-                'notification' : 'Set status of ' + uuid + ' to deleted',
-                '@graph': [ render_item(request, context, render) ]
+                'notification': f'Set status of {uuid} to deleted',
+                '@graph': [render_item(request, context, render)]
             }
 
     return {
         'status': 'failure',
         '@type': ['result'],
-        'notification' : 'Deletion failed',
+        'notification': 'Deletion failed',
         '@graph': [uuid]
     }
 
 
 @view_config(context=Item, permission='view', request_method='GET',
              name='validation-errors')
 @debug_log
```

### Comparing `dcicsnovault-8.0.1/snovault/elasticsearch/__init__.py` & `dcicsnovault-8.0.1.0b0/snovault/elasticsearch/__init__.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/elasticsearch/cached_views.py` & `dcicsnovault-8.0.1.0b0/snovault/elasticsearch/cached_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/elasticsearch/create_mapping.py` & `dcicsnovault-8.0.1.0b0/snovault/elasticsearch/create_mapping.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/elasticsearch/es_index_listener.py` & `dcicsnovault-8.0.1.0b0/snovault/elasticsearch/es_index_listener.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/elasticsearch/esstorage.py` & `dcicsnovault-8.0.1.0b0/snovault/elasticsearch/esstorage.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/elasticsearch/indexer.py` & `dcicsnovault-8.0.1.0b0/snovault/elasticsearch/indexer.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/elasticsearch/indexer_queue.py` & `dcicsnovault-8.0.1.0b0/snovault/elasticsearch/indexer_queue.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/elasticsearch/indexer_utils.py` & `dcicsnovault-8.0.1.0b0/snovault/elasticsearch/indexer_utils.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/elasticsearch/mpindexer.py` & `dcicsnovault-8.0.1.0b0/snovault/elasticsearch/mpindexer.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/embed.py` & `dcicsnovault-8.0.1.0b0/snovault/embed.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/etag.py` & `dcicsnovault-8.0.1.0b0/snovault/etag.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/indexing_views.py` & `dcicsnovault-8.0.1.0b0/snovault/indexing_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/interfaces.py` & `dcicsnovault-8.0.1.0b0/snovault/interfaces.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/invalidation.py` & `dcicsnovault-8.0.1.0b0/snovault/invalidation.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/json_renderer.py` & `dcicsnovault-8.0.1.0b0/snovault/json_renderer.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/jsongraph.py` & `dcicsnovault-8.0.1.0b0/snovault/jsongraph.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/jsonld_context.py` & `dcicsnovault-8.0.1.0b0/snovault/jsonld_context.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/predicates.py` & `dcicsnovault-8.0.1.0b0/snovault/predicates.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/redis/redis_connection.py` & `dcicsnovault-8.0.1.0b0/snovault/redis/redis_connection.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/resource_views.py` & `dcicsnovault-8.0.1.0b0/snovault/resource_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/resources.py` & `dcicsnovault-8.0.1.0b0/snovault/resources.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/schema_graph.py` & `dcicsnovault-8.0.1.0b0/snovault/schema_graph.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/schema_utils.py` & `dcicsnovault-8.0.1.0b0/snovault/schema_utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 import codecs
 import collections
 import uuid
 import json
-import requests
 
 from datetime import datetime
 from dcicutils.misc_utils import ignored
 from jsonschema_serialize_fork import (
     Draft4Validator,
     FormatChecker,
     RefResolver,
 )
-# TODO (C4-177): remove these imports (urlsplit, urlopen) when RefResolverOrdered is removed
-from jsonschema_serialize_fork.compat import urlsplit, urlopen
 from jsonschema_serialize_fork.exceptions import ValidationError
 from pyramid.path import AssetResolver, caller_package
 from pyramid.threadlocal import get_current_request
 from pyramid.traversal import find_resource
 from uuid import UUID
 from .util import ensurelist
 
@@ -28,70 +25,15 @@
 SERVER_DEFAULTS = {}
 
 
 def server_default(func):
     SERVER_DEFAULTS[func.__name__] = func
 
 
-class RefResolverOrdered(RefResolver):
-    """
-    Overwrite the resolve_remote method in the RefResolver class, written
-    by lrowe. See:
-    https://github.com/lrowe/jsonschema_serialize_fork/blob/master/jsonschema_serialize_fork/validators.py
-    With python <3.6, json.loads was losing schema order for properties, facets,
-    and columns. Pass in the object_pairs_hook=collections.OrderedDict
-    argument to fix this.
-    WHEN ELASTICBEANSTALK IS RUNNING PY 3.6 WE CAN REMOVE THIS
-    """
-    # TODO (C4-177): The stated condition is now met. We are reliably in Python 3.6, so this code should be removed.
-
-    def resolve_remote(self, uri):
-        """
-        Resolve a remote ``uri``.
-        Does not check the store first, but stores the retrieved document in
-        the store if :attr:`RefResolver.cache_remote` is True.
-        .. note::
-            If the requests_ library is present, ``jsonschema`` will use it to
-            request the remote ``uri``, so that the correct encoding is
-            detected and used.
-            If it isn't, or if the scheme of the ``uri`` is not ``http`` or
-            ``https``, UTF-8 is assumed.
-        :argument str uri: the URI to resolve
-        :returns: the retrieved document
-        .. _requests: http://pypi.python.org/pypi/requests/
-        """
-        scheme = urlsplit(uri).scheme
-
-        if scheme in self.handlers:
-            result = self.handlers[scheme](uri)
-        elif (
-            scheme in ["http", "https"] and
-            # TODO (C4-177): PyCharm flagged free references to 'requests' in this file as undefined,
-            #                so I've added an import at top of file. However, that suggests this 'elif'
-            #                branch is never entered. When this tangled code is removed, I'll be happier.
-            #                Meanwhile having a definition seems safer than not. -kmp 9-Jun-2020
-            requests and
-            getattr(requests.Response, "json", None) is not None
-        ):
-            # Requests has support for detecting the correct encoding of
-            # json over http
-            if callable(requests.Response.json):
-                result = collections.OrderedDict(requests.get(uri).json())
-            else:
-                result = collections.OrderedDict(requests.get(uri).json)
-        else:
-            # Otherwise, pass off to urllib and assume utf-8
-            result = json.loads(urlopen(uri).read().decode("utf-8"), object_pairs_hook=collections.OrderedDict)
-
-        if self.cache_remote:
-            self.store[uri] = result
-        return result
-
-
-class NoRemoteResolver(RefResolverOrdered):
+class NoRemoteResolver(RefResolver):
     def resolve_remote(self, uri):
         raise ValueError('Resolution disallowed for: %s' % uri)
 
 
 def mixinSchemas(schema, resolver, key_name='properties'):
     mixinKeyName = 'mixin' + key_name.capitalize()
     mixins = schema.get(mixinKeyName)
@@ -282,15 +224,15 @@
         schema = filename
         resolver = NoRemoteResolver.from_schema(schema)
     else:
         utf8 = codecs.getreader("utf-8")
         asset = AssetResolver(caller_package()).resolve(filename)
         schema = json.load(utf8(asset.stream()),
                            object_pairs_hook=collections.OrderedDict)
-        resolver = RefResolverOrdered('file://' + asset.abspath(), schema)
+        resolver = RefResolver('file://' + asset.abspath(), schema)
     # use mixinProperties, mixinFacets, mixinAggregations, and mixinColumns (if provided)
     schema = mixinSchemas(
         mixinSchemas(
             mixinSchemas(mixinSchemas(schema, resolver, 'properties'), resolver, 'facets'),
             resolver,
             'aggregations'
         ),
```

### Comparing `dcicsnovault-8.0.1/snovault/schema_views.py` & `dcicsnovault-8.0.1.0b0/snovault/schema_views.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     """
     schema = type_info.schema.copy()
     schema['@type'] = ['JSONSchema']
     jsonld_base = request.registry.settings['snovault.jsonld.terms_namespace']
     schema['rdfs:seeAlso'] = urlparse(jsonld_base).path + type_info.name
     # add links to profiles of children schemas
     schema['children'] = [
-        '/profiles/' +  t_name + '.json' for t_name in type_info.child_types
+        '/profiles/' + t_name + '.json' for t_name in type_info.child_types
     ]
 
     if type_info.factory is None:
         return schema
 
     # use first base_type that is not this type itself to handle abstract
     found_subtype = None
```

### Comparing `dcicsnovault-8.0.1/snovault/settings.py` & `dcicsnovault-8.0.1.0b0/snovault/settings.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/standalone_dev.py` & `dcicsnovault-8.0.1.0b0/snovault/standalone_dev.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/stats.py` & `dcicsnovault-8.0.1.0b0/snovault/stats.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/storage.py` & `dcicsnovault-8.0.1.0b0/snovault/storage.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/test_schemas/EmbeddingTest.json` & `dcicsnovault-8.0.1.0b0/snovault/test_schemas/EmbeddingTest.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/test_schemas/NestedObjectLinkTarget.json` & `dcicsnovault-8.0.1.0b0/snovault/test_schemas/NestedObjectLinkTarget.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/test_schemas/TestingBiosampleSno.json` & `dcicsnovault-8.0.1.0b0/snovault/test_schemas/TestingBiosampleSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/test_schemas/TestingBiosourceSno.json` & `dcicsnovault-8.0.1.0b0/snovault/test_schemas/TestingBiosourceSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/test_schemas/TestingCalculatedProperties.json` & `dcicsnovault-8.0.1.0b0/snovault/test_schemas/TestingCalculatedProperties.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/test_schemas/TestingDownload.json` & `dcicsnovault-8.0.1.0b0/snovault/test_schemas/TestingDownload.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6666666666666666%*

 * *Differences: {"'mixinProperties'": "[OrderedDict([('$ref', 'mixins.json#/status')]), OrderedDict([('$ref', "*

 * *                      "'mixins.json#/submitted')])]"}*

```diff
@@ -1,8 +1,16 @@
 {
+    "mixinProperties": [
+        {
+            "$ref": "mixins.json#/status"
+        },
+        {
+            "$ref": "mixins.json#/submitted"
+        }
+    ],
     "properties": {
         "attachment": {
             "attachment": true,
             "properties": {
                 "type": {
                     "enum": [
                         "image/png"
```

### Comparing `dcicsnovault-8.0.1/snovault/test_schemas/TestingIndividualSno.json` & `dcicsnovault-8.0.1.0b0/snovault/test_schemas/TestingIndividualSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/test_schemas/TestingLinkAggregateSno.json` & `dcicsnovault-8.0.1.0b0/snovault/test_schemas/TestingLinkAggregateSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/test_schemas/TestingLinkSourceSno.json` & `dcicsnovault-8.0.1.0b0/snovault/test_schemas/TestingLinkSourceSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/test_schemas/TestingNestedEnabled.json` & `dcicsnovault-8.0.1.0b0/snovault/test_schemas/TestingNestedEnabled.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/test_schemas/TestingNoteSno.json` & `dcicsnovault-8.0.1.0b0/snovault/test_schemas/TestingNoteSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/test_schemas/TestingPostPutPatchSno.json` & `dcicsnovault-8.0.1.0b0/snovault/test_schemas/TestingPostPutPatchSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/test_schemas/TestingServerDefault.json` & `dcicsnovault-8.0.1.0b0/snovault/test_schemas/TestingServerDefault.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/tests/conftest.py` & `dcicsnovault-8.0.1.0b0/snovault/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/tests/elasticsearch_fixture.py` & `dcicsnovault-8.0.1.0b0/snovault/tests/elasticsearch_fixture.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/tests/postgresql_fixture.py` & `dcicsnovault-8.0.1.0b0/snovault/tests/postgresql_fixture.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/tests/pyramidfixtures.py` & `dcicsnovault-8.0.1.0b0/snovault/tests/pyramidfixtures.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/tests/root.py` & `dcicsnovault-8.0.1.0b0/snovault/tests/root.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/tests/search.py` & `dcicsnovault-8.0.1.0b0/snovault/util.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,1435 +1,1185 @@
-import itertools
-import math
-import re
+import contextlib
+import datetime as datetime_module
+import functools
+import json
+import os
 import structlog
-import uuid
+import sys
+import re
 
-from collections import OrderedDict
-from copy import deepcopy
-from dcicutils.misc_utils import ignored
-from elasticsearch import TransportError, RequestError, ConnectionTimeout
-from elasticsearch_dsl import Search
-from pyramid.httpexceptions import HTTPBadRequest
-from pyramid.view import view_config
-from urllib.parse import urlencode
-from webob.multidict import MultiDict
-
-from ..elasticsearch import ELASTIC_SEARCH
-from ..elasticsearch.create_mapping import determine_if_is_date_field
-from ..elasticsearch.indexer_utils import get_namespaced_index
-from ..embed import make_subrequest
-from ..interfaces import TYPES, COLLECTIONS
-from ..resources import AbstractCollection
-from ..typeinfo import AbstractTypeInfo
-from ..util import find_collection_subtypes, crawl_schema
+from copy import copy
+from datetime import datetime, timedelta
+from pyramid.httpexceptions import HTTPForbidden
+from pyramid.threadlocal import manager as threadlocal_manager
 
+from .interfaces import CONNECTION, STORAGE, TYPES
+from .settings import Settings
 
-log = structlog.getLogger(__name__)
 
+log = structlog.getLogger(__name__)
 
-def includeme(config):
-    config.add_route('search', '/search{slash:/?}')
-    config.add_route('browse', '/browse{slash:/?}')
-    config.scan(__name__)
-
-
-sanitize_search_string_re = re.compile(r'[\\\+\-\&\|\!\(\)\{\}\[\]\^\~\:\/\\\*\?]')
-
-
-COMMON_EXCLUDED_URI_PARAMS = [
-    'frame', 'format', 'limit', 'sort', 'from', 'field',
-    'mode', 'redirected_from', 'datastore', 'referrer',
-    'currentAction'
-]
-
-
-@view_config(route_name='search', request_method='GET', permission='search')
-def search(context, request, search_type=None, return_generator=False, forced_type='Search', custom_aggregations=None):
-    """
-    Search view connects to ElasticSearch and returns the results
-    """
-    types = request.registry[TYPES]
-    # list of item types used from the query
-    doc_types = set_doc_types(request, types, search_type)
-    # sets request.normalized_params
-    search_base = normalize_query(request, types, doc_types)
-    # == INITIALIZE RESULT ==
-    result = {
-        '@context': request.route_path('jsonld_context'),
-        '@id': '/' + forced_type.lower() + '/' + search_base,
-        '@type': [forced_type],
-        'title': forced_type,
-        'filters': [],
-        'facets': [],
-        '@graph': [],
-        'notification': '',
-        'sort': {}
-    }
-    principals = request.effective_principals
-    es = request.registry[ELASTIC_SEARCH]
-
-    from_, size = get_pagination(request)
-
-    # get desired frame for this search
-    search_frame = request.normalized_params.get('frame', 'embedded')
-
-    # == PREPARE SEARCH TERM ==
-    prepared_terms = prepare_search_term(request)
-
-    schemas = [types[item_type].schema for item_type in doc_types]
-
-    # set ES index based on doc_type (one type per index)
-    # if doc_type is item, search all indexes by setting es_index to None
-    # If multiple, search all specified
-    namespaced_star = get_namespaced_index(request, '*')
-    if 'Item' in doc_types:
-        es_index = namespaced_star
-    else:
-        es_index = find_index_by_doc_types(request, doc_types, ['Item'])
 
-    # establish elasticsearch_dsl class that will perform the search
-    search = Search(using=es, index=es_index)
+###################
+# Misc. utilities #
+###################
+
+
+# These used to be in create_mapping.py
+# number of shards and replica, currently used for all indices
+NUM_SHARDS = 1
+NUM_REPLICAS = 1
+# memory safeguard; how many documents can be covered by from + size search req
+SEARCH_MAX = 100000
+# ignore above this number of kb when mapping keyword fields
+KW_IGNORE_ABOVE = 512
+# used to customize ngram filter behavior
+MIN_NGRAM = 2
+MAX_NGRAM = 10
+# used to enable nested mapping on array of object fields
+NESTED_ENABLED = 'enable_nested'
+# global index.refresh_interval - currently the default of 1s
+REFRESH_INTERVAL = '1s'
+
+# Schema keys to ignore when finding embeds
+SCHEMA_KEYS_TO_IGNORE_FOR_EMBEDS = {
+    "items", "properties", "additionalProperties", "patternProperties"
+}
 
-    # set up clear_filters path
-    result['clear_filters'] = clear_filters_setup(request, doc_types, forced_type)
 
-    # == SET TYPE FILTERS ==
-    build_type_filters(result, request, doc_types, types)
+class IndexSettings:
+    """ Object wrapping important ElasticSearch index settings. Previously these
+        settings were determined by the constants above, but depending on data model
+        structure and size it can be necessary to tune these.
+
+        number_of_shards: determines how many shards to split each replica into
+                          large collections can benefit from increasing this value
+        number_of_replicas: number of times to replicate the index across the cluster
+                            large collections also benefit from increasing this value,
+                            but note that it has a multiplicative effect on the number
+                            of shards ie: 2 replicas divided into 3 shards results in 6
+                            total shards across the cluster
+        min_ngram: shortest string length to map for string matching or q= searching
+        max_ngram: longest string length to map for string matching or q= searching
+                   the relationship between min and max ngram dictates both the amount of
+                   free text data that is generated and the length of strings that are
+                   indexed - for example min=2 and max=3 would produce ngrams for the word
+                   "sentence" = [se, en, nt, te, en, nc, ce, sen, ent, nte, ten, enc, nce]
+                   note the implications of this structure - if max is too low, terms may
+                   not be long enough to match your important terms, which will affect the
+                   accuracy of search results and may even be misleading to the user
+        refresh_interval: determines how often index refreshes occur - an index refresh is
+                          when a blocking forced update is triggered by the cluster for all
+                          replicas and shards of the index - note that this operation blocks
+                          even if no changes are present in the index, so tuning this value
+                          up from the default may be necessary if we can tolerate indexing
+                          delay for search results, which in many cases we can
+    """
+    def __init__(self, *, shard_count=NUM_SHARDS, replica_count=NUM_REPLICAS,
+                 min_ngram=MIN_NGRAM, max_ngram=MAX_NGRAM, refresh_interval=REFRESH_INTERVAL):
+        self.settings = {
+            'index': {
+                'number_of_shards': shard_count,
+                'number_of_replicas': replica_count,
+                'refresh_interval': refresh_interval,
+                'analysis': {
+                    'filter': {
+                        'ngram_filter': {
+                            'type': 'edgeNGram',
+                            'min_gram': min_ngram,
+                            'max_gram': max_ngram
+                        },
+                        # truncate tokens to size MAX_NGRAM
+                        'truncate_to_ngram': {
+                            'type': 'truncate',
+                            'length': max_ngram
+                        }
+                    }
+                }
+            }
+        }
 
-    # get the fields that will be used as source for the search
-    # currently, supports frame=raw/object but live faceting does not work
-    # this is okay because the only non-embedded access will be programmatic
-    source_fields = sorted(list_source_fields(request, doc_types, search_frame))
 
-    # == GET FILTERED QUERY ==
-    # Builds filtered query which supports multiple facet selection
-    search, string_query = build_query(search, prepared_terms, source_fields)
+@contextlib.contextmanager
+def mappings_use_nested(value=True):
+    """ Context manager that sets the MAPPINGS_USE_NESTED setting with the given value, default True """
+    old_setting = Settings.MAPPINGS_USE_NESTED
+    try:
+        Settings.MAPPINGS_USE_NESTED = value
+        yield
+    finally:
+        Settings.MAPPINGS_USE_NESTED = old_setting
+
+
+class DictionaryKeyError(KeyError):
+
+    def __init__(self, dictionary, key):
+        super(DictionaryKeyError, self).__init__(key)
+        self._dictionary = dictionary
+        self._dictionary_key = key
+
+    def __str__(self):
+        if isinstance(self._dictionary, dict):
+            return "%r has no %r key." % (self._dictionary, self._dictionary_key)
+        else:
+            return "%r is not a dictionary." % self._dictionary
 
-    # == Set sort order ==
-    search = set_sort_order(request, search, prepared_terms, types, doc_types, result)
-    # TODO: implement BOOST here?
 
-    # == Set filters ==
-    search, query_filters = set_filters(request, search, result, principals, doc_types)
+def dictionary_lookup(dictionary, key):
+    """
+    dictionary_lookup(d, k) is the same as d[k] but with more informative error reporting.
+    """
+    if not isinstance(dictionary, dict) or (key not in dictionary):
+        log.error('Got dictionary KeyError with %s and %s' % (dictionary, key))
+        return None
+        # raise DictionaryKeyError(dictionary=dictionary, key=key)  this causes MPIndexer exception - will 3/10/2020
+    else:
+        return dictionary[key]
 
-    # == Set starting facets ==
-    facets = initialize_facets(request, doc_types, prepared_terms, schemas)
 
-    # == Adding facets, plus any optional custom aggregations. ==
-    # Uses 'size' and 'from_' to conditionally skip (no facets if from > 0; no aggs if size > 0).
-    search = set_facets(search, facets, query_filters, string_query, request, doc_types, custom_aggregations, size, from_)
+def deduplicate_list(lst):
+    """ De-duplicates the given list by converting it to a set then back to a list.
 
-    # == Add preference from session, if available ==
-    search_session_id = None
-    if request.__parent__ is None and not return_generator and size != 'all':  # Probably unnecessary, but skip for non-paged, sub-reqs, etc.
-        search_session_id = request.cookies.get('searchSessionID', 'SESSION-' + str(uuid.uuid1()))
-        search = search.params(preference=search_session_id)
+    NOTES:
+    * The list must contain 'hashable' type elements that can be used in sets.
+    * The result list might not be ordered the same as the input list.
+    * This will also take tuples as input, though the result will be a list.
 
-    # == Execute the query ==
-    if size == 'all':
-        es_results = execute_search_for_all_results(search)
-    else:
-        size_search = search[from_:from_ + size]
-        es_results = execute_search(size_search)
+    :param lst: list to de-duplicate
+    :return: de-duplicated list
+    """
+    return list(set(lst))
 
-    # == Record total number of hits ==
-    result['total'] = total = es_results['hits']['total']['value']
-    result['facets'] = format_facets(es_results, facets, total, search_frame)
-    result['aggregations'] = format_extra_aggregations(es_results)
-
-    # Add batch actions
-    # TODO: figure out exactly what this does. Provide download URLs?
-    # Implement later
-    # result.update(search_result_actions(request, doc_types, es_results))
-
-    # == Add all link for collections ==
-    if size not in (None, 'all') and size < result['total']:
-        params = [(k, v) for k, v in request.normalized_params.items() if k != 'limit']
-        params.append(('limit', 'all'))
-        if context:
-            result['all'] = '%s?%s' % (request.resource_path(context), urlencode(params))
-
-    # add actions (namely 'add')
-    result['actions'] = get_collection_actions(request, types[doc_types[0]])
-
-    if not result['total']:
-        # http://googlewebmastercentral.blogspot.com/2014/02/faceted-navigation-best-and-5-of-worst.html
-        request.response.status_code = 404
-        result['notification'] = 'No results found'
-        result['@graph'] = []
-        return result if not return_generator else []
-
-    columns = build_table_columns(request, schemas, doc_types)
-    if columns:
-        result['columns'] = columns
-
-    result['notification'] = 'Success'
-
-    # == Format results for JSON-LD ==
-    graph = format_results(request, es_results['hits']['hits'], search_frame)
-
-    if request.__parent__ is not None or return_generator:
-        if return_generator:
-            return graph
-        else:
-            result['@graph'] = list(graph)
-            return result
 
-    result['@graph'] = list(graph)
-    if search_session_id:  # Is 'None' if e.g. limit=all
-        request.response.set_cookie('searchSessionID', search_session_id)  # Save session ID for re-requests / subsequent pages.
-    return result
+_skip_fields = ['@type', 'principals_allowed']  # globally accessible if need be in the future
 
 
-@view_config(route_name='browse', request_method='GET', permission='search')
-def browse(context, request, search_type='ExperimentSetReplicate', return_generator=False):
+# TODO: This is a priority candidate for unit testing. -kmp 27-Jul-2020
+def filter_embedded(embedded, effective_principals):
     """
-    Simply use search results for browse view
+    Filter the embedded items by principals_allowed, replacing them with
+    a 'no view allowed' error message if the effective principals on the
+    request are disjointed
     """
-    return search(context, request, search_type, return_generator, forced_type='Browse')
+    # handle dictionary
+    if isinstance(embedded, dict):
+        if 'principals_allowed' in embedded.keys():
+            obj_princ = embedded.get('principals_allowed')
+            allowed = set(obj_princ['view'])
+            if allowed.isdisjoint(effective_principals):
+                embedded = {'error': 'no view permissions'}
+                return embedded
 
+        for name, obj in embedded.items():
+            if isinstance(obj, (dict, list)) and name not in _skip_fields:
+                embedded[name] = filter_embedded(obj, effective_principals)
 
-@view_config(context=AbstractCollection, permission='list', request_method='GET')
-def collection_view(context, request):
-    """
-    Simply use search results for collections views (e.g./biosamples/)
-    This is a redirect directly to the search page
-    """
-    return search(context, request, context.type_info.name, False, forced_type='Search')
+    # handle array
+    elif isinstance(embedded, list):
+        for idx, item in enumerate(embedded):
+            embedded[idx] = filter_embedded(item, effective_principals)
 
+    # default just return the sucker
+    return embedded
 
-def get_collection_actions(request, type_info):
-    collection = request.registry[COLLECTIONS].get(type_info.name)
-    if collection and hasattr(collection, 'actions'):
-        return collection.actions(request)
-    else:
-        return None
+
+def debug_log(func):
+    """ Decorator that adds some debug output of the view to log that we got there """
+    @functools.wraps(func)
+    def log_decorator(*args, **kwargs):
+        log_function_call(log, func.__name__)
+        if not args:
+            return func(**kwargs)
+        elif not kwargs:
+            return func(*args)
+        return func(*args, **kwargs)
+    return log_decorator
 
 
-def get_pagination(request):
+def log_function_call(log_ref, func_name, extra=None):
     """
-    Fill from_ and size parameters for search if given in the query string
+    Logs that we have reached func_name in the application
+    Can log 'extra' information as well if specified
+    Helpful in debugging 500 errors on routes and logging entry to any particular function
     """
-    from_ = request.normalized_params.get('from', 0)
-    size = request.normalized_params.get('limit', 25)
-    if size in ('all', ''):
-        size = "all"
-    else:
-        try:
-            size = int(size)
-        except ValueError:
-            size = 25
-        try:
-            from_ = int(from_)
-        except ValueError:
-            size = 0
-    return from_, size
-
-
-def get_all_subsequent_results(initial_search_result, search, extra_requests_needed_count, size_increment):
-    from_ = 0
-    while extra_requests_needed_count > 0:
-        # print(str(extra_requests_needed_count) + " requests left to get all results.")
-        from_ = from_ + size_increment
-        subsequent_search = search[from_:from_ + size_increment]
-        subsequent_search_result = execute_search(subsequent_search)
-        extra_requests_needed_count -= 1
-        for hit in subsequent_search_result['hits'].get('hits', []):
-            yield hit
-
-
-def execute_search_for_all_results(search):
-    size_increment = 100  # Decrease this to like 5 or 10 to test.
-
-    first_search = search[0:size_increment]  # get aggregations from here
-    es_result = execute_search(first_search)
-
-    total_results_expected = es_result['hits'].get('total', 0)
-    extra_requests_needed_count = int(math.ceil(total_results_expected / size_increment)) - 1  # Decrease by 1 (first es_result already happened)
-
-    if extra_requests_needed_count > 0:
-        es_result['hits']['hits'] = itertools.chain(es_result['hits']['hits'], get_all_subsequent_results(es_result, search, extra_requests_needed_count, size_increment))
-    return es_result
-
-
-def normalize_query(request, types, doc_types):
-    """
-    Normalize the query by calculating and setting request.normalized_params
-    (a webob MultiDict) that is derived from custom query rules and also
-    the list of doc_types specified by set_doc_types(). The normalize_param
-    helper function finds field_schema for each query parameter and enforces
-    a set of rules (see below). If the query item types differ from doc_types,
-    override with doc_types
+    log_ref.info('DEBUG_FUNC -- Entering view config: %s' % func_name)
+    if extra:
+        log_ref.info('DEBUG_FUNC -- Extra info: %s' % extra)
 
-    Args:
-        request: the current Request
-        types: registry[TYPES]
-        doc_types (list): item_types to use for the search
 
-    Returns:
-        string: query string built from normalized params
-    """
-    def normalize_param(key, val):
-        """
-        Process each key/val in the original query param. As part of this,
-        obtain the field schema for each parameter.
-        Current rules:
-        - for 'type', get name from types (from the registry)
-        - append '.display_title' to any terminal linkTo query field
-        """
-        # type param is a special case. use the name from TypeInfo
-        if key == 'type' and val in types:
-            return (key, types[val].name)
-
-        # find schema for field parameter and drill down into arrays/subobjects
-        field_schema = schema_for_field(key, request, doc_types)
-        while field_schema and ('items' in field_schema or 'properties' in field_schema):
-            try:
-                field_schema = field_schema['items']
-            except KeyError:
-                pass
-            try:
-                field_schema = field_schema['properties']
-            except KeyError:
-                pass
-        if field_schema and 'linkTo' in field_schema:
-            # add display_title to terminal linkTo query fields
-            if key.endswith('!'):  # handle NOT
-                return (key[:-1] + '.display_title!', val)
-            return (key + '.display_title', val)
+def select_distinct_values(request, value_path, *from_paths):
+    if isinstance(value_path, str):
+        value_path = value_path.split('.')
+
+    values = from_paths
+    for name in value_path:
+        objs = (request.embed(member, '@@object') for member in values)
+        value_lists = (ensurelist(obj.get(name, [])) for obj in objs)
+        values = {value for value_list in value_lists for value in value_list}
+
+    return list(values)
+
+
+def includeme(config):
+    config.add_request_method(select_distinct_values)
+
+
+def get_root_request():
+    if threadlocal_manager.stack:
+        return threadlocal_manager.stack[0]['request']
+
+
+def ensurelist(value):
+    if isinstance(value, str):
+        return [value]
+    return value
+
+
+def uuid_to_path(request, obj, path):
+    if isinstance(path, str):
+        path = path.split('.')
+    if not path:
+        return
+    name = path[0]
+    remaining = path[1:]
+    value = obj.get(name, None)
+    if value is None:
+        return
+    if remaining:
+        if isinstance(value, list):
+            for v in value:
+                uuid_to_path(request, v, remaining)
         else:
-            return (key, val)
+            uuid_to_path(request, value, remaining)
+        return
+    conn = request.registry[CONNECTION]
+    if isinstance(value, list):
+        obj[name] = [
+            request.resource_path(conn[v])
+            for v in value
+        ]
+    else:
+        obj[name] = request.resource_path(conn[value])
 
-    normalized_params = (
-        normalize_param(k, v)
-        for k, v in request.params.items()
-    )
-    # use a MultiDict to emulate request.params
-    normalized_params = MultiDict(normalized_params)
-    # overwrite 'type' if not equal to doc_types
-    if set(normalized_params.getall('type')) != set(doc_types):
-        if 'type' in normalized_params:
-            del normalized_params['type']
-        for dtype in doc_types:
-            normalized_params.add('type', dtype)
-    # add the normalized params to the request
-    # these will be used in place of request.params for the rest of search
-    setattr(request, 'normalized_params', normalized_params)
-    # the query string of the normalized search
-    qs = '?' + urlencode([
-        (k.encode('utf-8'), v.encode('utf-8'))
-        for k, v in request.normalized_params.items()
-    ])
-    return qs
-
-
-def clear_filters_setup(request, doc_types, forced_type):
-    """
-    Clear Filters URI path
-
-    Make a URI path that clears all non-datatype filters
-    and leaves in `q` (search query) params, if present.
-    Also preserves currentAction=selection, if is set.
 
-    Returns:
-        A URL path
-    """
-    seach_query_specs = request.normalized_params.getall('q')
-    seach_query_url = urlencode([("q", seach_query) for seach_query in seach_query_specs])
-    # types_url will always be present (always >=1 doc_type)
-    types_url = urlencode([("type", typ) for typ in doc_types])
-    current_action = request.normalized_params.get('currentAction')
-
-    clear_qs = types_url or ''
-    if seach_query_url:
-        clear_qs += '&' + seach_query_url
-    if current_action == 'selection':
-        clear_qs += '&currentAction=selection'
-    current_search_sort = request.normalized_params.getall('sort')
-    current_search_sort_url = urlencode([("sort", s) for s in current_search_sort])
-    if current_search_sort_url:
-        clear_qs += '&' + current_search_sort_url
-    return request.route_path(forced_type.lower(), slash='/') + (('?' + clear_qs) if clear_qs else '')
+def simple_path_ids(obj, path):
+    if isinstance(path, str):
+        path = path.split('.')
+    if not path:
+        yield obj
+        return
+    name = path[0]
+    remaining = path[1:]
+    value = obj.get(name, None)
+    if value is None:
+        return
+    if not isinstance(value, list):
+        value = [value]
+    for member in value:
+        for result in simple_path_ids(member, remaining):
+            yield result
 
 
-def build_type_filters(result, request, doc_types, types):
+def expand_path(request, obj, path):
     """
-    Set the type filters for the search. If no doc_types, default to Item
+    Used with ?expand=... view. See resource_views.item_view_expand
     """
-    if not doc_types:
-        doc_types = ['Item']
+    if isinstance(path, str):
+        path = path.split('.')
+    if not path:
+        return
+    name = path[0]
+    remaining = path[1:]
+    value = obj.get(name, None)
+    if value is None:
+        return
+    if isinstance(value, list):
+        for index, member in enumerate(value):
+            if not isinstance(member, dict):
+                res = secure_embed(request, member, '@@object')
+                member = value[index] = res
+            expand_path(request, member, remaining)
     else:
-        for item_type in doc_types:
-            ti = types[item_type]
-            qs = urlencode([
-                (k.encode('utf-8'), v.encode('utf-8'))
-                for k, v in request.normalized_params.items() if not (k == 'type' and types.all.get('Item' if v == '*' else v) is ti)
-            ])
-            result['filters'].append({
-                'field': 'type',
-                'term': ti.name,
-                'remove': '{}?{}'.format(request.path, qs)
-            })
-
-
-def prepare_search_term(request):
-    """
-    Prepares search terms by making a dictionary where the keys are fields
-    and the values are arrays of query strings
-    Ignore certain keywords, such as type, format, and field
-    """
-    prepared_terms = {}
-    # prepared_vals = []
-    # In case it helps, I think request.normalized_params is a MultiDict. -kmp 7-Aug-2022
-    for field, val in request.normalized_params.items():  # was .iteritems(), but that went away in Python 3
-        if field.startswith('validation_errors') or field.startswith('aggregated_items'):
-            continue
-        elif field == 'q':  # searched string has field 'q'
-            # people shouldn't provide multiple queries, but if they do,
-            # combine them with AND logic
-            if 'q' in prepared_terms:
-                join_list = [prepared_terms['q'], val]
-                prepared_terms['q'] = ' AND '.join(join_list)
-            else:
-                prepared_terms['q'] = val
-        elif field not in COMMON_EXCLUDED_URI_PARAMS + ['type']:
-            if 'embedded.' + field not in prepared_terms.keys():
-                prepared_terms['embedded.' + field] = []
-            prepared_terms['embedded.' + field].append(val)
-    return prepared_terms
+        if not isinstance(value, dict):
+            res = secure_embed(request, value, '@@object')
+            value = obj[name] = res
+        expand_path(request, value, remaining)
 
 
-def set_doc_types(request, types, search_type):
-    """
-    Set the type of documents resulting from the search; order and check for
-    invalid types as well. If a forced search_type is enforced, use that;
-    otherwise, set types from the query params. Default to Item if none set.
+def find_collection_subtypes(registry, item_type, types_covered=None):
+    """
+    Given an item type (or item class name), find all subtypes for that type
+    and return a list containing all of them. types_covered is meant to be
+    used internally, but adding a item type to it will cause it to be removed
+    from the returned output
 
     Args:
-        request: the current Request
-        types: registry[TYPES]
-        search_type (str): forced search item type
+        registry: the current Registry
+        item_type (str): item type (or item class name) to find subtypes for
+        types_covered (list): used internally to track covered types
 
     Returns:
-        list: the string item types to use for the search
-
-    Raises:
-        HTTPBadRequest: if an invalid item type is supplied
+        list: all item types found when traversing substypes
     """
-    doc_types = []
-    if search_type is None:
-        doc_types = request.params.getall('type')
-        if '*' in doc_types:
-            doc_types = ['Item']
-    else:
-        doc_types = [search_type]
-    # Normalize to item_type
+    types_found = []
+    if types_covered is None:
+        types_covered = []  # initialize
     try:
-        doc_types = sorted({types[name].name for name in doc_types})
+        # this works for item name (MyItem) and item type (my_name)
+        registry_type = registry[TYPES][item_type]
     except KeyError:
-        # Check for invalid types
-        bad_types = [t for t in doc_types if t not in types]
-        msg = "Invalid type: {}".format(', '.join(bad_types))
-        raise HTTPBadRequest(explanation=msg)
-    if len(doc_types) == 0:
-        doc_types = ['Item']
-    return doc_types
-
-
-def get_search_fields(request, doc_types):
-    """
-    Returns set of columns that are being searched and highlights
-    """
-    fields = {'uuid'}
-    highlights = {}
-    types = request.registry[TYPES]
-    for doc_type in doc_types:
-        type_info = types[doc_type]
-        for value in type_info.schema.get('boost_values', ()):
-            fields.add('embedded.' + value)
-            highlights['embedded.' + value] = {}
-    return fields, highlights
-
-
-def list_source_fields(request, doc_types, frame):
-    """
-    Returns set of fields that are requested by user or default fields.
-    These fields are used to further limit the results from the search.
-    Note that you must provide the full fieldname with embeds, such as:
-    'field=biosample.biosource.individual.organism.name' and not just
-    'field=name'
-    """
-    fields_requested = request.normalized_params.getall('field')
-    if fields_requested:
-        fields = ['embedded.@id', 'embedded.@type']
-        for field in fields_requested:
-            fields.append('embedded.' + field)
-    elif frame in ['embedded', 'object', 'raw']:
-        if frame != 'embedded':
-            # frame=raw corresponds to 'properties' in ES
-            if frame == 'raw':
-                frame = 'properties'
-            # let embedded be searched as well (for faceting)
-            fields = ['embedded.*', frame + '.*']
-        else:
-            fields = [frame + '.*']
-    else:
-        fields = ['embedded.*']
-    return fields
-
+        return []  # no types found
+    # add the item_type of this collection if applicable
+    if hasattr(registry_type, 'item_type'):
+        if registry_type.name not in types_covered:
+            types_found.append(registry_type.item_type)
+        types_covered.append(registry_type.name)
+    # subtypes are given by name and include the registry_type.name itself
+    if hasattr(registry_type, 'subtypes'):
+        subtypes = registry_type.subtypes
+        for subtype in subtypes:
+            if subtype not in types_covered:
+                types_found.extend(
+                    find_collection_subtypes(registry, subtype, types_covered)
+                )
+    return types_found
+
+
+def crawl_schema(types, field_path, schema_cursor, split_path=None):
+    """
+    Given a field_path that is a sequence of fields joined by '.' and a starting
+    schema, will recursively drill down into the schema to find the schema value
+    of the terminal field. Will raise an Exception if the field cannot be found
+    Args:
+        types: Result of registry[TYPES].
+        field_path: string field path, joined by '.'
+        schema_cursor: dictionary schema starting point
+        split_path: array of remaining fields to traverse. Used internally
 
-def build_query(search, prepared_terms, source_fields):
-    """
-    Prepare the query within the Search object.
+    Returns:
+        Dictionary schema for the terminal field in field_path
     """
-    query_info = {}
-    string_query = None
-    # set _source fields for the search
-    search = search.source(list(source_fields))
-    # prepare the query from prepared_terms
-    for field, value in prepared_terms.items():
-        if field == 'q':
-            query_info['query'] = value
-            query_info['lenient'] = True
-            query_info['default_operator'] = 'AND'
-            query_info['fields'] = ['_all']
-            break
-    if query_info != {}:
-        string_query = {'must': {'simple_query_string': query_info}}
-        query_dict = {'query': {'bool': string_query}}
-    else:
-        query_dict = {'query': {'bool': {}}}
-    search.update_from_dict(query_dict)
-    return search, string_query
-
-
-def set_sort_order(request, search, search_term, types, doc_types, result):
-    """
-    sets sort order for elasticsearch results
-    example: /search/?type=Biosource&sort=display_title
-    will sort by display_title in ascending order. To set descending order,
-    use the "-" flag: sort_by=-date_created.
-    Sorting is done alphatbetically, case sensitive by default.
-    TODO: add a schema flag for case sensitivity/insensitivity?
-
-    ES5: simply pass in the sort OrderedDict into search.sort
-    """
-    sort = OrderedDict()
-    result_sort = OrderedDict()
-    if len(doc_types) == 1:
-        type_schema = types[doc_types[0]].schema
-    else:
-        type_schema = None
-
-    def add_to_sort_dict(requested_sort):
-        if requested_sort.startswith('-'):
-            name = requested_sort[1:]
-            order = 'desc'
-        else:
-            name = requested_sort
-            order = 'asc'
-        sort_schema = type_schema.get('properties', {}).get(name) if type_schema else None
-        if sort_schema:
-            sort_type = sort_schema.get('type')
-        else:
-            sort_type = 'string'
+    # true if we are just starting up
+    if split_path is None:
+        # ensure input schema is a dictionary
+        if not isinstance(schema_cursor, dict):
+            raise Exception('Could not find schema field for: %s. Invalid starting schema.' % field_path)
+
+        # drill into 'properties' of initial schema
+        if 'properties' in schema_cursor:
+            schema_cursor = schema_cursor['properties']
+        split_path = field_path.split('.')
+
+    curr_field = split_path[0]
+    schema_cursor = schema_cursor.get(curr_field)
+    if not schema_cursor:
+        raise Exception('Could not find schema field for: %s. Field not found. Failed at: %s'
+                        % (field_path, curr_field))
+
+    # schema_cursor should always be a dictionary
+    if not isinstance(schema_cursor, dict):
+        raise Exception('Could not find schema field for: %s. Non-dictionary schema. Failed at: %s'
+                        % (field_path, curr_field))
+
+    # base case. We have found the desired schema
+    if len(split_path) == 1:
+        return schema_cursor
+
+    # drill into 'items' or 'properties'. always check 'items' before 'properties'
+    # check if an array + drill into if so
+    if schema_cursor.get('type') == 'array' and 'items' in schema_cursor:
+        schema_cursor = schema_cursor['items']
+    # check if an object + drill into if so
+    if schema_cursor.get('type') == 'object' and 'properties' in schema_cursor:
+        schema_cursor = schema_cursor['properties']
+    # if we hit a linkTo, pull in the new schema of the linkTo type
+    if 'linkTo' in schema_cursor:
+        linkTo = schema_cursor['linkTo']
+        try:
+            linkTo_type = types.all[linkTo]
+        except KeyError:
+            raise Exception('Could not find schema field for: %s. Invalid linkTo. Failed at: %s'
+                            % (field_path, curr_field))
+        linkTo_schema = linkTo_type.schema
+        schema_cursor = linkTo_schema['properties'] if 'properties' in linkTo_schema else linkTo_schema
 
-        # ES type != schema types
-        if sort_type == 'integer':
-            sort['embedded.' + name] = result_sort[name] = {
-                'order': order,
-                'unmapped_type': 'long',
-                'missing': '_last'
-            }
-        elif sort_type == 'number':
-            sort['embedded.' + name] = result_sort[name] = {
-                'order': order,
-                'unmapped_type': 'float',
-                'missing': '_last'
-            }
-        else:
-            # fallback case, applies to all string type:string fields
-            sort['embedded.' + name + '.lower_case_sort'] = result_sort[name] = {
-                'order': order,
-                'unmapped_type': 'keyword',
-                'missing': '_last'
-            }
+    return crawl_schema(types, field_path, schema_cursor, split_path[1:])
 
-    # Prefer sort order specified in request, if any
-    requested_sorts = request.normalized_params.getall('sort')
-    if requested_sorts:
-        for rs in requested_sorts:
-            add_to_sort_dict(rs)
-
-    text_search = search_term.get('q')
-
-    # Otherwise we use a default sort only when there's no text search to be ranked
-    if not sort and (text_search == '*' or not text_search):
-        # If searching for a single type, look for sort options in its schema
-        if type_schema:
-            if 'sort_by' in type_schema:
-                for k, v in type_schema['sort_by'].items():
-                    # Should always sort on raw field rather than analyzed field
-                    # OR search on lower_case_sort for case insensitive results
-                    sort['embedded.' + k + '.lower_case_sort'] = result_sort[k] = v
-        # Default is most recent first, then alphabetical by label
-        if not sort:
-            sort['embedded.date_created.raw'] = result_sort['date_created'] = {
-                'order': 'desc',
-                'unmapped_type': 'keyword',
-            }
-            sort['embedded.label.raw'] = result_sort['label'] = {
-                'order': 'asc',
-                'missing': '_last',
-                'unmapped_type': 'keyword',
-            }
-    elif not sort and text_search and text_search != '*':
-        search = search.sort(                   # Multi-level sort. See http://www.elastic.co/guide/en/elasticsearch/guide/current/_sorting.html#_multilevel_sorting & https://stackoverflow.com/questions/46458803/python-elasticsearch-dsl-sorting-with-multiple-fields
-            {'_score': {"order": "desc"}},
-            {'embedded.date_created.raw': {'order': 'desc', 'unmapped_type': 'keyword'},
-             'embedded.label.raw': {'order': 'asc', 'unmapped_type': 'keyword', 'missing': '_last'}},
-            {'_uid': {'order': 'asc'}}  # 'embedded.uuid.raw' (instd of _uid) sometimes results in 400 bad request : 'org.elasticsearch.index.query.QueryShardException: No mapping found for [embedded.uuid.raw] in order to sort on'
-        )
-        result['sort'] = result_sort = {'_score': {"order": "desc"}}
-        return search
 
-    if sort and result_sort:
-        result['sort'] = result_sort
-        search = search.sort(sort)
-    return search
-
-
-def set_filters(request, search, result, principals, doc_types):
-    """
-    Sets filters in the query
-    """
-
-    # these next two dictionaries should each have keys equal to query_field
-    # and values: must_terms: [<list of terms>], must_not_terms: [<list of terms>], add_no_value: True/False/None
-    field_filters = {
-        'principals_allowed.view': {
-            'must_terms': principals,
-            'must_not_terms': [],
-            'add_no_value': None
-        },
-        'embedded.@type.raw': {
-            'must_terms': doc_types,
-            'must_not_terms': [],
-            'add_no_value': None
-        },
-        'embedded.status.raw': {
-            'must_terms': [],
-            'must_not_terms': [],
-            'add_no_value': None
-        }
-    }
+##########################################
+# Embedding / aggregated_items utilities #
+##########################################
 
-    range_filters = {}
 
-    # Exclude status=deleted Items unless explicitly requested/filtered-in.
-    if 'deleted' not in request.normalized_params.getall('status'):
-        field_filters['embedded.status.raw']['must_not_terms'].append('deleted')
-    if 'replaced' not in request.normalized_params.getall('status'):
-        field_filters['embedded.status.raw']['must_not_terms'].append('replaced')
-
-    # Exclude type=TrackingItem and type=OntologyTerm from results unless are explictly specified
-    if 'TrackingItem' not in doc_types:
-        field_filters['embedded.@type.raw']['must_not_terms'].append('TrackingItem')
-    if 'OntologyTerm' not in doc_types:
-        field_filters['embedded.@type.raw']['must_not_terms'].append('OntologyTerm')
-
-    for field, term in request.normalized_params.items():
-        not_field = False  # keep track if query is NOT (!)
-        exists_field = False  # keep track of null values
-        range_type = False  # If we determine is a range request (field.to, field.from), will be populated with string 'date' or 'numerical'
-        range_direction = None
-        if field in COMMON_EXCLUDED_URI_PARAMS + ['q']:
-            continue
-        elif field == 'type' and term != 'Item':
-            continue
-        elif term == 'No value':
-            exists_field = True
+# Terminal fields that are added to the embedded list for every embedded item
+# Status must now be a default embed, since it can effect principals_allowed
+DEFAULT_EMBEDS = ['.@id', '.@type', '.display_title', '.uuid', '.status', '.principals_allowed.*']
 
-        # Check for date or numerical range filters
-        if (len(field) > 3 and field[-3:] == '.to') or (len(field) > 5 and field[-5:] == '.from'):
-            if field[-3:] == '.to':
-                f_field = field[:-3]
-                range_direction = "lte"
-            else:
-                f_field = field[:-5]
-                range_direction = "gte"
 
-            # If schema for field is not found (and range_type thus not set),
-            # then treated as ordinary term filter (likely will get 0 results)
-            field_schema = schema_for_field(f_field, request, doc_types)
-            if field_schema:
-                range_type = 'date' if determine_if_is_date_field(f_field, field_schema) else 'numerical'
-
-        # Add filter to result
-        qs = urlencode([
-            (k.encode('utf-8'), v.encode('utf-8'))
-            for k, v in request.normalized_params.items()
-            if (k != field or v != term)
-        ])
-        remove_path = '{}?{}'.format(request.path, qs)
-
-        # default to searching type=Item rather than empty filter path
-        if remove_path[-1] == '?':
-            remove_path += 'type=Item'
-
-        result['filters'].append({
-            'field': field,
-            'term': term,
-            'remove': remove_path
-        })
-
-        # handle NOT
-        if field.endswith('!'):
-            field = field[:-1]
-            not_field = True
-
-        # Add filter to query
-        if range_type and f_field and range_type in ('date', 'numerical'):
-            query_field = 'embedded.' + f_field
-        elif field.startswith('validation_errors') or field.startswith('aggregated_items'):
-            query_field = field + '.raw'
-        elif field == 'type':
-            query_field = 'embedded.@type.raw'
+def secure_embed(request, item_path, addition='@@object'):
+    """
+    Make a call to embed() with the given item path and user status
+    Handles substituting a no view permissions message if a the given
+    request does not have permission to see the object
+    """
+    res = {'error': 'no view permissions'}
+    try:
+        # if empty item_path reqeust.embed returns just addition as a string
+        if item_path:
+            res = request.embed(str(item_path), addition, as_user=True)
         else:
-            query_field = 'embedded.' + field + '.raw'
+            res = ''
+        return res
+    except HTTPForbidden:
+        print("you don't have access to this object")
+
+    return res
+
+
+def expand_embedded_model(request, obj, model, parent_path='', embedded_path=None):
+    """
+    A similar idea to expand_path, but takes in model from build_embedded_model
+    instead. Takes in the @@object view of the item (obj) and returns a
+    fully embedded result.
+    This is also used recursively to handle dictionaries encountered during
+    this process.
+    parent_path and embedded_path are passed in for aggregated_items tracking.
 
-        if range_type:
-            if query_field not in range_filters:
-                range_filters[query_field] = {}
-                if range_type == 'date':
-                    range_filters[query_field]['format'] = 'yyyy-MM-dd HH:mm'
-
-            if range_direction in ('gt', 'gte', 'lt', 'lte'):
-                if len(term) == 10:
-                    # Correct term to have hours, e.g. 00:00 or 23:59, if not otherwise supplied.
-                    if range_direction == 'gt' or range_direction == 'lte':
-                        term += ' 23:59'
-                    elif range_direction == 'gte' or range_direction == 'lt':
-                        term += ' 00:00'
-
-                if range_filters[query_field].get(range_direction) is None:
-                    range_filters[query_field][range_direction] = term
-                else:
-                    # If have a value already (e.g. multiple ranges selected), choose the widening option.
-                    if range_direction == 'gt' or range_direction == 'gte':
-                        if term < range_filters[query_field][range_direction]:
-                            range_filters[query_field][range_direction] = term
-                    elif range_direction == 'lt' or range_direction == 'lte':
-                        if term > range_filters[query_field][range_direction]:
-                            range_filters[query_field][range_direction] = term
-        else:
-            if query_field not in field_filters:
-                field_filters[query_field] = {
-                    'must_terms': [],
-                    'must_not_terms': [],
-                    'add_no_value': None
-                }
-
-            # handle case of filtering for null values
-            if exists_field:
-                # the value below is True when we want to include 'No value' as a filter
-                field_filters[query_field]['add_no_value'] = False if not_field else True
-                continue
-
-            if not_field:
-                field_filters[query_field]['must_not_terms'].append(term)
-            else:
-                field_filters[query_field]['must_terms'].append(term)
+    Args:
+        request: current Request
+        obj (dict): item to expand the embedded model on
+        model (dict): model for embedding from build_embedded_model
+        parent_path (str): resource path of the parent linkTo item encountered
+            while embedding. If no external items embedded, is an empty string
+            Used for aggregated items
+        embedded_path (list): field names of all embedded fields traversed so
+            so far in the model. Used for aggregated_items
 
-    must_filters = []
-    must_not_filters = []
-    for query_field, filters in field_filters.items():
-        must_terms = {'terms': {query_field: filters['must_terms']}} if filters['must_terms'] else {}
-        must_not_terms = {'terms': {query_field: filters['must_not_terms']}} if filters['must_not_terms'] else {}
-        if filters['add_no_value'] is True:
-            # add to must_not in an OR case, which is equivalent to filtering on 'No value'
-            should_arr = [must_terms] if must_terms else []
-            should_arr.append({'bool': {'must_not': {'exists': {'field': query_field}}}})
-            must_filters.append({'bool': {'should': should_arr}})
-        elif filters['add_no_value'] is False:
-            # add to must_not in an OR case, which is equivalent to filtering on '! No value'
-            should_arr = [must_terms] if must_terms else []
-            should_arr.append({'exists': {'field': query_field}})
-            must_filters.append({'bool': {'should': should_arr}})
-        else:  # no filtering on 'No value'
-            if must_terms:
-                must_filters.append(must_terms)
-        if must_not_terms:
-            must_not_filters.append(must_not_terms)
-
-    # lastly, add range limits to filters if given
-    for range_field, range_def in range_filters.items():
-        must_filters.append({
-            'range': {range_field: range_def}
-        })
-
-    # To modify filters of elasticsearch_dsl Search, must call to_dict(),
-    # modify that, then update from the new dict
-    prev_search = search.to_dict()
-    # initialize filter hierarchy
-    final_filters = {'bool': {'must': must_filters, 'must_not': must_not_filters}}
-    prev_search['query']['bool']['filter'] = final_filters
-    search.update_from_dict(prev_search)
-
-    return search, final_filters
-
-
-def initialize_facets(request, doc_types, prepared_terms, schemas):
-    """
-    Initialize the facets used for the search. If searching across multiple
-    doc_types, only use the default 'Data Type' and 'Status' facets.
-    Add facets for custom url filters whether or not they're in the schema
+    Returns:
+        dict: embedded result
+    """
+    embedded_res = {}
+    if embedded_path is None:
+        embedded_path = []  # initialize
+    # first take care of the fields_to_use at this level; get them from obj
+    fields_to_use = model.get('fields_to_use')
+    if fields_to_use:
+        if '*' in fields_to_use:
+            embedded_res = obj
+        else:
+            for field in fields_to_use:
+                found = obj.get(field)
+                if found is not None:
+                    embedded_res[field] = found
+    # then handle objects at the next level
+    for to_embed in model:
+        if to_embed == 'fields_to_use':
+            continue
+        obj_val = obj.get(to_embed)
+        if obj_val is None:
+            continue
+        # branch embedded path for each field to embed
+        this_embedded_path = embedded_path.copy()
+        # pass to_embed (field name) to track aggregated_items
+        obj_embedded = expand_val_for_embedded_model(request, obj_val,
+                                                     model[to_embed],
+                                                     to_embed, parent_path,
+                                                     this_embedded_path)
+        if obj_embedded is not None:
+            embedded_res[to_embed] = obj_embedded
+    return embedded_res
+
+
+def expand_val_for_embedded_model(request, obj_val, downstream_model, field_name='',
+                                  parent_path='', embedded_path=None):
+    """
+    Take a value from an object and the relevant piece of the embedded_model
+    and perform embedding.
+    We have to account for lists, dictionaries, linkTos, and other values:
+        - lists: process each entry separately and join them. embedded_path
+            is branched for each entry
+        - dicts: run expand_embedded_model on the dict using the downstream
+            embedded model. Record in aggregated_items if necessary
+        - linkTo: attempt to get frame=object for item, taking permissions into
+            account. Record in aggregated_items if necessary
+        - other values: return them
+    field_name/parent_path are optional and used to track aggregated_items.
+    embedded_path is used to track the levels of embedding we've traversed
+    and is updated whenever a dict/linkTo is encountered
 
     Args:
-        doc_types (list): Item types (@type) for which we are performing a search for.
-        prepared_terms (dict): terms to match in ES, keyed by ES field name.
-        schemas (list): List of OrderedDicts of schemas for doc_types.
+        request: current Request
+        obj_val: value of the embedded field from the previous model
+        downstream_model (dict): model for downstream embedding, originally
+            from build_embedded_model
+        field_name (str): name of the current field being embedded. Used for
+            aggregated items
+        parent_path (str): resource path of the parent linkTo item encountered
+            while embedding. If no external items embedded, is an empty string
+            Used for aggregated items
+        embedded_path (list): field names of all embedded fields traversed so
+            so far in the model. Used for aggregated_items
 
     Returns:
-        list: tuples containing (0) ElasticSearch-formatted field name (e.g. `embedded.status`) and (1) list of terms for it.
+        The processed embed from the given obj_val and downstream_model
     """
+    agg_items = request._aggregated_items
+    # if the value is a list, process each value sequentially
+    # we are not actually progressing down the embedded model yet
+    if isinstance(obj_val, list):
+        obj_list = []
+        for idx, member in enumerate(obj_val):
+            # branch embedded_path for each item in list
+            this_embedded_path = embedded_path.copy()
+            # lists conserve field name and their order
+            obj_embedded = expand_val_for_embedded_model(request, member,
+                                                         downstream_model,
+                                                         field_name=field_name,
+                                                         parent_path=parent_path,
+                                                         embedded_path=this_embedded_path)
+            if obj_embedded is not None:
+                obj_list.append(obj_embedded)
+        return obj_list
+    else:
+        # for dict/linkTo/other values, we are progressing down the embed
+        embedded_path.append(field_name)
 
-    facets = [
-        # More facets will be appended to this list from item schema plus from any currently-active filters (as requested in URI params).
-        ('type', {'title': 'Data Type'})
-    ]
-    append_facets = [
-        # Facets which will be appended after those which are in & added to `facets`
-        ('status', {'title': 'Status'}),
+    if isinstance(obj_val, dict):
+        obj_embedded = expand_embedded_model(request, obj_val, downstream_model,
+                                             parent_path=parent_path, embedded_path=embedded_path)
+        # aggregate the item if applicable
+        if field_name and parent_path and field_name in agg_items:
+            agg_emb_path = '.'.join(embedded_path)
+            new_agg = {'parent': parent_path, 'embedded_path': agg_emb_path, 'item': obj_embedded}
+            agg_items[field_name]['items'].append(new_agg)
+        return obj_embedded
+    elif isinstance(obj_val, str):
+        # get the @@object view of obj to embed
+        # TODO: per-field invalidation by adding uuids to request._linked_uuids
+        # ONLY if the field is used in downstream_model (i.e. in embedded_list)
+        obj_val = secure_embed(request, obj_val, '@@object')
+        if not obj_val or obj_val == {'error': 'no view permissions'}:
+            return obj_val
+
+        # aggregate the item if applicable
+        if field_name and parent_path and field_name in agg_items:
+            agg_emb_path = '.'.join(embedded_path)
+            # we may need to merge the values with existing ones
+            new_agg = {'parent': parent_path, 'embedded_path': agg_emb_path, 'item': obj_val}
+            agg_items[field_name]['items'].append(new_agg)
+
+        # track the new parent object if we are indexing
+        new_parent_path = obj_val.get('@id') if request._indexing_view else None
+        obj_embedded = expand_embedded_model(request, obj_val, downstream_model,
+                                             parent_path=new_parent_path,
+                                             embedded_path=embedded_path)
+        return obj_embedded
+    else:
+        # this means the object should be returned as-is
+        return obj_val
 
-        # TODO: Re-enable below line if/when 'range' URI param queries for date & numerical fields are implemented.
-        # ('date_created', {'title': 'Date Created', 'hide_from_view' : True, 'aggregation_type' : 'date_histogram' })
-    ]
-    validation_error_facets = [
-        ('validation_errors.name', {'title': 'Validation Errors', 'order': 999})
-    ]
-    # hold disabled facets from schema; we also want to remove these from the prepared_terms facets
-    disabled_facets = []
 
-    # Add facets from schema if one Item type is defined.
-    # Also, conditionally add extra appendable facets if relevant for type from schema.
-    if len(doc_types) == 1 and doc_types[0] != 'Item':
-        current_type_schema = request.registry[TYPES][doc_types[0]].schema
-        if 'facets' in current_type_schema:
-            schema_facets = OrderedDict(current_type_schema['facets'])
-            for schema_facet in schema_facets.items():
-                if schema_facet[1].get('disabled', False):
-                    disabled_facets.append(schema_facet[0])
-                    continue  # Skip disabled facets.
-                facets.append(schema_facet)
-
-    # == Add facets for any non-schema ?field=value filters requested in the search (unless already set) ==
-    used_facets = [facet[0] for facet in facets + append_facets]
-    used_facet_titles = [facet[1]['title']
-                         for facet in facets + append_facets
-                         if 'title' in facet[1]]
-    for field in prepared_terms:
-        if field.startswith('embedded'):
-            split_field = field.strip().split('.')  # Will become, e.g. ['embedded', 'experiments_in_set', 'files', 'file_size', 'from']
-            use_field = '.'.join(split_field[1:])
-
-            # 'terms' is the default per-term bucket aggregation for all non-schema facets
-            aggregation_type = 'terms'
-
-            # Use the last part of the split field to get the field title
-            title_field = split_field[-1]
-
-            # if searching for a display_title, use the title of parent object
-            # use `is_object_title` to keep track of this
-            if title_field == 'display_title' and len(split_field) > 1:
-                title_field = split_field[-2]
-                is_object_title = True
+def build_embedded_model(fields_to_embed):
+    """
+    Takes a list of fields to embed and builds the framework used to generate
+    the fully embedded result. 'fields_to_use' refer to specific fields that are to
+    be embedded within an object. The base level object gets a special flag,
+    '*', which means all non-object fields are embedded by default.
+    Below is an example calculated from the following fields:
+    INPUT:
+    [modifications.modified_regions.chromosome,
+    lab.uuid,
+    award.*,
+    biosource.name]
+    OUTPUT:
+    {'modifications': {'modified_regions': {'fields_to_use': ['chromosome']}},
+     'lab': {'fields_to_use': ['uuid']},
+     'award': {'fields_to_use': ['*']},
+     'biosource': {'fields_to_use': ['name']},
+     'fields_to_use': ['*']}
+    """
+    FIELDS_TO_USE = 'fields_to_use'
+    embedded_model = {FIELDS_TO_USE: ['*']}
+    for field in fields_to_embed:
+        split_field = field.split('.')
+        max_idx = len(split_field) - 1
+        cursor = embedded_model
+        for idx, subfield in enumerate(split_field):
+            if idx == max_idx:  # terminal field
+                cursor[FIELDS_TO_USE] = fields_to_use = cursor.get(FIELDS_TO_USE, [])
+                fields_to_use.append(subfield)
             else:
-                is_object_title = False
+                if subfield not in cursor:
+                    cursor[subfield] = {}
+                cursor = cursor[subfield]
+    return embedded_model
+
+
+def add_default_embeds(item_type, types, embeds, schema=None):
+    """
+    Perform default processing on the embedded_list of an item_type.
+    Three part process that automatically builds a list of embed paths using
+    the embedded_list (embeds parameter), expanding all the top level linkTos,
+    and then finally adding the default embeds to all the linkTo paths generated.
+    Used in fourfront/../types/base.py AND snovault create mapping
+    """
+    if schema is None:
+        schema = {}
+    # remove duplicate embeds
+    embeds = list(set(list(embeds)))
+    embeds.sort()
+    if 'properties' in schema:
+        schema = schema['properties']
+    processed_embeds = set(embeds[:]) if len(embeds) > 0 else set()
+    # add default embeds for items in the embedded_list
+    embeds_to_add, processed_embeds = expand_embedded_list(item_type, types, embeds,
+                                                           schema, processed_embeds)
+    # automatically embed top level linkTo's not already embedded
+    # also find subobjects and embed those
+    embeds_to_add.extend(find_default_embeds_for_schema('', schema))
+    # finally actually add the default embeds
+    return build_default_embeds(embeds_to_add, processed_embeds)
+
+
+def expand_embedded_list(item_type, types, embeds, schema, processed_embeds):
+    """
+    Takes the embedded_list (as defined in types/ file for an item) and finds
+    all items that should have the default embeds added to them
+    """
+    embeds_to_add = []
+    # Handles the use of a terminal '*' in the embeds
+    for embed_path in embeds:
+        # ensure that the embed is valid
+        split_path = embed_path.strip().split('.')
+        error_message, path_embeds_to_add = crawl_schemas_by_embeds(item_type, types, split_path, schema)
+        if error_message:
+            # remove bad embeds
+            # check error_message rather than is_valid because there can
+            # be cases of fields that are not valid for default embeds
+            # but are still themselves valid fields
+            processed_embeds.remove(embed_path)
+            print(error_message, file=sys.stderr)
+        else:
+            embeds_to_add.extend(path_embeds_to_add)
+    return embeds_to_add, processed_embeds
 
-            if title_field in used_facets or title_field in disabled_facets:
-                # Cancel if already in facets or is disabled
-                continue
 
-            # If we have a range filter in the URL,
-            if title_field == 'from' or title_field == 'to':
-                if len(split_field) == 3:
-                    f_field = split_field[-2]
-                    field_schema = schema_for_field(f_field, request, doc_types)
-                    if field_schema:
-                        title_field = f_field
-                        use_field = '.'.join(split_field[1:-1])
-                        aggregation_type = 'stats'
-
-            for schema in schemas:
-                if title_field in schema['properties']:
-                    title_field = schema['properties'][title_field].get('title', title_field)
-                    # see if the title field conflicts for is_object_title facets
-                    if is_object_title and title_field in used_facet_titles:
-                        title_field += ' (Title)'
-                    break
-
-            facet_tuple = (use_field, {'title': title_field, 'aggregation_type': aggregation_type})
-
-            # At moment is equivalent to `if aggregation_type == 'stats'`` until/unless more agg types are added for _facets_.
-            if aggregation_type != 'terms':
-                facet_tuple[1]['hide_from_view'] = True  # Temporary until we handle these better on front-end.
-                # Facet would be otherwise added twice if both `.from` and `.to` are requested.
-                if facet_tuple in facets:
-                    continue
+def build_default_embeds(embeds_to_add, processed_embeds):
+    """
+    Actually add the embed path for default embeds using the embeds_to_add
+    list generated in add_default_embeds.
+    """
+    for add_embed in embeds_to_add:
+        if add_embed[-2:] == '.*':
+            processed_embeds.add(add_embed)
+        else:
+            # for neatness' sake, ensure redundant embeds are not getting added
+            check_wildcard = add_embed + '.*'
+            if check_wildcard not in processed_embeds and check_wildcard not in embeds_to_add:
+                # default embeds to add
+                for default_emb in DEFAULT_EMBEDS:
+                    processed_embeds.add(add_embed + default_emb)
+    return list(processed_embeds)
+
+
+def find_default_embeds_for_schema(path_thus_far, subschema):
+    """
+    For a given field and that field's subschema, return an array of paths
+    to the objects in that subschema. This includes all linkTo's and any
+    subobjects within the subschema. Recursive function.
+    """
+    linkTo_paths = []
+    if subschema.get('type') == 'array' and 'items' in subschema:
+        items_linkTos = find_default_embeds_for_schema(path_thus_far, subschema['items'])
+        linkTo_paths += items_linkTos
+    if subschema.get('type') == 'object' and 'properties' in subschema:
+        # we found an object in the schema. embed all its fields
+        linkTo_paths.append(path_thus_far + '.*')
+        props_linkTos = find_default_embeds_for_schema(path_thus_far, subschema['properties'])
+        linkTo_paths += props_linkTos
+    for key, val in subschema.items():
+        if key in SCHEMA_KEYS_TO_IGNORE_FOR_EMBEDS:
+            continue
+        elif key == 'linkTo':
+            linkTo_paths.append(path_thus_far)
+        elif isinstance(val, dict):
+            updated_path = key if path_thus_far == '' else path_thus_far + '.' + key
+            item_linkTos = find_default_embeds_for_schema(updated_path, val)
+            linkTo_paths += item_linkTos
+    return linkTo_paths
+
+
+def crawl_schemas_by_embeds(item_type, types, split_path, schema):
+    """
+    Take a split embed_path from the embedded_list and confirm that each item in the
+    path has a valid schema. Also return default embeds associated with embed_path.
+    If embed_path only has one element, return an error. This is because it is
+    a redundant embed (all top level fields and @id/display_title for
+    linkTos are added automatically).
+    - split_path is embed_path (e.g. biosource.biosample.*) split on '.', so
+      ['biosample', 'biosource', '*'] for the example above.
+    - types parameter is registry[TYPES].
+    A linkTo schema is considered valid if it has @id and display_title fields.
+    Return values:
+    1. error_message. Either None for no errors or a string to describe the error
+    2. embeds_to_add. List of embeds to add for the given embed_path. In the
+    case of embed_path ending with a *, this is the default embeds for that
+    object's schema. Otherwise, it may just be embed_path, once its validated.
+    """
+    schema_cursor = schema
+    embeds_to_add = []
+    error_message = None
+    linkTo_path = '.'.join(split_path)
+    if len(split_path) == 1:
+        error_message = ('{} has a bad embed: {} is a top-level field. Did you mean: "{}.*"?.'
+                         .format(item_type, split_path[0], split_path[0]))
+    for idx in range(len(split_path)):
+        element = split_path[idx]
+        # schema_cursor should always be a dictionary if we have more split_fields
+        if not isinstance(schema_cursor, dict):
+            error_message = f'{item_type} has a bad embed: {linkTo_path} does not have valid schemas throughout.'
+            return error_message, embeds_to_add
+        if element == '*':
+            linkTo_path = '.'.join(split_path[:-1])
+            if idx != len(split_path) - 1:
+                error_message = '{} has a bad embed: * can only be at the end of an embed.'.format(item_type)
+            if '@id' in schema_cursor and 'display_title' in schema_cursor:
+                # add default linkTos for the '*' object
+                embeds_to_add.extend(find_default_embeds_for_schema(linkTo_path, schema_cursor))
+            return error_message, embeds_to_add
+        elif element in schema_cursor:
+            # save prev_schema_cursor in case where last split_path is a non-linkTo field
+            prev_schema_cursor = copy(schema_cursor)
+            schema_cursor = schema_cursor[element]
+            # drill into 'items' or 'properties'. always check 'items' before 'properties'
+            # check if an array + drill into if so
+            if schema_cursor.get('type', None) == 'array' and 'items' in schema_cursor:
+                schema_cursor = schema_cursor['items']
+            # check if an object + drill into if so
+            if schema_cursor.get('type', None) == 'object' and 'properties' in schema_cursor:
+                schema_cursor = schema_cursor['properties']
+            # if we hit a linkTo, pull in the new schema of the linkTo type
+            # if this is a terminal linkTo, add display_title/@id
+            if 'linkTo' in schema_cursor:
+                linkTo = schema_cursor['linkTo']
+                try:
+                    linkTo_type = types.all[linkTo]
+                except KeyError:
+                    error_message = '{} has a bad embed: {} is not a valid type.'.format(item_type, linkTo)
+                    return error_message, embeds_to_add
+                linkTo_schema = linkTo_type.schema
+                schema_cursor = linkTo_schema['properties'] if 'properties' in linkTo_schema else linkTo_schema
+                if '@id' not in schema_cursor or 'display_title' not in schema_cursor:
+                    error_message = ('{} has a bad embed: {} object does not have @id/display_title.'
+                                     .format(item_type, linkTo_path))
+                    return error_message, embeds_to_add
+                # we found a terminal linkTo embed
+                if idx == len(split_path) - 1:
+                    embeds_to_add.append(linkTo_path)
+                    return error_message, embeds_to_add
+                else:  # also add default embeds for each intermediate item in the path
+                    intermediate_path = '.'.join(split_path[:idx+1])
+                    embeds_to_add.append(intermediate_path)
+            # not a linkTo. See if this is this is the terminal element
+            else:
+                # check if this is the last element in path
+                if idx == len(split_path) - 1:
+                    # in this case, the last element in the embed is a field
+                    # remove that from linkTo_path
+                    linkTo_path = '.'.join(split_path[:-1])
+                    if '@id' in prev_schema_cursor and 'display_title' in prev_schema_cursor:
+                        embeds_to_add.append(linkTo_path)
+                    return error_message, embeds_to_add
+        else:
+            error_message = ('{} has a bad embed: {} is not contained within the parent schema. See {}.'
+                             .format(item_type, element, linkTo_path))
+            return error_message, embeds_to_add
+    # really shouldn't hit this return, but leave as a back up
+    return error_message, embeds_to_add
 
-            facets.append(facet_tuple)
 
-    # Append additional facets (status, validation_errors, ...) at the end of
-    # list unless were already added via schemas, etc.
-    used_facets = [facet[0] for facet in facets]  # Reset this var
-    for ap_facet in append_facets + validation_error_facets:
-        if ap_facet[0] not in used_facets:
-            facets.append(ap_facet)
-        else:  # Update with better title if not already defined from e.g. requested filters.
-            existing_facet_index = used_facets.index(ap_facet[0])
-            if facets[existing_facet_index][1].get('title') in (None, facets[existing_facet_index][0]):
-                facets[existing_facet_index][1]['title'] = ap_facet[1]['title']
-
-    return facets
-
-
-def schema_for_field(field, request, doc_types, should_log=False):
-    """
-    Find the schema for the given field (in embedded '.' format). Uses
-    ff_utils.crawl_schema from snovault and logs any cases where there is an
-    error finding the field from the schema
+def process_aggregated_items(request):
+    """
+    After all aggregated items have been found, process them on the request
+    to narrow down to the fields we wish to aggregated on. This reduces the
+    amount of info carried on the request, which is important because it
+    will have to be carried through the subrequest chain.
 
     Args:
-        field (string): embedded field path, separated by '.'
-        request: current Request object
-        doc_types (list): @types for the search
-        should_log (bool): logging will only occur if set to True
+        request: the current request
 
     Returns:
-        Dictionary schema for the field, or None if not found
+        None
     """
-    types = request.registry[TYPES]
-    schemas = [types[dt].schema
-               for dt in doc_types]
-
-    # We cannot hash dict by list (of doc_types) so we convert to unique ordered string
-    doc_type_string = ','.join(doc_types)
-
-    cache = getattr(request, '_field_schema_cache', {})
-    if (field, doc_type_string) in cache:
-        return cache[(field, doc_type_string)]
-
-    field_schema = None
-
-    # for 'validation_errors.*' and 'aggregated_items.*',
-    # schema will never be found and logging isn't helpful
-    if (schemas
-            and not field.startswith('validation_errors.')
-            and not field.startswith('aggregated_items.')):
-        # 'type' field is really '@type' in the schema
-        use_field = '@type' if field == 'type' else field
-        # eliminate '!' from not fields
-        use_field = use_field[:-1] if use_field.endswith('!') else use_field
-        for schema in schemas:
-            try:
-                field_schema = crawl_schema(types, use_field, schema)
-            except Exception as exc:  # cannot find schema. Log and Return None
-                if should_log:
-                    log.warning(f'Cannot find schema in search.py. Type: {doc_types[0]}. Field: {field}',
-                                field=field, error=str(exc))
-            else:
-                if field_schema is not None:
-                    break
-
-    # Cache result, even if not found, for this request.
-    cache[(field, doc_type_string)] = field_schema
-    if not hasattr(request, '_field_schema_cache'):
-        setattr(request, '_field_schema_cache', cache)
-
-    return field_schema
-
-
-def is_linkto_or_object_array_root_field(field, types, doc_types):
-    """Not used currently. May be useful for if we want to enabled "type" : "nested" mappings on lists of dictionaries"""
-    schema = types[doc_types[0]].schema
-    field_root = field.split('.')[0]
-    fr_schema = (schema and schema.get('properties', {}).get(field_root, None)) or None
-    if fr_schema and fr_schema['type'] == 'array' and (fr_schema['items'].get('linkTo') is not None or fr_schema['items']['type'] == 'object'):
-        return True
-    return False
-
+    for agg_on, agg_body in request._aggregated_items.items():
+        covered_json_items = []  # compare agg items using json.dumps
+        item_idxs_to_remove = []  # remove these items after processing
+        agg_fields = agg_body['_fields']
+        # automatically aggregate on uuid if no fields provided
+        # if you want to change this default, also change in create_mapping
+        if not agg_fields:
+            agg_fields = ['uuid']
+        # handle badly formatted agg_fields here (?)
+        if not isinstance(agg_fields, list):
+            agg_fields = [agg_fields]
+        for agg_idx, agg_item in enumerate(agg_body['items']):
+            # deduplicate aggregated items by comparing sorted json
+            # use whole agg_item (w/ 'parent' and 'embedded_path') for dedup
+            if json.dumps(agg_item, sort_keys=True) in covered_json_items:
+                item_idxs_to_remove.append(agg_idx)
+                continue
+            covered_json_items.append(json.dumps(agg_item, sort_keys=True))
+            proc_item = {}
+            for field in agg_fields:
+                pointer = agg_item['item']
+                split_field = field.strip().split('.')
+                found_value = recursively_process_field(pointer, split_field)
+                # terminal dicts will create issues with the mapping. Print a warning and skip
+                if isinstance(found_value, dict):
+                    log.error('ERROR. Found dictionary terminal value for field %s when aggregating %s items.'
+                              ' Context is: %s'
+                              % (field, agg_on, str(request.context.uuid)))
+                    continue
+                proc_pointer = proc_item
+                for idx, split in enumerate(split_field):
+                    if idx == len(split_field) - 1:
+                        proc_pointer.update({split: found_value})
+                    else:
+                        if split not in proc_pointer:
+                            proc_pointer[split] = {}
+                        proc_pointer = proc_pointer[split]
+            # replace the unprocessed item with the processed one
+            agg_body['items'][agg_idx]['item'] = proc_item
+        # remove deduplicated items by index in reverse order
+        for dedup_idx in reversed(item_idxs_to_remove):
+            del agg_body['items'][dedup_idx]
 
-def generate_filters_for_terms_agg_from_search_filters(query_field, search_filters, string_query):
-    """
-    We add a copy of our filters to each facet, minus that of
-    facet's field itself so that we can get term counts for other terms filters.
-    And be able to filter w/ it.
 
-    Remove filters from fields they apply to.
-    For example, the 'biosource_type' aggs should not have any
-    biosource_type filter in place.
-    Handle 'must' and 'must_not' filters separately
+def recursively_process_field(item, split_fields):
+    """
+    Recursive function to pull out a field, in split-on-dot format, from
+    the given item. Example of split format is:
+        'subobject.value' --> ['subobject', 'value']
+    Args:
+        item: dictionary item to pull fields from
+        split_fields: list resulting from field.split('.')
 
-    Returns
-        Copy of search_filters, minus filter for current query_field (if one set).
+    Returns:
+        The found value
     """
+    try:
+        next_level = item.get(split_fields[0])
+    except AttributeError:
+        # happens if a string/int is encountered at the top level
+        return item
+    if next_level is None:
+        return None
+    if len(split_fields[1:]) == 0:
+        # we are at the end of the path
+        return next_level
+    elif isinstance(next_level, list):
+        return [recursively_process_field(entry, split_fields[1:]) for entry in next_level]
+    elif isinstance(next_level, dict):
+        # can't drill down anymore
+        return recursively_process_field(next_level, split_fields[1:])
+    else:
+        # can't drill down if not a list or dict. just return
+        return next_level
 
-    facet_filters = deepcopy(search_filters['bool'])
-
-    for filter_type in ['must', 'must_not']:
-        if not search_filters['bool'][filter_type]:
-            continue
-        for active_filter in search_filters['bool'][filter_type]:  # active_filter => e.g. { 'terms' : { 'embedded.@type.raw': ['ExperimentSetReplicate'] } }
-            if 'bool' in active_filter and 'should' in active_filter['bool']:
-                # handle No value case
-                inner_bool = None
-                inner_should = active_filter.get('bool').get('should', [])
-                for or_term in inner_should:
-                    # this may be naive, but assume first non-terms
-                    # filter is the No value quqery
-                    if 'terms' in or_term:
-                        continue
-                    else:
-                        inner_bool = or_term
-                        break
-                if 'exists' in inner_bool:
-                    compare_field = inner_bool['exists'].get('field')
-                else:
-                    # attempt to get the field from the alternative No value syntax
-                    compare_field = inner_bool.get('bool', {}).get('must_not', {}).get('exists', {}).get('field')
-                if compare_field == query_field and query_field != 'embedded.@type.raw':
-                    facet_filters[filter_type].remove(active_filter)
-
-            if 'terms' in active_filter:
-                # there should only be one key here
-                for compare_field in active_filter['terms'].keys():
-                    # remove filter for a given field for that facet
-                    # skip this for type facet (field = 'type')
-                    # since we always want to include that filter.
-                    if compare_field == query_field and query_field != 'embedded.@type.raw':
-                        facet_filters[filter_type].remove(active_filter)
-
-            elif 'range' in active_filter:
-                for compare_field in active_filter['range'].keys():
-                    # Do same as for terms
-                    if compare_field == query_field:
-                        facet_filters[filter_type].remove(active_filter)
-
-    # add the string_query, if present, to the bool term with facet_filters
-    if string_query and string_query['must']:
-        # combine statements within 'must' for each
-        facet_filters['must'].append(string_query['must'])
-
-    return facet_filters
-
-
-def set_facets(search, facets, search_filters, string_query, request, doc_types, custom_aggregations=None,
-               size=25, from_=0):
-    """
-    Sets facets in the query as ElasticSearch aggregations, with each aggregation to be
-    filtered by search_filters minus filter affecting facet field in order to get counts
-    for other facet term options.
-    ES5 - simply sets aggs by calling update_from_dict after adding them in
-
-        :param facets:         Facet field (0) in object dot notation, and a dict or OrderedDict with title property (1).
-        :type  facets:         List of tuples.
-        :param search_filters: Dict of filters which are set for the ES query in set_filters
-        :param string_query:   Dict holding the query_string used in the search
-    """
-
-    if from_ != 0:
-        return search
-
-    aggs = OrderedDict()
-
-    for field, facet in facets:  # E.g. 'type','experimentset_type','experiments_in_set.award.project', ...
-        field_schema = schema_for_field(field, request, doc_types, should_log=True)
-        is_date_field = field_schema and determine_if_is_date_field(field, field_schema)
-        is_numerical_field = field_schema and field_schema['type'] in ("integer", "float", "number")
-
-        if field == 'type':
-            query_field = 'embedded.@type.raw'
-        elif field.startswith('validation_errors') or field.startswith('aggregated_items'):
-            query_field = field + '.raw'
-        elif facet.get('aggregation_type') in ('stats', 'date_histogram', 'histogram', 'range'):
-            query_field = 'embedded.' + field
-        else:
-            query_field = 'embedded.' + field + '.raw'
 
-        # Create the aggregation itself, extend facet with info to pass down to front-end
-        agg_name = field.replace('.', '-')
+###########################
+# Resource view utilities #
+###########################
 
-        if facet.get('aggregation_type') == 'stats':
 
-            if is_date_field:
-                facet['field_type'] = 'date'
-            elif is_numerical_field:
-                facet['field_type'] = 'number'
-
-            aggs[facet['aggregation_type'] + ":" + agg_name] = {
-                'aggs': {
-                    "primary_agg": {
-                        'stats': {
-                            'field': query_field
-                        }
-                    }
-                },
-                'filter': search_filters
-            }
+def _sid_cache(request):
+    return request._sid_cache  # noQA. Centrally ignore that it's an access to a protected member.
 
-        else:  # Default -- facetable terms
 
-            facet['aggregation_type'] = 'terms'
-            facet_filters = generate_filters_for_terms_agg_from_search_filters(query_field, search_filters, string_query)
-            term_aggregation = {
-                "terms": {
-                    'size': 100,            # Maximum terms returned (default=10); see https://github.com/10up/ElasticPress/wiki/Working-with-Aggregations
-                    'field': query_field,
-                    'missing': facet.get("missing_value_replacement", "No value")
-                }
-            }
+def _sid_cache_update(request, new_value):
+    request._sid_cache.update(new_value)  # noQA. Centrally ignore that it's an access to a protected member.
 
-            aggs[facet['aggregation_type'] + ":" + agg_name] = {
-                'aggs': {
-                    "primary_agg": term_aggregation
-                },
-                'filter': {'bool': facet_filters},
-            }
 
-        # Update facet with title, description from field_schema, if missing.
-        if facet.get('title') is None and field_schema and 'title' in field_schema:
-            facet['title'] = field_schema['title']
-        if facet.get('description') is None and field_schema and 'description' in field_schema:
-            facet['description'] = field_schema['description']
-
-    # to achieve OR behavior within facets, search among GLOBAL results,
-    # not just returned ones. to do this, wrap aggs in ['all_items']
-    # and add "global": {} to top level aggs query
-    # see elasticsearch global aggs for documentation (should be ES5 compliant)
-    search_as_dict = search.to_dict()
-    search_as_dict['aggs'] = {
-        'all_items': {
-            'global': {},
-            'aggs': aggs
-        }
-    }
+def check_es_and_cache_linked_sids(context, request, view='embedded'):
+    """
+    For the given context and request, see if the desired item is present in
+    Elasticsearch and, if so, retrieve it cache all sids of the linked objects
+    that correspond to the given view. Store these in request's sid cache.
 
-    if size == 0:
-        # Only perform aggs if size==0 requested, to improve performance for search page queries.
-        # We do currently have (hidden) monthly date histogram facets which may yet to be utilized for common size!=0 agg use cases.
-        set_additional_aggregations(search_as_dict, request, doc_types, custom_aggregations)
+    Args:
+        context: current Item
+        request: current Request
+        view (str): 'embedded' or 'object', depending on the desired view
 
-    search.update_from_dict(search_as_dict)
-    return search
+    Returns:
+        The _source of the Elasticsearch result, if found. None otherwise
+    """
+    es_model = request.registry[STORAGE].get_by_uuid_direct(str(context.uuid), context.item_type)
+    if es_model is None:
+        return None
+    es_res = es_model.get('_source')
+    es_links_field = 'linked_uuids_object' if view == 'object' else 'linked_uuids_embedded'
+    if es_res and es_res.get(es_links_field):
+        linked_uuids = [link['uuid'] for link in es_res[es_links_field]
+                        if link['uuid'] not in _sid_cache(request)]
+        to_cache = request.registry[STORAGE].write.get_sids_by_uuids(linked_uuids)
+        _sid_cache_update(request, to_cache)
+        return es_res
+    return None
+
+
+def validate_es_content(context, request, es_res, view='embedded'):
+    """
+    For the given context, request, and found Elasticsearch result, determine
+    whether that result is valid. This depends on the view (either 'embedded' or
+    'object'). This is based off of the following:
+        1. All sids from the ES result must match those in request._sid_cache
+        2. All rev_links from the ES result must be up-to-date
+    This function will automatically add sids to _sid_cache from the DB if
+    they are not already present.
 
+    Args:
+        context: current Item
+        request: current Request
+        es_res (dict): dictionary Elasticsearch result
+        view (str): 'embedded' or 'object', depending on the desired view
 
-def set_additional_aggregations(search_as_dict, request, doc_types, extra_aggregations=None):
-    """
-    Per-type aggregations may be defined in schemas. Apply them OUTSIDE of globals so they act on our current search filters.
-    Warning: `search_as_dict` is modified IN PLACE.
+    Returns:
+        bool: True if es_res is valid, otherwise False
     """
+    if view not in ['object', 'embedded']:
+        return False
+    es_links_field = 'linked_uuids_object' if view == 'object' else 'linked_uuids_embedded'
+    linked_es_sids = es_res[es_links_field]
+    if not linked_es_sids:  # there should always be context.uuid here. abort
+        return False
+    use_es_result = True
+    # check to see if there are any new rev links from the item
+    for rev_name in context.rev:
+        # the call below updates request._rev_linked_uuids_by_item.
+        db_rev_uuids = context.get_filtered_rev_links(request, rev_name)
+        es_rev_uuids = es_res['rev_link_names'].get(rev_name, [])
+        if set(db_rev_uuids) != set(es_rev_uuids):
+            return False
+    for linked in linked_es_sids:
+        # infrequently, may need to add sids from the db to the _sid_cache
+        cached = _sid_cache(request)
+        found_sid = cached.get(linked['uuid'])
+        if not found_sid:
+            db_res = request.registry[STORAGE].write.get_by_uuid(linked['uuid'])
+            if db_res:
+                cached[linked['uuid']] = found_sid = db_res.sid
+        if found_sid is None or linked['sid'] < found_sid:
+            use_es_result = False
+            break
+    return use_es_result
 
-    types = request.registry[TYPES]
-    schema = types[doc_types[0]].schema
-
-    if schema.get('aggregations'):
-        for schema_agg_name in schema['aggregations'].keys():
-            if schema_agg_name == 'all_items':
-                raise Exception('all_items is a reserved agg name and not allowed as an extra aggregation name.')
-            search_as_dict['aggs'][schema_agg_name] = schema['aggregations'][schema_agg_name]
 
-    if extra_aggregations:
-        for extra_agg_name in extra_aggregations.keys():
-            if extra_agg_name == 'all_items':
-                raise Exception('all_items is a reserved agg name and not allowed as an extra aggregation name.')
-            search_as_dict['aggs'][extra_agg_name] = extra_aggregations[extra_agg_name]
+class CalculatedOverrideOfBasePropertiesNotPermitted(ValueError):
+    """ Helper exception for below method """
+    def __init__(self, calculated_props, base_props):
+        self.calculated_props = calculated_props
+        self.base_props = base_props
+        super().__init__('Calculated properties are not permitted to override'
+                         ' base properties of a sub-embedded object:'
+                         '\n calculated: %s'
+                         '\n base props: %s' % (calculated_props, base_props))
 
-    return search_as_dict
 
+def merge_calculated_into_properties(properties: dict, calculated: dict):
+    """ Performs a depth 2 dictionary merge into properties.
 
-def execute_search(search):
-    """
-    Execute the given Elasticsearch-dsl search. Raise HTTPBadRequest for any
-    exceptions that arise.
-    Args:
-        search: the Elasticsearch-dsl prepared in the search() function
-    Returns:
-        Dictionary search results
+    :param properties: base item properties
+    :param calculated: calculated properties
     """
-    err_exp = None
-    try:
-        es_results = search.execute().to_dict()
-    except ConnectionTimeout as exc:
-        ignored(exc)
-        err_exp = 'The search failed due to a timeout. Please try a different query.'
-    except RequestError as exc:
-        # try to get a specific error message. May fail in some cases
-        try:
-            err_detail = str(exc.info['error']['root_cause'][0]['reason'])
-        except Exception:
-            err_detail = str(exc)
-        err_exp = 'The search failed due to a request error: ' + err_detail
-    except TransportError as exc:
-        # most general exception
-        exc_status = getattr(exc, 'status_code')
-        if exc_status == 'TIMEOUT':
-            err_exp = 'The search failed due to a timeout. Please try a different query.'
+    for key, value in calculated.items():
+        if key not in properties:
+            properties[key] = value
         else:
-            err_exp = 'The search failed due to a transport error: ' + str(exc)
-    except Exception as exc:
-        ignored(exc)
-        err_exp = 'The search failed. The DCIC team has been notified.'
-    if err_exp:
-        raise HTTPBadRequest(explanation=err_exp)
-    return es_results  # noQA - PyCharm wrongly worries this might not have been set.
-
-
-def format_facets(es_results, facets, total, search_frame='embedded'):
-    """
-    Format the facets for the final results based on the es results.
-    Sort based off of the 'order' of the facets
-    These are stored within 'aggregations' of the result.
-
-    If the frame for the search != embedded, return no facets
-    """
-    ignored(total)
-    result = []
-    if search_frame != 'embedded':
-        return result
-
-    # Loading facets in to the results
-    if 'aggregations' not in es_results:
-        return result
-
-    aggregations = es_results['aggregations']['all_items']
-    used_facets = set()
-
-    # Sort facets by order (ascending).
-    # If no order is provided, assume 0 to
-    # retain order of non-explicitly ordered facets
-    for field, facet in sorted(facets, key=lambda fct: fct[1].get('order', 0)):
-        result_facet = {
-            'field': field,
-            'title': facet.get('title', field),
-            'total': 0
-            # To be added depending on facet['aggregation_type']: 'terms', 'min', 'max', 'min_as_string', 'max_as_string', ...
-        }
+            calculated_sub_values = calculated[key]
+            properties_sub_values = properties[key]
+            if isinstance(calculated_sub_values, dict) and isinstance(properties_sub_values, dict):
+                for k, v in calculated_sub_values.items():
+                    if k in properties_sub_values:
+                        raise CalculatedOverrideOfBasePropertiesNotPermitted(calculated_sub_values,
+                                                                             properties_sub_values)
+                    properties_sub_values[k] = v
+            elif isinstance(calculated_sub_values, list) and isinstance(properties_sub_values, list):
+                for calculated_entry, props_entry in zip(calculated_sub_values, properties_sub_values):
+                    for k, v in calculated_entry.items():
+                        if k in props_entry:
+                            raise CalculatedOverrideOfBasePropertiesNotPermitted(calculated_sub_values,
+                                                                                 properties_sub_values)
+                        props_entry[k] = v
+            else:
+                raise ValueError('Got unexpected types for calculated/properties sub-values: '
+                                 'calculated: %s \n properties: %s' % (calculated_sub_values, properties_sub_values))
 
-        result_facet.update({k: v
-                             for k, v in facet.items()
-                             if k not in result_facet.keys()})
-        used_facets.add(field)
-        field_agg_name = field.replace('.', '-')
-        full_agg_name = facet['aggregation_type'] + ':' + field_agg_name
-
-        if full_agg_name in aggregations:
-            if facet['aggregation_type'] == 'stats':
-                result_facet['total'] = aggregations[full_agg_name]['doc_count']
-                # Used for fields on which can do range filter on, to provide min + max bounds
-                for k in aggregations[full_agg_name]["primary_agg"].keys():
-                    result_facet[k] = aggregations[full_agg_name]["primary_agg"][k]
-            else:  # 'terms' assumed.
-                # Default - terms, range, or histogram buckets. Buckets may not be present
-                result_facet['terms'] = aggregations[full_agg_name]["primary_agg"]["buckets"]
-                # Choosing to show facets with one term for summary info on search it provides
-                if len(result_facet.get('terms', [])) < 1:
-                    continue
 
-            if len(aggregations[full_agg_name].keys()) > 2:
-                result_facet['extra_aggs'] = {k: v
-                                              for k, v in aggregations[field_agg_name].items()
-                                              if k not in ('doc_count', "primary_agg")}
+class CachedField:
+    def __init__(self, name, update_function, timeout=600):
+        """ Provides a named field that is cached for a certain period of time. The value is computed
+            on calls to __init__, after which the get() method should be used.
+
+        :param name: name of property
+        :param update_function: lambda to be invoked to update the value
+        :param timeout: TTL of this field, in seconds
+        """
+        self.name = name
+        self._update_function = update_function
+        self.timeout = timeout
+        self.value = update_function()
+        self.time_of_next_update = datetime.utcnow() + timedelta(seconds=timeout)
+
+    def _update_timestamp(self):
+        self.time_of_next_update = datetime.utcnow() + timedelta(seconds=self.timeout)
+
+    def _update_value(self):
+        self.value = self._update_function()
+        self._update_timestamp()
+
+    def get(self):
+        """ Intended for normal use - to get the value subject to the given TTL on creation. """
+        now = datetime.utcnow()
+        if now > self.time_of_next_update:
+            self._update_value()
+        return self.value
+
+    def get_updated(self, push_ttl=False):
+        """ Intended to force an update to the value and potentially push back the timeout from now. """
+        self.value = self._update_function()
+        if push_ttl:
+            self.time_of_next_update = datetime.utcnow() + timedelta(seconds=self.timeout)
+        return self.value
+
+    def set_timeout(self, new_timeout):
+        """ Sets a new value for timeout and restarts the timeout counter."""
+        self.timeout = new_timeout
+        self._update_timestamp()
+
+    def __repr__(self):
+        return 'CachedField %s with update function %s on timeout %s' % (
+            self.name, self._update_function, self.timeout
+        )
 
-        result.append(result_facet)
 
-    return result
+def generate_indexer_namespace_for_testing(prefix='sno'):
+    test_job_id = os.environ.get('TEST_JOB_ID') or os.environ.get('TRAVIS_JOB_ID')
+    if test_job_id:
+        if '-test-' in test_job_id:
+            # We need to manage some set of ids unchanged at the command line,
+            # so if the caller has segmented things, trust it to have added a repo prefix
+            # and just return it unaltered. -kmp 9-Mar-2021
+            return test_job_id
+        # Nowadays, this might be a GitHub run id, which isn't globally unique.
+        # Each repo is monotonic but at different pace and they can collide. Repo prefix is essential.
+        return "%s-test-%s-" % (prefix, test_job_id)
+    else:
+        # We've experimentally determined that it works pretty well to just use the timestamp.
+        return "%s-test-%s-" % (prefix, int(datetime_module.datetime.now().timestamp() * 1000000))
 
 
-def format_extra_aggregations(es_results):
-    if 'aggregations' not in es_results:
-        return {}
-    return {k: v
-            for k, v in es_results['aggregations'].items()
-            if k != 'all_items'}
+INDEXER_NAMESPACE_FOR_TESTING = generate_indexer_namespace_for_testing()
 
 
-def format_results(request, hits, search_frame):
+def is_admin_request(request):
+    """ Checks for 'group.admin' in effective_principals on request - if present we know this
+        request was submitted by an admin
     """
-    Loads results to pass onto UI
-    Will retrieve the desired frame from the search hits and automatically
-    add 'validation_errors' and 'aggregated_items' frames if they are present
-    """
-    fields_requested = request.normalized_params.getall('field')
-    if fields_requested:
-        frame = 'embedded'
-    elif search_frame:
-        frame = search_frame
-    else:
-        frame = 'embedded'
+    return 'group.admin' in request.effective_principals
 
-    if frame in ['embedded', 'object', 'raw']:
-        # transform 'raw' to 'properties', which is what is stored in ES
-        if frame == 'raw':
-            frame = 'properties'
-        for hit in hits:
-            frame_result = hit['_source'][frame]
-            if 'validation_errors' in hit['_source'] and 'validation_errors' not in frame_result:
-                frame_result['validation_errors'] = hit['_source']['validation_errors']
-            if 'aggregated_items' in hit['_source'] and 'aggregated_items' not in frame_result:
-                frame_result['aggregated_items'] = hit['_source']['aggregated_items']
-            yield frame_result
-        return
 
+def get_item_or_none(request, value, itype=None, frame='object'):
+    """
+    Return the view of an item with given frame. Can specify different types
+    of `value` for item lookup
 
-def find_index_by_doc_types(request, doc_types, ignore):
+    Args:
+        request: the current Request
+        value (str): String item identifier or a dict containing @id/uuid
+        itype (str): Optional string collection name for the item (e.g. /file-formats/)
+        frame (str): Optional frame to return. Defaults to 'object'
+
+    Returns:
+        dict: given view of the item or None on failure
     """
-    Find the correct index(es) to be search given a list of doc_types.
-    The types in doc_types are the item class names, formatted like
-    'Experiment HiC' and index names are the item types, formatted like
-    'experiment_hi_c'.
-    Ignore any collection names provided in the ignore param, an array.
-    Formats output indexes as a string usable by elasticsearch
-    """
-    indexes = []
-    for doc_type in doc_types:
-        if doc_type in ignore:
-            continue
-        else:
-            result = find_collection_subtypes(request.registry, doc_type)
-            namespaced_results = map(lambda t: get_namespaced_index(request, t), result)
-            indexes.extend(namespaced_results)
-    # remove any duplicates
-    indexes = list(set(indexes))
-    index_string = ','.join(indexes)
-    return index_string
-
-
-def make_search_subreq(request, path):
-    subreq = make_subrequest(request, path)
-    if hasattr(request, "_stats"):
-        subreq._stats = request._stats
-    subreq.registry = request.registry
-    if hasattr(request, "context"):
-        subreq.context = request.context
-    else:
-        subreq.context = None
-    subreq.headers['Accept'] = 'application/json'
-    return subreq
+    item = None
+
+    if isinstance(value, dict):
+        if 'uuid' in value:
+            value = value['uuid']
+        elif '@id' in value:
+            value = value['@id']
+
+    svalue = str(value)
+
+    # Below case is for UUIDs & unique_keys such as accessions, but not @ids
+    if not svalue.startswith('/') and not svalue.endswith('/'):
+        svalue = '/' + svalue + '/'
+        if itype is not None:
+            svalue = '/' + itype + svalue
+
+    # Request.embed will attempt to get from ES for frame=object/embedded
+    # If that fails, get from DB. Use '@@' syntax instead of 'frame=' because
+    # these paths are cached in indexing
+    try:
+        item = request.embed(svalue, '@@' + frame)
+    except Exception:
+        pass
+
+    # could lead to unexpected errors if == None
+    return item
 
 
-DEFAULT_BROWSE_PARAM_LISTS = {
-    'type': ["ExperimentSetReplicate"],
-    'experimentset_type': ['replicate'],
-    'award.project': ['4DN']
+CONTENT_TYPE_SPECIAL_CASES = {
+    'application/x-www-form-urlencoded': [
+        # Single legacy special case to allow us to POST to metadata TSV requests via form submission.
+        # All other special case values should be added using register_path_content_type.
+        '/metadata/',
+        '/variant-sample-search-spreadsheet/',
+        re.compile(r'/variant-sample-lists/[\da-z-]+/@@spreadsheet/'),
+    ]
 }
 
 
-def get_iterable_search_results(request, search_path='/search/', param_lists=None, **kwargs):
+def register_path_content_type(*, path, content_type):
     """
-    Loops through search results, returns 100 (or search_results_chunk_row_size) results at a time.
-    Pass it through itertools.chain.from_iterable to get one big iterable of results.
-    TODO: Maybe make 'limit=all', and instead of calling invoke_subrequest(subrequest), instead call iter_search_results!
-
-    :param request: Only needed to pass to do_subreq to make a subrequest with.
-    :param search_path: Root path to call, defaults to /search/ (can also use /browse/).
-    :param param_lists: Dictionary of param:lists_of_vals which is converted to URL query.
-    :param search_results_chunk_row_size: Amount of results to get per chunk. Default should be fine.
+    Registers that endpoints that begin with the specified path use the indicated content_type.
+
+    This is part of an inelegant workaround for an issue in renderers.py that maybe we can make go away in the future.
+    See the 'implementation note' in ingestion/common.py for more details.
     """
-    if param_lists is None:
-        param_lists = deepcopy(DEFAULT_BROWSE_PARAM_LISTS)
-    else:
-        param_lists = deepcopy(param_lists)
-    param_lists['limit'] = ['all']
-    param_lists['from'] = [0]  # TODO: Should be ['0'] ??
-    param_lists['sort'] = param_lists.get('sort', 'uuid')  # TODO: Default should be ['uuid'] ??
-    subreq = make_search_subreq(request, f'{search_path}?{urlencode(param_lists, True)}')
-    return iter_search_results(None, subreq, **kwargs)
-
-
-# Update? used in ./batch_download.py
-def iter_search_results(context, request, **kwargs):
-    return search(context, request, return_generator=True, **kwargs)
-
-
-def build_table_columns(request, schemas, doc_types):
-
-    any_abstract_types = 'Item' in doc_types
-    if not any_abstract_types:  # Check explictly-defined types to see if any are abstract.
-        type_infos = [request.registry[TYPES][type] for type in doc_types if type != 'Item']
-        for ti in type_infos:
-            # We use `type` instead of `isinstance` since we don't want to catch subclasses.
-            if type(ti) == AbstractTypeInfo:
-                any_abstract_types = True
-                break
-
-    columns = OrderedDict()
-
-    # Add title column, at beginning always
-    columns['display_title'] = {
-        "title": "Title",
-        "order": -100
-    }
-
-    # Add type column if any abstract types in search
-    if any_abstract_types and request.normalized_params.get('currentAction') != 'selection':
-        columns['@type'] = {
-            "title": "Item Type",
-            "colTitle": "Type",
-            "order": -80,
-            "description": "Type or category of Item",
-            # Alternative below, if we want type column to be available but hidden by default in selection mode:
-            # "default_hidden": request.normalized_params.get('currentAction') == 'selection'
-        }
+    exceptions = CONTENT_TYPE_SPECIAL_CASES.get(content_type, None)
+    if exceptions is None:
+        CONTENT_TYPE_SPECIAL_CASES[content_type] = exceptions = []
+    if path not in exceptions:
+        exceptions.append(path)
 
-    for schema in schemas:
-        if 'columns' in schema:
-            schema_columns = OrderedDict(schema['columns'])
-            # Add all columns defined in schema
-            for name, obj in schema_columns.items():
-                if name not in columns:
-                    columns[name] = obj
-                else:
-                    # If @type or display_title etc. column defined in schema, then override defaults.
-                    for prop in schema_columns[name]:
-                        columns[name][prop] = schema_columns[name][prop]
-                # Add description from field schema, if none otherwise.
-                if not columns[name].get('description'):
-                    field_schema = schema_for_field(name, request, doc_types)
-                    if field_schema:
-                        if field_schema.get('description') is not None:
-                            columns[name]['description'] = field_schema['description']
-
-    # Add status column, if not present, at end.
-    if 'status' not in columns:
-        columns['status'] = {
-            "title": "Status",
-            "default_hidden": True,
-            "order": 501
-        }
-    # Add date column, if not present, at end.
-    if 'date_created' not in columns:
-        columns['date_created'] = {
-            "title": "Date Created",
-            "colTitle": "Created",
-            "default_hidden": True,
-            "order": 510
-        }
-    return columns
 
+compiled_regexp_class = type(re.compile("foo.bar"))  # Hides that it's _sre.SRE_Pattern in 3.6, but re.Pattern in 3.7
 
-_ASSEMBLY_MAPPER = {
-    'GRCh38-minimal': 'hg38',
-    'GRCh38': 'hg38',
-    'GRCh37': 'hg19',
-    'GRCm38': 'mm10',
-    'GRCm37': 'mm9',
-    'BDGP6': 'dm4',
-    'BDGP5': 'dm3',
-    'WBcel235': 'WBcel235'
-}
 
-hgConnect = ''.join([
-    'http://genome.ucsc.edu/cgi-bin/hgTracks',
-    '?hubClear=',
-])
+def content_type_allowed(request):
+    """
+    Returns True if the current request allows the requested content type.
+
+    This is part of an inelegant workaround for an issue in renderers.py that maybe we can make go away in the future.
+    See the 'implementation note' in ingestion/common.py for more details.
+    """
+    if request.content_type == "application/json":
+        # For better or worse, we always allow this.
+        return True
+
+    exceptions = CONTENT_TYPE_SPECIAL_CASES.get(request.content_type)
+
+    if exceptions:
+        for path_condition in exceptions:
+            if isinstance(path_condition, str):
+                if path_condition in request.path:
+                    return True
+            elif isinstance(path_condition, compiled_regexp_class):
+                if path_condition.match(request.path):
+                    return True
+            else:
+                raise NotImplementedError(f"Unrecognized path_condition: {path_condition}")
+
+    return False
```

### Comparing `dcicsnovault-8.0.1/snovault/tests/serverfixtures.py` & `dcicsnovault-8.0.1.0b0/snovault/tests/serverfixtures.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     # SNOVAULT_DB_TEST_PORT,
     make_snovault_db_test_url,
 )
 
 
 NO_SERVER_FIXTURES = environ_bool("NO_SERVER_FIXTURES")
 
+
 def pytest_configure():
     logging.basicConfig(format='')
     logging.getLogger('sqlalchemy.engine').setLevel(logging.WARNING)
 
     class Shorten(logging.Filter):
         max_len = 500
```

### Comparing `dcicsnovault-8.0.1/snovault/tests/snowflake_hash.py` & `dcicsnovault-8.0.1.0b0/snovault/edw_hash.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 )
 from hashlib import sha384
 from passlib.registry import register_crypt_handler
 from passlib.utils import handlers as uh
 
 
 def includeme(config):
-    register_crypt_handler(SNOWHash)
+    register_crypt_handler(EDWHash)
 
 
-class SNOWHash(uh.StaticHandler):
-    """ a special snowflake of a  password hashing scheme
+class EDWHash(uh.StaticHandler):
+    """ EDW's password hashing scheme
 
     Cryptographic strength of the hashing function is less of a concern for
     randomly generated passwords.
     """
-    name = 'snowflake_hash'
+    name = 'edw_hash'
     checksum_chars = uh.PADDED_BASE64_CHARS
     checksum_size = 64
 
     setting_kwds = ('salt_before', 'salt_after', 'salt_base')
     salt_before = b"186ED79BAEXzeusdioIsdklnw88e86cd73"
     salt_after = b"<*#$*(#)!DSDFOUIHLjksdf"
     salt_base = b64decode(b"""\
```

### Comparing `dcicsnovault-8.0.1/snovault/tests/test_attachment.py` & `dcicsnovault-8.0.1.0b0/snovault/tests/test_attachment.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/tests/test_authentication.py` & `dcicsnovault-8.0.1.0b0/snovault/tests/test_authentication.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import unittest
 
 from pyramid.interfaces import IAuthenticationPolicy
 from pyramid.security import Authenticated, Everyone
 from pyramid.testing import DummyRequest
 from zope.interface.verify import verifyObject, verifyClass
-from .authentication import NamespacedAuthenticationPolicy
+from ..authentication import NamespacedAuthenticationPolicy
 
 
 class TestNamespacedAuthenticationPolicy(unittest.TestCase):
     """ This is a modified version of TestRemoteUserAuthenticationPolicy
     """
     def _getTargetClass(self):
         return NamespacedAuthenticationPolicy
@@ -27,47 +27,47 @@
 
     def test_unauthenticated_userid_returns_None(self):
         request = DummyRequest(environ={})
         policy = self._makeOne()
         self.assertEqual(policy.unauthenticated_userid(request), None)
 
     def test_unauthenticated_userid(self):
-        request = DummyRequest(environ={'REMOTE_USER':'fred'})
+        request = DummyRequest(environ={'REMOTE_USER': 'fred'})
         policy = self._makeOne()
         self.assertEqual(policy.unauthenticated_userid(request), 'user.fred')
 
     def test_authenticated_userid_None(self):
         request = DummyRequest(environ={})
         policy = self._makeOne()
         self.assertEqual(policy.authenticated_userid(request), None)
 
     def test_authenticated_userid(self):
-        request = DummyRequest(environ={'REMOTE_USER':'fred'})
+        request = DummyRequest(environ={'REMOTE_USER': 'fred'})
         policy = self._makeOne()
         self.assertEqual(policy.authenticated_userid(request), 'user.fred')
 
     def test_effective_principals_None(self):
         request = DummyRequest(environ={})
         policy = self._makeOne()
         self.assertEqual(policy.effective_principals(request), [Everyone])
 
     def test_effective_principals(self):
-        request = DummyRequest(environ={'REMOTE_USER':'fred'})
+        request = DummyRequest(environ={'REMOTE_USER': 'fred'})
         policy = self._makeOne()
         self.assertEqual(policy.effective_principals(request),
                          [Everyone, Authenticated, 'user.fred'])
 
     def test_remember(self):
         request = DummyRequest(environ={'REMOTE_USER':'fred'})
         policy = self._makeOne()
         result = policy.remember(request, 'fred')
         self.assertEqual(result, [])
 
     def test_forget(self):
-        request = DummyRequest(environ={'REMOTE_USER':'fred'})
+        request = DummyRequest(environ={'REMOTE_USER': 'fred'})
         policy = self._makeOne()
         result = policy.forget(request)
         self.assertEqual(result, [])
 
     # From TestSessionAuthenticationPolicy
 
     def test_session_remember(self):
```

### Comparing `dcicsnovault-8.0.1/snovault/tests/test_calculated.py` & `dcicsnovault-8.0.1.0b0/snovault/tests/test_calculated.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/tests/test_create_mapping.py` & `dcicsnovault-8.0.1.0b0/snovault/tests/test_create_mapping.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/tests/test_embed_utils.py` & `dcicsnovault-8.0.1.0b0/snovault/tests/test_embed_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,16 @@
         for emb in expected_embeds
     ]
     embs_to_add, _ = expand_embedded_list('EmbeddingTest', registry[TYPES], dummy_emb_list, schema_props, set())
     expected_to_add = [
         'attachment',
         'attachment.attachment.*',
         'attachment.attachment2.*',
-        'attachment.principals_allowed.*'
+        'attachment.principals_allowed.*',
+        'attachment.submitted_by'
     ]
     assert set(embs_to_add) == set(expected_to_add)
 
     # add default embeds for all items 'attachment'
     test_embed = ['attachment.attachment.*']
     embs_to_add2, _ = expand_embedded_list('EmbeddingTest', registry[TYPES], test_embed, schema_props, set())
     expected_to_add2 = ['attachment']
```

### Comparing `dcicsnovault-8.0.1/snovault/tests/test_embedding.py` & `dcicsnovault-8.0.1.0b0/snovault/tests/test_embedding.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/tests/test_es_permissions.py` & `dcicsnovault-8.0.1.0b0/snovault/tests/test_es_permissions.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/tests/test_indexing.py` & `dcicsnovault-8.0.1.0b0/snovault/tests/test_indexing.py`

 * *Files 12% similar despite different names*

```diff
@@ -50,19 +50,21 @@
 
 from .testing_views import TestingLinkSourceSno
 
 
 notice_pytest_fixtures(TestingLinkSourceSno)
 
 
-pytestmark = [pytest.mark.indexing]
+pytestmark = [pytest.mark.indexing, pytest.mark.es]
 
 
 TEST_COLL = '/testing-post-put-patch-sno/'
 TEST_TYPE = 'testing_post_put_patch_sno'  # use one collection for testing
+TEST_TYPE_HIDDEN_FACETS = 'testing_hidden_facets'
+TEST_TYPE_BUCKET_RANGE = 'testing_bucket_range_facets'
 
 # we just need single shard for these tests
 # XXX: use new type
 create_mapping.NUM_SHARDS = 1
 
 
 @pytest.fixture(scope='session')
@@ -90,15 +92,15 @@
     INDEXER_APP_PARAMS = [False]
 elif INDEXER_MODE == "BOTH":
     INDEXER_APP_PARAMS = [False, True]
 else:
     raise Exception("Bad value of INDEXER_MODE: %s. Possible values are MPINDEX, INDEX, and BOTH." % INDEXER_MODE)
 
 
-@pytest.fixture(scope='module', params=INDEXER_APP_PARAMS)  # must happen AFTER scope='session' moto setup
+@pytest.fixture(scope='session', params=INDEXER_APP_PARAMS)  # must happen AFTER scope='session' moto setup
 def app(app_settings, request):
     old_mpindexer = app_settings['mpindexer']
     with override_dict(app_settings, mpindexer=old_mpindexer):  # we plan to set it inside here
         if request.param:  # run tests both with and without mpindexer
             print("TEMPORARILY SETTING mpindexer=True in app_settings")
             app_settings['mpindexer'] = True  # This will get cleaned up by the override_dict
         app = main({}, **app_settings)
@@ -109,24 +111,26 @@
         try:
             DBSession.bind.pool.dispose()
         except AttributeError:
             # TODO: The .bind may be a connection, which doesn't have a .pool, so maybe sometime try this instead?
             #       DBSession.bind.engine.pool.dispose()
             pass
 
+
 # XXX C4-312: refactor tests so this can be module scope.
 # Having to have to drop DB tables and re-run create_mapping for every test is slow.
 @pytest.fixture(scope='function', autouse=True)
 def setup_and_teardown(app):
     """
     Run create mapping and purge queue before tests and clear out the
     DB tables after the test
     """
-    # BEFORE THE TEST - just run CM for the TEST_TYPE by default
-    create_mapping.run(app, collections=[TEST_TYPE], skip_indexing=True, purge_queue=True)
+    # BEFORE THE TEST - just run CM for the TEST_TYPEs above by default
+    create_mapping.run(app, collections=[TEST_TYPE, TEST_TYPE_HIDDEN_FACETS, TEST_TYPE_BUCKET_RANGE],
+                       skip_indexing=True, purge_queue=True)
 
     yield  # run the test
 
     # AFTER THE TEST
     session = app.registry[DBSESSION]
     connection = session.connection()  # was session.connection().connect(), rewritten for SA2.0
     # The reflect=True argument to MetaData was deprecated. Instead, one is supposed to call the .reflect()
@@ -206,15 +210,15 @@
         raw_idx = indexer_utils.get_namespaced_index(app, TEST_TYPE)
         star_idx = indexer_utils.get_namespaced_index(app.registry, '*')  # registry should work as well
         assert raw_idx == TEST_TYPE
         assert star_idx == '*'
         # app.registry.settings['indexer.namespace'] = indexer_namespace  # reset indexer_namespace
 
 
-@pytest.mark.es
+# @pytest.mark.es - Specified at top of file for whole file
 def test_indexer_queue_adds_telemetry_id(app):
     indexer_queue = app.registry[INDEXER_QUEUE]
     indexer_queue.clear_queue()
     test_message = 'abc123'
     telem = 'test_telemetry_id'
     to_index, failed = indexer_queue.add_uuids(app.registry, [test_message], strict=True,
                                                telemetry_id=telem)
@@ -228,15 +232,15 @@
     assert msg_body['strict'] is True
     assert msg_body['telemetry_id'] == telem
 
     # finally, delete
     indexer_queue.delete_messages(received)
 
 
-@pytest.mark.es
+# @pytest.mark.es - Specified at top of file for whole file
 @pytest.mark.flaky
 def test_indexer_queue(app):
     indexer_queue_mirror = app.registry[INDEXER_QUEUE_MIRROR]
     # An indexing queue mirror would only be set up for production servers.
     assert indexer_queue_mirror is None
 
     indexer_queue = app.registry[INDEXER_QUEUE]
@@ -1949,14 +1953,372 @@
     ])
     def test_invalidation_scope_view_error(self, indexer_testapp, req):
         """ Test failure cases """
         with pytest.raises(webtest.AppError):
             indexer_testapp.post_json('/compute_invalidation_scope', req)
 
 
+@pytest.fixture(scope='session')
+def hidden_facet_data_one():
+    """ Sample TestingHiddenFacets object we are going to facet on """
+    return {
+        'first_name': 'John',
+        'last_name': 'Doe',
+        'sid': 1,
+        'status': 'current',
+        'unfaceted_string': 'hello',
+        'unfaceted_integer': 123,
+        'disabled_string': 'orange',
+        'disabled_integer': 789,
+        'unfaceted_object': {
+            'mother': 'Anne',
+            'father': 'Bob'
+        },
+        'unfaceted_array_of_objects': [
+            {
+                'fruit': 'orange',
+                'color': 'orange',
+                'uid': 1
+            },
+            {
+                'fruit': 'banana',
+                'color': 'yellow',
+                'uid': 2
+            },
+        ]
+    }
+
+
+@pytest.fixture(scope='session')
+def hidden_facet_data_two():
+    """ A second sample TestingHiddenFacets object we are going to facet on """
+    return {
+        'first_name': 'Boston',
+        'last_name': 'Bruins',
+        'sid': 2,
+        'status': 'current',
+        'unfaceted_string': 'world',
+        'unfaceted_integer': 456,
+        'disabled_string': 'apple',
+        'disabled_integer': 101112,
+        'unfaceted_object': {
+            'mother': 'Candice',
+            'father': 'Doug'
+        },
+        'unfaceted_array_of_objects': [
+            {
+                'fruit': 'blueberry',
+                'color': 'blue',
+                'uid': 3
+            },
+            {
+                'fruit': 'mango',
+                'color': 'yellow',
+                'uid': 4
+            },
+        ]
+    }
+
+
+@pytest.fixture(scope='function')
+def hidden_facet_test_data(testapp, hidden_facet_data_one, hidden_facet_data_two):
+    testapp.post_json('/TestingHiddenFacets', hidden_facet_data_one, status=201)
+    testapp.post_json('/TestingHiddenFacets', hidden_facet_data_two, status=201)
+    index_n_items_for_testing(testapp, 2)
+
+
+class TestSearchHiddenAndAdditionalFacets:
+    """ Encapsulates tests meant for testing behavior associated with default_hidden, hidden
+        and additional_facets
+    """
+    DEFAULT_FACETS = ['first_name']  # 'validation_errors.name'
+    DEFAULT_HIDDEN_FACETS = ['last_name', 'sid']
+    ADDITIONAL_FACETS = ['unfaceted_string', 'unfaceted_integer']
+    DISABLED_FACETS = ['disabled_string', 'disabled_integer']
+
+    @staticmethod
+    def check_and_verify_result(facets, desired_facet, number_expected):
+        """ Helper method for later tests that checks terms count and average. """
+        for facet in facets:
+            field = facet['field']
+            if field == desired_facet and 'terms' in facet:
+                assert len(facet['terms']) == number_expected
+            elif field == facet and 'avg' in facet:
+                assert facet['avg'] == number_expected
+            else:
+                continue
+            break
+
+    @staticmethod
+    def assert_facet_set_equal(expected, facets):
+        """ Takes list of expect results and raw facet response and checks that they
+            are identical. """
+        assert sorted(expected) == sorted([facet['field'] for facet in facets])
+
+    def test_search_default_hidden_facets_dont_show(self, testapp, hidden_facet_test_data):
+        facets = testapp.get('/search/?type=TestingHiddenFacets').json['facets']
+        self.assert_facet_set_equal(self.DEFAULT_FACETS, facets)
+
+    @pytest.mark.parametrize('facet', ADDITIONAL_FACETS)
+    def test_search_one_additional_facet(self, testapp, hidden_facet_test_data, facet):
+        """ Tests that specifying each of the 'additional' facets works correctly """
+        facets = testapp.get('/search/?type=TestingHiddenFacets&additional_facet=%s' % facet).json['facets']
+        expected = self.DEFAULT_FACETS + [facet]
+        self.assert_facet_set_equal(expected, facets)
+
+    def test_search_multiple_additional_facets(self, testapp, hidden_facet_test_data):
+        """ Tests that enabling multiple additional facets works """
+        facets = testapp.get('/search/?type=TestingHiddenFacets'
+                                '&additional_facet=unfaceted_string'
+                                '&additional_facet=unfaceted_integer').json['facets']
+        expected = self.DEFAULT_FACETS + self.ADDITIONAL_FACETS
+        self.assert_facet_set_equal(expected, facets)
+        for facet in facets:  # verify facet type
+            if facet['field'] == 'unfaceted_integer':
+                assert facet['aggregation_type'] == 'stats'
+            else:  # facet['field'] == 'unfaceted_string'
+                assert facet['aggregation_type'] == 'terms'
+
+    @pytest.mark.parametrize('facet', DEFAULT_HIDDEN_FACETS)
+    def test_search_one_additional_default_hidden_facet(self, testapp, hidden_facet_test_data, facet):
+        """ Tests that passing default_hidden facets to additional_facets works correctly """
+        facets = testapp.get('/search/?type=TestingHiddenFacets&additional_facet=%s' % facet).json['facets']
+        expected = self.DEFAULT_FACETS + [facet]
+        self.assert_facet_set_equal(expected, facets)
+
+    def test_search_multiple_additional_default_hidden_facets(self, testapp, hidden_facet_test_data):
+        """ Tests that passing multiple hidden_facets as additionals works correctly """
+        facets = testapp.get('/search/?type=TestingHiddenFacets'
+                                '&additional_facet=last_name'
+                                '&additional_facet=sid').json['facets']
+        expected = self.DEFAULT_FACETS + self.DEFAULT_HIDDEN_FACETS
+        self.assert_facet_set_equal(expected, facets)
+        for facet in facets:
+            if facet['field'] == 'sid':
+                assert facet['aggregation_type'] == 'stats'
+            else:
+                assert facet['aggregation_type'] == 'terms'
+
+    @pytest.mark.parametrize('_facets', [
+        ['last_name', 'unfaceted_integer'],  # second slot holds number field
+        ['unfaceted_string', 'sid']
+    ])
+    def test_search_mixing_additional_and_default_hidden(self, testapp, hidden_facet_test_data, _facets):
+        """ Tests that we can mix additional_facets with those both on and off schema """
+        facets = testapp.get('/search/?type=TestingHiddenFacets'
+                                '&additional_facet=%s'
+                                '&additional_facet=%s' % (_facets[0], _facets[1])).json['facets']
+        expected = self.DEFAULT_FACETS + _facets
+        self.assert_facet_set_equal(expected, facets)
+        for facet in facets:
+            if facet['field'] == _facets[1]:  # second slot holds number field
+                assert facet['aggregation_type'] == 'stats'
+            else:
+                assert facet['aggregation_type'] == 'terms'
+
+    @pytest.mark.parametrize('_facet', DISABLED_FACETS)
+    def test_search_disabled_overrides_additional(self, testapp, hidden_facet_test_data, _facet):
+        """ Hidden facets should NEVER be faceted on """
+        facets = testapp.get('/search/?type=TestingHiddenFacets&additional_facet=%s' % _facet).json['facets']
+        field_names = [facet['field'] for facet in facets]
+        assert _facet not in field_names  # always hidden should not be here, even if specified
+
+    @pytest.mark.parametrize('_facets', [
+        ('last_name', 'unfaceted_integer', 'disabled_integer'),  # default_hidden second
+        ('sid', 'unfaceted_string', 'disabled_string')  # disabled always last
+    ])
+    def test_search_additional_mixing_disabled_default_hidden(self, testapp, hidden_facet_test_data, _facets):
+        """ Tests that supplying multiple additional facets combined with hidden still respects the
+            hidden restriction. """
+        facets = testapp.get('/search/?type=TestingHiddenFacets'
+                                '&additional_facet=%s'
+                                '&additional_facet=%s' 
+                                '&additional_facet=%s' % (_facets[0], _facets[1], _facets[2])).json['facets']
+        expected = self.DEFAULT_FACETS + [_facets[0], _facets[1]]  # first two should show
+        self.assert_facet_set_equal(expected, facets)
+
+    @pytest.mark.parametrize('_facet', [
+        'unfaceted_object.mother',
+        'unfaceted_object.father'
+    ])
+    def test_search_additional_object_facets(self, testapp, hidden_facet_test_data, _facet):
+        """ Tests that specifying an object field as an additional_facet works correctly """
+        facets = testapp.get('/search/?type=TestingHiddenFacets'
+                                '&additional_facet=%s' % _facet).json['facets']
+        expected = self.DEFAULT_FACETS + [_facet]
+        self.assert_facet_set_equal(expected, facets)
+
+    @pytest.mark.parametrize('_facet, n_expected', [
+        ('unfaceted_array_of_objects.fruit', 4),
+        ('unfaceted_array_of_objects.color', 3),
+        ('unfaceted_array_of_objects.uid', 2.5)  # stats avg
+    ])
+    def test_search_additional_nested_facets(self, testapp, hidden_facet_test_data, _facet, n_expected):
+        """ Tests that specifying an array of object field mapped with nested as an additional_facet
+            works correctly. """
+        [desired_facet] = [facet for facet in testapp.get('/search/?type=TestingHiddenFacets'
+                                                             '&additional_facet=%s' % _facet).json['facets']
+                           if facet['field'] == _facet]
+        if 'terms' in desired_facet:
+            assert len(desired_facet['terms']) == n_expected
+        else:
+            assert desired_facet['avg'] == n_expected
+
+    @pytest.fixture
+    def many_non_nested_facets(self, testapp, hidden_facet_test_data):
+        return testapp.get('/search/?type=TestingHiddenFacets'  
+                              '&additional_facet=non_nested_array_of_objects.fruit'
+                              '&additional_facet=non_nested_array_of_objects.color'
+                              '&additional_facet=non_nested_array_of_objects.uid').json['facets']
+
+    @pytest.mark.parametrize('_facet, n_expected', [
+        ('unfaceted_array_of_objects.fruit', 4),
+        ('unfaceted_array_of_objects.color', 3),
+        ('unfaceted_array_of_objects.uid', 2.5)  # stats avg
+    ])
+    def test_search_additional_non_nested_facets(self, many_non_nested_facets, _facet, n_expected):
+        """ Tests trying to facet on an array of objects field that is not nested, requesting
+            all at the same time.
+        """
+        self.check_and_verify_result(many_non_nested_facets, _facet, n_expected)
+
+
+@pytest.fixture(scope='session')
+def bucket_range_data_raw():
+    """ 9 objects with a numerical field we will bucket on.
+            'special_integer' has i in it.
+            'special_object_that_holds_integer' holds a single integer field with i as well
+            'array_of_objects_that_holds_integer' holds 2 objects that are mirrors of one another
+        +
+        1 object with a value for no_value_integer, to test that filtering on a field that sets
+        'add_no_value' to True will not filter documents with 'No value'.
+    """
+    entries = [{
+        'special_integer': i,
+        'special_object_that_holds_integer': {
+            'embedded_integer': i
+        },
+        'array_of_objects_that_holds_integer': [
+            {
+                'embedded_identifier': 'forward',
+                'embedded_integer': 0 if i < 5 else 9
+            },
+            {
+                'embedded_identifier': 'reverse',
+                'embedded_integer': 9 if i < 5 else 0
+            },
+        ]
+    } for i in range(10)]
+    # set no value int on the last element
+    entries[-1]['no_value_integer'] = 8
+    entries[-1]['no_value_integer_array'] = [8]
+    return entries
+
+
+@pytest.fixture(scope='function')
+def bucket_range_data(testapp, bucket_range_data_raw):
+    for entry in bucket_range_data_raw:
+        testapp.post_json('/TestingBucketRangeFacets', entry, status=201)
+    index_n_items_for_testing(testapp, 10)
+
+
+class TestSearchBucketRangeFacets:
+    """ Class that encapsulates tests for BucketRanges """
+
+    @staticmethod
+    def verify_facet_counts(facets, expected_fields, expected_cardinality, expected_count):
+        """ Checks for given expected facets, checking bucket cardinality and document count
+            Note that the actual range properties are trivial (we are not testing elasticsearch)
+        """
+        for facet in facets:
+            if facet['field'] in expected_fields:
+                assert len(facet['ranges']) == expected_cardinality
+                for bucket in facet['ranges']:
+                    assert bucket['doc_count'] == expected_count
+
+    @staticmethod
+    def verify_counts(response, expected_count):
+        assert len(response['@graph']) == expected_count
+
+    @staticmethod
+    def select_facet(facets, facet_name):
+        result = None
+        for facet in facets:
+            if facet['field'] == facet_name:
+                result = facet
+                break
+        return result
+
+    @pytest.mark.parametrize('expected_fields, expected_counts', [
+        (['special_integer'], 5),
+        (['special_object_that_holds_integer.embedded_integer'], 5),
+        (['array_of_objects_that_holds_integer.embedded_integer'], 10)
+    ])
+    def test_search_bucket_range_simple(self, testapp, bucket_range_data, expected_fields, expected_counts):
+        """ Tests searching a collection of documents with varying integer field types that
+            have the same distribution - all of which should give the same results. """
+        res = testapp.get('/search/?type=TestingBucketRangeFacets').json['facets']
+        self.verify_facet_counts(res, expected_fields, 2, expected_counts)
+
+    # XXX: The following 2 tests don't function correctly because the facet doesn't utilize reverse_nested
+    @pytest.mark.parametrize('identifier', [
+        'reverse', 'forward'
+    ])
+    def test_search_bucket_range_nested_qualifier(self, testapp, bucket_range_data, identifier):
+        """ Tests aggregating on a nested field while selecting for a field within the nested object. """
+        res = testapp.get('/search/?type=TestingBucketRangeFacets'
+                             '&array_of_objects_that_holds_integer.embedded_identifier=%s' % identifier).json['facets']
+        self.verify_facet_counts(res, ['array_of_objects_that_holds_integer.embedded_integer'],
+                                 2, 10)
+
+    @pytest.mark.parametrize('identifier', [
+        'reverse', 'forward'
+    ])
+    def test_search_bucket_range_nested_qualifier_multiple(self, testapp, bucket_range_data, identifier):
+        """ Tests aggregating on a nested field while selecting for a field within the nested object (no change). """
+        res = testapp.get('/search/?type=TestingBucketRangeFacets'
+                             '&array_of_objects_that_holds_integer.embedded_integer.from=6'
+                             '&array_of_objects_that_holds_integer.embedded_identifier=%s' % identifier).json['facets']
+        self.verify_facet_counts(res, ['array_of_objects_that_holds_integer.embedded_integer'],
+                                 2, 10)
+        facet_with_labels = self.select_facet(res, 'array_of_objects_that_holds_integer.embedded_integer')
+        for r in facet_with_labels['ranges']:
+            assert 'label' in r
+            assert r['label'] in ['Low', 'High']
+
+    def test_search_bucket_range_add_no_value(self, testapp, bucket_range_data):
+        """ Tests that providing a range filter on a field that specifies 'add_no_value' does not
+            filter documents that have no value for that field.
+        """
+        res = testapp.get('/search/?type=TestingBucketRangeFacets&no_value_integer.from=0').json  # should detect
+        self.verify_counts(res, 10)
+        testapp.get('/search/?type=TestingBucketRangeFacets&no_value_integer.from=10', status=404)  # should not detect
+        res = testapp.get('/search/?type=TestingBucketRangeFacets&no_value_integer.to=10').json  # should detect
+        self.verify_counts(res, 10)
+        res = testapp.get('/search/?type=TestingBucketRangeFacets&no_value_integer.from=0'
+                             '&no_value_integer.to=10').json  # should detect
+        self.verify_counts(res, 10)
+        res = testapp.get('/search/?type=TestingBucketRangeFacets'
+                             '&no_value_integer_array.from=0').json  # should detect
+        self.verify_counts(res, 10)
+        res = testapp.get('/search/?type=TestingBucketRangeFacets'
+                             '&no_value_integer_array.from=8').json  # should detect
+        self.verify_counts(res, 1)
+        res = testapp.get('/search/?type=TestingBucketRangeFacets'
+                             '&no_value_integer_array.from=0&no_value_integer_array.to=7').json  # should detect
+        self.verify_counts(res, 9)
+        res = testapp.get('/search/?type=TestingBucketRangeFacets'
+                             '&no_value_integer_array.from=-1&no_value_integer_array.to=7').json  # should detect
+        self.verify_counts(res, 9)
+        res = testapp.get('/search/?type=TestingBucketRangeFacets'
+                             '&no_value_integer_array.from=-1&no_value_integer_array.to=9').json  # should detect
+        self.verify_counts(res, 10)
+
+
+
 def test_assert_transactions_table_is_gone(app):
     """
     A bit of a strange location for this test, but we need the app and
     serverfixtures to be established (used for indexing)
     """
     session = app.registry[DBSESSION]
     conn = session.connection()
```

### Comparing `dcicsnovault-8.0.1/snovault/tests/test_invalidation_scope.py` & `dcicsnovault-8.0.1.0b0/snovault/tests/test_invalidation_scope.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/tests/test_key.py` & `dcicsnovault-8.0.1.0b0/snovault/tests/test_key.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import pytest
 
 from dcicutils.qa_utils import notice_pytest_fixtures
-from pyramid.config import Configurator
-from ..interfaces import DBSESSION
 
 
 # Test for storage.keys
 
 items = [
     {'name': 'one', 'accession': 'TEST1'},
     {'name': 'two', 'accession': 'TEST2'},
@@ -14,24 +12,14 @@
 
 bad_items = [
     {'name': 'one', 'accession': 'BAD1'},
     {'name': 'bad', 'accession': 'TEST1'},
 ]
 
 
-@pytest.fixture(scope='session')
-def app(DBSession):
-    notice_pytest_fixtures(DBSession)
-    config = Configurator()
-    config.registry[DBSESSION] = DBSession
-    config.include('snovault')
-    config.include('.testing_key')
-    return config.make_wsgi_app()
-
-
 @pytest.fixture
 def content(testapp):
     notice_pytest_fixtures(testapp)
     url = '/testing-keys/'
     for item in items:
         testapp.post_json(url, item, status=201)
```

### Comparing `dcicsnovault-8.0.1/snovault/tests/test_link.py` & `dcicsnovault-8.0.1.0b0/snovault/tests/test_link.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/tests/test_logging.py` & `dcicsnovault-8.0.1.0b0/snovault/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/tests/test_misc.py` & `dcicsnovault-8.0.1.0b0/snovault/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/tests/test_post_put_patch.py` & `dcicsnovault-8.0.1.0b0/snovault/tests/test_post_put_patch.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/tests/test_postgresql_fixture.py` & `dcicsnovault-8.0.1.0b0/snovault/tests/test_postgresql_fixture.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/tests/test_schemas.py` & `dcicsnovault-8.0.1.0b0/snovault/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/tests/test_serverfixtures.py` & `dcicsnovault-8.0.1.0b0/snovault/tests/test_serverfixtures.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/tests/test_standalone_dev.py` & `dcicsnovault-8.0.1.0b0/snovault/tests/test_standalone_dev.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/tests/test_stats.py` & `dcicsnovault-8.0.1.0b0/snovault/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/tests/test_storage.py` & `dcicsnovault-8.0.1.0b0/snovault/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/tests/test_upgrader.py` & `dcicsnovault-8.0.1.0b0/snovault/tests/test_upgrader.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/tests/test_util.py` & `dcicsnovault-8.0.1.0b0/snovault/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/tests/test_views.py` & `dcicsnovault-8.0.1.0b0/snovault/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/tests/testappfixtures.py` & `dcicsnovault-8.0.1.0b0/snovault/tests/testappfixtures.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,29 +28,29 @@
                 'prompt': 'select_account'
             }
         },
         'allowedConnections': [
             'github', 'google-oauth2', 'partners'
         ]
     },
-    'multiauth.policies': 'session remoteuser accesskey webuser',
-    'multiauth.groupfinder': 'snovault.tests.authorization.groupfinder',
-    'multiauth.policy.session.use': 'snovault.tests.authentication.NamespacedAuthenticationPolicy',
+    'multiauth.policies': 'session remoteuser accesskey auth0',
+    'multiauth.groupfinder': 'snovault.authorization.groupfinder',
+    'multiauth.policy.session.use': 'snovault.authentication.NamespacedAuthenticationPolicy',
     'multiauth.policy.session.base': 'pyramid.authentication.SessionAuthenticationPolicy',
     'multiauth.policy.session.namespace': 'mailto',
-    'multiauth.policy.remoteuser.use': 'snovault.tests.authentication.NamespacedAuthenticationPolicy',
+    'multiauth.policy.remoteuser.use': 'snovault.authentication.NamespacedAuthenticationPolicy',
     'multiauth.policy.remoteuser.namespace': 'remoteuser',
     'multiauth.policy.remoteuser.base': 'pyramid.authentication.RemoteUserAuthenticationPolicy',
-    'multiauth.policy.accesskey.use': 'snovault.tests.authentication.NamespacedAuthenticationPolicy',
+    'multiauth.policy.accesskey.use': 'snovault.authentication.NamespacedAuthenticationPolicy',
     'multiauth.policy.accesskey.namespace': 'accesskey',
-    'multiauth.policy.accesskey.base': 'snovault.tests.authentication.BasicAuthAuthenticationPolicy',
-    'multiauth.policy.accesskey.check': 'snovault.tests.authentication.basic_auth_check',
-    'multiauth.policy.webuser.use':  'snovault.tests.authentication.NamespacedAuthenticationPolicy',
-    'multiauth.policy.webuser.namespace': 'webuser',
-    'multiauth.policy.webuser.base': 'snovault.tests.authentication.WebUserAuthenticationPolicy'
+    'multiauth.policy.accesskey.base': 'snovault.authentication.BasicAuthAuthenticationPolicy',
+    'multiauth.policy.accesskey.check': 'snovault.authentication.basic_auth_check',
+    'multiauth.policy.auth0.use': 'snovault.authentication.NamespacedAuthenticationPolicy',
+    'multiauth.policy.auth0.namespace': 'auth0',
+    'multiauth.policy.auth0.base': 'snovault.authentication.Auth0AuthenticationPolicy',
 }
 
 
 @pytest.fixture(scope="session")
 def basic_app_settings():
     return _app_settings.copy()
 
@@ -89,15 +89,15 @@
     environ = {
         'HTTP_ACCEPT': 'application/json',
         'REMOTE_USER': 'TEST',
     }
     return webtest.TestApp(encrypted_app, environ)
 
 
-@pytest.fixture
+@pytest.fixture(scope='session')
 def testapp(app):
     """ TestApp with JSON accept header. """
     environ = {
         'HTTP_ACCEPT': 'application/json',
         'REMOTE_USER': 'TEST',
     }
     return webtest.TestApp(app, environ)
```

### Comparing `dcicsnovault-8.0.1/snovault/tests/testing_upgrader.py` & `dcicsnovault-8.0.1.0b0/snovault/tests/testing_upgrader.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/tests/testing_views.py` & `dcicsnovault-8.0.1.0b0/snovault/tests/testing_views.py`

 * *Files 22% similar despite different names*

```diff
@@ -424,14 +424,46 @@
     },
 )
 class TestingDownload(ItemWithAttachment):
     item_type = 'testing_download'
     schema = load_schema('snovault:test_schemas/TestingDownload.json')
 
 
+@view_config(name='drs', context=TestingDownload, request_method='GET',
+             permission='view', subpath_segments=[0, 1])
+def drs(context, request):
+    """ Example DRS object implementation. Write this for all object classes that
+        you want to render a DRS object. This structure is minimally validated by the
+        downstream API (see drs.py).
+    """
+    rendered_object = request.embed(str(context.uuid), '@@object', as_user=True)
+    drs_object = {
+        'id': rendered_object['@id'],
+        'created_time': rendered_object['date_created'],
+        'drs_id': rendered_object['uuid'],
+        'self_uri': f'drs://{request.host}{request.path}',
+        'size': 0,
+        'checksums': [
+            {
+                'checksum': 'something',
+                'type': 'md5'
+            }
+        ],
+        'access_methods': [
+            {
+                'access_url': {
+                    'url': f'http://{request.host}/{context.uuid}/@@download'
+                },
+                'type': 'http'
+            },
+        ]
+    }
+    return drs_object
+
+
 @collection('testing-link-sources-sno', unique_key='testing_link_sources-sno:name')
 class TestingLinkSourceSno(Item):
     item_type = 'testing_link_source_sno'
     schema = load_schema('snovault:test_schemas/TestingLinkSourceSno.json')
     embedded_list = ['target_es.status', 'target.status']
 
 
@@ -802,7 +834,230 @@
     name_key = 'name'
     schema = load_schema('snovault:test_schemas/TestingBiogroupSno.json')
     embedded_list = [
         'sources.counter',  # get the counter
         'sources.samples.*',  # embed everything at top level
         'sources.contributor.*'
     ]
+
+
+@collection(
+    'testing-keys',
+    properties={
+        'title': 'Test keys',
+        'description': 'Testing. Testing. 1, 2, 3.',
+    },
+    unique_key='testing_accession',
+)
+class TestingKey(Item):
+    item_type = 'testing_key'
+    schema = {
+        'type': 'object',
+        'properties': {
+            'name': {
+                'type': 'string',
+                'uniqueKey': True,
+            },
+            'accession': {
+                'type': 'string',
+                'uniqueKey': 'testing_accession',
+            },
+        }
+    }
+
+
+@collection('testing-hidden-facets')
+class TestingHiddenFacets(Item):
+    """ Collection designed to test searching with hidden facets. Yes this is large, but this is a complex feature
+        with many possible cases. """
+    item_type = 'testing_hidden_facets'
+    schema = {
+        'type': 'object',
+        'properties': {
+            'first_name': {
+                'type': 'string'
+            },
+            'last_name': {
+                'type': 'string'
+            },
+            'sid': {
+                'type': 'integer'
+            },
+            'unfaceted_string': {
+                'type': 'string'
+            },
+            'unfaceted_integer': {
+                'type': 'integer'
+            },
+            'disabled_string': {
+                'type': 'string',
+            },
+            'disabled_integer': {
+                'type': 'integer',
+            },
+            'unfaceted_object': {
+                'type': 'object',
+                'properties': {
+                    'mother': {
+                        'type': 'string'
+                    },
+                    'father': {
+                        'type': 'string'
+                    }
+                }
+            },
+            'unfaceted_array_of_objects': {
+                'type': 'array',
+                'enable_nested': True,
+                'items': {
+                    'type': 'object',
+                    'properties': {
+                        'fruit': {
+                            'type': 'string'
+                        },
+                        'color': {
+                            'type': 'string'
+                        },
+                        'uid': {
+                            'type': 'integer'
+                        }
+                    }
+                }
+            }
+        },
+        'facets': {
+            'first_name': {
+                'title': 'First Name'
+            },
+            'last_name': {
+                'default_hidden': True,
+                'title': 'Last Name'
+            },
+            'sid': {
+                'default_hidden': True,
+                'title': 'SID',
+                'aggregation_type': 'stats',
+                'number_step': 1
+            },
+            'disabled_string': {
+                'disabled': True
+            },
+            'disabled_integer': {
+                'disabled': True
+            }
+        }
+    }
+
+    @calculated_property(schema={
+        'type': 'array',
+        'items': {
+            'type': 'object',
+            'properties': {
+                'fruit': {
+                    'type': 'string'
+                },
+                'color': {
+                    'type': 'string'
+                },
+                'uid': {
+                    'type': 'integer'
+                }
+            }
+        }
+    })
+    def non_nested_array_of_objects(self, unfaceted_array_of_objects):
+        """ Non-nested view of the unfaceted_array_of_objects field """
+        return unfaceted_array_of_objects
+
+
+@collection('testing-bucket-range-facets')
+class TestingBucketRangeFacets(Item):
+    """ Collection for testing BucketRange facets.
+        Also tests 'add_no_value' schema param behavior.
+    """
+    item_type = 'testing_bucket_range_facets'
+    schema = {
+        'type': 'object',
+        'properties': {
+            'no_value_integer': {
+                'type': 'integer',
+                'add_no_value': True  # if a range query is specified on this field, include documents that
+                                      # have 'No value' for the field
+            },
+            'no_value_integer_array': {
+                'type': 'array',
+                'items': {
+                    'type': 'integer',
+                    'add_no_value': True
+                }
+            },
+            'special_integer': {
+                'type': 'integer'
+            },
+            'special_object_that_holds_integer': {
+                'type': 'object',
+                'properties': {
+                    'embedded_integer': {
+                        'type': 'integer'
+                    }
+                }
+            },
+            'array_of_objects_that_holds_integer': {
+                'type': 'array',
+                'items': {
+                    'type': 'object',
+                    'enable_nested': False,
+                    'properties': {
+                        'embedded_identifier': {
+                            'type': 'string'
+                        },
+                        'embedded_integer': {
+                            'type': 'integer'
+                        }
+                    }
+                }
+            }
+        },
+        'facets': {
+            'no_value_integer': {
+                'title': 'No value integer',
+                'aggregation_type': 'range',
+                'ranges': [
+                    {'from': 0, 'to': 5},
+                    {'from': 5, 'to': 10}
+                ]
+            },
+            'no_value_integer_array': {
+                'title': 'No value integer array',
+                'aggregation_type': 'range',
+                'ranges': [
+                    {'from': 0, 'to': 0},  # test zero range faceting behavior
+                    {'from': 0, 'to': 5},
+                    {'from': 5, 'to': 10}
+                ]
+            },
+            'special_integer': {
+                'title': 'Special Integer',
+                'aggregation_type': 'range',
+                'ranges': [
+                    {'from': 0, 'to': 5},
+                    {'from': 5, 'to': 10}
+                ]
+            },
+            'special_object_that_holds_integer.embedded_integer': {
+                'title': 'Single Object Embedded Integer',
+                'aggregation_type': 'range',
+                'ranges': [
+                    {'from': 0, 'to': 5},
+                    {'from': 5, 'to': 10}
+                ]
+            },
+            'array_of_objects_that_holds_integer.embedded_integer': {
+                'title': 'Array of Objects Embedded Integer',
+                'aggregation_type': 'range',
+                'ranges': [
+                    {'from': 0, 'to': 5, 'label': 'Low'},
+                    {'from': 5, 'to': 10, 'label': 'High'}
+                ]
+            }
+        }
+    }
```

### Comparing `dcicsnovault-8.0.1/snovault/tests/toolfixtures.py` & `dcicsnovault-8.0.1.0b0/snovault/tests/toolfixtures.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/tools.py` & `dcicsnovault-8.0.1.0b0/snovault/tools.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/typeinfo.py` & `dcicsnovault-8.0.1.0b0/snovault/typeinfo.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/upgrader.py` & `dcicsnovault-8.0.1.0b0/snovault/upgrader.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/validation.py` & `dcicsnovault-8.0.1.0b0/snovault/validation.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/snovault/validators.py` & `dcicsnovault-8.0.1.0b0/snovault/validators.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1/PKG-INFO` & `dcicsnovault-8.0.1.0b0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: dcicsnovault
-Version: 8.0.1
+Version: 8.0.1.0b0
 Summary: Storage support for 4DN Data Portals.
 Home-page: https://github.com/4dn-dcic/snovault
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
-Requires-Python: >=3.8.1,<3.9
+Requires-Python: >=3.8.1,<3.10
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pyramid
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Database :: Database Engines/Servers
 Requires-Dist: PyBrowserID (>=0.10.0,<1)
 Requires-Dist: SPARQLWrapper (>=1.8.5,<2.0.0)
 Requires-Dist: SQLAlchemy (>=1.4.41,<2.0.0)
 Requires-Dist: WSGIProxy2 (==0.4.2)
@@ -32,14 +33,15 @@
 Requires-Dist: html5lib (>=1.1)
 Requires-Dist: humanfriendly (>=1.44.9,<2.0.0)
 Requires-Dist: jsonschema_serialize_fork (>=2.1.1,<3.0.0)
 Requires-Dist: netaddr (>=0.8.0,<1)
 Requires-Dist: passlib (>=1.7.4,<2.0.0)
 Requires-Dist: psutil (>=5.9.0,<6.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.1,<3.0.0)
+Requires-Dist: pyjwt (>=2.6.0,<3.0.0)
 Requires-Dist: pyramid (==1.10.4)
 Requires-Dist: pyramid-multiauth (>=0.9.0,<1)
 Requires-Dist: pyramid-retry (>=1.0,<2.0)
 Requires-Dist: pyramid-tm (>=2.5,<3.0)
 Requires-Dist: pyramid-translogger (>=0.1,<0.2)
 Requires-Dist: pyramid_localroles (>=0.1,<1)
 Requires-Dist: pytest-redis (>=2.0.0,<3.0.0)
```

