# Comparing `tmp/ultima_scraper_collection-0.1.4.tar.gz` & `tmp/ultima_scraper_collection-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultima_scraper_collection-0.1.4.tar", max compression
+gzip compressed data, was "ultima_scraper_collection-1.0.0.tar", max compression
```

## Comparing `ultima_scraper_collection-0.1.4.tar` & `ultima_scraper_collection-1.0.0.tar`

### file list

```diff
@@ -1,73 +1,73 @@
--rw-r--r--   0        0        0      701 2023-03-14 10:03:51.217717 ultima_scraper_collection-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      293 2023-02-26 12:00:14.727199 ultima_scraper_collection-0.1.4/ultima_scraper_collection/__init__.py
--rw-r--r--   0        0        0        0 2023-02-26 11:42:41.007744 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/__init__.py
--rw-r--r--   0        0        0        0 2023-02-26 11:42:54.441267 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/__init__.py
--rw-r--r--   0        0        0        0 2023-03-06 01:27:30.462039 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/__init__.py
--rw-r--r--   0        0        0        0 2023-03-04 04:03:12.661102 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/__init__.py
--rw-r--r--   0        0        0        0 2023-02-26 11:42:54.461267 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/__init__.py
--rw-r--r--   0        0        0       38 2022-01-17 19:20:07.000000 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/README
--rw-r--r--   0        0        0     2150 2023-03-05 04:16:43.534861 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/env.py
--rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/script.py.mako
--rw-r--r--   0        0        0      662 2023-03-05 04:20:42.303797 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/0d4d92c0498e_content.py
--rw-r--r--   0        0        0      941 2023-03-05 04:20:47.520466 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/1454e4d1c6b8_content.py
--rw-r--r--   0        0        0      861 2022-04-25 23:29:43.807242 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/37c4f2719d65_content.py
--rw-r--r--   0        0        0     3182 2022-01-17 19:20:07.000000 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/5493253cc03c_content.py
--rw-r--r--   0        0        0     1651 2022-01-17 19:20:07.000000 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/b791cf213df9_content.py
--rw-r--r--   0        0        0     1415 2023-03-05 04:20:57.727140 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/d2f2002f3c36_content.py
--rw-r--r--   0        0        0     2201 2023-03-03 17:13:51.407142 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic.ini
--rw-r--r--   0        0        0    77824 2023-02-14 03:46:10.695467 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/base_user_database.db
--rw-r--r--   0        0        0        0 2023-03-10 12:28:15.033139 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/__init__.py
--rw-r--r--   0        0        0        0 2023-03-10 12:28:22.753355 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/__init__.py
--rw-r--r--   0        0        0        0 2023-03-10 12:27:11.408006 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/__init__.py
--rw-r--r--   0        0        0     2296 2023-03-10 12:28:05.882882 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/env.py
--rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/script.py.mako
--rw-r--r--   0        0        0     1769 2022-01-17 19:20:07.000000 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/2c36fcc0b921_content.py
--rw-r--r--   0        0        0     1649 2022-01-17 19:20:07.000000 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/7c1c6e101059_content.py
--rw-r--r--   0        0        0      794 2022-01-17 19:20:07.000000 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/aeb9fe314556_content.py
--rw-r--r--   0        0        0      798 2022-01-17 19:20:07.000000 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/bf20242a238f_content.py
--rw-r--r--   0        0        0      797 2022-01-17 19:20:07.000000 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/d0118d8ec0b4_content.py
--rw-r--r--   0        0        0     2011 2022-01-17 19:20:07.000000 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic.ini
--rw-r--r--   0        0        0      493 2023-03-10 12:30:45.700616 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/messages.py
--rw-r--r--   0        0        0    36864 2022-01-17 19:20:07.000000 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/test_messages.db
--rw-r--r--   0        0        0     2288 2023-03-10 12:32:59.654189 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/env.py
--rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/script.py.mako
--rw-r--r--   0        0        0     1762 2022-01-17 19:20:07.000000 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/194e05269f09_content.py
--rw-r--r--   0        0        0      797 2022-01-17 19:20:07.000000 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/5b4bea08c27f_content.py
--rw-r--r--   0        0        0      794 2022-01-17 19:20:07.000000 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/6b1b10eb67de_content.py
--rw-r--r--   0        0        0      798 2022-01-17 19:20:07.000000 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/990fc1108317_content.py
--rw-r--r--   0        0        0     1643 2022-01-17 19:20:07.000000 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/a918b6b05d2f_content.py
--rw-r--r--   0        0        0     2011 2022-01-17 19:20:07.000000 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic.ini
--rw-r--r--   0        0        0      488 2023-03-10 12:32:58.467491 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/posts.py
--rw-r--r--   0        0        0    36864 2022-01-17 19:20:07.000000 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/test_posts.db
--rw-r--r--   0        0        0     2294 2023-03-10 12:32:46.997189 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/env.py
--rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/script.py.mako
--rw-r--r--   0        0        0      797 2022-01-17 19:20:07.000000 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/29f675c35eee_content.py
--rw-r--r--   0        0        0     1647 2022-01-17 19:20:07.000000 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/2e4f8364f7e2_content.py
--rw-r--r--   0        0        0     1766 2022-01-17 19:20:07.000000 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/3076beb33c1b_content.py
--rw-r--r--   0        0        0      798 2022-01-17 19:20:07.000000 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/e0c73f066547_content.py
--rw-r--r--   0        0        0      794 2022-01-17 19:20:07.000000 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/ebc3f4bb0782_content.py
--rw-r--r--   0        0        0     2011 2022-01-17 19:20:07.000000 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic.ini
--rw-r--r--   0        0        0      490 2023-03-10 12:32:57.520800 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/stories.py
--rw-r--r--   0        0        0    36864 2022-01-17 19:20:07.000000 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/test_stories.db
--rw-r--r--   0        0        0        0 2022-12-05 14:27:20.696663 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/__init__.py
--rw-r--r--   0        0        0     1271 2023-03-12 15:22:13.138180 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/api_model.py
--rw-r--r--   0        0        0     2764 2023-03-05 04:24:29.397986 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/media_model.py
--rw-r--r--   0        0        0     2052 2023-03-05 04:24:48.768120 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/user_database.py
--rw-r--r--   0        0        0     9739 2023-03-10 10:54:33.201028 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/sqlite_database.py
--rw-r--r--   0        0        0      442 2023-03-12 15:01:42.766490 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/database_manager.py
--rw-r--r--   0        0        0        0 2023-02-26 16:06:18.482305 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/datascraper_manager/__init__.py
--rw-r--r--   0        0        0     1558 2023-03-12 13:14:10.302489 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/datascraper_manager/datascraper_manager.py
--rw-r--r--   0        0        0        0 2023-02-26 16:04:46.426896 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/datascraper_manager/datascrapers/__init__.py
--rw-r--r--   0        0        0    13165 2023-03-11 13:07:51.266257 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/datascraper_manager/datascrapers/fansly.py
--rw-r--r--   0        0        0    13053 2023-03-10 12:33:21.298092 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/datascraper_manager/datascrapers/onlyfans.py
--rw-r--r--   0        0        0     3464 2023-03-13 08:37:30.292230 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/download_manager.py
--rw-r--r--   0        0        0    14951 2023-03-10 12:14:58.292289 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/filesystem_manager.py
--rw-r--r--   0        0        0     6102 2023-03-05 04:29:30.964171 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/legacy_code.py
--rw-r--r--   0        0        0        0 2023-01-26 08:21:03.864558 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/metadata_manager/__init__.py
--rw-r--r--   0        0        0     8514 2023-03-12 15:02:26.648051 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/metadata_manager/metadata_manager.py
--rw-r--r--   0        0        0     6673 2023-03-14 10:02:12.828825 ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/option_manager.py
--rw-r--r--   0        0        0        0 2023-03-14 06:55:35.872202 ultima_scraper_collection-0.1.4/ultima_scraper_collection/modules/__init__.py
--rw-r--r--   0        0        0    18172 2023-03-14 00:24:30.656765 ultima_scraper_collection-0.1.4/ultima_scraper_collection/modules/module_streamliner.py
--rw-r--r--   0        0        0        0 2023-02-26 16:07:35.717380 ultima_scraper_collection-0.1.4/ultima_scraper_collection/py.typed
--rw-r--r--   0        0        0     2962 1970-01-01 00:00:00.000000 ultima_scraper_collection-0.1.4/setup.py
--rw-r--r--   0        0        0      616 1970-01-01 00:00:00.000000 ultima_scraper_collection-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      701 2023-04-20 23:22:21.833915 ultima_scraper_collection-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      293 2023-02-26 12:00:14.727199 ultima_scraper_collection-1.0.0/ultima_scraper_collection/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-26 11:42:41.007744 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-26 11:42:54.441267 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-06 01:27:30.462039 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-04 04:03:12.661102 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-26 11:42:54.461267 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/__init__.py
+-rw-r--r--   0        0        0       38 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/README
+-rw-r--r--   0        0        0     2150 2023-03-05 04:16:43.534861 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/env.py
+-rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/script.py.mako
+-rw-r--r--   0        0        0      662 2023-03-05 04:20:42.303797 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/0d4d92c0498e_content.py
+-rw-r--r--   0        0        0      941 2023-03-05 04:20:47.520466 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/1454e4d1c6b8_content.py
+-rw-r--r--   0        0        0      861 2022-04-25 23:29:43.807242 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/37c4f2719d65_content.py
+-rw-r--r--   0        0        0     3182 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/5493253cc03c_content.py
+-rw-r--r--   0        0        0     1651 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/b791cf213df9_content.py
+-rw-r--r--   0        0        0     1415 2023-03-05 04:20:57.727140 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/d2f2002f3c36_content.py
+-rw-r--r--   0        0        0     2201 2023-03-03 17:13:51.407142 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic.ini
+-rw-r--r--   0        0        0    77824 2023-02-14 03:46:10.695467 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/base_user_database.db
+-rw-r--r--   0        0        0        0 2023-03-10 12:28:15.033139 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-10 12:28:22.753355 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-10 12:27:11.408006 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/__init__.py
+-rw-r--r--   0        0        0     2296 2023-03-10 12:28:05.882882 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/env.py
+-rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/script.py.mako
+-rw-r--r--   0        0        0     1769 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/2c36fcc0b921_content.py
+-rw-r--r--   0        0        0     1649 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/7c1c6e101059_content.py
+-rw-r--r--   0        0        0      794 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/aeb9fe314556_content.py
+-rw-r--r--   0        0        0      798 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/bf20242a238f_content.py
+-rw-r--r--   0        0        0      797 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/d0118d8ec0b4_content.py
+-rw-r--r--   0        0        0     2011 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic.ini
+-rw-r--r--   0        0        0      493 2023-03-10 12:30:45.700616 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/messages.py
+-rw-r--r--   0        0        0    36864 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/test_messages.db
+-rw-r--r--   0        0        0     2288 2023-03-10 12:32:59.654189 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/env.py
+-rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/script.py.mako
+-rw-r--r--   0        0        0     1762 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/194e05269f09_content.py
+-rw-r--r--   0        0        0      797 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/5b4bea08c27f_content.py
+-rw-r--r--   0        0        0      794 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/6b1b10eb67de_content.py
+-rw-r--r--   0        0        0      798 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/990fc1108317_content.py
+-rw-r--r--   0        0        0     1643 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/a918b6b05d2f_content.py
+-rw-r--r--   0        0        0     2011 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic.ini
+-rw-r--r--   0        0        0      488 2023-03-10 12:32:58.467491 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/posts.py
+-rw-r--r--   0        0        0    36864 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/test_posts.db
+-rw-r--r--   0        0        0     2294 2023-03-10 12:32:46.997189 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/env.py
+-rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/script.py.mako
+-rw-r--r--   0        0        0      797 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/29f675c35eee_content.py
+-rw-r--r--   0        0        0     1647 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/2e4f8364f7e2_content.py
+-rw-r--r--   0        0        0     1766 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/3076beb33c1b_content.py
+-rw-r--r--   0        0        0      798 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/e0c73f066547_content.py
+-rw-r--r--   0        0        0      794 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/ebc3f4bb0782_content.py
+-rw-r--r--   0        0        0     2011 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic.ini
+-rw-r--r--   0        0        0      490 2023-03-10 12:32:57.520800 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/stories.py
+-rw-r--r--   0        0        0    36864 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/test_stories.db
+-rw-r--r--   0        0        0        0 2022-12-05 14:27:20.696663 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/__init__.py
+-rw-r--r--   0        0        0     1611 2023-04-20 22:10:05.846209 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/api_model.py
+-rw-r--r--   0        0        0     2764 2023-04-20 22:14:44.815046 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/media_model.py
+-rw-r--r--   0        0        0     2073 2023-04-20 22:22:10.068827 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/user_database.py
+-rw-r--r--   0        0        0     9406 2023-04-20 22:22:19.565161 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/sqlite_database.py
+-rw-r--r--   0        0        0      442 2023-03-12 15:01:42.766490 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/database_manager.py
+-rw-r--r--   0        0        0        0 2023-02-26 16:06:18.482305 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/datascraper_manager/__init__.py
+-rw-r--r--   0        0        0     1558 2023-03-12 13:14:10.302489 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/datascraper_manager/datascraper_manager.py
+-rw-r--r--   0        0        0        0 2023-02-26 16:04:46.426896 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/datascraper_manager/datascrapers/__init__.py
+-rw-r--r--   0        0        0    15824 2023-04-20 22:28:12.293022 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/datascraper_manager/datascrapers/fansly.py
+-rw-r--r--   0        0        0     6714 2023-04-20 22:28:23.059323 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/datascraper_manager/datascrapers/onlyfans.py
+-rw-r--r--   0        0        0     4455 2023-04-20 23:09:45.165667 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/download_manager.py
+-rw-r--r--   0        0        0    14027 2023-04-20 23:10:21.532555 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/filesystem_manager.py
+-rw-r--r--   0        0        0     6102 2023-03-05 04:29:30.964171 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/legacy_code.py
+-rw-r--r--   0        0        0        0 2023-01-26 08:21:03.864558 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/metadata_manager/__init__.py
+-rw-r--r--   0        0        0    27544 2023-04-20 23:06:36.616983 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/metadata_manager/metadata_manager.py
+-rw-r--r--   0        0        0     6673 2023-03-14 10:02:12.828825 ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/option_manager.py
+-rw-r--r--   0        0        0        0 2023-03-14 06:55:35.872202 ultima_scraper_collection-1.0.0/ultima_scraper_collection/modules/__init__.py
+-rw-r--r--   0        0        0    17712 2023-04-20 23:15:15.709578 ultima_scraper_collection-1.0.0/ultima_scraper_collection/modules/module_streamliner.py
+-rw-r--r--   0        0        0        0 2023-02-26 16:07:35.717380 ultima_scraper_collection-1.0.0/ultima_scraper_collection/py.typed
+-rw-r--r--   0        0        0     2962 1970-01-01 00:00:00.000000 ultima_scraper_collection-1.0.0/setup.py
+-rw-r--r--   0        0        0      616 1970-01-01 00:00:00.000000 ultima_scraper_collection-1.0.0/PKG-INFO
```

### Comparing `ultima_scraper_collection-0.1.4/pyproject.toml` & `ultima_scraper_collection-1.0.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "ultima-scraper-collection"
-version = "0.1.4"
+version = "1.0.0"
 description = ""
 authors = [
     "DIGITALCRIMINALS <89371864+digitalcriminals@users.noreply.github.com>",
 ]
 packages = [{include = "ultima_scraper_collection"}]
 include = ["ultima_scraper_collection/py.typed"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 
 sqlalchemy = "^2.0.1"
 psycopg2 = "^2.9.5"
 alembic = "^1.9.2"
 tqdm = "^4.65.0"
-ultima-scraper-api = "^0.1.3"
-ultima-scraper-renamer = "^0.1.3"
+ultima-scraper-api = "^1.0.0"
+ultima-scraper-renamer = "^1.0.0"
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.2"
 
 [tool.semantic_release]
 version_toml = "pyproject.toml:tool.poetry.version"
```

### Comparing `ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/env.py` & `ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/env.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/0d4d92c0498e_content.py` & `ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/0d4d92c0498e_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/1454e4d1c6b8_content.py` & `ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/1454e4d1c6b8_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/37c4f2719d65_content.py` & `ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/37c4f2719d65_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/5493253cc03c_content.py` & `ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/5493253cc03c_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/b791cf213df9_content.py` & `ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/b791cf213df9_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/d2f2002f3c36_content.py` & `ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/d2f2002f3c36_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic.ini` & `ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic.ini`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/base_user_database.db` & `ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/base_user_database.db`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/env.py` & `ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/env.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/2c36fcc0b921_content.py` & `ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/2c36fcc0b921_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/7c1c6e101059_content.py` & `ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/7c1c6e101059_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/aeb9fe314556_content.py` & `ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/aeb9fe314556_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/bf20242a238f_content.py` & `ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/bf20242a238f_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/d0118d8ec0b4_content.py` & `ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/d0118d8ec0b4_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic.ini` & `ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic.ini`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/test_messages.db` & `ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/test_messages.db`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/env.py` & `ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/env.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/194e05269f09_content.py` & `ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/194e05269f09_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/5b4bea08c27f_content.py` & `ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/5b4bea08c27f_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/6b1b10eb67de_content.py` & `ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/6b1b10eb67de_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/990fc1108317_content.py` & `ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/990fc1108317_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/a918b6b05d2f_content.py` & `ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/a918b6b05d2f_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic.ini` & `ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic.ini`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/test_posts.db` & `ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/test_posts.db`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/env.py` & `ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/env.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/29f675c35eee_content.py` & `ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/29f675c35eee_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/2e4f8364f7e2_content.py` & `ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/2e4f8364f7e2_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/3076beb33c1b_content.py` & `ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/3076beb33c1b_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/e0c73f066547_content.py` & `ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/e0c73f066547_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/ebc3f4bb0782_content.py` & `ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/ebc3f4bb0782_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic.ini` & `ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic.ini`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/test_stories.db` & `ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/test_stories.db`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/media_model.py` & `ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/media_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/user_database.py` & `ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/user_database.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-### messages.py ###
-
 from typing import Optional, cast
 
 import sqlalchemy
 from sqlalchemy.orm.decl_api import declarative_base
 
 from ultima_scraper_collection.managers.database_manager.connections.sqlite.models.api_model import (
     ApiModel,
@@ -55,19 +53,19 @@
 class media_table(TemplateMediaModel, Base):
     class media_legacy_table(TemplateMediaModel().legacy_2(LegacyBase), LegacyBase):
         pass
 
 
 def table_picker(table_name: str, legacy: bool = False):
     match table_name:
-        case "Stories":
+        case "Stories" | "Highlights":
             table = stories_table
         case "Posts":
             table = posts_table
-        case "Messages":
+        case "Messages" | "Chats" | "MassMessages":
             table = messages_table if not legacy else messages_table().api_legacy_table
         case "Products":
             table = products_table
         case "Others":
             table = others_table
         case _:
             raise Exception(f'"{table_name}" is an invalid table name')
```

### Comparing `ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/database_manager/connections/sqlite/sqlite_database.py` & `ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/sqlite_database.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 from datetime import datetime
 from pathlib import Path
-from typing import Any
+from typing import TYPE_CHECKING, Any
 
 import ultima_scraper_api
 from alembic import command
 from alembic.config import Config
 from alembic.migration import MigrationContext
 from sqlalchemy import create_engine, func
 from sqlalchemy.orm import DeclarativeBase, scoped_session, sessionmaker
 
 from ultima_scraper_collection.managers.database_manager.connections.sqlite.models import (
     user_database,
 )
 
+if TYPE_CHECKING:
+
+    from ultima_scraper_collection.managers.metadata_manager.metadata_manager import (
+        ContentMetadata,
+    )
+
 user_types = ultima_scraper_api.user_types
 
 
 class DBCollection(object):
     def __init__(self) -> None:
         self.user_database = user_database
 
@@ -118,92 +124,95 @@
                 alembic_cfg.set_main_option("sqlalchemy.url", self.info)
                 command.downgrade(alembic_cfg, "-1")
                 break
             except Exception as e:
                 print(e)
                 pass
 
-    def import_metadata(self, api_type: str, datas: list[dict[str, Any]]):
+    def import_metadata(
+        self, datas: list["ContentMetadata"], api_type: str | None = None
+    ):
         database_path = self.name
         database_path.parent.mkdir(parents=True, exist_ok=True)
         self.run_migrations()
         db_collection = DBCollection()
         database = db_collection.database_picker(database_path.stem)
         database_session = self.session
-        api_table = database.table_picker(api_type)
-        if not api_table:
-            return
         for post in datas:
-            post_id = post["post_id"]
-            postedAt = post["postedAt"]
+            if post.api_type:
+                api_type = post.api_type
+            api_table = database.table_picker(api_type)
+            if not api_table:
+                return
+            post_id = post.content_id
+            created_at_string = post.created_at_string
             date_object = None
-            if postedAt:
-                if not isinstance(postedAt, datetime):
-                    date_object = datetime.strptime(postedAt, "%d-%m-%Y %H:%M:%S")
-                else:
-                    date_object = postedAt
+            if created_at_string:
+                date_object = datetime.strptime(created_at_string, "%d-%m-%Y %H:%M:%S")
             result = database_session.query(api_table)
             post_db = result.filter_by(post_id=post_id).first()
             if not post_db:
                 post_db = api_table()
-            if api_type == "Products":
-                post_db.title = post["title"]
+            else:
+                pass
             if api_type == "Messages":
-                post_db.user_id = post.get("user_id", None)
+                post_db.user_id = post.user_id
             post_db.post_id = post_id
-            post_db.text = post["text"]
-            if post["price"] is None:
-                post["price"] = 0
-            post_db.price = post["price"]
-            post_db.paid = post["paid"]
-            post_db.archived = post["archived"]
+            post_db.text = post.text
+            post_db.price = post.price
+            post_db.paid = post.paid
+            post_db.archived = post.archived
             if date_object:
                 post_db.created_at = date_object
             database_session.add(post_db)
-            for media in post["medias"]:
-                if media["media_type"] == "Texts":
+            for media in post.medias:
+                if media.media_type == "Texts":
                     continue
-                created_at = media.get("created_at", postedAt)
+                created_at = media.created_at
                 if not isinstance(created_at, datetime):
                     date_object = datetime.strptime(created_at, "%d-%m-%Y %H:%M:%S")
-                else:
-                    date_object = postedAt
-                media_id = media.get("media_id", None)
+                media_id = media.id
                 result = database_session.query(database.media_table)
                 media_db = result.filter_by(post_id=post_id, media_id=media_id).first()
                 if not media_db:
                     media_db = result.filter_by(
-                        filename=media["filename"], created_at=date_object
+                        filename=media.filename, created_at=date_object
                     ).first()
                     if not media_db:
                         media_db = database.media_table()
+                else:
+                    pass
+                if (
+                    post.__legacy__
+                    and media_db.media_id != media.id
+                    and media_db.media_id
+                ):
+                    media_id = media_db.media_id
+
                 media_db.media_id = media_id
                 media_db.post_id = post_id
-                if "_sa_instance_state" in post:
-                    media_db.size = media["size"]
-                    media_db.downloaded = media["downloaded"]
-                media_db.link = media["links"][0]
-                media_db.preview = media.get("preview", False)
-                media_db.directory = media["directory"]
-                media_db.filename = media["filename"]
+                media_db.size = media.size if media_db.size is None else media_db.size
+                media_db.link = media.urls[0]
+                media_db.preview = media.preview
+                media_db.directory = media.directory.as_posix()
+                media_db.filename = media.filename
                 media_db.api_type = api_type
-                media_db.media_type = media["media_type"]
-                media_db.linked = media.get("linked", None)
+                media_db.media_type = media.media_type
+                media_db.linked = media.linked
                 if date_object:
                     media_db.created_at = date_object
                 database_session.add(media_db)
         database_session.commit()
         database_session.close()
         return True
 
     def legacy_sqlite_updater(
         self,
         api_type: str,
         subscription: user_types,
-        delete_metadatas: list[Path],
     ):
         final_result: list[dict[str, Any]] = []
         legacy_metadata_path = self.name
         if legacy_metadata_path.exists():
             self.run_migrations(legacy=True)
             database_name = "user_data"
             database_session = self.session
@@ -215,28 +224,22 @@
                 else:
                     api_table_table = database.table_picker(api_type)
                 media_table_table = database.media_table.media_legacy_table
                 if api_table_table:
                     result = database_session.query(api_table_table).all()
                     result2 = database_session.query(media_table_table).all()
                     for item in result:
-                        item: dict[str, int | list[Any]] = item.__dict__
-                        item["medias"] = []
                         for item2 in result2:
-                            if item["post_id"] != item2.post_id:
+                            if item.post_id != item2.post_id:
                                 continue
-                            item2 = item2.__dict__
-                            item2["links"] = [item2["link"]]
-                            item["medias"].append(item2)
-                        item["user_id"] = subscription.id
-                        item["postedAt"] = item["created_at"]
+                            item.medias.append(item2)
+                        item.user_id = subscription.id
                         final_result.append(item)
-                    delete_metadatas.append(legacy_metadata_path)
             database_session.close()
-        return final_result, delete_metadatas
+        return final_result
 
     def find_table(self, name: str):
         table = [x for x in self.metadata.sorted_tables if x.name == name]
         if table:
             return table[0]
 
     def get_count(self, q: Any):
```

### Comparing `ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/datascraper_manager/datascraper_manager.py` & `ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/datascraper_manager/datascraper_manager.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/datascraper_manager/datascrapers/fansly.py` & `ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/datascraper_manager/datascrapers/fansly.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,20 +2,23 @@
 from datetime import datetime
 from pathlib import Path
 from typing import Any, Union
 from urllib.parse import urlparse
 
 from ultima_scraper_api.apis.fansly.classes.auth_model import create_auth
 from ultima_scraper_api.apis.fansly.classes.collection_model import create_collection
-from ultima_scraper_api.apis.fansly.classes.create_story import create_story
 from ultima_scraper_api.apis.fansly.classes.message_model import create_message
 from ultima_scraper_api.apis.fansly.classes.post_model import create_post
+from ultima_scraper_api.apis.fansly.classes.story_model import create_story
 from ultima_scraper_api.apis.fansly.classes.user_model import create_user
 from ultima_scraper_api.apis.fansly.fansly import FanslyAPI
 
+from ultima_scraper_collection.managers.metadata_manager.metadata_manager import (
+    ContentMetadata,
+)
 from ultima_scraper_collection.managers.option_manager import OptionManager
 from ultima_scraper_collection.modules.module_streamliner import StreamlinedDatascraper
 
 
 class FanslyDataScraper(StreamlinedDatascraper):
     def __init__(self, api: FanslyAPI, option_manager: OptionManager) -> None:
         self.api = api
@@ -43,19 +46,67 @@
             pass
         if api_type == "Archived":
             pass
         if api_type == "Posts":
             pass
         if api_type == "Messages":
             pass
-        post_result.media.extend(post_result.previews)
-
         download_path = formatted_directory
         model_username = subscription.username
         date_format = site_settings.date_format
+        from ultima_scraper_collection.managers.metadata_manager.metadata_manager import (
+            Extractor,
+        )
+
+        content_metadata = ContentMetadata(post_result.id, api_type)
+        content_metadata.resolve_extractor(Extractor(post_result))
+        matches = [
+            s for s in site_settings.ignored_keywords if s in content_metadata.text
+        ]
+        if matches:
+            print("Ignoring - ", f"PostID: {content_metadata.content_id}")
+            return
+        for asset in content_metadata.medias:
+            filename = urlparse(asset.urls[0]).path.split("/")[-1]
+            name, ext = filename.rsplit(".", 1)
+            final_api_type = (
+                os.path.join("Archived", api_type)
+                if content_metadata.archived
+                else api_type
+            )
+            option: dict[str, Any] = {}
+            option = option | content_metadata.__dict__
+            option["site_name"] = api.site_name
+            option["media_id"] = asset.id
+            option["filename"] = name
+            option["api_type"] = final_api_type
+            option["media_type"] = asset.media_type
+            option["ext"] = ext
+            option["profile_username"] = authed.username
+            option["model_username"] = model_username
+            option["date_format"] = date_format
+            option["postedAt"] = asset.created_at
+            option["text_length"] = site_settings.text_length
+            option["directory"] = download_path
+            option["preview"] = asset.preview
+            option["archived"] = content_metadata.archived
+
+            prepared_format = prepare_reformat(option)
+            file_directory = await prepared_format.reformat_2(
+                site_settings.file_directory_format
+            )
+            prepared_format.directory = file_directory
+            file_path = await prepared_format.reformat_2(site_settings.filename_format)
+            asset.directory = file_directory
+            asset.filename = file_path.name
+            if file_directory not in directories:
+                directories.append(file_directory)
+        new_set["content"].append(content_metadata)
+        new_set["directories"] = directories
+        return new_set
         locations = self.media_types
         for media_type, alt_media_types in locations.__dict__.items():
             date_today = datetime.now()
             master_date = datetime.strftime(date_today, "%d-%m-%Y %H:%M:%S")
             file_directory_format = site_settings.file_directory_format
             post_id = post_result.id
             new_post: dict[str, Any | dict[str, Any]] = {}
@@ -71,24 +122,24 @@
                 date = post_result.createdAt
             if isinstance(post_result, create_post):
                 if post_result.isReportedByMe:
                     continue
                 rawText = post_result.rawText
                 text = post_result.text
                 _previews = post_result.previews
-                date = post_result.postedAt
+                date = post_result.createdAt
                 price = post_result.price
                 new_post["archived"] = post_result.isArchived
             if isinstance(post_result, create_collection):
                 if post_result.isReportedByMe:
                     continue
                 rawText = post_result.rawText
                 text = post_result.text
                 _previews = post_result.preview
-                date = post_result.postedAt
+                date = post_result.createdAt
                 price = post_result.price
                 new_post["archived"] = post_result.isArchived
             if isinstance(post_result, create_message):
                 if post_result.isReportedByMe:
                     continue
                 text = post_result.text
                 _previews = post_result.previews
@@ -256,14 +307,23 @@
         list[create_story]: A list containing all stories and archived stories from the subscription.
         """
         master_set: list[create_story] = []
         master_set.extend(await subscription.get_stories())
         # master_set.extend(await subscription.get_archived_stories())
         return master_set
 
+    async def get_all_posts(self, subscription: create_user):
+        temp_master_set = await subscription.get_posts()
+        collections = await subscription.get_collections()
+        for collection in collections:
+            temp_master_set.append(
+                await subscription.get_collection_content(collection)
+            )
+        return temp_master_set
+
     async def get_all_subscriptions(
         self,
         authed: create_auth,
         identifiers: list[int | str] = [],
         refresh: bool = True,
     ):
         """
```

### Comparing `ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/download_manager.py` & `ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/download_manager.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,64 +5,88 @@
 from ultima_scraper_api.helpers import main_helper
 from ultima_scraper_api.managers.session_manager import SessionManager
 
 from ultima_scraper_collection.managers.database_manager.connections.sqlite.models.media_model import (
     TemplateMediaModel,
 )
 from ultima_scraper_collection.managers.filesystem_manager import FilesystemManager
+from ultima_scraper_collection.managers.metadata_manager.metadata_manager import (
+    ContentMetadata,
+    MediaMetadata,
+)
 
 
 class DownloadManager:
     def __init__(
         self,
         filesystem_manager: FilesystemManager,
         session_manager: SessionManager,
-        download_list: set[TemplateMediaModel] = set(),
+        content_list: set[ContentMetadata] = set(),
         reformat: bool = True,
     ) -> None:
         self.filesystem_manager = filesystem_manager
         self.session_manager = session_manager
-        self.download_list: set[TemplateMediaModel] = download_list
+        self.content_list: set[ContentMetadata] = content_list
         self.errors: list[TemplateMediaModel] = []
         self.reformat = reformat
 
     async def bulk_download(self):
-        _result = await asyncio.gather(
-            *[self.download(x) for x in self.download_list], return_exceptions=True
-        )
-
-    async def download(self, download_item: TemplateMediaModel):
-        while True:
-            async with self.session_manager.semaphore:
-                result = await self.session_manager.request(download_item.link)
-                download_path = Path(download_item.directory, download_item.filename)
-                async with result as response:
-                    download = await self.check(download_item, response)
-                    if not download:
-                        break
-                    failed = await self.filesystem_manager.write_data(
-                        response, download_path
+        final_list: list[MediaMetadata] = [
+            self.download(media_item)
+            for download_item in self.content_list
+            for media_item in download_item.medias
+        ]
+        _result = await asyncio.gather(*final_list, return_exceptions=True)
+
+    async def download(self, download_item: MediaMetadata):
+        attempt = 0
+        content_metadata = download_item.__content_metadata__
+        db_content = content_metadata.__db_content__
+        db_media = db_content.find_media(download_item.id)
+        pass
+        while attempt < self.session_manager.max_attempts + 1:
+            try:
+                async with self.session_manager.semaphore:
+                    result = await self.session_manager.request(download_item.urls[0])
+                    download_path = Path(
+                        download_item.directory, download_item.filename
                     )
-                    if not failed:
-                        timestamp = download_item.created_at.timestamp()
-                        await main_helper.format_image(
-                            download_path,
-                            timestamp,
-                            self.reformat,
-                        )
-                        download_item.size = response.content_length
-                        download_item.downloaded = True
-                        break
-                    elif failed == 1:
-                        # Server Disconnect Error
+                    if result.status == 403:
+                        attempt += 1
+                        # test = await content_metadata._soft_.refresh()
                         continue
-                    elif failed == 2:
-                        # Resource Not Found Error
-                        break
+                    async with result as response:
+                        download = await self.check(db_media, response)
+                        if not download:
+                            break
+                        failed = await self.filesystem_manager.write_data(
+                            response, download_path
+                        )
+                        if not failed:
+                            timestamp = db_media.created_at.timestamp()
+                            await main_helper.format_image(
+                                download_path,
+                                timestamp,
+                                self.reformat,
+                            )
+                            db_media.size = response.content_length
+                            db_media.downloaded = True
+                            break
+                        elif failed == 1:
+                            # Server Disconnect Error
+                            continue
+                        elif failed == 2:
+                            # Resource Not Found Error
+                            break
+                        pass
                     pass
+            except asyncio.TimeoutError as e:
+                pass
+            except Exception as e:
+                print(e)
                 pass
 
     async def check(self, download_item: TemplateMediaModel, response: ClientResponse):
         filepath = Path(download_item.directory, download_item.filename)
         response_status = False
         if response.status == 200:
             response_status = True
```

### Comparing `ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/filesystem_manager.py` & `ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/filesystem_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,14 +41,17 @@
             yield each
 
     def check(self):
         for directory in self:
             if isinstance(directory, Path):
                 directory.mkdir(exist_ok=True)
 
+    def move(self, src: Path, trg: Path):
+        shutil.move(src, trg)
+
     def remove_mandatory_files(
         self, files: list[Path] | Generator[Path, None, None], keep: list[str] = []
     ):
         folders = [x for x in files if x.name not in self.ignore_files]
         if keep:
             folders = [x for x in files if x.name in keep]
         return folders
@@ -152,18 +155,15 @@
                 self.directory_manager, "metadata_directory_format"
             )
             # f_d_p_2.mkdir(parents=True, exist_ok=True)
             self.directory_manager_users[user.id] = directory_manager
             self.file_manager_users[user.id] = FileManager(directory_manager)
             return directory_manager
 
-    async def format_directories(
-        self,
-        subscription: user_types,
-    ) -> DirectoryManager:
+    async def format_directories(self, subscription: user_types) -> DirectoryManager:
 
         directory_manager = self.get_directory_manager(subscription.id)
         file_manager = self.get_file_manager(subscription.id)
         authed = subscription.get_authed()
         api = authed.api
         site_settings = authed.api.get_site_settings()
         if site_settings:
@@ -198,36 +198,17 @@
             )
             directory_manager.user.download_directory = (
                 formtatted_root_download_directory
             )
             await file_manager.set_default_files(
                 prepared_metadata_format, prepared_download_format
             )
-            metadata_filepaths = await file_manager.find_metadata_files(
+            _metadata_filepaths = await file_manager.find_metadata_files(
                 legacy_files=False
             )
-            for metadata_filepath in metadata_filepaths:
-                new_m_f = directory_manager.user.metadata_directory.joinpath(
-                    metadata_filepath.name
-                )
-                if metadata_filepath != new_m_f:
-                    counter = 0
-                    while True:
-                        if not new_m_f.exists():
-                            # If there's metadata present already before the directory is created, we'll create it here
-                            directory_manager.user.metadata_directory.mkdir(
-                                exist_ok=True, parents=True
-                            )
-                            shutil.move(metadata_filepath, new_m_f)
-                            break
-                        else:
-                            new_m_f = new_m_f.with_stem(
-                                f"{metadata_filepath.stem}_{counter}"
-                            )
-                            counter += 1
             # I forgot why we need to set default file twice
             await file_manager.set_default_files(
                 prepared_metadata_format, prepared_download_format
             )
             user_metadata_directory = directory_manager.user.metadata_directory
             _user_download_directory = directory_manager.user.download_directory
             legacy_metadata_directory = user_metadata_directory
```

### Comparing `ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/legacy_code.py` & `ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/legacy_code.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-0.1.4/ultima_scraper_collection/managers/option_manager.py` & `ultima_scraper_collection-1.0.0/ultima_scraper_collection/managers/option_manager.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-0.1.4/ultima_scraper_collection/modules/module_streamliner.py` & `ultima_scraper_collection-1.0.0/ultima_scraper_collection/modules/module_streamliner.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 from __future__ import annotations
 
 import copy
 from itertools import product
 from typing import Any, Optional
 
 import ultima_scraper_api
-import ultima_scraper_api.apis.fansly.classes as fansly_classes
 import ultima_scraper_api.classes.make_settings as make_settings
 from sqlalchemy.exc import OperationalError
 from tqdm.asyncio import tqdm_asyncio
-from ultima_scraper_api.helpers import main_helper
 from ultima_scraper_renamer import renamer
 
-from ultima_scraper_collection.managers.database_manager.connections.sqlite.models.media_model import (
-    TemplateMediaModel,
+from ultima_scraper_collection.managers.database_manager.connections.sqlite.models.api_model import (
+    ApiModel,
 )
 from ultima_scraper_collection.managers.database_manager.connections.sqlite.sqlite_database import (
     DBCollection,
 )
 from ultima_scraper_collection.managers.database_manager.database_manager import (
     DatabaseManager,
 )
@@ -37,14 +35,17 @@
 if TYPE_CHECKING:
     from ultima_scraper_collection.managers.datascraper_manager.datascrapers.fansly import (
         FanslyDataScraper,
     )
     from ultima_scraper_collection.managers.datascraper_manager.datascrapers.onlyfans import (
         OnlyFansDataScraper,
     )
+    from ultima_scraper_collection.managers.metadata_manager.metadata_manager import (
+        ContentMetadata,
+    )
 
     datascraper_types = OnlyFansDataScraper | FanslyDataScraper
 
 
 class download_session(tqdm_asyncio):
     def start(
         self,
@@ -69,16 +70,17 @@
 
 
 class StreamlinedDatascraper:
     def __init__(self, datascraper: datascraper_types) -> None:
         self.datascraper = datascraper
         self.filesystem_manager = FilesystemManager()
         self.content_types = self.datascraper.api.ContentTypes()
-        self.media_types = self.datascraper.api.Locations()
+        self.media_types = self.datascraper.api.MediaTypes()
         self.user_list: set[user_types] = set()
+        self.metadata_manager_users: dict[int, MetadataManager] = {}
 
     async def configure_datascraper_jobs(self):
         api = self.datascraper.api
         site_settings = api.get_site_settings()
         available_jobs = site_settings.jobs.scrape
         option_manager = self.datascraper.option_manager
         performer_options = option_manager.performer_options
@@ -112,15 +114,15 @@
             [valid_user_list.add(x) for x in chat_users]
 
         if available_jobs.paid_contents:
             for authed in self.datascraper.api.auths:
                 paid_contents = await authed.get_paid_content()
                 if not isinstance(paid_contents, error_types):
                     for paid_content in paid_contents:
-                        author = await paid_content.get_author()
+                        author = paid_content.get_author()
                         if identifiers:
                             found = await author.match_identifiers(identifiers)
                             if not found:
                                 continue
                         if author:
                             performer = await authed.get_subscription(
                                 identifier=author.id,
@@ -152,32 +154,23 @@
         current_job = subscription.get_current_job()
         if not current_job:
             return
         temp_master_set: list[Any] = copy.copy(master_set)
         if not temp_master_set:
             match content_type:
                 case "Stories":
-                    pass
                     temp_master_set.extend(
                         await self.datascraper.get_all_stories(subscription)
                     )
                     pass
                 case "Posts":
-                    temp_master_set = await subscription.get_posts()
-                    # Archived Posts
-                    if isinstance(subscription, fansly_classes.user_model.create_user):
-                        collections = await subscription.get_collections()
-                        for collection in collections:
-                            temp_master_set.append(
-                                await subscription.get_collection_content(collection)
-                            )
-                        pass
-                    else:
-                        temp_master_set += await subscription.get_archived_posts()
+                    temp_master_set = await self.datascraper.get_all_posts(subscription)
+                    pass
                 case "Messages":
+                    pass
                     unrefined_set: list[
                         message_types | Any
                     ] = await subscription.get_messages()
                     mass_messages = getattr(authed, "mass_messages")
                     if subscription.is_me() and mass_messages:
                         mass_messages = getattr(authed, "mass_messages")
                         # Need access to a creator's account to fix this
@@ -207,15 +200,16 @@
         master_set: list[dict[str, Any]],
         api_type: str,
         subscription: user_types,
         metadata_manager: MetadataManager,
     ):
         if not master_set:
             return False
-
+        # if  api_type != "Posts":
+        #     return
         authed = subscription.get_authed()
         subscription_directory_manager = self.filesystem_manager.get_directory_manager(
             subscription.id
         )
         formatted_metadata_directory = (
             subscription_directory_manager.user.metadata_directory
         )
@@ -231,127 +225,114 @@
                     [api_type],
                 ),
             )
             settings = {"colour": "MAGENTA"}
             unrefined_set: list[dict[str, Any]] = await tqdm_asyncio.gather(
                 *tasks, **settings
             )
-            new_metadata: dict[str, Any] = await main_helper.format_media_set(
-                unrefined_set
-            )
+            new_metadata = metadata_manager.merge_content_and_directories(unrefined_set)
+            final_content, _final_directories = new_metadata
             metadata_path = formatted_metadata_directory.joinpath("user_data.db")
             metadata_manager.db_manager = DatabaseManager().get_sqlite_db(metadata_path)
-            legacy_metadata_path = formatted_metadata_directory.joinpath(
-                api_type + ".db"
-            )
             if new_metadata:
-                new_metadata_content: list[dict[str, Any]] = new_metadata["content"]
+                new_metadata_content = final_content
+                metadata_manager.content_metadatas.extend(new_metadata_content)
                 print("Processing metadata.")
-                (
-                    old_metadata,
-                    delete_metadatas,
-                ) = await metadata_manager.process_legacy_metadata(
-                    subscription,
-                    api_type,
-                    metadata_path,
-                    subscription_directory_manager,
-                )
-                new_metadata_content.extend(old_metadata)
-                subscription.set_scraped(api_type, new_metadata_content)
-                result = await metadata_manager.process_metadata(
-                    legacy_metadata_path,
-                    new_metadata_content,
-                    api_type,
-                    subscription,
-                    delete_metadatas,
-                )
-                if result:
+                subscription.scrape_manager.set_scraped(api_type, new_metadata_content)
+                if new_metadata_content:
                     import_status = metadata_manager.db_manager.import_metadata(
-                        api_type, result
+                        new_metadata_content, api_type
                     )
                     if import_status:
                         Session = metadata_manager.db_manager.session_factory
                         if authed.api.config.settings.helpers.renamer:
-                            print("Renaming files.")
+                            print(f"{subscription.username}: Renaming files.")
                             _new_metadata_object = await renamer.start(
                                 subscription,
                                 subscription_directory_manager,
                                 api_type,
                                 Session,
                             )
-                        metadata_manager.delete_metadatas()
                         pass
             else:
                 print(f"No {api_type} found.")
         return True
 
     # Downloads scraped content
 
-    async def prepare_downloads(self, subscription: user_types, api_type: str):
-        global_settings = subscription.get_api().get_global_settings()
-        site_settings = subscription.get_api().get_site_settings()
+    async def prepare_downloads(self, performer: user_types, api_type: str):
+        metadata_manager = self.metadata_manager_users[performer.id]
+        global_settings = performer.get_api().get_global_settings()
+        site_settings = performer.get_api().get_site_settings()
         if not (global_settings and site_settings):
             return
         filesystem_manager = self.datascraper.filesystem_manager
-        subscription_directory_manager = filesystem_manager.get_directory_manager(
-            subscription.id
+        performer_directory_manager = filesystem_manager.get_directory_manager(
+            performer.id
         )
-        directory = subscription_directory_manager.root_download_directory
-        current_job = subscription.get_current_job()
+        directory = performer_directory_manager.root_download_directory
+        current_job = performer.get_current_job()
 
-        metadata_path = subscription_directory_manager.user.metadata_directory.joinpath(
+        metadata_path = performer_directory_manager.user.metadata_directory.joinpath(
             "user_data.db"
         )
         user_data_db = DatabaseManager().get_sqlite_db(metadata_path)
         if user_data_db and user_data_db.name.exists():
             database_session = user_data_db.session
             db_collection = DBCollection()
             database = db_collection.database_picker("user_data")
+            api_table = database.table_picker(api_type)
+            media_table = database.media_table
+            overwrite_files = site_settings.overwrite_files
+            media_set_count = 0
+            final_download_list: set[ContentMetadata] = set()
             if database:
-                media_table = database.media_table
-                overwrite_files = site_settings.overwrite_files
-                if overwrite_files:
-                    download_list: list[TemplateMediaModel] = (
-                        database_session.query(media_table)
-                        .filter(media_table.api_type == api_type)
-                        .all()
-                    )
-                    media_set_count = len(download_list)
-                else:
-                    download_list: list[TemplateMediaModel] = (
-                        database_session.query(media_table)
-                        .filter(media_table.downloaded == False)
-                        .filter(media_table.api_type == api_type)
-                    )
-                    media_set_count = user_data_db.get_count(download_list)
-                    pass
-                # Unique download list
-                final_download_list: set[TemplateMediaModel] = set()
-                for download_item in download_list:
-                    found = [
-                        x
-                        for x in download_list
-                        if download_item.media_id == x.media_id
-                        and download_item.api_type == x.api_type
-                    ]
-                    final_download_list.add(found[0])
+                db_content_dict = {}
+                db_posts: list[ApiModel] = database_session.query(api_table)
+                for db_post in db_posts:
+                    if db_post.post_id not in db_content_dict:
+                        db_content_dict[db_post.post_id] = db_post
+                    else:
+                        raise Exception("Duplicate key in db_content_dict")
+
+                content_metadatas = metadata_manager.content_metadatas
+                for content_metadata in content_metadatas:
+                    if content_metadata.api_type == api_type:
+                        db_post = db_content_dict[content_metadata.content_id]
+                        if content_metadata.content_id == db_post.post_id:
+                            content_metadata.__db_content__ = db_post
+                            db_media_query = (
+                                database_session.query(media_table)
+                                .filter(media_table.post_id == db_post.post_id)
+                                .filter(media_table.api_type == api_type)
+                            )
+                            if overwrite_files:
+                                db_post.medias = db_media_query.all()
+                            else:
+                                db_post.medias = db_media_query.filter(
+                                    media_table.downloaded == False
+                                ).all()
+                            if content_metadata.medias:
+                                final_download_list.add(content_metadata)
+                                media_set_count += len(db_post.medias)
                 download_manager = DownloadManager(
                     filesystem_manager,
-                    subscription.get_session_manager(),
+                    performer.get_session_manager(),
                     final_download_list,
                     global_settings.helpers.reformat_media,
                 )
                 location = ""
                 download_count = len(final_download_list)
                 duplicate_count = media_set_count - download_count
                 string = "Download Processing\n"
-                string += f"Name: {subscription.username} | Type: {api_type} | Downloading: {download_count} | Total: {media_set_count} | Duplicates: {duplicate_count} {location} | Directory: {directory}\n"
+                string += f"Name: {performer.username} | Type: {api_type} | Downloading: {download_count} | Total: {media_set_count} | Duplicates: {duplicate_count} {location} | Directory: {directory}\n"
                 if media_set_count:
                     print(string)
                     result = await download_manager.bulk_download()
+                    pass
                 while True:
                     try:
                         database_session.commit()
                         break
                     except OperationalError:
                         database_session.rollback()
                 database_session.close()
```

### Comparing `ultima_scraper_collection-0.1.4/setup.py` & `ultima_scraper_collection-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,20 +31,20 @@
 {'': ['*']}
 
 install_requires = \
 ['alembic>=1.9.2,<2.0.0',
  'psycopg2>=2.9.5,<3.0.0',
  'sqlalchemy>=2.0.1,<3.0.0',
  'tqdm>=4.65.0,<5.0.0',
- 'ultima-scraper-api>=0.1.3,<0.2.0',
- 'ultima-scraper-renamer>=0.1.3,<0.2.0']
+ 'ultima-scraper-api>=1.0.0,<2.0.0',
+ 'ultima-scraper-renamer>=1.0.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'ultima-scraper-collection',
-    'version': '0.1.4',
+    'version': '1.0.0',
     'description': '',
     'long_description': 'None',
     'author': 'DIGITALCRIMINALS',
     'author_email': '89371864+digitalcriminals@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `ultima_scraper_collection-0.1.4/PKG-INFO` & `ultima_scraper_collection-1.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ultima-scraper-collection
-Version: 0.1.4
+Version: 1.0.0
 Summary: 
 Author: DIGITALCRIMINALS
 Author-email: 89371864+digitalcriminals@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: alembic (>=1.9.2,<2.0.0)
 Requires-Dist: psycopg2 (>=2.9.5,<3.0.0)
 Requires-Dist: sqlalchemy (>=2.0.1,<3.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
-Requires-Dist: ultima-scraper-api (>=0.1.3,<0.2.0)
-Requires-Dist: ultima-scraper-renamer (>=0.1.3,<0.2.0)
+Requires-Dist: ultima-scraper-api (>=1.0.0,<2.0.0)
+Requires-Dist: ultima-scraper-renamer (>=1.0.0,<2.0.0)
```

