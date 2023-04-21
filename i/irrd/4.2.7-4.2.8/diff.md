# Comparing `tmp/irrd-4.2.7.tar.gz` & `tmp/irrd-4.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irrd-4.2.7.tar", last modified: Wed Feb 15 09:29:37 2023, max compression
+gzip compressed data, was "irrd-4.2.8.tar", last modified: Wed Apr 19 11:33:40 2023, max compression
```

## Comparing `irrd-4.2.7.tar` & `irrd-4.2.8.tar`

### file list

```diff
@@ -1,133 +1,275 @@
-drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-02-15 09:29:37.475542 irrd-4.2.7/
--rw-r--r--   0 sasha      (501) staff       (20)     3780 2023-02-10 10:32:21.000000 irrd-4.2.7/LICENSE
--rw-r--r--   0 sasha      (501) staff       (20)     2912 2023-02-15 09:29:37.475731 irrd-4.2.7/PKG-INFO
--rw-r--r--   0 sasha      (501) staff       (20)     2209 2022-06-22 14:54:59.000000 irrd-4.2.7/README.rst
-drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-02-15 09:29:37.414053 irrd-4.2.7/irrd/
--rw-r--r--   0 sasha      (501) staff       (20)       69 2023-02-15 09:29:07.000000 irrd-4.2.7/irrd/__init__.py
-drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-02-15 09:29:37.418935 irrd-4.2.7/irrd/conf/
--rw-r--r--   0 sasha      (501) staff       (20)    19785 2023-02-15 09:28:42.000000 irrd-4.2.7/irrd/conf/__init__.py
--rw-r--r--   0 sasha      (501) staff       (20)     2586 2023-02-15 09:28:40.000000 irrd-4.2.7/irrd/conf/default_config.yaml
--rw-r--r--   0 sasha      (501) staff       (20)      188 2023-01-05 13:14:13.000000 irrd-4.2.7/irrd/conf/defaults.py
--rw-r--r--   0 sasha      (501) staff       (20)    14923 2023-02-15 09:28:42.000000 irrd-4.2.7/irrd/conf/test_conf.py
-drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-02-15 09:29:37.419616 irrd-4.2.7/irrd/daemon/
--rw-r--r--   0 sasha      (501) staff       (20)        0 2020-11-10 14:53:47.000000 irrd-4.2.7/irrd/daemon/__init__.py
--rwxr-xr-x   0 sasha      (501) staff       (20)     7232 2023-02-15 09:28:40.000000 irrd-4.2.7/irrd/daemon/main.py
-drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-02-15 09:29:37.422521 irrd-4.2.7/irrd/mirroring/
--rw-r--r--   0 sasha      (501) staff       (20)        0 2018-08-22 10:47:06.000000 irrd-4.2.7/irrd/mirroring/__init__.py
--rw-r--r--   0 sasha      (501) staff       (20)     3838 2023-02-01 19:41:43.000000 irrd-4.2.7/irrd/mirroring/mirror_runners_export.py
--rw-r--r--   0 sasha      (501) staff       (20)    16245 2023-02-15 09:28:40.000000 irrd-4.2.7/irrd/mirroring/mirror_runners_import.py
--rw-r--r--   0 sasha      (501) staff       (20)     3860 2023-02-15 09:28:42.000000 irrd-4.2.7/irrd/mirroring/nrtm_generator.py
--rw-r--r--   0 sasha      (501) staff       (20)     5085 2023-02-01 19:41:43.000000 irrd-4.2.7/irrd/mirroring/nrtm_operation.py
--rw-r--r--   0 sasha      (501) staff       (20)    19716 2023-02-01 19:41:43.000000 irrd-4.2.7/irrd/mirroring/parsers.py
--rw-r--r--   0 sasha      (501) staff       (20)     6461 2023-02-01 19:41:43.000000 irrd-4.2.7/irrd/mirroring/scheduler.py
-drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-02-15 09:29:37.424740 irrd-4.2.7/irrd/rpki/
--rw-r--r--   0 sasha      (501) staff       (20)        0 2020-11-10 14:53:47.000000 irrd-4.2.7/irrd/rpki/__init__.py
--rw-r--r--   0 sasha      (501) staff       (20)     9467 2023-01-05 13:20:40.000000 irrd-4.2.7/irrd/rpki/importer.py
--rw-r--r--   0 sasha      (501) staff       (20)     5071 2023-02-15 09:28:40.000000 irrd-4.2.7/irrd/rpki/notifications.py
--rw-r--r--   0 sasha      (501) staff       (20)      115 2023-02-01 19:41:43.000000 irrd-4.2.7/irrd/rpki/status.py
--rw-r--r--   0 sasha      (501) staff       (20)     9248 2023-02-15 09:28:40.000000 irrd-4.2.7/irrd/rpki/validators.py
-drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-02-15 09:29:37.427577 irrd-4.2.7/irrd/rpsl/
--rw-r--r--   0 sasha      (501) staff       (20)        0 2020-10-12 17:35:22.000000 irrd-4.2.7/irrd/rpsl/__init__.py
--rw-r--r--   0 sasha      (501) staff       (20)      122 2023-02-15 09:28:40.000000 irrd-4.2.7/irrd/rpsl/config.py
--rw-r--r--   0 sasha      (501) staff       (20)    24126 2023-02-15 09:28:40.000000 irrd-4.2.7/irrd/rpsl/fields.py
--rw-r--r--   0 sasha      (501) staff       (20)    22222 2023-02-15 09:28:40.000000 irrd-4.2.7/irrd/rpsl/parser.py
--rw-r--r--   0 sasha      (501) staff       (20)     1614 2023-02-15 09:28:40.000000 irrd-4.2.7/irrd/rpsl/parser_state.py
--rw-r--r--   0 sasha      (501) staff       (20)    27633 2023-02-15 09:28:40.000000 irrd-4.2.7/irrd/rpsl/rpsl_objects.py
-drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-02-15 09:29:37.429329 irrd-4.2.7/irrd/scopefilter/
--rw-r--r--   0 sasha      (501) staff       (20)        0 2020-11-10 14:53:47.000000 irrd-4.2.7/irrd/scopefilter/__init__.py
--rw-r--r--   0 sasha      (501) staff       (20)      152 2023-02-01 19:41:43.000000 irrd-4.2.7/irrd/scopefilter/status.py
--rw-r--r--   0 sasha      (501) staff       (20)     6354 2023-02-15 09:28:40.000000 irrd-4.2.7/irrd/scopefilter/validators.py
-drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-02-15 09:29:37.440948 irrd-4.2.7/irrd/scripts/
--rw-r--r--   0 sasha      (501) staff       (20)        0 2018-05-11 14:51:11.000000 irrd-4.2.7/irrd/scripts/__init__.py
--rwxr-xr-x   0 sasha      (501) staff       (20)     1243 2023-01-05 13:20:40.000000 irrd-4.2.7/irrd/scripts/database_downgrade.py
--rwxr-xr-x   0 sasha      (501) staff       (20)     1228 2023-01-05 13:20:40.000000 irrd-4.2.7/irrd/scripts/database_upgrade.py
--rwxr-xr-x   0 sasha      (501) staff       (20)     2406 2023-01-05 13:20:40.000000 irrd-4.2.7/irrd/scripts/load_database.py
--rwxr-xr-x   0 sasha      (501) staff       (20)     1859 2023-01-05 13:20:40.000000 irrd-4.2.7/irrd/scripts/load_pgp_keys.py
--rwxr-xr-x   0 sasha      (501) staff       (20)     1472 2023-01-05 13:20:40.000000 irrd-4.2.7/irrd/scripts/load_test.py
--rwxr-xr-x   0 sasha      (501) staff       (20)     1236 2023-01-05 13:20:40.000000 irrd-4.2.7/irrd/scripts/mirror_force_reload.py
--rwxr-xr-x   0 sasha      (501) staff       (20)     8954 2023-01-05 13:20:40.000000 irrd-4.2.7/irrd/scripts/query_qa_comparison.py
--rwxr-xr-x   0 sasha      (501) staff       (20)     4499 2023-01-05 13:20:40.000000 irrd-4.2.7/irrd/scripts/rpsl_read.py
--rwxr-xr-x   0 sasha      (501) staff       (20)     2169 2023-01-05 13:20:40.000000 irrd-4.2.7/irrd/scripts/set_last_modified_auth.py
--rwxr-xr-x   0 sasha      (501) staff       (20)     1281 2023-01-05 13:20:40.000000 irrd-4.2.7/irrd/scripts/submit_changes.py
--rwxr-xr-x   0 sasha      (501) staff       (20)     1464 2023-01-05 13:20:40.000000 irrd-4.2.7/irrd/scripts/submit_email.py
--rw-r--r--   0 sasha      (501) staff       (20)     2176 2023-01-05 13:20:40.000000 irrd-4.2.7/irrd/scripts/update_database.py
-drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-02-15 09:29:37.443113 irrd-4.2.7/irrd/server/
--rw-r--r--   0 sasha      (501) staff       (20)        0 2018-07-06 10:44:00.000000 irrd-4.2.7/irrd/server/__init__.py
--rw-r--r--   0 sasha      (501) staff       (20)     1490 2023-02-15 09:28:40.000000 irrd-4.2.7/irrd/server/access_check.py
-drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-02-15 09:29:37.446960 irrd-4.2.7/irrd/server/graphql/
--rw-r--r--   0 sasha      (501) staff       (20)       67 2023-01-05 13:14:13.000000 irrd-4.2.7/irrd/server/graphql/__init__.py
--rw-r--r--   0 sasha      (501) staff       (20)     1887 2023-01-05 13:20:40.000000 irrd-4.2.7/irrd/server/graphql/extensions.py
--rw-r--r--   0 sasha      (501) staff       (20)    13936 2023-02-01 19:41:43.000000 irrd-4.2.7/irrd/server/graphql/resolvers.py
--rw-r--r--   0 sasha      (501) staff       (20)     3430 2023-01-05 13:20:40.000000 irrd-4.2.7/irrd/server/graphql/schema_builder.py
--rw-r--r--   0 sasha      (501) staff       (20)    12876 2023-02-01 19:41:43.000000 irrd-4.2.7/irrd/server/graphql/schema_generator.py
-drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-02-15 09:29:37.449857 irrd-4.2.7/irrd/server/http/
--rw-r--r--   0 sasha      (501) staff       (20)        0 2018-09-25 09:23:35.000000 irrd-4.2.7/irrd/server/http/__init__.py
--rw-r--r--   0 sasha      (501) staff       (20)     2958 2023-02-15 09:28:40.000000 irrd-4.2.7/irrd/server/http/app.py
--rw-r--r--   0 sasha      (501) staff       (20)     3406 2023-02-15 09:28:40.000000 irrd-4.2.7/irrd/server/http/endpoints.py
--rw-r--r--   0 sasha      (501) staff       (20)     1359 2023-02-15 09:28:40.000000 irrd-4.2.7/irrd/server/http/server.py
--rw-r--r--   0 sasha      (501) staff       (20)     8129 2023-02-01 19:41:43.000000 irrd-4.2.7/irrd/server/http/status_generator.py
--rw-r--r--   0 sasha      (501) staff       (20)    18566 2023-02-15 09:28:40.000000 irrd-4.2.7/irrd/server/query_resolver.py
--rw-r--r--   0 sasha      (501) staff       (20)     2019 2023-01-05 13:20:40.000000 irrd-4.2.7/irrd/server/test_access_check.py
-drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-02-15 09:29:37.452679 irrd-4.2.7/irrd/server/whois/
--rw-r--r--   0 sasha      (501) staff       (20)        0 2018-07-06 10:44:00.000000 irrd-4.2.7/irrd/server/whois/__init__.py
--rw-r--r--   0 sasha      (501) staff       (20)    23973 2023-02-15 09:28:40.000000 irrd-4.2.7/irrd/server/whois/query_parser.py
--rw-r--r--   0 sasha      (501) staff       (20)     3535 2023-01-05 13:20:40.000000 irrd-4.2.7/irrd/server/whois/query_response.py
--rw-r--r--   0 sasha      (501) staff       (20)     8709 2023-02-15 09:28:40.000000 irrd-4.2.7/irrd/server/whois/server.py
-drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-02-15 09:29:37.455541 irrd-4.2.7/irrd/storage/
--rw-r--r--   0 sasha      (501) staff       (20)     1496 2023-02-15 09:28:40.000000 irrd-4.2.7/irrd/storage/__init__.py
-drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-02-15 09:29:37.457093 irrd-4.2.7/irrd/storage/alembic/
--rw-r--r--   0 sasha      (501) staff       (20)        0 2018-08-22 10:47:06.000000 irrd-4.2.7/irrd/storage/alembic/__init__.py
--rw-r--r--   0 sasha      (501) staff       (20)     1765 2023-01-05 13:20:40.000000 irrd-4.2.7/irrd/storage/alembic/env.py
--rw-r--r--   0 sasha      (501) staff       (20)      494 2018-08-22 10:47:06.000000 irrd-4.2.7/irrd/storage/alembic/script.py.mako
-drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-02-15 09:29:37.467739 irrd-4.2.7/irrd/storage/alembic/versions/
--rw-r--r--   0 sasha      (501) staff       (20)      594 2023-01-05 13:14:13.000000 irrd-4.2.7/irrd/storage/alembic/versions/1743f98a456d_add_serial_newest_mirror.py
--rw-r--r--   0 sasha      (501) staff       (20)     1226 2023-01-05 13:20:40.000000 irrd-4.2.7/irrd/storage/alembic/versions/181670a62643_add_journal_entry_origin.py
--rw-r--r--   0 sasha      (501) staff       (20)    10369 2023-01-05 13:20:40.000000 irrd-4.2.7/irrd/storage/alembic/versions/28dc1cd85bdc_initial_db.py
--rw-r--r--   0 sasha      (501) staff       (20)     1401 2023-01-05 13:20:40.000000 irrd-4.2.7/irrd/storage/alembic/versions/39e4f15ed80c_add_bogon_status.py
--rw-r--r--   0 sasha      (501) staff       (20)     2251 2023-01-05 13:20:40.000000 irrd-4.2.7/irrd/storage/alembic/versions/4a514ead8fc2_bogon_to_scope_filter.py
--rw-r--r--   0 sasha      (501) staff       (20)     1145 2023-01-05 13:20:40.000000 irrd-4.2.7/irrd/storage/alembic/versions/64a3d6faf6d4_add_prefix_length_rpki_status_to_rpsl_objects.py
--rw-r--r--   0 sasha      (501) staff       (20)     1049 2023-01-05 13:20:40.000000 irrd-4.2.7/irrd/storage/alembic/versions/8744b4b906bb_fix_rpsl_unique_key.py
--rw-r--r--   0 sasha      (501) staff       (20)      550 2023-01-05 13:20:40.000000 irrd-4.2.7/irrd/storage/alembic/versions/893d0d5363b3_add_rpsl_prefix_idx.py
--rw-r--r--   0 sasha      (501) staff       (20)        0 2018-08-22 10:47:06.000000 irrd-4.2.7/irrd/storage/alembic/versions/__init__.py
--rw-r--r--   0 sasha      (501) staff       (20)     1083 2023-01-05 13:20:40.000000 irrd-4.2.7/irrd/storage/alembic/versions/a7766c144d61_add_synchronised_serial_to_database_.py
--rw-r--r--   0 sasha      (501) staff       (20)     1518 2023-01-05 13:20:40.000000 irrd-4.2.7/irrd/storage/alembic/versions/a8609af97aa3_set_prefix_length_in_existing_rpsl_.py
--rw-r--r--   0 sasha      (501) staff       (20)      510 2023-01-05 13:20:40.000000 irrd-4.2.7/irrd/storage/alembic/versions/b175c262448f_set_rpsl_prefix.py
--rw-r--r--   0 sasha      (501) staff       (20)     1713 2023-01-05 13:20:40.000000 irrd-4.2.7/irrd/storage/alembic/versions/e07863eac52f_add_roa_object_table.py
--rw-r--r--   0 sasha      (501) staff       (20)      511 2023-01-05 13:14:13.000000 irrd-4.2.7/irrd/storage/alembic/versions/f4c837d8258c_add_rpsl_prefix.py
--rw-r--r--   0 sasha      (501) staff       (20)    34740 2023-02-15 09:28:40.000000 irrd-4.2.7/irrd/storage/database_handler.py
--rw-r--r--   0 sasha      (501) staff       (20)     8347 2023-02-15 09:28:40.000000 irrd-4.2.7/irrd/storage/models.py
--rw-r--r--   0 sasha      (501) staff       (20)    15540 2023-02-15 09:28:40.000000 irrd-4.2.7/irrd/storage/preload.py
--rw-r--r--   0 sasha      (501) staff       (20)    20251 2023-02-15 09:28:40.000000 irrd-4.2.7/irrd/storage/queries.py
-drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-02-15 09:29:37.470209 irrd-4.2.7/irrd/updates/
--rw-r--r--   0 sasha      (501) staff       (20)        0 2018-07-31 14:50:32.000000 irrd-4.2.7/irrd/updates/__init__.py
--rw-r--r--   0 sasha      (501) staff       (20)     2831 2023-02-10 10:32:21.000000 irrd-4.2.7/irrd/updates/email.py
--rw-r--r--   0 sasha      (501) staff       (20)    13269 2023-02-15 09:28:40.000000 irrd-4.2.7/irrd/updates/handler.py
--rw-r--r--   0 sasha      (501) staff       (20)    19472 2023-02-15 09:28:40.000000 irrd-4.2.7/irrd/updates/parser.py
--rw-r--r--   0 sasha      (501) staff       (20)      654 2023-02-15 09:28:40.000000 irrd-4.2.7/irrd/updates/parser_state.py
--rw-r--r--   0 sasha      (501) staff       (20)    16514 2023-02-15 09:28:40.000000 irrd-4.2.7/irrd/updates/validators.py
-drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-02-15 09:29:37.473854 irrd-4.2.7/irrd/utils/
--rw-r--r--   0 sasha      (501) staff       (20)        0 2023-01-30 15:26:42.000000 irrd-4.2.7/irrd/utils/__init__.py
--rw-r--r--   0 sasha      (501) staff       (20)     3290 2023-02-10 10:32:21.000000 irrd-4.2.7/irrd/utils/email.py
--rw-r--r--   0 sasha      (501) staff       (20)     3000 2023-02-15 09:28:40.000000 irrd-4.2.7/irrd/utils/pgp.py
--rw-r--r--   0 sasha      (501) staff       (20)     1612 2023-02-09 20:20:50.000000 irrd-4.2.7/irrd/utils/process_support.py
--rw-r--r--   0 sasha      (501) staff       (20)    40716 2023-02-15 09:28:40.000000 irrd-4.2.7/irrd/utils/rpsl_samples.py
--rw-r--r--   0 sasha      (501) staff       (20)      800 2023-02-15 09:28:40.000000 irrd-4.2.7/irrd/utils/test_utils.py
--rw-r--r--   0 sasha      (501) staff       (20)     3521 2023-02-15 09:28:40.000000 irrd-4.2.7/irrd/utils/text.py
--rw-r--r--   0 sasha      (501) staff       (20)     2252 2023-02-15 09:28:40.000000 irrd-4.2.7/irrd/utils/validators.py
--rw-r--r--   0 sasha      (501) staff       (20)     4752 2023-02-15 09:28:40.000000 irrd-4.2.7/irrd/utils/whois_client.py
-drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-02-15 09:29:37.474148 irrd-4.2.7/irrd/vendor/
--rw-r--r--   0 sasha      (501) staff       (20)        0 2020-11-10 14:53:47.000000 irrd-4.2.7/irrd/vendor/__init__.py
-drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-02-15 09:29:37.474621 irrd-4.2.7/irrd/vendor/dotted/
--rw-r--r--   0 sasha      (501) staff       (20)        0 2022-06-22 14:54:59.000000 irrd-4.2.7/irrd/vendor/dotted/__init__.py
--rw-r--r--   0 sasha      (501) staff       (20)    12374 2023-02-15 09:28:40.000000 irrd-4.2.7/irrd/vendor/dotted/collection.py
-drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-02-15 09:29:37.475129 irrd-4.2.7/irrd/vendor/postgres_copy/
--rw-r--r--   0 sasha      (501) staff       (20)     6359 2023-02-15 09:28:40.000000 irrd-4.2.7/irrd/vendor/postgres_copy/__init__.py
-drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-02-15 09:29:37.416742 irrd-4.2.7/irrd.egg-info/
--rw-r--r--   0 sasha      (501) staff       (20)     2912 2023-02-15 09:29:37.000000 irrd-4.2.7/irrd.egg-info/PKG-INFO
--rw-r--r--   0 sasha      (501) staff       (20)     3571 2023-02-15 09:29:37.000000 irrd-4.2.7/irrd.egg-info/SOURCES.txt
--rw-r--r--   0 sasha      (501) staff       (20)        1 2023-02-15 09:29:37.000000 irrd-4.2.7/irrd.egg-info/dependency_links.txt
--rw-r--r--   0 sasha      (501) staff       (20)      519 2023-02-15 09:29:37.000000 irrd-4.2.7/irrd.egg-info/entry_points.txt
--rw-r--r--   0 sasha      (501) staff       (20)      625 2023-02-15 09:29:37.000000 irrd-4.2.7/irrd.egg-info/requires.txt
--rw-r--r--   0 sasha      (501) staff       (20)        5 2023-02-15 09:29:37.000000 irrd-4.2.7/irrd.egg-info/top_level.txt
--rw-r--r--   0 sasha      (501) staff       (20)      782 2023-02-15 09:29:37.476599 irrd-4.2.7/setup.cfg
--rwxr-xr-x   0 sasha      (501) staff       (20)     3096 2023-02-15 09:28:40.000000 irrd-4.2.7/setup.py
+drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-04-19 11:33:40.007154 irrd-4.2.8/
+drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-04-19 11:33:39.775033 irrd-4.2.8/.circleci/
+-rw-r--r--   0 sasha      (501) staff       (20)     6602 2023-04-19 11:28:23.000000 irrd-4.2.8/.circleci/config.yml
+-rw-r--r--   0 sasha      (501) staff       (20)      859 2023-04-19 11:28:23.000000 irrd-4.2.8/.coveragerc
+drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-04-19 11:33:39.746613 irrd-4.2.8/.github/
+drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-04-19 11:33:39.776923 irrd-4.2.8/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 sasha      (501) staff       (20)      560 2018-12-20 15:44:20.000000 irrd-4.2.8/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 sasha      (501) staff       (20)      592 2018-12-20 15:44:20.000000 irrd-4.2.8/.github/ISSUE_TEMPLATE/new-feature-requests.md
+-rw-r--r--   0 sasha      (501) staff       (20)      193 2022-06-22 14:54:59.000000 irrd-4.2.8/.gitignore
+-rw-r--r--   0 sasha      (501) staff       (20)      127 2018-05-07 13:20:05.000000 irrd-4.2.8/.pyup.yml
+-rw-r--r--   0 sasha      (501) staff       (20)     3184 2022-06-22 14:54:59.000000 irrd-4.2.8/CONTRIBUTING.md
+-rw-r--r--   0 sasha      (501) staff       (20)     3780 2023-04-19 10:20:23.000000 irrd-4.2.8/LICENSE
+-rw-r--r--   0 sasha      (501) staff       (20)     2912 2023-04-19 11:33:40.007454 irrd-4.2.8/PKG-INFO
+-rw-r--r--   0 sasha      (501) staff       (20)     2209 2022-06-22 14:54:59.000000 irrd-4.2.8/README.rst
+-rw-r--r--   0 sasha      (501) staff       (20)     2254 2022-06-22 14:54:59.000000 irrd-4.2.8/SECURITY.rst
+-rw-r--r--   0 sasha      (501) staff       (20)       78 2018-12-11 13:18:23.000000 irrd-4.2.8/alembic.ini
+-rw-r--r--   0 sasha      (501) staff       (20)     2195 2023-04-19 10:20:23.000000 irrd-4.2.8/conftest.py
+drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-04-19 11:33:39.782940 irrd-4.2.8/docs/
+-rw-r--r--   0 sasha      (501) staff       (20)      619 2021-06-28 13:39:26.000000 irrd-4.2.8/docs/Makefile
+drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-04-19 11:33:39.783898 irrd-4.2.8/docs/_static/
+-rw-r--r--   0 sasha      (501) staff       (20)    63722 2021-06-28 13:39:26.000000 irrd-4.2.8/docs/_static/logo.png
+drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-04-19 11:33:39.793893 irrd-4.2.8/docs/admins/
+-rw-r--r--   0 sasha      (501) staff       (20)    12688 2023-02-23 13:04:37.000000 irrd-4.2.8/docs/admins/availability-and-migration.rst
+-rw-r--r--   0 sasha      (501) staff       (20)    37400 2023-04-19 11:28:23.000000 irrd-4.2.8/docs/admins/configuration.rst
+-rw-r--r--   0 sasha      (501) staff       (20)    13000 2023-04-19 11:28:23.000000 irrd-4.2.8/docs/admins/deployment.rst
+-rw-r--r--   0 sasha      (501) staff       (20)     1619 2022-06-22 14:54:59.000000 irrd-4.2.8/docs/admins/faq.rst
+-rw-r--r--   0 sasha      (501) staff       (20)     5147 2022-06-22 14:54:59.000000 irrd-4.2.8/docs/admins/migrating-legacy-irrd.rst
+-rw-r--r--   0 sasha      (501) staff       (20)     5833 2023-04-19 11:28:23.000000 irrd-4.2.8/docs/admins/object-validation.rst
+-rw-r--r--   0 sasha      (501) staff       (20)     8830 2023-04-19 11:28:23.000000 irrd-4.2.8/docs/admins/rpki.rst
+-rw-r--r--   0 sasha      (501) staff       (20)     3677 2023-04-19 11:28:23.000000 irrd-4.2.8/docs/admins/scopefilter.rst
+-rw-r--r--   0 sasha      (501) staff       (20)     3218 2022-06-22 14:54:59.000000 irrd-4.2.8/docs/admins/status_page.rst
+-rwxr-xr-x   0 sasha      (501) staff       (20)     5487 2023-04-19 11:28:23.000000 irrd-4.2.8/docs/conf.py
+drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-04-19 11:33:39.797260 irrd-4.2.8/docs/development/
+-rw-r--r--   0 sasha      (501) staff       (20)    19639 2022-06-22 14:54:59.000000 irrd-4.2.8/docs/development/architecture.rst
+-rw-r--r--   0 sasha      (501) staff       (20)     5383 2023-04-19 11:28:23.000000 irrd-4.2.8/docs/development/development-setup.rst
+-rw-r--r--   0 sasha      (501) staff       (20)     9604 2021-06-28 13:39:26.000000 irrd-4.2.8/docs/development/storage.rst
+-rw-r--r--   0 sasha      (501) staff       (20)     3155 2023-04-19 11:28:23.000000 irrd-4.2.8/docs/index.rst
+-rw-r--r--   0 sasha      (501) staff       (20)       49 2021-06-28 13:39:26.000000 irrd-4.2.8/docs/license.rst
+-rw-r--r--   0 sasha      (501) staff       (20)      780 2021-06-28 13:39:26.000000 irrd-4.2.8/docs/make.bat
+drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-04-19 11:33:39.829248 irrd-4.2.8/docs/releases/
+-rw-r--r--   0 sasha      (501) staff       (20)      618 2021-06-28 13:39:26.000000 irrd-4.2.8/docs/releases/4.0.1.rst
+-rw-r--r--   0 sasha      (501) staff       (20)      957 2021-06-28 13:39:26.000000 irrd-4.2.8/docs/releases/4.0.2.rst
+-rw-r--r--   0 sasha      (501) staff       (20)     1099 2021-06-28 13:39:26.000000 irrd-4.2.8/docs/releases/4.0.3.rst
+-rw-r--r--   0 sasha      (501) staff       (20)      710 2021-06-28 13:39:26.000000 irrd-4.2.8/docs/releases/4.0.4.rst
+-rw-r--r--   0 sasha      (501) staff       (20)      502 2021-06-28 13:39:26.000000 irrd-4.2.8/docs/releases/4.0.5.rst
+-rw-r--r--   0 sasha      (501) staff       (20)      420 2021-06-28 13:39:26.000000 irrd-4.2.8/docs/releases/4.0.6.rst
+-rw-r--r--   0 sasha      (501) staff       (20)      404 2021-06-28 13:39:26.000000 irrd-4.2.8/docs/releases/4.0.7.rst
+-rw-r--r--   0 sasha      (501) staff       (20)      353 2021-06-28 13:39:26.000000 irrd-4.2.8/docs/releases/4.0.8.rst
+-rw-r--r--   0 sasha      (501) staff       (20)     8974 2023-04-19 11:28:23.000000 irrd-4.2.8/docs/releases/4.1.0.rst
+-rw-r--r--   0 sasha      (501) staff       (20)      342 2021-06-28 13:39:26.000000 irrd-4.2.8/docs/releases/4.1.1.rst
+-rw-r--r--   0 sasha      (501) staff       (20)     1259 2021-06-28 13:39:26.000000 irrd-4.2.8/docs/releases/4.1.2.rst
+-rw-r--r--   0 sasha      (501) staff       (20)     1327 2021-06-28 13:39:26.000000 irrd-4.2.8/docs/releases/4.1.3.rst
+-rw-r--r--   0 sasha      (501) staff       (20)      564 2021-06-28 13:39:26.000000 irrd-4.2.8/docs/releases/4.1.4.rst
+-rw-r--r--   0 sasha      (501) staff       (20)     1429 2021-08-23 13:43:15.000000 irrd-4.2.8/docs/releases/4.1.5.rst
+-rw-r--r--   0 sasha      (501) staff       (20)      349 2021-08-30 18:30:20.000000 irrd-4.2.8/docs/releases/4.1.6.rst
+-rw-r--r--   0 sasha      (501) staff       (20)      755 2021-09-07 17:56:33.000000 irrd-4.2.8/docs/releases/4.1.7.rst
+-rw-r--r--   0 sasha      (501) staff       (20)      712 2022-03-31 09:45:31.000000 irrd-4.2.8/docs/releases/4.1.8.rst
+-rw-r--r--   0 sasha      (501) staff       (20)     8090 2022-06-22 14:54:59.000000 irrd-4.2.8/docs/releases/4.2.0.rst
+-rw-r--r--   0 sasha      (501) staff       (20)      763 2022-03-31 09:45:31.000000 irrd-4.2.8/docs/releases/4.2.1.rst
+-rw-r--r--   0 sasha      (501) staff       (20)     2914 2022-06-22 14:54:59.000000 irrd-4.2.8/docs/releases/4.2.2.rst
+-rw-r--r--   0 sasha      (501) staff       (20)     4449 2023-04-19 11:28:23.000000 irrd-4.2.8/docs/releases/4.2.3.rst
+-rw-r--r--   0 sasha      (501) staff       (20)      827 2022-06-22 14:54:59.000000 irrd-4.2.8/docs/releases/4.2.4.rst
+-rw-r--r--   0 sasha      (501) staff       (20)     1099 2022-06-24 08:51:21.000000 irrd-4.2.8/docs/releases/4.2.5.rst
+-rw-r--r--   0 sasha      (501) staff       (20)      610 2023-04-19 11:28:23.000000 irrd-4.2.8/docs/releases/4.2.6.rst
+-rw-r--r--   0 sasha      (501) staff       (20)     1015 2023-02-23 13:04:37.000000 irrd-4.2.8/docs/releases/4.2.7.rst
+-rw-r--r--   0 sasha      (501) staff       (20)      366 2023-04-19 11:33:22.000000 irrd-4.2.8/docs/releases/4.2.8.rst
+-rw-r--r--   0 sasha      (501) staff       (20)      156 2022-06-22 14:54:59.000000 irrd-4.2.8/docs/releases/index.rst
+-rw-r--r--   0 sasha      (501) staff       (20)       29 2022-06-22 14:54:59.000000 irrd-4.2.8/docs/security.rst
+-rw-r--r--   0 sasha      (501) staff       (20)      642 2023-04-19 11:28:23.000000 irrd-4.2.8/docs/spelling_wordlist.txt
+drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-04-19 11:33:39.831081 irrd-4.2.8/docs/users/
+-rw-r--r--   0 sasha      (501) staff       (20)    15100 2023-04-19 11:28:23.000000 irrd-4.2.8/docs/users/database-changes.rst
+-rw-r--r--   0 sasha      (501) staff       (20)    14439 2022-06-22 14:54:59.000000 irrd-4.2.8/docs/users/mirroring.rst
+drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-04-19 11:33:39.834221 irrd-4.2.8/docs/users/queries/
+-rw-r--r--   0 sasha      (501) staff       (20)    28712 2023-04-19 11:28:23.000000 irrd-4.2.8/docs/users/queries/graphql.rst
+-rw-r--r--   0 sasha      (501) staff       (20)     4186 2022-06-22 14:54:59.000000 irrd-4.2.8/docs/users/queries/index.rst
+-rw-r--r--   0 sasha      (501) staff       (20)    14712 2023-04-19 11:28:23.000000 irrd-4.2.8/docs/users/queries/whois.rst
+drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-04-19 11:33:39.834951 irrd-4.2.8/irrd/
+-rw-r--r--   0 sasha      (501) staff       (20)       69 2023-04-19 11:33:22.000000 irrd-4.2.8/irrd/__init__.py
+drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-04-19 11:33:39.844792 irrd-4.2.8/irrd/conf/
+-rw-r--r--   0 sasha      (501) staff       (20)    19785 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/conf/__init__.py
+-rw-r--r--   0 sasha      (501) staff       (20)     2586 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/conf/default_config.yaml
+-rw-r--r--   0 sasha      (501) staff       (20)      188 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/conf/defaults.py
+-rw-r--r--   0 sasha      (501) staff       (20)    14923 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/conf/test_conf.py
+drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-04-19 11:33:39.846225 irrd-4.2.8/irrd/daemon/
+-rw-r--r--   0 sasha      (501) staff       (20)        0 2020-11-10 14:53:47.000000 irrd-4.2.8/irrd/daemon/__init__.py
+-rwxr-xr-x   0 sasha      (501) staff       (20)     7232 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/daemon/main.py
+drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-04-19 11:33:39.849507 irrd-4.2.8/irrd/integration_tests/
+-rw-r--r--   0 sasha      (501) staff       (20)        0 2019-01-16 10:28:28.000000 irrd-4.2.8/irrd/integration_tests/__init__.py
+-rw-r--r--   0 sasha      (501) staff       (20)      302 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/integration_tests/constants.py
+-rw-r--r--   0 sasha      (501) staff       (20)     2709 2020-11-10 14:53:47.000000 irrd-4.2.8/irrd/integration_tests/mailserver.tac
+-rw-r--r--   0 sasha      (501) staff       (20)    45365 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/integration_tests/run.py
+drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-04-19 11:33:39.858152 irrd-4.2.8/irrd/mirroring/
+-rw-r--r--   0 sasha      (501) staff       (20)        0 2018-08-22 10:47:06.000000 irrd-4.2.8/irrd/mirroring/__init__.py
+-rw-r--r--   0 sasha      (501) staff       (20)     3838 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/mirroring/mirror_runners_export.py
+-rw-r--r--   0 sasha      (501) staff       (20)    16245 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/mirroring/mirror_runners_import.py
+-rw-r--r--   0 sasha      (501) staff       (20)     3891 2023-04-19 11:28:27.000000 irrd-4.2.8/irrd/mirroring/nrtm_generator.py
+-rw-r--r--   0 sasha      (501) staff       (20)     5085 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/mirroring/nrtm_operation.py
+-rw-r--r--   0 sasha      (501) staff       (20)    19716 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/mirroring/parsers.py
+-rw-r--r--   0 sasha      (501) staff       (20)     6461 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/mirroring/scheduler.py
+drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-04-19 11:33:39.865334 irrd-4.2.8/irrd/mirroring/tests/
+-rw-r--r--   0 sasha      (501) staff       (20)        0 2018-08-22 10:47:06.000000 irrd-4.2.8/irrd/mirroring/tests/__init__.py
+-rw-r--r--   0 sasha      (501) staff       (20)     1908 2021-09-07 16:54:18.000000 irrd-4.2.8/irrd/mirroring/tests/nrtm_samples.py
+-rw-r--r--   0 sasha      (501) staff       (20)     7139 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/mirroring/tests/test_mirror_runners_export.py
+-rw-r--r--   0 sasha      (501) staff       (20)    25267 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/mirroring/tests/test_mirror_runners_import.py
+-rw-r--r--   0 sasha      (501) staff       (20)     7237 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/mirroring/tests/test_nrtm_generator.py
+-rw-r--r--   0 sasha      (501) staff       (20)     8398 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/mirroring/tests/test_nrtm_operation.py
+-rw-r--r--   0 sasha      (501) staff       (20)    16913 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/mirroring/tests/test_parsers.py
+-rw-r--r--   0 sasha      (501) staff       (20)     8973 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/mirroring/tests/test_scheduler.py
+drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-04-19 11:33:39.868754 irrd-4.2.8/irrd/rpki/
+-rw-r--r--   0 sasha      (501) staff       (20)        0 2020-11-10 14:53:47.000000 irrd-4.2.8/irrd/rpki/__init__.py
+-rw-r--r--   0 sasha      (501) staff       (20)     9467 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/rpki/importer.py
+-rw-r--r--   0 sasha      (501) staff       (20)     5071 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/rpki/notifications.py
+-rw-r--r--   0 sasha      (501) staff       (20)      115 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/rpki/status.py
+drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-04-19 11:33:39.872129 irrd-4.2.8/irrd/rpki/tests/
+-rw-r--r--   0 sasha      (501) staff       (20)        0 2020-11-10 14:53:47.000000 irrd-4.2.8/irrd/rpki/tests/__init__.py
+-rw-r--r--   0 sasha      (501) staff       (20)     9976 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/rpki/tests/test_importer.py
+-rw-r--r--   0 sasha      (501) staff       (20)     6271 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/rpki/tests/test_notifications.py
+-rw-r--r--   0 sasha      (501) staff       (20)    14142 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/rpki/tests/test_validators.py
+-rw-r--r--   0 sasha      (501) staff       (20)     9248 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/rpki/validators.py
+drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-04-19 11:33:39.883612 irrd-4.2.8/irrd/rpsl/
+-rw-r--r--   0 sasha      (501) staff       (20)        0 2020-10-12 17:35:22.000000 irrd-4.2.8/irrd/rpsl/__init__.py
+-rw-r--r--   0 sasha      (501) staff       (20)      122 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/rpsl/config.py
+-rw-r--r--   0 sasha      (501) staff       (20)    24126 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/rpsl/fields.py
+-rw-r--r--   0 sasha      (501) staff       (20)    22222 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/rpsl/parser.py
+-rw-r--r--   0 sasha      (501) staff       (20)     1614 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/rpsl/parser_state.py
+-rw-r--r--   0 sasha      (501) staff       (20)    27633 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/rpsl/rpsl_objects.py
+drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-04-19 11:33:39.886755 irrd-4.2.8/irrd/rpsl/tests/
+-rw-r--r--   0 sasha      (501) staff       (20)        0 2018-05-07 12:40:56.000000 irrd-4.2.8/irrd/rpsl/tests/__init__.py
+-rw-r--r--   0 sasha      (501) staff       (20)    19630 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/rpsl/tests/test_fields.py
+-rw-r--r--   0 sasha      (501) staff       (20)    24886 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/rpsl/tests/test_rpsl_objects.py
+drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-04-19 11:33:39.889971 irrd-4.2.8/irrd/scopefilter/
+-rw-r--r--   0 sasha      (501) staff       (20)        0 2020-11-10 14:53:47.000000 irrd-4.2.8/irrd/scopefilter/__init__.py
+-rw-r--r--   0 sasha      (501) staff       (20)      152 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/scopefilter/status.py
+drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-04-19 11:33:39.891651 irrd-4.2.8/irrd/scopefilter/tests/
+-rw-r--r--   0 sasha      (501) staff       (20)        0 2020-11-10 14:53:47.000000 irrd-4.2.8/irrd/scopefilter/tests/__init__.py
+-rw-r--r--   0 sasha      (501) staff       (20)     9113 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/scopefilter/tests/test_scopefilter.py
+-rw-r--r--   0 sasha      (501) staff       (20)     6354 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/scopefilter/validators.py
+drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-04-19 11:33:39.904297 irrd-4.2.8/irrd/scripts/
+-rw-r--r--   0 sasha      (501) staff       (20)        0 2018-05-11 14:51:11.000000 irrd-4.2.8/irrd/scripts/__init__.py
+-rwxr-xr-x   0 sasha      (501) staff       (20)     1243 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/scripts/database_downgrade.py
+-rwxr-xr-x   0 sasha      (501) staff       (20)     1228 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/scripts/database_upgrade.py
+-rwxr-xr-x   0 sasha      (501) staff       (20)     2406 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/scripts/load_database.py
+-rwxr-xr-x   0 sasha      (501) staff       (20)     1859 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/scripts/load_pgp_keys.py
+-rwxr-xr-x   0 sasha      (501) staff       (20)     1472 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/scripts/load_test.py
+-rwxr-xr-x   0 sasha      (501) staff       (20)     1236 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/scripts/mirror_force_reload.py
+-rwxr-xr-x   0 sasha      (501) staff       (20)     8954 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/scripts/query_qa_comparison.py
+-rwxr-xr-x   0 sasha      (501) staff       (20)     4499 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/scripts/rpsl_read.py
+-rwxr-xr-x   0 sasha      (501) staff       (20)     2169 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/scripts/set_last_modified_auth.py
+-rwxr-xr-x   0 sasha      (501) staff       (20)     1281 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/scripts/submit_changes.py
+-rwxr-xr-x   0 sasha      (501) staff       (20)     1464 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/scripts/submit_email.py
+drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-04-19 11:33:39.912979 irrd-4.2.8/irrd/scripts/tests/
+-rw-r--r--   0 sasha      (501) staff       (20)        0 2018-05-11 14:43:40.000000 irrd-4.2.8/irrd/scripts/tests/__init__.py
+-rw-r--r--   0 sasha      (501) staff       (20)     2427 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/scripts/tests/test_load_database.py
+-rw-r--r--   0 sasha      (501) staff       (20)     1227 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/scripts/tests/test_load_pgp_keys.py
+-rw-r--r--   0 sasha      (501) staff       (20)      519 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/scripts/tests/test_mirror_force_reload.py
+-rw-r--r--   0 sasha      (501) staff       (20)     3244 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/scripts/tests/test_rpsl_read.py
+-rw-r--r--   0 sasha      (501) staff       (20)     1566 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/scripts/tests/test_set_last_modified_auth.py
+-rw-r--r--   0 sasha      (501) staff       (20)      769 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/scripts/tests/test_submit_email.py
+-rw-r--r--   0 sasha      (501) staff       (20)      575 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/scripts/tests/test_submit_update.py
+-rw-r--r--   0 sasha      (501) staff       (20)     2299 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/scripts/tests/test_update_database.py
+-rw-r--r--   0 sasha      (501) staff       (20)     2176 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/scripts/update_database.py
+drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-04-19 11:33:39.917094 irrd-4.2.8/irrd/server/
+-rw-r--r--   0 sasha      (501) staff       (20)        0 2018-07-06 10:44:00.000000 irrd-4.2.8/irrd/server/__init__.py
+-rw-r--r--   0 sasha      (501) staff       (20)     1490 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/server/access_check.py
+drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-04-19 11:33:39.921975 irrd-4.2.8/irrd/server/graphql/
+-rw-r--r--   0 sasha      (501) staff       (20)       67 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/server/graphql/__init__.py
+-rw-r--r--   0 sasha      (501) staff       (20)     1887 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/server/graphql/extensions.py
+-rw-r--r--   0 sasha      (501) staff       (20)    13936 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/server/graphql/resolvers.py
+-rw-r--r--   0 sasha      (501) staff       (20)     3430 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/server/graphql/schema_builder.py
+-rw-r--r--   0 sasha      (501) staff       (20)    12876 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/server/graphql/schema_generator.py
+drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-04-19 11:33:39.925315 irrd-4.2.8/irrd/server/graphql/tests/
+-rw-r--r--   0 sasha      (501) staff       (20)        0 2022-06-22 14:54:59.000000 irrd-4.2.8/irrd/server/graphql/tests/__init__.py
+-rw-r--r--   0 sasha      (501) staff       (20)     1463 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/server/graphql/tests/test_extensions.py
+-rw-r--r--   0 sasha      (501) staff       (20)    15060 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/server/graphql/tests/test_resolvers.py
+-rw-r--r--   0 sasha      (501) staff       (20)    12987 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/server/graphql/tests/test_schema_generator.py
+drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-04-19 11:33:39.929412 irrd-4.2.8/irrd/server/http/
+-rw-r--r--   0 sasha      (501) staff       (20)        0 2018-09-25 09:23:35.000000 irrd-4.2.8/irrd/server/http/__init__.py
+-rw-r--r--   0 sasha      (501) staff       (20)     2958 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/server/http/app.py
+-rw-r--r--   0 sasha      (501) staff       (20)     3406 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/server/http/endpoints.py
+-rw-r--r--   0 sasha      (501) staff       (20)     1359 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/server/http/server.py
+-rw-r--r--   0 sasha      (501) staff       (20)     8129 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/server/http/status_generator.py
+drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-04-19 11:33:39.931964 irrd-4.2.8/irrd/server/http/tests/
+-rw-r--r--   0 sasha      (501) staff       (20)        0 2018-09-25 09:23:35.000000 irrd-4.2.8/irrd/server/http/tests/__init__.py
+-rw-r--r--   0 sasha      (501) staff       (20)     7696 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/server/http/tests/test_endpoints.py
+-rw-r--r--   0 sasha      (501) staff       (20)     9830 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/server/http/tests/test_status_generator.py
+-rw-r--r--   0 sasha      (501) staff       (20)    18566 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/server/query_resolver.py
+-rw-r--r--   0 sasha      (501) staff       (20)     2019 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/server/test_access_check.py
+drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-04-19 11:33:39.939345 irrd-4.2.8/irrd/server/tests/
+-rw-r--r--   0 sasha      (501) staff       (20)        0 2022-06-22 14:54:59.000000 irrd-4.2.8/irrd/server/tests/__init__.py
+-rw-r--r--   0 sasha      (501) staff       (20)    32444 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/server/tests/test_query_resolver.py
+drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-04-19 11:33:39.945163 irrd-4.2.8/irrd/server/whois/
+-rw-r--r--   0 sasha      (501) staff       (20)        0 2018-07-06 10:44:00.000000 irrd-4.2.8/irrd/server/whois/__init__.py
+-rw-r--r--   0 sasha      (501) staff       (20)    23973 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/server/whois/query_parser.py
+-rw-r--r--   0 sasha      (501) staff       (20)     3535 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/server/whois/query_response.py
+-rw-r--r--   0 sasha      (501) staff       (20)     8709 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/server/whois/server.py
+drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-04-19 11:33:39.949994 irrd-4.2.8/irrd/server/whois/tests/
+-rw-r--r--   0 sasha      (501) staff       (20)        0 2018-07-06 10:44:00.000000 irrd-4.2.8/irrd/server/whois/tests/__init__.py
+-rw-r--r--   0 sasha      (501) staff       (20)    39550 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/server/whois/tests/test_query_parser.py
+-rw-r--r--   0 sasha      (501) staff       (20)     5132 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/server/whois/tests/test_query_response.py
+-rw-r--r--   0 sasha      (501) staff       (20)     6040 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/server/whois/tests/test_server.py
+drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-04-19 11:33:39.957742 irrd-4.2.8/irrd/storage/
+-rw-r--r--   0 sasha      (501) staff       (20)     1496 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/storage/__init__.py
+drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-04-19 11:33:39.960479 irrd-4.2.8/irrd/storage/alembic/
+-rw-r--r--   0 sasha      (501) staff       (20)        0 2018-08-22 10:47:06.000000 irrd-4.2.8/irrd/storage/alembic/__init__.py
+-rw-r--r--   0 sasha      (501) staff       (20)     1765 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/storage/alembic/env.py
+-rw-r--r--   0 sasha      (501) staff       (20)      494 2018-08-22 10:47:06.000000 irrd-4.2.8/irrd/storage/alembic/script.py.mako
+drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-04-19 11:33:39.972556 irrd-4.2.8/irrd/storage/alembic/versions/
+-rw-r--r--   0 sasha      (501) staff       (20)      594 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/storage/alembic/versions/1743f98a456d_add_serial_newest_mirror.py
+-rw-r--r--   0 sasha      (501) staff       (20)     1226 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/storage/alembic/versions/181670a62643_add_journal_entry_origin.py
+-rw-r--r--   0 sasha      (501) staff       (20)    10369 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/storage/alembic/versions/28dc1cd85bdc_initial_db.py
+-rw-r--r--   0 sasha      (501) staff       (20)     1401 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/storage/alembic/versions/39e4f15ed80c_add_bogon_status.py
+-rw-r--r--   0 sasha      (501) staff       (20)     2251 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/storage/alembic/versions/4a514ead8fc2_bogon_to_scope_filter.py
+-rw-r--r--   0 sasha      (501) staff       (20)     1145 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/storage/alembic/versions/64a3d6faf6d4_add_prefix_length_rpki_status_to_rpsl_objects.py
+-rw-r--r--   0 sasha      (501) staff       (20)     1049 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/storage/alembic/versions/8744b4b906bb_fix_rpsl_unique_key.py
+-rw-r--r--   0 sasha      (501) staff       (20)      550 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/storage/alembic/versions/893d0d5363b3_add_rpsl_prefix_idx.py
+-rw-r--r--   0 sasha      (501) staff       (20)        0 2018-08-22 10:47:06.000000 irrd-4.2.8/irrd/storage/alembic/versions/__init__.py
+-rw-r--r--   0 sasha      (501) staff       (20)     1083 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/storage/alembic/versions/a7766c144d61_add_synchronised_serial_to_database_.py
+-rw-r--r--   0 sasha      (501) staff       (20)     1518 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/storage/alembic/versions/a8609af97aa3_set_prefix_length_in_existing_rpsl_.py
+-rw-r--r--   0 sasha      (501) staff       (20)      510 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/storage/alembic/versions/b175c262448f_set_rpsl_prefix.py
+-rw-r--r--   0 sasha      (501) staff       (20)     1713 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/storage/alembic/versions/e07863eac52f_add_roa_object_table.py
+-rw-r--r--   0 sasha      (501) staff       (20)      511 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/storage/alembic/versions/f4c837d8258c_add_rpsl_prefix.py
+-rw-r--r--   0 sasha      (501) staff       (20)    34740 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/storage/database_handler.py
+-rw-r--r--   0 sasha      (501) staff       (20)     8347 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/storage/models.py
+-rw-r--r--   0 sasha      (501) staff       (20)    15540 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/storage/preload.py
+-rw-r--r--   0 sasha      (501) staff       (20)    20251 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/storage/queries.py
+drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-04-19 11:33:39.975870 irrd-4.2.8/irrd/storage/tests/
+-rw-r--r--   0 sasha      (501) staff       (20)        0 2018-08-22 10:47:06.000000 irrd-4.2.8/irrd/storage/tests/__init__.py
+-rw-r--r--   0 sasha      (501) staff       (20)    40358 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/storage/tests/test_database.py
+-rw-r--r--   0 sasha      (501) staff       (20)     8690 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/storage/tests/test_preload.py
+drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-04-19 11:33:39.980142 irrd-4.2.8/irrd/updates/
+-rw-r--r--   0 sasha      (501) staff       (20)        0 2018-07-31 14:50:32.000000 irrd-4.2.8/irrd/updates/__init__.py
+-rw-r--r--   0 sasha      (501) staff       (20)     2831 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/updates/email.py
+-rw-r--r--   0 sasha      (501) staff       (20)    13269 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/updates/handler.py
+-rw-r--r--   0 sasha      (501) staff       (20)    19472 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/updates/parser.py
+-rw-r--r--   0 sasha      (501) staff       (20)      654 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/updates/parser_state.py
+drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-04-19 11:33:39.983775 irrd-4.2.8/irrd/updates/tests/
+-rw-r--r--   0 sasha      (501) staff       (20)        0 2018-07-31 14:50:32.000000 irrd-4.2.8/irrd/updates/tests/__init__.py
+-rw-r--r--   0 sasha      (501) staff       (20)     6010 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/updates/tests/test_email.py
+-rw-r--r--   0 sasha      (501) staff       (20)    42451 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/updates/tests/test_handler.py
+-rw-r--r--   0 sasha      (501) staff       (20)    58198 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/updates/tests/test_parser.py
+-rw-r--r--   0 sasha      (501) staff       (20)    16514 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/updates/validators.py
+drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-04-19 11:33:39.992354 irrd-4.2.8/irrd/utils/
+-rw-r--r--   0 sasha      (501) staff       (20)        0 2023-01-30 15:26:42.000000 irrd-4.2.8/irrd/utils/__init__.py
+-rw-r--r--   0 sasha      (501) staff       (20)     3290 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/utils/email.py
+-rw-r--r--   0 sasha      (501) staff       (20)     3000 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/utils/pgp.py
+-rw-r--r--   0 sasha      (501) staff       (20)     1612 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/utils/process_support.py
+-rw-r--r--   0 sasha      (501) staff       (20)    40716 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/utils/rpsl_samples.py
+-rw-r--r--   0 sasha      (501) staff       (20)      800 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/utils/test_utils.py
+drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-04-19 11:33:40.003262 irrd-4.2.8/irrd/utils/tests/
+-rw-r--r--   0 sasha      (501) staff       (20)        0 2023-01-30 15:26:37.000000 irrd-4.2.8/irrd/utils/tests/__init__.py
+-rw-r--r--   0 sasha      (501) staff       (20)    26217 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/utils/tests/test_email.py
+-rw-r--r--   0 sasha      (501) staff       (20)     7059 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/utils/tests/test_pgp.py
+-rw-r--r--   0 sasha      (501) staff       (20)     2084 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/utils/tests/test_text.py
+-rw-r--r--   0 sasha      (501) staff       (20)     1931 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/utils/tests/test_validators.py
+-rw-r--r--   0 sasha      (501) staff       (20)    10324 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/utils/tests/test_whois_client.py
+-rw-r--r--   0 sasha      (501) staff       (20)     3521 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/utils/text.py
+-rw-r--r--   0 sasha      (501) staff       (20)     2252 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/utils/validators.py
+-rw-r--r--   0 sasha      (501) staff       (20)     4752 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/utils/whois_client.py
+drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-04-19 11:33:40.004092 irrd-4.2.8/irrd/vendor/
+-rw-r--r--   0 sasha      (501) staff       (20)        0 2020-11-10 14:53:47.000000 irrd-4.2.8/irrd/vendor/__init__.py
+drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-04-19 11:33:40.005193 irrd-4.2.8/irrd/vendor/dotted/
+-rw-r--r--   0 sasha      (501) staff       (20)        0 2022-06-22 14:54:59.000000 irrd-4.2.8/irrd/vendor/dotted/__init__.py
+-rw-r--r--   0 sasha      (501) staff       (20)    12374 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/vendor/dotted/collection.py
+drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-04-19 11:33:40.006315 irrd-4.2.8/irrd/vendor/postgres_copy/
+-rw-r--r--   0 sasha      (501) staff       (20)     6359 2023-04-19 11:28:23.000000 irrd-4.2.8/irrd/vendor/postgres_copy/__init__.py
+drwxr-xr-x   0 sasha      (501) staff       (20)        0 2023-04-19 11:33:39.838994 irrd-4.2.8/irrd.egg-info/
+-rw-r--r--   0 sasha      (501) staff       (20)     2912 2023-04-19 11:33:38.000000 irrd-4.2.8/irrd.egg-info/PKG-INFO
+-rw-r--r--   0 sasha      (501) staff       (20)     7206 2023-04-19 11:33:39.000000 irrd-4.2.8/irrd.egg-info/SOURCES.txt
+-rw-r--r--   0 sasha      (501) staff       (20)        1 2023-04-19 11:33:38.000000 irrd-4.2.8/irrd.egg-info/dependency_links.txt
+-rw-r--r--   0 sasha      (501) staff       (20)      519 2023-04-19 11:33:38.000000 irrd-4.2.8/irrd.egg-info/entry_points.txt
+-rw-r--r--   0 sasha      (501) staff       (20)      625 2023-04-19 11:33:38.000000 irrd-4.2.8/irrd.egg-info/requires.txt
+-rw-r--r--   0 sasha      (501) staff       (20)        5 2023-04-19 11:33:38.000000 irrd-4.2.8/irrd.egg-info/top_level.txt
+-rw-r--r--   0 sasha      (501) staff       (20)     2213 2023-04-19 11:28:23.000000 irrd-4.2.8/requirements.txt
+-rw-r--r--   0 sasha      (501) staff       (20)      782 2023-04-19 11:33:40.008641 irrd-4.2.8/setup.cfg
+-rwxr-xr-x   0 sasha      (501) staff       (20)     3096 2023-04-19 11:28:23.000000 irrd-4.2.8/setup.py
```

### Comparing `irrd-4.2.7/LICENSE` & `irrd-4.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/PKG-INFO` & `irrd-4.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irrd
-Version: 4.2.7
+Version: 4.2.8
 Summary: Internet Routing Registry daemon (IRRd)
 Home-page: https://github.com/irrdnet/irrd
 Author: Reliably Coded for NTT Ltd. and others
 Author-email: irrd@reliablycoded.nl
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `irrd-4.2.7/README.rst` & `irrd-4.2.8/README.rst`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/conf/__init__.py` & `irrd-4.2.8/irrd/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/conf/default_config.yaml` & `irrd-4.2.8/irrd/conf/default_config.yaml`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/conf/test_conf.py` & `irrd-4.2.8/irrd/conf/test_conf.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/daemon/main.py` & `irrd-4.2.8/irrd/daemon/main.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/mirroring/mirror_runners_export.py` & `irrd-4.2.8/irrd/mirroring/mirror_runners_export.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/mirroring/mirror_runners_import.py` & `irrd-4.2.8/irrd/mirroring/mirror_runners_import.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/mirroring/nrtm_generator.py` & `irrd-4.2.8/irrd/mirroring/nrtm_generator.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,22 +59,21 @@
 
         range_limit = get_setting(f'sources.{source}.nrtm_query_serial_range_limit')
         if range_limit and int(range_limit) < (serial_end_display - serial_start_requested):
             raise NRTMGeneratorException(f'Serial range requested exceeds maximum range of {range_limit}')
 
         q = RPSLDatabaseJournalQuery().sources([source]).serial_range(serial_start_requested, serial_end_requested)
 
-        operations = list(database_handler.execute_query(q))
+        output = [f"%START Version: {version} {source} {serial_start_requested}-{serial_end_display}\n"]
 
-        output = f'%START Version: {version} {source} {serial_start_requested}-{serial_end_display}\n'
-
-        for operation in operations:
-            output += '\n' + operation['operation'].value
-            if version == '3':
-                output += ' ' + str(operation['serial_nrtm'])
-            text = operation['object_text']
+        for operation in database_handler.execute_query(q):
+            operation_str = operation["operation"].value
+            if version == "3":
+                operation_str += " " + str(operation["serial_nrtm"])
+            text = operation["object_text"]
             if remove_auth_hashes:
                 text = remove_auth_hashes_func(text)
-            output += '\n\n' + text
+            operation_str += "\n\n" + text
+            output.append(operation_str)
 
-        output += f'\n%END {source}'
-        return output
+        output.append(f"%END {source}")
+        return "\n".join(output)
```

### Comparing `irrd-4.2.7/irrd/mirroring/nrtm_operation.py` & `irrd-4.2.8/irrd/mirroring/nrtm_operation.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/mirroring/parsers.py` & `irrd-4.2.8/irrd/mirroring/parsers.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/mirroring/scheduler.py` & `irrd-4.2.8/irrd/mirroring/scheduler.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/rpki/importer.py` & `irrd-4.2.8/irrd/rpki/importer.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/rpki/notifications.py` & `irrd-4.2.8/irrd/rpki/notifications.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/rpki/validators.py` & `irrd-4.2.8/irrd/rpki/validators.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/rpsl/fields.py` & `irrd-4.2.8/irrd/rpsl/fields.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/rpsl/parser.py` & `irrd-4.2.8/irrd/rpsl/parser.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/rpsl/parser_state.py` & `irrd-4.2.8/irrd/rpsl/parser_state.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/rpsl/rpsl_objects.py` & `irrd-4.2.8/irrd/rpsl/rpsl_objects.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/scopefilter/validators.py` & `irrd-4.2.8/irrd/scopefilter/validators.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/scripts/database_downgrade.py` & `irrd-4.2.8/irrd/scripts/database_downgrade.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/scripts/database_upgrade.py` & `irrd-4.2.8/irrd/scripts/database_upgrade.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/scripts/load_database.py` & `irrd-4.2.8/irrd/scripts/load_database.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/scripts/load_pgp_keys.py` & `irrd-4.2.8/irrd/scripts/load_pgp_keys.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/scripts/load_test.py` & `irrd-4.2.8/irrd/scripts/load_test.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/scripts/mirror_force_reload.py` & `irrd-4.2.8/irrd/scripts/mirror_force_reload.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/scripts/query_qa_comparison.py` & `irrd-4.2.8/irrd/scripts/query_qa_comparison.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/scripts/rpsl_read.py` & `irrd-4.2.8/irrd/scripts/rpsl_read.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/scripts/set_last_modified_auth.py` & `irrd-4.2.8/irrd/scripts/set_last_modified_auth.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/scripts/submit_changes.py` & `irrd-4.2.8/irrd/scripts/submit_changes.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/scripts/submit_email.py` & `irrd-4.2.8/irrd/scripts/submit_email.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/scripts/update_database.py` & `irrd-4.2.8/irrd/scripts/update_database.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/server/access_check.py` & `irrd-4.2.8/irrd/server/access_check.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/server/graphql/extensions.py` & `irrd-4.2.8/irrd/server/graphql/extensions.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/server/graphql/resolvers.py` & `irrd-4.2.8/irrd/server/graphql/resolvers.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/server/graphql/schema_builder.py` & `irrd-4.2.8/irrd/server/graphql/schema_builder.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/server/graphql/schema_generator.py` & `irrd-4.2.8/irrd/server/graphql/schema_generator.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/server/http/app.py` & `irrd-4.2.8/irrd/server/http/app.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/server/http/endpoints.py` & `irrd-4.2.8/irrd/server/http/endpoints.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/server/http/server.py` & `irrd-4.2.8/irrd/server/http/server.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/server/http/status_generator.py` & `irrd-4.2.8/irrd/server/http/status_generator.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/server/query_resolver.py` & `irrd-4.2.8/irrd/server/query_resolver.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/server/test_access_check.py` & `irrd-4.2.8/irrd/server/test_access_check.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/server/whois/query_parser.py` & `irrd-4.2.8/irrd/server/whois/query_parser.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/server/whois/query_response.py` & `irrd-4.2.8/irrd/server/whois/query_response.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/server/whois/server.py` & `irrd-4.2.8/irrd/server/whois/server.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/storage/__init__.py` & `irrd-4.2.8/irrd/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/storage/alembic/env.py` & `irrd-4.2.8/irrd/storage/alembic/env.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/storage/alembic/versions/1743f98a456d_add_serial_newest_mirror.py` & `irrd-4.2.8/irrd/storage/alembic/versions/1743f98a456d_add_serial_newest_mirror.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/storage/alembic/versions/181670a62643_add_journal_entry_origin.py` & `irrd-4.2.8/irrd/storage/alembic/versions/181670a62643_add_journal_entry_origin.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/storage/alembic/versions/28dc1cd85bdc_initial_db.py` & `irrd-4.2.8/irrd/storage/alembic/versions/28dc1cd85bdc_initial_db.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/storage/alembic/versions/39e4f15ed80c_add_bogon_status.py` & `irrd-4.2.8/irrd/storage/alembic/versions/39e4f15ed80c_add_bogon_status.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/storage/alembic/versions/4a514ead8fc2_bogon_to_scope_filter.py` & `irrd-4.2.8/irrd/storage/alembic/versions/4a514ead8fc2_bogon_to_scope_filter.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/storage/alembic/versions/64a3d6faf6d4_add_prefix_length_rpki_status_to_rpsl_objects.py` & `irrd-4.2.8/irrd/storage/alembic/versions/64a3d6faf6d4_add_prefix_length_rpki_status_to_rpsl_objects.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/storage/alembic/versions/8744b4b906bb_fix_rpsl_unique_key.py` & `irrd-4.2.8/irrd/storage/alembic/versions/8744b4b906bb_fix_rpsl_unique_key.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/storage/alembic/versions/893d0d5363b3_add_rpsl_prefix_idx.py` & `irrd-4.2.8/irrd/storage/alembic/versions/893d0d5363b3_add_rpsl_prefix_idx.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/storage/alembic/versions/a7766c144d61_add_synchronised_serial_to_database_.py` & `irrd-4.2.8/irrd/storage/alembic/versions/a7766c144d61_add_synchronised_serial_to_database_.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/storage/alembic/versions/a8609af97aa3_set_prefix_length_in_existing_rpsl_.py` & `irrd-4.2.8/irrd/storage/alembic/versions/a8609af97aa3_set_prefix_length_in_existing_rpsl_.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/storage/alembic/versions/e07863eac52f_add_roa_object_table.py` & `irrd-4.2.8/irrd/storage/alembic/versions/e07863eac52f_add_roa_object_table.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/storage/database_handler.py` & `irrd-4.2.8/irrd/storage/database_handler.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/storage/models.py` & `irrd-4.2.8/irrd/storage/models.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/storage/preload.py` & `irrd-4.2.8/irrd/storage/preload.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/storage/queries.py` & `irrd-4.2.8/irrd/storage/queries.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/updates/email.py` & `irrd-4.2.8/irrd/updates/email.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/updates/handler.py` & `irrd-4.2.8/irrd/updates/handler.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/updates/parser.py` & `irrd-4.2.8/irrd/updates/parser.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/updates/parser_state.py` & `irrd-4.2.8/irrd/updates/parser_state.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/updates/validators.py` & `irrd-4.2.8/irrd/updates/validators.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/utils/email.py` & `irrd-4.2.8/irrd/utils/email.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/utils/pgp.py` & `irrd-4.2.8/irrd/utils/pgp.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/utils/process_support.py` & `irrd-4.2.8/irrd/utils/process_support.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/utils/rpsl_samples.py` & `irrd-4.2.8/irrd/utils/rpsl_samples.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/utils/test_utils.py` & `irrd-4.2.8/irrd/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/utils/text.py` & `irrd-4.2.8/irrd/utils/text.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/utils/validators.py` & `irrd-4.2.8/irrd/utils/validators.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/utils/whois_client.py` & `irrd-4.2.8/irrd/utils/whois_client.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/vendor/dotted/collection.py` & `irrd-4.2.8/irrd/vendor/dotted/collection.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd/vendor/postgres_copy/__init__.py` & `irrd-4.2.8/irrd/vendor/postgres_copy/__init__.py`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd.egg-info/PKG-INFO` & `irrd-4.2.8/irrd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irrd
-Version: 4.2.7
+Version: 4.2.8
 Summary: Internet Routing Registry daemon (IRRd)
 Home-page: https://github.com/irrdnet/irrd
 Author: Reliably Coded for NTT Ltd. and others
 Author-email: irrd@reliablycoded.nl
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `irrd-4.2.7/irrd.egg-info/entry_points.txt` & `irrd-4.2.8/irrd.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/irrd.egg-info/requires.txt` & `irrd-4.2.8/irrd.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/setup.cfg` & `irrd-4.2.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `irrd-4.2.7/setup.py` & `irrd-4.2.8/setup.py`

 * *Files identical despite different names*

