# Comparing `tmp/lndb-0.42.0.tar.gz` & `tmp/lndb-0.43.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lndb-0.42.0.tar", last modified: Tue Apr 18 16:35:27 2023, max compression
+gzip compressed data, was "lndb-0.43.0.tar", last modified: Fri Apr 21 00:22:24 2023, max compression
```

## Comparing `lndb-0.42.0.tar` & `lndb-0.43.0.tar`

### file list

```diff
@@ -1,79 +1,80 @@
--rw-r--r--   0        0        0     3832 2023-04-10 13:46:35.171473 lndb-0.42.0/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-01-15 12:18:16.566196 lndb-0.42.0/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-01-15 12:18:16.566256 lndb-0.42.0/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1204 2023-01-15 12:18:16.566326 lndb-0.42.0/.gitignore
--rw-r--r--   0        0        0     1772 2023-01-16 03:13:03.815140 lndb-0.42.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2023-01-15 12:18:16.566501 lndb-0.42.0/LICENSE
--rw-r--r--   0        0        0      173 2023-03-27 04:37:15.707800 lndb-0.42.0/README.md
--rw-r--r--   0        0        0       52 2023-03-06 11:50:26.265030 lndb-0.42.0/docs/api.md
--rw-r--r--   0        0        0    46143 2023-04-18 16:35:03.521407 lndb-0.42.0/docs/changelog.md
--rw-r--r--   0        0        0     4832 2023-03-22 14:41:54.962234 lndb-0.42.0/docs/faq/check-synchronization.ipynb
--rw-r--r--   0        0        0     3334 2023-03-09 09:28:04.965028 lndb-0.42.0/docs/faq/clone.ipynb
--rw-r--r--   0        0        0     8397 2023-03-22 05:59:33.863010 lndb-0.42.0/docs/faq/edge-cases-login-init.ipynb
--rw-r--r--   0        0        0      166 2023-03-22 14:56:35.817208 lndb-0.42.0/docs/faq/index.md
--rw-r--r--   0        0        0     1180 2023-04-05 05:10:26.112382 lndb-0.42.0/docs/faq/manage-migrations.ipynb
--rw-r--r--   0        0        0     3248 2023-03-09 09:28:04.965998 lndb-0.42.0/docs/faq/switch-environment.ipynb
--rw-r--r--   0        0        0     2798 2023-04-05 05:10:26.112662 lndb-0.42.0/docs/faq/test-migrations-e2e.ipynb
--rw-r--r--   0        0        0     2073 2023-04-05 05:10:26.112933 lndb-0.42.0/docs/faq/test-migrations-unit.ipynb
--rw-r--r--   0        0        0     5163 2023-04-10 13:41:10.762652 lndb-0.42.0/docs/guide/01-setup-user.ipynb
--rw-r--r--   0        0        0    10679 2023-04-07 09:41:26.324653 lndb-0.42.0/docs/guide/02-init-instance.ipynb
--rw-r--r--   0        0        0     5573 2023-03-22 14:56:35.818426 lndb-0.42.0/docs/guide/03-load-instance.ipynb
--rw-r--r--   0        0        0     5290 2023-03-09 09:28:04.966850 lndb-0.42.0/docs/guide/04-set-storage.ipynb
--rw-r--r--   0        0        0     3724 2023-03-22 05:59:33.864269 lndb-0.42.0/docs/guide/05-schema-modules.ipynb
--rw-r--r--   0        0        0     1496 2023-03-22 05:59:33.864524 lndb-0.42.0/docs/guide/06-info.ipynb
--rw-r--r--   0        0        0     3282 2023-03-22 05:59:33.864793 lndb-0.42.0/docs/guide/07-delete.ipynb
--rw-r--r--   0        0        0      129 2023-02-16 15:52:14.590660 lndb-0.42.0/docs/guide/index.md
--rw-r--r--   0        0        0     3152 2023-03-25 20:23:06.444401 lndb-0.42.0/docs/guide/migrate.md
--rw-r--r--   0        0        0      126 2023-02-16 21:53:37.660107 lndb-0.42.0/docs/index.md
--rw-r--r--   0        0        0      118 2023-02-17 10:58:37.191812 lndb-0.42.0/lamin-project.yaml
--rw-r--r--   0        0        0     1932 2023-04-18 16:34:47.279466 lndb-0.42.0/lndb/__init__.py
--rw-r--r--   0        0        0     4242 2023-02-27 18:35:12.951712 lndb-0.42.0/lndb/__main__.py
--rw-r--r--   0        0        0      100 2023-02-12 04:51:38.272115 lndb-0.42.0/lndb/_assets/__init__.py
--rw-r--r--   0        0        0     1414 2023-04-10 10:56:05.782722 lndb-0.42.0/lndb/_check_instance_setup.py
--rw-r--r--   0        0        0      216 2023-04-18 16:33:57.539501 lndb-0.42.0/lndb/_check_versions.py
--rw-r--r--   0        0        0      567 2023-04-08 10:27:51.832949 lndb-0.42.0/lndb/_close.py
--rw-r--r--   0        0        0     2146 2023-04-05 13:47:39.618861 lndb-0.42.0/lndb/_delete.py
--rw-r--r--   0        0        0      222 2023-02-16 21:53:37.660919 lndb-0.42.0/lndb/_info.py
--rw-r--r--   0        0        0     5710 2023-04-08 10:27:51.833294 lndb-0.42.0/lndb/_init_instance.py
--rw-r--r--   0        0        0     3980 2023-04-16 17:51:14.687298 lndb-0.42.0/lndb/_load_instance.py
--rw-r--r--   0        0        0      135 2023-04-05 05:10:26.113647 lndb-0.42.0/lndb/_migrate/__init__.py
--rw-r--r--   0        0        0      723 2023-04-05 05:10:26.113978 lndb-0.42.0/lndb/_migrate/alembic.ini
--rw-r--r--   0        0        0     3469 2023-04-05 12:41:02.533096 lndb-0.42.0/lndb/_migrate/core.py
--rw-r--r--   0        0        0     6303 2023-04-05 05:10:26.114561 lndb-0.42.0/lndb/_migrate/deploy.py
--rw-r--r--   0        0        0     3179 2023-02-16 21:53:37.661733 lndb-0.42.0/lndb/_migrate/env.py
--rw-r--r--   0        0        0      341 2023-02-16 21:53:37.661843 lndb-0.42.0/lndb/_migrate/script.py.mako
--rw-r--r--   0        0        0     4840 2023-04-05 05:10:26.114776 lndb-0.42.0/lndb/_migrate/utils.py
--rw-r--r--   0        0        0     1020 2023-02-12 04:51:38.274334 lndb-0.42.0/lndb/_schema.py
--rw-r--r--   0        0        0     1493 2023-04-08 10:27:51.833937 lndb-0.42.0/lndb/_set.py
--rw-r--r--   0        0        0     2181 2023-04-07 09:41:26.325000 lndb-0.42.0/lndb/_settings.py
--rw-r--r--   0        0        0       87 2023-02-16 21:53:37.662311 lndb-0.42.0/lndb/_settings_load.py
--rw-r--r--   0        0        0       72 2023-02-16 21:53:37.662460 lndb-0.42.0/lndb/_settings_store.py
--rw-r--r--   0        0        0     4927 2023-04-11 15:29:00.205425 lndb-0.42.0/lndb/_setup_user.py
--rw-r--r--   0        0        0      533 2023-04-08 10:27:51.834128 lndb-0.42.0/lndb/dev/__init__.py
--rw-r--r--   0        0        0     4030 2023-03-27 17:35:42.591834 lndb-0.42.0/lndb/dev/_clone.py
--rw-r--r--   0        0        0     6226 2023-04-07 09:41:26.325330 lndb-0.42.0/lndb/dev/_db.py
--rw-r--r--   0        0        0     2491 2023-02-16 21:53:37.663214 lndb-0.42.0/lndb/dev/_deprecated.py
--rw-r--r--   0        0        0      240 2023-02-16 21:53:37.663286 lndb-0.42.0/lndb/dev/_docs.py
--rw-r--r--   0        0        0     5317 2023-04-08 10:27:51.834481 lndb-0.42.0/lndb/dev/_exclusion.py
--rw-r--r--   0        0        0     8429 2023-04-08 10:27:51.834794 lndb-0.42.0/lndb/dev/_settings_instance.py
--rw-r--r--   0        0        0     2629 2023-03-22 05:59:33.865686 lndb-0.42.0/lndb/dev/_settings_load.py
--rw-r--r--   0        0        0     2061 2023-02-16 21:53:37.663723 lndb-0.42.0/lndb/dev/_settings_save.py
--rw-r--r--   0        0        0     2314 2023-04-07 05:02:28.778847 lndb-0.42.0/lndb/dev/_settings_store.py
--rw-r--r--   0        0        0      976 2023-02-16 21:53:37.663901 lndb-0.42.0/lndb/dev/_settings_user.py
--rw-r--r--   0        0        0     2446 2023-03-21 06:52:10.981980 lndb-0.42.0/lndb/dev/_setup_knowledge.py
--rw-r--r--   0        0        0     6997 2023-04-17 13:30:19.225702 lndb-0.42.0/lndb/dev/_setup_schema.py
--rw-r--r--   0        0        0     4917 2023-04-08 10:27:51.835175 lndb-0.42.0/lndb/dev/_storage.py
--rw-r--r--   0        0        0      140 2023-02-24 20:31:36.945684 lndb-0.42.0/lndb/dev/_testdb.py
--rw-r--r--   0        0        0     2536 2023-04-08 10:27:51.835422 lndb-0.42.0/lndb/dev/upath.py
--rw-r--r--   0        0        0      356 2023-04-05 05:10:26.115134 lndb-0.42.0/lndb/test/__init__.py
--rw-r--r--   0        0        0       50 2023-02-24 20:31:36.946187 lndb-0.42.0/lndb/test/_env.py
--rw-r--r--   0        0        0     3856 2023-03-30 17:54:01.454075 lndb-0.42.0/lndb/test/_migrations_e2e.py
--rw-r--r--   0        0        0     6646 2023-04-05 05:10:26.115464 lndb-0.42.0/lndb/test/_migrations_unit.py
--rw-r--r--   0        0        0      310 2023-02-24 20:31:36.946490 lndb-0.42.0/lndb/test/_nox.py
--rw-r--r--   0        0        0      188 2023-02-22 22:13:54.788863 lndb-0.42.0/lndb/test/nox.py
--rw-r--r--   0        0        0     1003 2023-04-10 13:46:02.409554 lndb-0.42.0/noxfile.py
--rw-r--r--   0        0        0     1395 2023-04-18 16:33:57.539648 lndb-0.42.0/pyproject.toml
--rw-r--r--   0        0        0      513 2023-04-10 13:57:46.942655 lndb-0.42.0/tests/test_bionty.py
--rw-r--r--   0        0        0      680 2023-03-09 09:28:04.969725 lndb-0.42.0/tests/test_init_instance.py
--rw-r--r--   0        0        0      384 2023-04-18 16:23:45.828153 lndb-0.42.0/tests/test_notebooks.py
--rw-r--r--   0        0        0     1197 1970-01-01 00:00:00.000000 lndb-0.42.0/PKG-INFO
+-rw-r--r--   0        0        0     3832 2023-04-10 13:46:35.171473 lndb-0.43.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-01-15 12:18:16.566196 lndb-0.43.0/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-01-15 12:18:16.566256 lndb-0.43.0/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1204 2023-01-15 12:18:16.566326 lndb-0.43.0/.gitignore
+-rw-r--r--   0        0        0     1772 2023-01-16 03:13:03.815140 lndb-0.43.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2023-01-15 12:18:16.566501 lndb-0.43.0/LICENSE
+-rw-r--r--   0        0        0      173 2023-03-27 04:37:15.707800 lndb-0.43.0/README.md
+-rw-r--r--   0        0        0       52 2023-03-06 11:50:26.265030 lndb-0.43.0/docs/api.md
+-rw-r--r--   0        0        0    46932 2023-04-21 00:21:53.441957 lndb-0.43.0/docs/changelog.md
+-rw-r--r--   0        0        0     4832 2023-03-22 14:41:54.962234 lndb-0.43.0/docs/faq/check-synchronization.ipynb
+-rw-r--r--   0        0        0     3334 2023-03-09 09:28:04.965028 lndb-0.43.0/docs/faq/clone.ipynb
+-rw-r--r--   0        0        0     8397 2023-03-22 05:59:33.863010 lndb-0.43.0/docs/faq/edge-cases-login-init.ipynb
+-rw-r--r--   0        0        0      166 2023-03-22 14:56:35.817208 lndb-0.43.0/docs/faq/index.md
+-rw-r--r--   0        0        0     1180 2023-04-05 05:10:26.112382 lndb-0.43.0/docs/faq/manage-migrations.ipynb
+-rw-r--r--   0        0        0     3248 2023-03-09 09:28:04.965998 lndb-0.43.0/docs/faq/switch-environment.ipynb
+-rw-r--r--   0        0        0     2798 2023-04-05 05:10:26.112662 lndb-0.43.0/docs/faq/test-migrations-e2e.ipynb
+-rw-r--r--   0        0        0     2073 2023-04-05 05:10:26.112933 lndb-0.43.0/docs/faq/test-migrations-unit.ipynb
+-rw-r--r--   0        0        0     5163 2023-04-10 13:41:10.762652 lndb-0.43.0/docs/guide/01-setup-user.ipynb
+-rw-r--r--   0        0        0    11110 2023-04-21 00:21:08.924113 lndb-0.43.0/docs/guide/02-init-instance.ipynb
+-rw-r--r--   0        0        0     5355 2023-04-21 00:21:08.924266 lndb-0.43.0/docs/guide/03-load-instance.ipynb
+-rw-r--r--   0        0        0     5418 2023-04-20 08:37:12.609361 lndb-0.43.0/docs/guide/04-set-storage.ipynb
+-rw-r--r--   0        0        0     3724 2023-03-22 05:59:33.864269 lndb-0.43.0/docs/guide/05-schema-modules.ipynb
+-rw-r--r--   0        0        0     1496 2023-03-22 05:59:33.864524 lndb-0.43.0/docs/guide/06-info.ipynb
+-rw-r--r--   0        0        0     2689 2023-04-20 14:48:13.955039 lndb-0.43.0/docs/guide/07-delete.ipynb
+-rw-r--r--   0        0        0      129 2023-02-16 15:52:14.590660 lndb-0.43.0/docs/guide/index.md
+-rw-r--r--   0        0        0     3152 2023-03-25 20:23:06.444401 lndb-0.43.0/docs/guide/migrate.md
+-rw-r--r--   0        0        0      126 2023-02-16 21:53:37.660107 lndb-0.43.0/docs/index.md
+-rw-r--r--   0        0        0      118 2023-02-17 10:58:37.191812 lndb-0.43.0/lamin-project.yaml
+-rw-r--r--   0        0        0     1993 2023-04-21 00:21:42.236801 lndb-0.43.0/lndb/__init__.py
+-rw-r--r--   0        0        0     4507 2023-04-21 00:21:08.924595 lndb-0.43.0/lndb/__main__.py
+-rw-r--r--   0        0        0      100 2023-02-12 04:51:38.272115 lndb-0.43.0/lndb/_assets/__init__.py
+-rw-r--r--   0        0        0     1414 2023-04-10 10:56:05.782722 lndb-0.43.0/lndb/_check_instance_setup.py
+-rw-r--r--   0        0        0      216 2023-04-18 16:33:57.539501 lndb-0.43.0/lndb/_check_versions.py
+-rw-r--r--   0        0        0      567 2023-04-08 10:27:51.832949 lndb-0.43.0/lndb/_close.py
+-rw-r--r--   0        0        0     2146 2023-04-05 13:47:39.618861 lndb-0.43.0/lndb/_delete.py
+-rw-r--r--   0        0        0      222 2023-02-16 21:53:37.660919 lndb-0.43.0/lndb/_info.py
+-rw-r--r--   0        0        0     6042 2023-04-21 00:21:08.924753 lndb-0.43.0/lndb/_init_instance.py
+-rw-r--r--   0        0        0     4003 2023-04-19 13:17:39.106450 lndb-0.43.0/lndb/_load_instance.py
+-rw-r--r--   0        0        0      135 2023-04-05 05:10:26.113647 lndb-0.43.0/lndb/_migrate/__init__.py
+-rw-r--r--   0        0        0      723 2023-04-05 05:10:26.113978 lndb-0.43.0/lndb/_migrate/alembic.ini
+-rw-r--r--   0        0        0     3469 2023-04-05 12:41:02.533096 lndb-0.43.0/lndb/_migrate/core.py
+-rw-r--r--   0        0        0     6303 2023-04-05 05:10:26.114561 lndb-0.43.0/lndb/_migrate/deploy.py
+-rw-r--r--   0        0        0     3179 2023-02-16 21:53:37.661733 lndb-0.43.0/lndb/_migrate/env.py
+-rw-r--r--   0        0        0      341 2023-02-16 21:53:37.661843 lndb-0.43.0/lndb/_migrate/script.py.mako
+-rw-r--r--   0        0        0     4840 2023-04-05 05:10:26.114776 lndb-0.43.0/lndb/_migrate/utils.py
+-rw-r--r--   0        0        0      700 2023-04-21 00:21:08.924850 lndb-0.43.0/lndb/_register_instance.py
+-rw-r--r--   0        0        0     1020 2023-02-12 04:51:38.274334 lndb-0.43.0/lndb/_schema.py
+-rw-r--r--   0        0        0     1313 2023-04-20 08:37:12.610024 lndb-0.43.0/lndb/_set.py
+-rw-r--r--   0        0        0     2189 2023-04-18 20:05:50.820265 lndb-0.43.0/lndb/_settings.py
+-rw-r--r--   0        0        0       87 2023-02-16 21:53:37.662311 lndb-0.43.0/lndb/_settings_load.py
+-rw-r--r--   0        0        0       72 2023-02-16 21:53:37.662460 lndb-0.43.0/lndb/_settings_store.py
+-rw-r--r--   0        0        0     3902 2023-04-21 00:21:08.925324 lndb-0.43.0/lndb/_setup_user.py
+-rw-r--r--   0        0        0      533 2023-04-08 10:27:51.834128 lndb-0.43.0/lndb/dev/__init__.py
+-rw-r--r--   0        0        0     4030 2023-03-27 17:35:42.591834 lndb-0.43.0/lndb/dev/_clone.py
+-rw-r--r--   0        0        0     6226 2023-04-07 09:41:26.325330 lndb-0.43.0/lndb/dev/_db.py
+-rw-r--r--   0        0        0     2491 2023-02-16 21:53:37.663214 lndb-0.43.0/lndb/dev/_deprecated.py
+-rw-r--r--   0        0        0      240 2023-02-16 21:53:37.663286 lndb-0.43.0/lndb/dev/_docs.py
+-rw-r--r--   0        0        0     5317 2023-04-08 10:27:51.834481 lndb-0.43.0/lndb/dev/_exclusion.py
+-rw-r--r--   0        0        0     8649 2023-04-21 00:21:08.925542 lndb-0.43.0/lndb/dev/_settings_instance.py
+-rw-r--r--   0        0        0     2629 2023-03-22 05:59:33.865686 lndb-0.43.0/lndb/dev/_settings_load.py
+-rw-r--r--   0        0        0     2061 2023-02-16 21:53:37.663723 lndb-0.43.0/lndb/dev/_settings_save.py
+-rw-r--r--   0        0        0     2314 2023-04-20 14:59:21.978668 lndb-0.43.0/lndb/dev/_settings_store.py
+-rw-r--r--   0        0        0      976 2023-02-16 21:53:37.663901 lndb-0.43.0/lndb/dev/_settings_user.py
+-rw-r--r--   0        0        0     2446 2023-03-21 06:52:10.981980 lndb-0.43.0/lndb/dev/_setup_knowledge.py
+-rw-r--r--   0        0        0     6997 2023-04-17 13:30:19.225702 lndb-0.43.0/lndb/dev/_setup_schema.py
+-rw-r--r--   0        0        0     4917 2023-04-08 10:27:51.835175 lndb-0.43.0/lndb/dev/_storage.py
+-rw-r--r--   0        0        0      140 2023-02-24 20:31:36.945684 lndb-0.43.0/lndb/dev/_testdb.py
+-rw-r--r--   0        0        0     2536 2023-04-08 10:27:51.835422 lndb-0.43.0/lndb/dev/upath.py
+-rw-r--r--   0        0        0      356 2023-04-05 05:10:26.115134 lndb-0.43.0/lndb/test/__init__.py
+-rw-r--r--   0        0        0       50 2023-02-24 20:31:36.946187 lndb-0.43.0/lndb/test/_env.py
+-rw-r--r--   0        0        0     3870 2023-04-19 13:17:39.107152 lndb-0.43.0/lndb/test/_migrations_e2e.py
+-rw-r--r--   0        0        0     6646 2023-04-05 05:10:26.115464 lndb-0.43.0/lndb/test/_migrations_unit.py
+-rw-r--r--   0        0        0      310 2023-02-24 20:31:36.946490 lndb-0.43.0/lndb/test/_nox.py
+-rw-r--r--   0        0        0      188 2023-02-22 22:13:54.788863 lndb-0.43.0/lndb/test/nox.py
+-rw-r--r--   0        0        0     1003 2023-04-10 13:46:02.409554 lndb-0.43.0/noxfile.py
+-rw-r--r--   0        0        0     1395 2023-04-18 16:33:57.539648 lndb-0.43.0/pyproject.toml
+-rw-r--r--   0        0        0      513 2023-04-10 13:57:46.942655 lndb-0.43.0/tests/test_bionty.py
+-rw-r--r--   0        0        0      680 2023-03-09 09:28:04.969725 lndb-0.43.0/tests/test_init_instance.py
+-rw-r--r--   0        0        0      384 2023-04-18 16:23:45.828153 lndb-0.43.0/tests/test_notebooks.py
+-rw-r--r--   0        0        0     1197 1970-01-01 00:00:00.000000 lndb-0.43.0/PKG-INFO
```

### Comparing `lndb-0.42.0/.github/workflows/build.yml` & `lndb-0.43.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lndb-0.42.0/.github/workflows/latest-changes.yml` & `lndb-0.43.0/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lndb-0.42.0/.gitignore` & `lndb-0.43.0/.gitignore`

 * *Files identical despite different names*

### Comparing `lndb-0.42.0/.pre-commit-config.yaml` & `lndb-0.43.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lndb-0.42.0/LICENSE` & `lndb-0.43.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lndb-0.42.0/docs/changelog.md` & `lndb-0.43.0/docs/changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+🚸 Allow registering local postgres instances on the hub | [361](https://github.com/laminlabs/lndb/pull/361) | [falexwolf](https://github.com/falexwolf) | 2023-04-21 | 0.43.0
+🚸 Add a `is_db_setup()` check after init and make it more robust | [362](https://github.com/laminlabs/lndb/pull/362) | [falexwolf](https://github.com/falexwolf) | 2023-04-20 |
+👷 Remove lnhub-rest CI calls | [360](https://github.com/laminlabs/lndb/pull/360) | [falexwolf](https://github.com/falexwolf) | 2023-04-20 |
+🚸 Enable non-owner to set storage | [358](https://github.com/laminlabs/lndb/pull/358) | [falexwolf](https://github.com/falexwolf) | 2023-04-19 |
+♻️ Restructure hub imports | [357](https://github.com/laminlabs/lndb/pull/357) | [falexwolf](https://github.com/falexwolf) | 2023-04-18 |
 ⬆️ Upgrade to lnhub_rest 0.8.1 | [356](https://github.com/laminlabs/lndb/pull/356) | [falexwolf](https://github.com/falexwolf) | 2023-04-18 | 0.42.0
 ✅ Use nbproject-test directly | [355](https://github.com/laminlabs/lndb/pull/355) | [Koncopd](https://github.com/Koncopd) | 2023-04-18 |
 🔊 Clarify access based on locally cached instance metadata | [354](https://github.com/laminlabs/lndb/pull/354) | [falexwolf](https://github.com/falexwolf) | 2023-04-11 | 0.41.0
 🎨 Move setup checks from lamindb here | [352](https://github.com/laminlabs/lndb/pull/352) | [falexwolf](https://github.com/falexwolf) | 2023-04-08 | 0.41rc1
 🔧 Increase configure-aws-credentials version from v1 to v2 | [344](https://github.com/laminlabs/lndb/pull/344) | [Zethson](https://github.com/Zethson) | 2023-04-07 |
 🚸 Expose `id` in `StorageSettings` | [351](https://github.com/laminlabs/lndb/pull/351) | [falexwolf](https://github.com/falexwolf) | 2023-04-07 | 0.40.2
 ➕ Add cloudpathlib back | [350](https://github.com/laminlabs/lndb/pull/350) | [falexwolf](https://github.com/falexwolf) | 2023-04-07 | 0.40.1
```

### Comparing `lndb-0.42.0/docs/faq/check-synchronization.ipynb` & `lndb-0.43.0/docs/faq/check-synchronization.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.42.0/docs/faq/clone.ipynb` & `lndb-0.43.0/docs/faq/clone.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.42.0/docs/faq/edge-cases-login-init.ipynb` & `lndb-0.43.0/docs/faq/edge-cases-login-init.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.42.0/docs/faq/manage-migrations.ipynb` & `lndb-0.43.0/docs/faq/manage-migrations.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.42.0/docs/faq/switch-environment.ipynb` & `lndb-0.43.0/docs/faq/switch-environment.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.42.0/docs/faq/test-migrations-e2e.ipynb` & `lndb-0.43.0/docs/faq/test-migrations-e2e.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.42.0/docs/faq/test-migrations-unit.ipynb` & `lndb-0.43.0/docs/faq/test-migrations-unit.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.42.0/docs/guide/01-setup-user.ipynb` & `lndb-0.43.0/docs/guide/01-setup-user.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.42.0/docs/guide/02-init-instance.ipynb` & `lndb-0.43.0/docs/guide/02-init-instance.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9863140792031098%*

 * *Differences: {"'cells'": '{3: {\'source\': [\'ln.setup.login("testuser1")  # CLI: lamin login testuser1\']}, 6: '*

 * *            "{'source': {insert: [(1, '!lamin init --storage ./mydata\\n')], delete: [1]}, "*

 * *            "'attachments': OrderedDict()}, 8: {'source': ['This automatically assigns an instance "*

 * *            "name that equals the name of the storage root along with a few other settings:'], "*

 * *            "'attachments': OrderedDict()}, 9: {'source': ['ln.setup.settings.instance']}, 18: "*

 * *            "{'source': […]*

```diff
@@ -29,15 +29,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln.setup.login(\"testuser1\")  # shell: lamin login testuser1"
+                "ln.setup.login(\"testuser1\")  # CLI: lamin login testuser1"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Init a local instance"
@@ -47,45 +47,47 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### SQLite"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "```\n",
-                "!lamin init --storage mydata\n",
+                "!lamin init --storage ./mydata\n",
                 "```"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "ln.setup.init(storage=\"./mydata\")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "This automatically assigns an instance name that equals the name of the storage root:"
+                "This automatically assigns an instance name that equals the name of the storage root along with a few other settings:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln.setup.settings.instance.name"
+                "ln.setup.settings.instance"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": [
@@ -184,31 +186,28 @@
             "metadata": {
                 "tags": [
                     "hide-cell"
                 ]
             },
             "outputs": [],
             "source": [
-                "# clean up settings\n",
-                "ln.setup.delete(\"pgtest\")"
+                "!lamin delete pgtest\n",
+                "!docker stop pgtest && docker rm pgtest"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": [
                     "hide-cell"
                 ]
             },
             "outputs": [],
-            "source": [
-                "# clean up docker\n",
-                "!docker stop pgtest && docker rm pgtest"
-            ]
+            "source": []
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Provide a custom instance name"
             ]
@@ -256,15 +255,18 @@
                 "assert ln.setup.settings.instance.owner == ln.setup.settings.user.handle\n",
                 "assert ln.setup.settings.instance.dialect == \"postgresql\"\n",
                 "assert ln.setup.settings.instance.db == pgurl\n",
                 "assert (\n",
                 "    ln.setup.settings.instance.storage.root.as_posix()\n",
                 "    == Path(\"mystorage\").absolute().as_posix()\n",
                 ")\n",
-                "assert ln.setup.settings.instance.storage.cache_dir is None"
+                "assert ln.setup.settings.instance.storage.cache_dir is None\n",
+                "\n",
+                "!lamin delete mydata2\n",
+                "!docker stop pgtest && docker rm pgtest"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Configure with cloud storage"
@@ -305,42 +307,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln.setup.settings.instance.name"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "ln.setup.settings.instance.storage.root"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "ln.setup.settings.instance.storage.cache_dir"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "ln.setup.settings.instance.db"
+                "ln.setup.settings.instance"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -432,14 +407,58 @@
                 "ln.setup.delete(\"lndb-setup-ci-us\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
+                "## Register a local instance on the hub"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "pgurl = setup_local_test_postgres(name=\"pgtest-registered\")"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "```\n",
+                "!lamin init --storage ./mydatapg --name pgtest-registered --hub\n",
+                "```"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "ln.setup.init(storage=\"s3://lndb-setup-ci\", db=pgurl)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "ln.setup.register()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
                 "## Re-initializing an existing instance"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
```

### Comparing `lndb-0.42.0/docs/guide/03-load-instance.ipynb` & `lndb-0.43.0/docs/guide/03-load-instance.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9928039965986395%*

 * *Differences: {"'cells'": '{7: {\'source\': {insert: [(1, \'ln.setup.load("pgtest-registered")\\n\'), (2, '*

 * *            "'assert settings.instance.storage.is_cloud == True\\n'), (3, 'assert "*

 * *            'settings.instance.name == "pgtest-registered"\\n\'), (4, \'assert '*

 * *            'settings.instance.storage.root_as_str == "s3://lndb-setup-ci"\')], delete: [5, 4, 3, '*

 * *            "2, 1]}}, 11: {'source': {insert: [(1, 'assert settings.instance.storage.root_as_str "*

 * *            '== "s3://lndb-setup-ci"\\n\'), (2, \'asse […]*

```diff
@@ -85,19 +85,18 @@
                 "tags": [
                     "hide-cell"
                 ]
             },
             "outputs": [],
             "source": [
                 "# another test case, this time with a manually configured instance name\n",
-                "ln.setup.load(\"mydata2\")\n",
-                "assert settings.instance.storage.is_cloud == False\n",
-                "assert settings.instance.name == \"mydata2\"\n",
-                "assert settings.instance.storage.root.as_posix() == f\"{os.getcwd()}/mystorage\"\n",
-                "assert settings.instance.storage.cache_dir is None"
+                "ln.setup.load(\"pgtest-registered\")\n",
+                "assert settings.instance.storage.is_cloud == True\n",
+                "assert settings.instance.name == \"pgtest-registered\"\n",
+                "assert settings.instance.storage.root_as_str == \"s3://lndb-setup-ci\""
             ]
         },
         {
             "cell_type": "markdown",
             "id": "3f47a1d4",
             "metadata": {},
             "source": [
@@ -137,16 +136,18 @@
                 "tags": [
                     "hide-cell"
                 ]
             },
             "outputs": [],
             "source": [
                 "assert settings.instance.storage.is_cloud == True\n",
-                "assert str(settings.instance.storage.root) == \"s3://lndb-setup-ci/\"\n",
-                "assert str(settings.instance._sqlite_file) == \"s3://lndb-setup-ci/lndb-setup-ci.lndb\""
+                "assert settings.instance.storage.root_as_str == \"s3://lndb-setup-ci\"\n",
+                "assert (\n",
+                "    settings.instance._sqlite_file.as_posix() == \"s3://lndb-setup-ci/lndb-setup-ci.lndb\"\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "914af9a6",
             "metadata": {},
             "source": [
@@ -215,30 +216,16 @@
                 "tags": [
                     "hide-cell"
                 ]
             },
             "outputs": [],
             "source": [
                 "# clean up\n",
-                "ln.setup.delete(\"mydata2\")"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "35c91d7f-8fbf-455f-ae61-6690eaf29154",
-            "metadata": {
-                "tags": [
-                    "hide-cell"
-                ]
-            },
-            "outputs": [],
-            "source": [
-                "# clean up\n",
-                "!docker stop pgtest && docker rm pgtest"
+                "!lamin delete pgtest-registered\n",
+                "!docker stop pgtest-registered && docker rm pgtest-registered"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
```

### Comparing `lndb-0.42.0/docs/guide/04-set-storage.ipynb` & `lndb-0.43.0/docs/guide/04-set-storage.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9899147727272727%*

 * *Differences: {"'cells'": "{1: {'source': ['import lamindb as ln\\n', 'from pathlib import Path\\n', 'import "*

 * *            "laminci']}, 3: {'source': ['pgurl = laminci.db.setup_local_test_postgres()']}, 5: "*

 * *            "{'source': {insert: [(2, '!lamin set --storage ./storage_2\\n')], delete: [2]}, "*

 * *            "'attachments': OrderedDict()}, 7: {'metadata': {'tags': []}, 'source': ['assert "*

 * *            'ln.setup.settings.storage.root_as_str == f"{Path.cwd()}/storage_2"\']}, 10: '*

 * *            "{'source': ['assert ln.s […]*

```diff
@@ -13,15 +13,17 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "33c2bb76-d61f-4866-87e2-780e61600022",
             "metadata": {},
             "outputs": [],
             "source": [
-                "import lamindb as ln"
+                "import lamindb as ln\n",
+                "from pathlib import Path\n",
+                "import laminci"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "a7cf42fb",
             "metadata": {},
             "source": [
@@ -35,37 +37,36 @@
             "metadata": {
                 "tags": [
                     "hide-cell"
                 ]
             },
             "outputs": [],
             "source": [
-                "import lndb\n",
-                "\n",
-                "pgurl = lndb.dev.setup_local_test_postgres()"
+                "pgurl = laminci.db.setup_local_test_postgres()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "d6b0bd5e",
             "metadata": {},
             "outputs": [],
             "source": [
                 "ln.setup.init(storage=\"./storage_1\", db=pgurl)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "ceb57cc9",
             "metadata": {},
             "source": [
                 "Running \n",
                 "```\n",
-                "!lamin set --storage storage_2\n",
+                "!lamin set --storage ./storage_2\n",
                 "```\n",
                 "on the command line runs the following Python function:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -77,23 +78,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "8e481aa0",
             "metadata": {
-                "tags": [
-                    "hide-cell"
-                ]
+                "tags": []
             },
             "outputs": [],
             "source": [
-                "from pathlib import Path\n",
-                "\n",
-                "assert ln.setup.settings.instance.storage.root.as_posix() == f\"{Path.cwd()}/storage_2\""
+                "assert ln.setup.settings.storage.root_as_str == f\"{Path.cwd()}/storage_2\""
             ]
         },
         {
             "cell_type": "markdown",
             "id": "25a13298",
             "metadata": {},
             "source": [
@@ -122,16 +119,16 @@
             "metadata": {
                 "tags": [
                     "hide-cell"
                 ]
             },
             "outputs": [],
             "source": [
-                "assert ln.setup.settings.instance.storage.is_cloud == True\n",
-                "assert str(ln.setup.settings.instance.storage.root) == \"s3://lndb-setup-ci/\""
+                "assert ln.setup.settings.storage.is_cloud\n",
+                "assert ln.setup.settings.storage.root_as_str == \"s3://lndb-setup-ci\""
             ]
         },
         {
             "cell_type": "markdown",
             "id": "529e68e5-9b10-4fdb-9d4c-ac8206bbbb68",
             "metadata": {},
             "source": [
@@ -151,21 +148,33 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "2ed8716f-852f-4ce9-8eef-5b824d6e92b3",
             "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "ln.setup.set.storage(\"./storage_3\")"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "cad87623",
+            "metadata": {
                 "tags": [
                     "hide-cell"
                 ]
             },
             "outputs": [],
             "source": [
-                "assert ln.setup.set.storage(\"storage_3\") == \"only-owner-can-set-storage\""
+                "assert ln.setup.settings.storage.root_as_str == f\"{Path.cwd()}/storage_3\""
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "78a819fa-48d6-4c6f-95d4-7dc7e94283bb",
             "metadata": {
@@ -218,17 +227,15 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "e4f2545f",
             "metadata": {
-                "tags": [
-                    "hide-cell"
-                ]
+                "tags": []
             },
             "outputs": [],
             "source": [
                 "assert ln.setup.set.storage(\"mydata_storage_2\") == \"set-storage-failed\""
             ]
         },
         {
```

### Comparing `lndb-0.42.0/docs/guide/05-schema-modules.ipynb` & `lndb-0.43.0/docs/guide/05-schema-modules.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.42.0/docs/guide/06-info.ipynb` & `lndb-0.43.0/docs/guide/06-info.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.42.0/docs/guide/07-delete.ipynb` & `lndb-0.43.0/docs/guide/07-delete.ipynb`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9674479166666666%*

 * *Differences: {"'cells'": "{1: {'source': ['import lamindb as ln']}, 2: {'source': "*

 * *            '[\'ln.setup.login("testuser1")\']}, 4: {\'source\': '*

 * *            '[\'ln.setup.init(storage="mydata-delete")\']}, 6: {\'source\': '*

 * *            '[\'ln.setup.delete("mydata-delete")\']}, 7: {\'metadata\': {replace: '*

 * *            "OrderedDict([('tags', ['hide-cell'])])}, 'source': {insert: [(0, 'from "*

 * *            "lndb.dev._settings_store import instance_settings_file\\n'), (1, '\\n'), (2, "*

 * *            '\'settings_file = ins […]*

```diff
@@ -13,28 +13,25 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "33c2bb76-d61f-4866-87e2-780e61600022",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from lndb import delete, load, login, init, settings\n",
-                "from lndb.dev._settings_store import instance_settings_file\n",
-                "from pathlib import Path\n",
-                "from datetime import datetime"
+                "import lamindb as ln"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "485f5ee1",
             "metadata": {},
             "outputs": [],
             "source": [
-                "login(\"testuser1\")"
+                "ln.setup.login(\"testuser1\")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "cceb6b43",
             "metadata": {},
             "source": [
@@ -44,16 +41,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "2609e58d",
             "metadata": {},
             "outputs": [],
             "source": [
-                "init(storage=\"mydata-delete\")\n",
-                "settings_file = instance_settings_file(\"mydata-delete\", \"testuser1\")"
+                "ln.setup.init(storage=\"mydata-delete\")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "25a13298",
             "metadata": {},
             "source": [
@@ -66,83 +62,60 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "8436575d",
             "metadata": {},
             "outputs": [],
             "source": [
-                "delete(\"mydata-delete\")"
+                "ln.setup.delete(\"mydata-delete\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "d2e607c9",
-            "metadata": {},
+            "metadata": {
+                "tags": [
+                    "hide-cell"
+                ]
+            },
             "outputs": [],
             "source": [
+                "from lndb.dev._settings_store import instance_settings_file\n",
+                "\n",
+                "settings_file = instance_settings_file(\"mydata-delete\", \"testuser1\")\n",
                 "assert settings_file.exists() == False"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "3286fbcc",
             "metadata": {},
             "source": [
                 "## With remote default storage"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "fa1efbce",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "instance_name = f\"lamin.ci.instance.{datetime.now().timestamp()}\""
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
             "id": "037f38a3",
             "metadata": {},
             "outputs": [],
             "source": [
-                "init(storage=\"s3://lndb-setup-delete-ci\", name=instance_name)"
+                "ln.setup.init(storage=\"s3://lndb-setup-delete-ci\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "b2593ef8",
             "metadata": {},
             "outputs": [],
             "source": [
-                "delete(instance_name)"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "06a22900",
-            "metadata": {},
-            "source": [
-                "Clean up instances."
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "9117428e",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "from lnhub_rest._clean_ci import delete_ci_instances\n",
-                "\n",
-                "delete_ci_instances()"
+                "ln.setup.delete(\"lndb-setup-delete-ci\")"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
```

### Comparing `lndb-0.42.0/docs/guide/migrate.md` & `lndb-0.43.0/docs/guide/migrate.md`

 * *Files identical despite different names*

### Comparing `lndb-0.42.0/lndb/__init__.py` & `lndb-0.43.0/lndb/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 .. autosummary::
    :toctree:
 
    close
    delete
    info
    set
+   register
 
 Manage creating and testing migrations (deployment is automatic):
 
 .. autosummary::
    :toctree:
 
    migrate
@@ -46,27 +47,28 @@
 
 .. autosummary::
    :toctree:
 
    dev
 """
 
-__version__ = "0.42.0"  # denote a release candidate for 0.1.0 with 0.1rc1
+__version__ = "0.43.0"  # denote a release candidate for 0.1.0 with 0.1rc1
 
 import sys
 from os import name as _os_name
 
 from . import _check_versions  # noqa
 from . import dev, test
 from ._close import close  # noqa
 from ._delete import delete  # noqa
 from ._info import info  # noqa
 from ._init_instance import init  # noqa
 from ._load_instance import load  # noqa
 from ._migrate import migrate
+from ._register_instance import register  # noqa
 from ._schema import schema  # noqa
 from ._set import set, set_storage  # noqa
 from ._settings import settings  # noqa
 from ._setup_user import login, signup  # noqa
 
 
 # unlock and clear even if an uncaught exception happens
```

### Comparing `lndb-0.42.0/lndb/__main__.py` & `lndb-0.43.0/lndb/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 import argparse
 import os
 import sys
 
 from lamin_logger import logger
 
-from . import _init_instance, _setup_user, delete, info, set_storage
+from . import _init_instance, _setup_user, delete, info, register, set
 from ._close import close as close_instance
 from ._init_instance import description as instance
 from .dev._settings_user import user_description as user
 
 signup_help = "First time sign up."
 login_help = "Log in an already-signed-up user."
 init_help = "Init & config instance with db & storage."
 load_help = "Load instance by name."
 set_storage_help = "Set storage used by an instance."
 info_help = "Show current instance information."
 close_help = "Close instance."
 migr_help = "Manage migrations."
 delete_help = "Delete an instance."
+register_help = (
+    "Register instance on hub (local instances are not automatically registered)."
+)
+
 
 description_cli = "Configure LaminDB and perform simple actions."
 parser = argparse.ArgumentParser(
     description=description_cli, formatter_class=argparse.RawTextHelpFormatter
 )
 subparsers = parser.add_subparsers(dest="command")
 
@@ -67,15 +71,18 @@
 
 # set storage
 set_storage_parser = subparsers.add_parser("set", help=set_storage_help)
 aa = set_storage_parser.add_argument
 aa("--storage", type=str, metavar="s", help=instance.storage_root)
 
 # close instance
-close = subparsers.add_parser("close", help=close_help)
+subparsers.add_parser("close", help=close_help)
+
+# register instance
+subparsers.add_parser("register", help=register_help)
 
 # migrate
 migr = subparsers.add_parser("migrate", help=migr_help)
 aa = migr.add_argument
 aa("action", choices=["generate"], help="Generate migration.")
 
 # parse args
@@ -97,32 +104,37 @@
     if args.command == "login":
         return _setup_user.login(
             args.user,
             password=args.password,
         )
     elif args.command == "init":
         result = _init_instance.init(
-            storage=args.storage, db=args.db, schema=args.schema, name=args.name
+            storage=args.storage,
+            db=args.db,
+            schema=args.schema,
+            name=args.name,
         )
         return process_result(result)
     elif args.command == "load":
         result = _init_instance.load(
             identifier=args.instance,
         )
         return process_result(result)
     elif args.command == "close":
         return close_instance()
+    elif args.command == "register":
+        return register()
     elif args.command == "delete":
         return delete(
             instance_name=args.instance,
         )
     elif args.command == "info":
         return info()
     elif args.command == "set":
-        return set_storage(storage=args.storage)
+        return set.storage(args.storage)
     elif args.command == "migrate":
         from . import migrate
 
         if args.action == "generate":
             return migrate.generate()
     else:
         logger.error("Invalid command. Try `lamin -h`.")
```

### Comparing `lndb-0.42.0/lndb/_check_instance_setup.py` & `lndb-0.43.0/lndb/_check_instance_setup.py`

 * *Files identical despite different names*

### Comparing `lndb-0.42.0/lndb/_close.py` & `lndb-0.43.0/lndb/_close.py`

 * *Files identical despite different names*

### Comparing `lndb-0.42.0/lndb/_delete.py` & `lndb-0.43.0/lndb/_delete.py`

 * *Files identical despite different names*

### Comparing `lndb-0.42.0/lndb/_init_instance.py` & `lndb-0.43.0/lndb/_init_instance.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import importlib
 import sys
 from pathlib import Path
 from typing import Optional, Union
 
 from lamin_logger import logger
-from lnhub_rest._add_storage import get_storage_region
-from lnhub_rest._init_instance import init_instance as init_instance_hub
-from lnhub_rest._init_instance import (
+from lnhub_rest.core.instance._init_instance import init_instance as init_instance_hub
+from lnhub_rest.core.instance._init_instance import (
     validate_db_arg,
     validate_schema_arg,
     validate_storage_arg,
 )
+from lnhub_rest.core.storage._add_storage import get_storage_region
 from pydantic import PostgresDsn
 
 from lndb.dev.upath import UPath
 
 from ._load_instance import load, load_from_isettings
 from ._settings import settings
 from .dev import InstanceSettings
@@ -117,36 +117,44 @@
         ):
             raise RuntimeError(
                 ERROR_SQLITE_CACHE.format(
                     isettings._sqlite_file, isettings._sqlite_file_local
                 )
             )
 
-    # for remote instance, a lot of validation happens in the next function
-    # if this errors, the whole function errors
     if isettings.is_remote:
         result = init_instance_hub(
             owner=owner,
             name=name_str,
             storage=str(storage),
             db=db,
             schema=schema,
         )
         if result == "instance-exists-already":
             pass  # everything is alright!
         elif isinstance(result, str):
             raise RuntimeError(f"Creating instance on hub failed:\n{result}")
+        logger.success(f"Registered instance on hub: https://lamin.ai/{owner}/{name}")
+    else:
+        logger.info(
+            "Not registering instance on hub, if you want, call `lamin register`"
+        )
 
+    # this does not yet setup a setup for a new database
     persist_settings_load_schema(isettings)
 
     message = None
     if not isettings._is_db_setup()[0]:
         setup_schema(isettings, settings.user)
         register(isettings, settings.user)
         write_bionty_versions(isettings)
+        # now ensure that everything worked
+        check, msg = isettings._is_db_setup()
+        if not check:
+            raise RuntimeError(msg)
     else:
         # we're currently using this for testing migrations
         # passing connection strings of databases that need to be tested
         # for migrations
         logger.warning("Your instance seems already set up, attempt load:")
         message = load_from_isettings(isettings, migrate=_migrate)
```

### Comparing `lndb-0.42.0/lndb/_load_instance.py` & `lndb-0.43.0/lndb/_load_instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import os
 from typing import Optional
 
 from lamin_logger import logger
-from lnhub_rest._load_instance import load_instance as load_instance_from_hub
+from lnhub_rest.core.instance._load_instance import (
+    load_instance as load_instance_from_hub,
+)
 
 from ._settings import InstanceSettings, settings
 from .dev._settings_load import load_instance_settings
 from .dev._settings_store import instance_settings_file
 
 
 def load(
```

### Comparing `lndb-0.42.0/lndb/_migrate/alembic.ini` & `lndb-0.43.0/lndb/_migrate/alembic.ini`

 * *Files identical despite different names*

### Comparing `lndb-0.42.0/lndb/_migrate/core.py` & `lndb-0.43.0/lndb/_migrate/core.py`

 * *Files identical despite different names*

### Comparing `lndb-0.42.0/lndb/_migrate/deploy.py` & `lndb-0.43.0/lndb/_migrate/deploy.py`

 * *Files identical despite different names*

### Comparing `lndb-0.42.0/lndb/_migrate/env.py` & `lndb-0.43.0/lndb/_migrate/env.py`

 * *Files identical despite different names*

### Comparing `lndb-0.42.0/lndb/_migrate/utils.py` & `lndb-0.43.0/lndb/_migrate/utils.py`

 * *Files identical despite different names*

### Comparing `lndb-0.42.0/lndb/_schema.py` & `lndb-0.43.0/lndb/_schema.py`

 * *Files identical despite different names*

### Comparing `lndb-0.42.0/lndb/_set.py` & `lndb-0.43.0/lndb/_set.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pathlib import Path
 from typing import Union
 
 from lamin_logger import logger
-from lnhub_rest._add_storage import add_storage as add_storage_hub
+from lnhub_rest.core.storage._add_storage import add_storage as add_storage_hub
 
 from lndb.dev.upath import UPath
 
 from ._init_instance import register
 from ._settings import settings
 from .dev import deprecated
 from .dev._settings_instance import InstanceSettings
@@ -14,18 +14,14 @@
 
 class set:
     """Set properties of current instance."""
 
     @staticmethod
     def storage(root: Union[str, Path, UPath]):
         """Set storage."""
-        if settings.instance.owner != settings.user.handle:
-            logger.error("Can only set storage if current user is instance owner.")
-            return "only-owner-can-set-storage"
-
         if settings.instance.dialect == "sqlite":
             logger.error("Can't set storage for sqlite instances.")
             return "set-storage-failed"
 
         new_isettings = InstanceSettings(
             owner=settings.instance.owner,
             name=settings.instance.name,
```

### Comparing `lndb-0.42.0/lndb/_settings.py` & `lndb-0.43.0/lndb/_settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         return self.fget(owner_cls)
 
 
 class settings:
     """Settings access.
 
     - :class:`~lndb.dev.InstanceSettings`
-    - :class:`~lndb.dev.Storage`
+    - :class:`~lndb.dev.StorageSettings`
     - :class:`~lndb.dev.UserSettings`
     """
 
     _user_settings: Union[UserSettings, None] = None
     _instance_settings: Union[InstanceSettings, None] = None
 
     _user_settings_env: Union[str, None] = None
```

### Comparing `lndb-0.42.0/lndb/dev/__init__.py` & `lndb-0.43.0/lndb/dev/__init__.py`

 * *Files identical despite different names*

### Comparing `lndb-0.42.0/lndb/dev/_clone.py` & `lndb-0.43.0/lndb/dev/_clone.py`

 * *Files identical despite different names*

### Comparing `lndb-0.42.0/lndb/dev/_db.py` & `lndb-0.43.0/lndb/dev/_db.py`

 * *Files identical despite different names*

### Comparing `lndb-0.42.0/lndb/dev/_deprecated.py` & `lndb-0.43.0/lndb/dev/_deprecated.py`

 * *Files identical despite different names*

### Comparing `lndb-0.42.0/lndb/dev/_exclusion.py` & `lndb-0.43.0/lndb/dev/_exclusion.py`

 * *Files identical despite different names*

### Comparing `lndb-0.42.0/lndb/dev/_settings_instance.py` & `lndb-0.43.0/lndb/dev/_settings_instance.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import shutil
 from pathlib import Path
 from typing import Literal, Optional, Set, Tuple, Union
 
 import sqlalchemy as sa
 import sqlmodel as sqm
+from lamin_logger import logger
 from pydantic import PostgresDsn
 from sqlalchemy.future import Engine
 
 from ._exclusion import empty_locker, get_locker
 from ._settings_save import save_instance_settings
 from ._settings_store import current_instance_settings_file, instance_settings_file
 from ._storage import Storage
@@ -53,15 +54,15 @@
     def __repr__(self):
         """Rich string representation."""
         representation = f"Current instance: {self.identifier}"
         attrs = ["owner", "name", "storage", "db", "schema"]
         for attr in attrs:
             value = getattr(self, attr)
             if attr == "storage":
-                representation += f"\n- storage root: {value.root}"
+                representation += f"\n- storage root: {value.root_as_str}"
                 representation += f"\n- storage region: {value.region}"
             else:
                 representation += f"\n- {attr}: {value}"
         return representation
 
     @property
     def owner(self) -> str:
@@ -211,33 +212,36 @@
         # need to import here to avoid circular import
         from .._settings import settings
 
         settings._instance_settings = self
 
     def _is_db_setup(self) -> Tuple[bool, str]:
         """Is the database available and initialized as LaminDB?"""
+        if not self._is_db_reachable():
+            if self.dialect == "sqlite":
+                return False, f"SQLite file {self._sqlite_file} does not exist"
+            else:
+                return False, f"Connection {self.db} not reachable"
+        # cannot import lnschema_core here, yet!
+
+        with self.engine.connect() as conn:
+            try:
+                result = conn.execute(sa.text("select * from version_yvzi")).first()
+            except Exception as e:
+                return False, f"Your DB is not initialized: {e}"
+            if result is None:
+                return False, "Your DB is not initialized: version_yvzi has no row"
+        return True, ""
+
+    def _is_db_reachable(self) -> bool:
         if self.dialect == "sqlite":
             if not self._sqlite_file.exists():
-                return False, "SQLite file does not exist"
-            else:
-                return True, ""
-        else:  # postgres
-            assert self.dialect == "postgresql"
-            with self.engine.connect() as conn:
-                results = conn.execute(
-                    sa.text(
-                        """
-                    SELECT EXISTS (
-                        SELECT FROM
-                            information_schema.tables
-                        WHERE
-                            table_schema LIKE 'public' AND
-                            table_name = 'version_yvzi'
-                    );
-                """
-                    )
-                ).first()  # returns tuple of boolean
-                check = results[0]
-                if not check:
-                    return False, "Postgres does not seem initialized."
-                else:
-                    return True, ""
+                logger.warning(f"SQLite file {self._sqlite_file} does not exist")
+                return False
+        else:
+            engine = sa.create_engine(self.db)
+            try:
+                engine.connect()
+            except Exception:
+                logger.warning(f"Connection {self.db} not reachable")
+                return False
+        return True
```

### Comparing `lndb-0.42.0/lndb/dev/_settings_load.py` & `lndb-0.43.0/lndb/dev/_settings_load.py`

 * *Files identical despite different names*

### Comparing `lndb-0.42.0/lndb/dev/_settings_save.py` & `lndb-0.43.0/lndb/dev/_settings_save.py`

 * *Files identical despite different names*

### Comparing `lndb-0.42.0/lndb/dev/_settings_store.py` & `lndb-0.43.0/lndb/dev/_settings_store.py`

 * *Files identical despite different names*

### Comparing `lndb-0.42.0/lndb/dev/_settings_user.py` & `lndb-0.43.0/lndb/dev/_settings_user.py`

 * *Files identical despite different names*

### Comparing `lndb-0.42.0/lndb/dev/_setup_knowledge.py` & `lndb-0.43.0/lndb/dev/_setup_knowledge.py`

 * *Files identical despite different names*

### Comparing `lndb-0.42.0/lndb/dev/_setup_schema.py` & `lndb-0.43.0/lndb/dev/_setup_schema.py`

 * *Files identical despite different names*

### Comparing `lndb-0.42.0/lndb/dev/_storage.py` & `lndb-0.43.0/lndb/dev/_storage.py`

 * *Files identical despite different names*

### Comparing `lndb-0.42.0/lndb/dev/upath.py` & `lndb-0.43.0/lndb/dev/upath.py`

 * *Files identical despite different names*

### Comparing `lndb-0.42.0/lndb/test/_migrations_e2e.py` & `lndb-0.43.0/lndb/test/_migrations_e2e.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from subprocess import run
 from typing import Optional
 
 from lamin_logger import logger
 from lnhub_rest._assets import instances as test_instances
-from lnhub_rest._init_instance import (
+from lnhub_rest.core.instance._init_instance import (
     validate_db_arg,
     validate_schema_arg,
     validate_storage_arg,
 )
 
 from lndb._init_instance import infer_instance_name, init
 from lndb._settings import settings
```

### Comparing `lndb-0.42.0/lndb/test/_migrations_unit.py` & `lndb-0.43.0/lndb/test/_migrations_unit.py`

 * *Files identical despite different names*

### Comparing `lndb-0.42.0/noxfile.py` & `lndb-0.43.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `lndb-0.42.0/pyproject.toml` & `lndb-0.43.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lndb-0.42.0/tests/test_bionty.py` & `lndb-0.43.0/tests/test_bionty.py`

 * *Files identical despite different names*

### Comparing `lndb-0.42.0/tests/test_init_instance.py` & `lndb-0.43.0/tests/test_init_instance.py`

 * *Files identical despite different names*

### Comparing `lndb-0.42.0/PKG-INFO` & `lndb-0.43.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lndb
-Version: 0.42.0
+Version: 0.43.0
 Summary: LaminDB setup.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: lnhub_rest==0.8.1
 Requires-Dist: laminci>=0.3.0
 Requires-Dist: lnschema_core>=0.28.0
 Requires-Dist: lamin_logger>=0.2.3
```

