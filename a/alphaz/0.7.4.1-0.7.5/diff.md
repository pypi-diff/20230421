# Comparing `tmp/alphaz-0.7.4.1.tar.gz` & `tmp/alphaz-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alphaz-0.7.4.1.tar", last modified: Wed Apr 19 12:08:17 2023, max compression
+gzip compressed data, was "dist/alphaz-0.7.5.tar", last modified: Fri Apr 21 07:48:01 2023, max compression
```

## Comparing `alphaz-0.7.4.1.tar` & `alphaz-0.7.5.tar`

### file list

```diff
@@ -1,389 +1,391 @@
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.278191 alphaz-0.7.4.1/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    11114 2023-04-19 12:08:16.000000 alphaz-0.7.4.1/MANIFEST.in
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      589 2023-04-19 12:08:17.282191 alphaz-0.7.4.1/PKG-INFO
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1348 2021-07-12 18:07:51.000000 alphaz-0.7.4.1/README.md
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.218191 alphaz-0.7.4.1/alphaz/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        9 2023-04-18 09:00:04.000000 alphaz-0.7.4.1/alphaz/README.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      333 2023-04-13 12:43:58.000000 alphaz-0.7.4.1/alphaz/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      104 2021-03-29 08:42:45.000000 alphaz-0.7.4.1/alphaz/alphaz.bat
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       70 2021-03-29 08:42:45.000000 alphaz-0.7.4.1/alphaz/alphaz.code-workspace
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      208 2022-04-19 08:43:27.000000 alphaz-0.7.4.1/alphaz/alphaz.sh
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       48 2021-03-29 08:42:45.000000 alphaz-0.7.4.1/alphaz/api.bat
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      713 2023-04-18 09:00:04.000000 alphaz-0.7.4.1/alphaz/api.json
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      770 2022-04-13 09:59:51.000000 alphaz-0.7.4.1/alphaz/api.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.222191 alphaz-0.7.4.1/alphaz/apis/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.4.1/alphaz/apis/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2022-07-21 11:35:27.000000 alphaz-0.7.4.1/alphaz/apis/log.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2721 2023-03-17 07:06:42.000000 alphaz-0.7.4.1/alphaz/apis/mails.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.222191 alphaz-0.7.4.1/alphaz/apis/routes/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.4.1/alphaz/apis/routes/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1577 2023-02-23 09:08:35.000000 alphaz-0.7.4.1/alphaz/apis/routes/admin.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1137 2021-03-29 08:42:45.000000 alphaz-0.7.4.1/alphaz/apis/routes/api.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3062 2023-02-23 09:08:35.000000 alphaz-0.7.4.1/alphaz/apis/routes/basic_tests.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3094 2023-04-18 09:00:04.000000 alphaz-0.7.4.1/alphaz/apis/routes/database.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      413 2022-04-12 11:53:03.000000 alphaz-0.7.4.1/alphaz/apis/routes/git.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     7225 2023-02-01 13:59:24.000000 alphaz-0.7.4.1/alphaz/apis/routes/logs.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1810 2022-04-12 11:53:03.000000 alphaz-0.7.4.1/alphaz/apis/routes/mails.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6262 2023-03-17 07:21:40.000000 alphaz-0.7.4.1/alphaz/apis/routes/main.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1330 2023-02-23 09:08:35.000000 alphaz-0.7.4.1/alphaz/apis/routes/tests.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.222191 alphaz-0.7.4.1/alphaz/apis/routes/user_management/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      114 2022-04-27 13:24:50.000000 alphaz-0.7.4.1/alphaz/apis/routes/user_management/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2475 2022-05-09 13:31:06.000000 alphaz-0.7.4.1/alphaz/apis/routes/user_management/application_management.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2228 2022-05-09 13:31:06.000000 alphaz-0.7.4.1/alphaz/apis/routes/user_management/permission_management.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4058 2022-08-31 08:56:44.000000 alphaz-0.7.4.1/alphaz/apis/routes/user_management/role_management.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1291 2022-08-31 08:56:44.000000 alphaz-0.7.4.1/alphaz/apis/routes/user_management/user_management.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3025 2023-03-17 18:14:36.000000 alphaz-0.7.4.1/alphaz/apis/routes/users.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      584 2023-02-23 09:08:35.000000 alphaz-0.7.4.1/alphaz/apis/tests.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.222191 alphaz-0.7.4.1/alphaz/apis/users/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2022-07-21 11:35:27.000000 alphaz-0.7.4.1/alphaz/apis/users/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2718 2023-01-25 21:39:07.000000 alphaz-0.7.4.1/alphaz/apis/users/ldap.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    11543 2023-03-28 08:47:21.000000 alphaz-0.7.4.1/alphaz/apis/users/users.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.226191 alphaz-0.7.4.1/alphaz/config/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.4.1/alphaz/config/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      795 2021-03-29 08:42:45.000000 alphaz-0.7.4.1/alphaz/config/config.css
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    12602 2021-03-29 08:42:45.000000 alphaz-0.7.4.1/alphaz/config/config.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      707 2022-08-11 06:44:17.000000 alphaz-0.7.4.1/alphaz/config/main_configuration.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      823 2021-03-29 08:42:45.000000 alphaz-0.7.4.1/alphaz/config/page.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1700 2021-03-29 08:42:45.000000 alphaz-0.7.4.1/alphaz/config/source.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1564 2021-03-29 08:42:45.000000 alphaz-0.7.4.1/alphaz/config.json
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      238 2023-01-06 09:14:28.000000 alphaz-0.7.4.1/alphaz/core.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.226191 alphaz-0.7.4.1/alphaz/documentations/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.226191 alphaz-0.7.4.1/alphaz/documentations/docs/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2022-07-21 11:35:27.000000 alphaz-0.7.4.1/alphaz/documentations/docs/alpha_admin.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1408 2023-04-12 11:28:51.000000 alphaz-0.7.4.1/alphaz/documentations/docs/alpha_core.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2595 2022-07-21 11:35:27.000000 alphaz-0.7.4.1/alphaz/documentations/docs/alpha_screens.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2222 2023-04-12 11:28:51.000000 alphaz-0.7.4.1/alphaz/documentations/docs/alpha_setup.md
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.226191 alphaz-0.7.4.1/alphaz/documentations/docs/api/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1527 2023-04-18 09:00:04.000000 alphaz-0.7.4.1/alphaz/documentations/docs/api/authorizations.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       72 2023-04-18 09:00:04.000000 alphaz-0.7.4.1/alphaz/documentations/docs/api/cache.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2932 2023-04-18 09:00:04.000000 alphaz-0.7.4.1/alphaz/documentations/docs/api/configuration.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       24 2023-04-18 09:00:04.000000 alphaz-0.7.4.1/alphaz/documentations/docs/api/issues.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      705 2023-04-18 09:00:04.000000 alphaz-0.7.4.1/alphaz/documentations/docs/api/main.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      559 2023-04-18 09:00:04.000000 alphaz-0.7.4.1/alphaz/documentations/docs/api/methods.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1728 2023-04-18 09:00:04.000000 alphaz-0.7.4.1/alphaz/documentations/docs/api/parameters.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1197 2023-04-18 09:00:04.000000 alphaz-0.7.4.1/alphaz/documentations/docs/api/routes.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      486 2023-04-18 09:00:04.000000 alphaz-0.7.4.1/alphaz/documentations/docs/api/sqlalchemy.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1129 2023-04-18 09:00:04.000000 alphaz-0.7.4.1/alphaz/documentations/docs/api_database.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2520 2023-01-06 09:14:28.000000 alphaz-0.7.4.1/alphaz/documentations/docs/configuration.md
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.226191 alphaz-0.7.4.1/alphaz/documentations/docs/database/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2187 2023-04-18 09:00:04.000000 alphaz-0.7.4.1/alphaz/documentations/docs/database/init.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      442 2023-04-18 09:00:04.000000 alphaz-0.7.4.1/alphaz/documentations/docs/database/instantiate.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      113 2023-04-18 09:00:04.000000 alphaz-0.7.4.1/alphaz/documentations/docs/database/main.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1806 2023-04-18 09:00:04.000000 alphaz-0.7.4.1/alphaz/documentations/docs/database/model.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      373 2023-04-18 09:00:04.000000 alphaz-0.7.4.1/alphaz/documentations/docs/database/relations.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1087 2023-04-18 09:00:04.000000 alphaz-0.7.4.1/alphaz/documentations/docs/database/schema.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      615 2023-04-18 09:00:04.000000 alphaz-0.7.4.1/alphaz/documentations/docs/database/update.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      357 2021-04-14 08:59:25.000000 alphaz-0.7.4.1/alphaz/documentations/docs/documentation.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3526 2023-04-12 11:28:51.000000 alphaz-0.7.4.1/alphaz/documentations/docs/index.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1090 2023-04-18 09:00:04.000000 alphaz-0.7.4.1/alphaz/documentations/mkdocs.yml
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.230191 alphaz-0.7.4.1/alphaz/documentations/site/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    13156 2023-04-19 12:08:15.000000 alphaz-0.7.4.1/alphaz/documentations/site/404.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.230191 alphaz-0.7.4.1/alphaz/documentations/site/alpha_admin/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    14222 2023-04-19 12:08:15.000000 alphaz-0.7.4.1/alphaz/documentations/site/alpha_admin/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.230191 alphaz-0.7.4.1/alphaz/documentations/site/alpha_core/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    22752 2023-04-19 12:08:15.000000 alphaz-0.7.4.1/alphaz/documentations/site/alpha_core/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.230191 alphaz-0.7.4.1/alphaz/documentations/site/alpha_screens/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    21873 2023-04-19 12:08:15.000000 alphaz-0.7.4.1/alphaz/documentations/site/alpha_screens/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.230191 alphaz-0.7.4.1/alphaz/documentations/site/alpha_setup/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    24071 2023-04-19 12:08:15.000000 alphaz-0.7.4.1/alphaz/documentations/site/alpha_setup/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.210191 alphaz-0.7.4.1/alphaz/documentations/site/api/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.230191 alphaz-0.7.4.1/alphaz/documentations/site/api/authorizations/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    17905 2023-04-19 12:08:15.000000 alphaz-0.7.4.1/alphaz/documentations/site/api/authorizations/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.230191 alphaz-0.7.4.1/alphaz/documentations/site/api/cache/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    14918 2023-04-19 12:08:15.000000 alphaz-0.7.4.1/alphaz/documentations/site/api/cache/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.230191 alphaz-0.7.4.1/alphaz/documentations/site/api/configuration/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    27646 2023-04-19 12:08:15.000000 alphaz-0.7.4.1/alphaz/documentations/site/api/configuration/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.230191 alphaz-0.7.4.1/alphaz/documentations/site/api/issues/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    16365 2023-04-19 12:08:15.000000 alphaz-0.7.4.1/alphaz/documentations/site/api/issues/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.230191 alphaz-0.7.4.1/alphaz/documentations/site/api/main/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    17987 2023-04-19 12:08:16.000000 alphaz-0.7.4.1/alphaz/documentations/site/api/main/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.230191 alphaz-0.7.4.1/alphaz/documentations/site/api/methods/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    17722 2023-04-19 12:08:16.000000 alphaz-0.7.4.1/alphaz/documentations/site/api/methods/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.230191 alphaz-0.7.4.1/alphaz/documentations/site/api/parameters/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    20075 2023-04-19 12:08:16.000000 alphaz-0.7.4.1/alphaz/documentations/site/api/parameters/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.230191 alphaz-0.7.4.1/alphaz/documentations/site/api/routes/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    19333 2023-04-19 12:08:16.000000 alphaz-0.7.4.1/alphaz/documentations/site/api/routes/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.230191 alphaz-0.7.4.1/alphaz/documentations/site/api/sqlalchemy/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    17109 2023-04-19 12:08:16.000000 alphaz-0.7.4.1/alphaz/documentations/site/api/sqlalchemy/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.230191 alphaz-0.7.4.1/alphaz/documentations/site/api_database/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    22959 2023-04-19 12:08:15.000000 alphaz-0.7.4.1/alphaz/documentations/site/api_database/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.210191 alphaz-0.7.4.1/alphaz/documentations/site/assets/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.230191 alphaz-0.7.4.1/alphaz/documentations/site/assets/images/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1870 2023-04-19 12:08:15.000000 alphaz-0.7.4.1/alphaz/documentations/site/assets/images/favicon.png
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.230191 alphaz-0.7.4.1/alphaz/documentations/site/assets/javascripts/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    79520 2023-04-19 12:08:15.000000 alphaz-0.7.4.1/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)   384391 2023-04-19 12:08:15.000000 alphaz-0.7.4.1/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js.map
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.234191 alphaz-0.7.4.1/alphaz/documentations/site/assets/javascripts/lunr/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.234191 alphaz-0.7.4.1/alphaz/documentations/site/assets/javascripts/lunr/min/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    17058 2023-04-19 12:08:15.000000 alphaz-0.7.4.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ar.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4654 2023-04-19 12:08:15.000000 alphaz-0.7.4.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.da.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6119 2023-04-19 12:08:15.000000 alphaz-0.7.4.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.de.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6208 2023-04-19 12:08:15.000000 alphaz-0.7.4.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.du.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    11499 2023-04-19 12:08:15.000000 alphaz-0.7.4.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.es.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     9342 2023-04-19 12:08:15.000000 alphaz-0.7.4.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fi.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    10669 2023-04-19 12:08:15.000000 alphaz-0.7.4.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fr.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     9437 2023-04-19 12:08:15.000000 alphaz-0.7.4.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.hu.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    11232 2023-04-19 12:08:15.000000 alphaz-0.7.4.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.it.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2313 2023-04-19 12:08:15.000000 alphaz-0.7.4.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ja.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       36 2023-04-19 12:08:15.000000 alphaz-0.7.4.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.jp.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      817 2023-04-19 12:08:15.000000 alphaz-0.7.4.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.multi.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6026 2023-04-19 12:08:15.000000 alphaz-0.7.4.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.nl.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4754 2023-04-19 12:08:15.000000 alphaz-0.7.4.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.no.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    10171 2023-04-19 12:08:15.000000 alphaz-0.7.4.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.pt.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    10958 2023-04-19 12:08:15.000000 alphaz-0.7.4.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ro.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    10331 2023-04-19 12:08:15.000000 alphaz-0.7.4.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ru.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3647 2023-04-19 12:08:15.000000 alphaz-0.7.4.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4523 2023-04-19 12:08:15.000000 alphaz-0.7.4.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.sv.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    15009 2023-04-19 12:08:15.000000 alphaz-0.7.4.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.tr.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      784 2023-04-19 12:08:15.000000 alphaz-0.7.4.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.vi.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    22878 2023-04-19 12:08:15.000000 alphaz-0.7.4.1/alphaz/documentations/site/assets/javascripts/lunr/tinyseg.js
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.238191 alphaz-0.7.4.1/alphaz/documentations/site/assets/javascripts/workers/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    34936 2023-04-19 12:08:15.000000 alphaz-0.7.4.1/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)   167496 2023-04-19 12:08:15.000000 alphaz-0.7.4.1/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js.map
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.238191 alphaz-0.7.4.1/alphaz/documentations/site/assets/stylesheets/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    87332 2023-04-19 12:08:15.000000 alphaz-0.7.4.1/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css
--rw-rw-r--   0 aurele    (1000) aurele    (1000)   319950 2023-04-19 12:08:15.000000 alphaz-0.7.4.1/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css.map
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    10915 2023-04-19 12:08:15.000000 alphaz-0.7.4.1/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    37512 2023-04-19 12:08:15.000000 alphaz-0.7.4.1/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css.map
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.238191 alphaz-0.7.4.1/alphaz/documentations/site/configuration/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    28465 2023-04-19 12:08:15.000000 alphaz-0.7.4.1/alphaz/documentations/site/configuration/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.210191 alphaz-0.7.4.1/alphaz/documentations/site/database/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.238191 alphaz-0.7.4.1/alphaz/documentations/site/database/init/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    23027 2023-04-19 12:08:16.000000 alphaz-0.7.4.1/alphaz/documentations/site/database/init/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.238191 alphaz-0.7.4.1/alphaz/documentations/site/database/instantiate/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    17445 2023-04-19 12:08:16.000000 alphaz-0.7.4.1/alphaz/documentations/site/database/instantiate/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.238191 alphaz-0.7.4.1/alphaz/documentations/site/database/main/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    14939 2023-04-19 12:08:16.000000 alphaz-0.7.4.1/alphaz/documentations/site/database/main/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.238191 alphaz-0.7.4.1/alphaz/documentations/site/database/model/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    24758 2023-04-19 12:08:16.000000 alphaz-0.7.4.1/alphaz/documentations/site/database/model/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.238191 alphaz-0.7.4.1/alphaz/documentations/site/database/relations/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    16511 2023-04-19 12:08:16.000000 alphaz-0.7.4.1/alphaz/documentations/site/database/relations/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.238191 alphaz-0.7.4.1/alphaz/documentations/site/database/schema/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    18704 2023-04-19 12:08:16.000000 alphaz-0.7.4.1/alphaz/documentations/site/database/schema/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.238191 alphaz-0.7.4.1/alphaz/documentations/site/database/update/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    20308 2023-04-19 12:08:16.000000 alphaz-0.7.4.1/alphaz/documentations/site/database/update/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.238191 alphaz-0.7.4.1/alphaz/documentations/site/documentation/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    17065 2023-04-19 12:08:15.000000 alphaz-0.7.4.1/alphaz/documentations/site/documentation/index.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    29467 2023-04-19 12:08:15.000000 alphaz-0.7.4.1/alphaz/documentations/site/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.238191 alphaz-0.7.4.1/alphaz/documentations/site/search/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    54137 2023-04-19 12:08:16.000000 alphaz-0.7.4.1/alphaz/documentations/site/search/search_index.json
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2809 2023-04-19 12:08:15.000000 alphaz-0.7.4.1/alphaz/documentations/site/sitemap.xml
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      208 2023-04-19 12:08:15.000000 alphaz-0.7.4.1/alphaz/documentations/site/sitemap.xml.gz
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       50 2022-04-19 08:43:27.000000 alphaz-0.7.4.1/alphaz/git.sh
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       45 2022-05-14 15:57:01.000000 alphaz-0.7.4.1/alphaz/help.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      905 2021-03-29 08:42:45.000000 alphaz-0.7.4.1/alphaz/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.242191 alphaz-0.7.4.1/alphaz/libs/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.4.1/alphaz/libs/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     5785 2023-04-13 20:34:53.000000 alphaz-0.7.4.1/alphaz/libs/api_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1901 2021-03-29 08:42:45.000000 alphaz-0.7.4.1/alphaz/libs/barcode_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    13999 2023-04-18 09:00:04.000000 alphaz-0.7.4.1/alphaz/libs/config_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2420 2023-03-29 19:04:59.000000 alphaz-0.7.4.1/alphaz/libs/converter_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     9073 2023-04-18 11:53:08.000000 alphaz-0.7.4.1/alphaz/libs/database_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4223 2023-02-06 12:52:51.000000 alphaz-0.7.4.1/alphaz/libs/date_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6324 2023-04-18 09:00:04.000000 alphaz-0.7.4.1/alphaz/libs/dict_lib.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.242191 alphaz-0.7.4.1/alphaz/libs/emulation/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1758 2023-02-02 21:07:35.000000 alphaz-0.7.4.1/alphaz/libs/emulation/vt102_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1642 2021-03-29 08:42:45.000000 alphaz-0.7.4.1/alphaz/libs/events.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3351 2022-01-17 10:25:20.000000 alphaz-0.7.4.1/alphaz/libs/files_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1184 2023-04-18 09:00:04.000000 alphaz-0.7.4.1/alphaz/libs/flask_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       49 2021-03-29 08:42:45.000000 alphaz-0.7.4.1/alphaz/libs/ftp_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1093 2022-07-21 11:35:27.000000 alphaz-0.7.4.1/alphaz/libs/img_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6212 2023-04-11 14:13:25.000000 alphaz-0.7.4.1/alphaz/libs/io_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3248 2023-03-16 19:44:05.000000 alphaz-0.7.4.1/alphaz/libs/json_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1143 2022-07-21 11:35:27.000000 alphaz-0.7.4.1/alphaz/libs/logs_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    12786 2023-03-17 15:11:43.000000 alphaz-0.7.4.1/alphaz/libs/mail_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      508 2021-03-29 08:42:45.000000 alphaz-0.7.4.1/alphaz/libs/nav_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      614 2022-09-07 06:57:10.000000 alphaz-0.7.4.1/alphaz/libs/notifications_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1348 2021-03-29 08:42:45.000000 alphaz-0.7.4.1/alphaz/libs/number_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      177 2021-03-29 08:42:45.000000 alphaz-0.7.4.1/alphaz/libs/os_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2782 2021-03-29 08:42:45.000000 alphaz-0.7.4.1/alphaz/libs/process_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    11058 2023-03-16 15:41:50.000000 alphaz-0.7.4.1/alphaz/libs/py_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      657 2021-03-29 08:42:45.000000 alphaz-0.7.4.1/alphaz/libs/scp_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     8082 2022-01-17 10:25:20.000000 alphaz-0.7.4.1/alphaz/libs/search_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6397 2023-04-13 20:34:53.000000 alphaz-0.7.4.1/alphaz/libs/secure_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3018 2023-04-03 15:21:20.000000 alphaz-0.7.4.1/alphaz/libs/soap_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      139 2021-03-29 08:42:45.000000 alphaz-0.7.4.1/alphaz/libs/sql_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    18289 2023-03-16 15:41:50.000000 alphaz-0.7.4.1/alphaz/libs/ssh_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    11021 2023-04-08 08:30:59.000000 alphaz-0.7.4.1/alphaz/libs/string_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     5139 2023-02-23 09:08:35.000000 alphaz-0.7.4.1/alphaz/libs/test_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      703 2023-03-16 15:41:50.000000 alphaz-0.7.4.1/alphaz/libs/time_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4200 2022-04-12 11:53:03.000000 alphaz-0.7.4.1/alphaz/libs/transactions_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     5041 2022-12-01 15:14:08.000000 alphaz-0.7.4.1/alphaz/libs/user_lib.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.242191 alphaz-0.7.4.1/alphaz/libs/user_management/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2022-04-27 13:24:50.000000 alphaz-0.7.4.1/alphaz/libs/user_management/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1354 2022-05-09 13:31:06.000000 alphaz-0.7.4.1/alphaz/libs/user_management/application_management_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1621 2022-10-07 10:05:05.000000 alphaz-0.7.4.1/alphaz/libs/user_management/permission_management_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3367 2022-10-07 10:05:05.000000 alphaz-0.7.4.1/alphaz/libs/user_management/role_management_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2336 2023-01-25 21:39:07.000000 alphaz-0.7.4.1/alphaz/libs/user_management/user_management_lib.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.246191 alphaz-0.7.4.1/alphaz/mails/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.250191 alphaz-0.7.4.1/alphaz/mails/Images/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)   948952 2021-03-29 08:42:45.000000 alphaz-0.7.4.1/alphaz/mails/Images/Background.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1835 2021-03-29 08:42:45.000000 alphaz-0.7.4.1/alphaz/mails/Images/Facebook_logo.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2484 2021-03-29 08:42:45.000000 alphaz-0.7.4.1/alphaz/mails/Images/Twitter_logo.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3522 2021-03-29 08:42:45.000000 alphaz-0.7.4.1/alphaz/mails/Images/Web_logo.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.4.1/alphaz/mails/Images/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)   966605 2021-03-29 08:42:45.000000 alphaz-0.7.4.1/alphaz/mails/Mail.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     5097 2022-04-13 09:59:51.000000 alphaz-0.7.4.1/alphaz/mails/Webmail.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.4.1/alphaz/mails/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    22029 2023-03-17 05:42:16.000000 alphaz-0.7.4.1/alphaz/mails/debug.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    23078 2023-03-16 20:48:51.000000 alphaz-0.7.4.1/alphaz/mails/mail.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2331 2021-03-29 08:42:45.000000 alphaz-0.7.4.1/alphaz/mails/password_reset.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    24598 2022-04-13 09:59:51.000000 alphaz-0.7.4.1/alphaz/mails/stay_in_touch.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       40 2021-03-29 08:42:45.000000 alphaz-0.7.4.1/alphaz/mails/template.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.250191 alphaz-0.7.4.1/alphaz/models/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      145 2023-02-06 09:05:20.000000 alphaz-0.7.4.1/alphaz/models/__init__.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.250191 alphaz-0.7.4.1/alphaz/models/api/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      185 2022-04-12 11:53:03.000000 alphaz-0.7.4.1/alphaz/models/api/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      884 2023-04-12 16:11:09.000000 alphaz-0.7.4.1/alphaz/models/api/_answer.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2179 2021-09-13 12:55:49.000000 alphaz-0.7.4.1/alphaz/models/api/_colorations.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      133 2021-09-06 13:56:36.000000 alphaz-0.7.4.1/alphaz/models/api/_methods.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    14253 2023-02-23 09:08:35.000000 alphaz-0.7.4.1/alphaz/models/api/_parameter.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2240 2022-08-26 12:58:11.000000 alphaz-0.7.4.1/alphaz/models/api/_requests.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    18649 2023-04-13 20:07:38.000000 alphaz-0.7.4.1/alphaz/models/api/_route.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    21563 2023-03-23 07:52:23.000000 alphaz-0.7.4.1/alphaz/models/api/_structures.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      651 2022-02-01 21:43:05.000000 alphaz-0.7.4.1/alphaz/models/api/_utils.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      388 2022-07-22 14:00:51.000000 alphaz-0.7.4.1/alphaz/models/base.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.250191 alphaz-0.7.4.1/alphaz/models/config/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       32 2021-03-29 08:42:45.000000 alphaz-0.7.4.1/alphaz/models/config/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    25438 2023-01-06 09:14:28.000000 alphaz-0.7.4.1/alphaz/models/config/_config.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    12129 2021-08-12 12:49:09.000000 alphaz-0.7.4.1/alphaz/models/config/_utils.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.254191 alphaz-0.7.4.1/alphaz/models/database/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       53 2022-01-13 15:32:15.000000 alphaz-0.7.4.1/alphaz/models/database/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     5495 2023-03-17 15:16:42.000000 alphaz-0.7.4.1/alphaz/models/database/main_definitions.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    10028 2023-03-19 14:55:26.000000 alphaz-0.7.4.1/alphaz/models/database/models.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      609 2022-04-28 08:55:29.000000 alphaz-0.7.4.1/alphaz/models/database/operators.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1164 2023-01-25 21:39:07.000000 alphaz-0.7.4.1/alphaz/models/database/requests.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1087 2021-03-29 08:42:45.000000 alphaz-0.7.4.1/alphaz/models/database/row.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    55701 2023-04-19 12:08:12.000000 alphaz-0.7.4.1/alphaz/models/database/structure.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1826 2023-02-23 09:08:35.000000 alphaz-0.7.4.1/alphaz/models/database/tests.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4418 2023-03-16 19:51:01.000000 alphaz-0.7.4.1/alphaz/models/database/users_definitions.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     9285 2022-08-02 08:51:28.000000 alphaz-0.7.4.1/alphaz/models/database/utils.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1061 2022-04-12 11:53:03.000000 alphaz-0.7.4.1/alphaz/models/database/views.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1241 2021-03-29 08:42:45.000000 alphaz-0.7.4.1/alphaz/models/excel.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     5126 2022-01-17 10:25:20.000000 alphaz-0.7.4.1/alphaz/models/ftp.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      150 2022-07-19 09:10:48.000000 alphaz-0.7.4.1/alphaz/models/img.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.254191 alphaz-0.7.4.1/alphaz/models/json/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       41 2021-03-29 08:42:45.000000 alphaz-0.7.4.1/alphaz/models/json/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2609 2023-01-06 09:14:28.000000 alphaz-0.7.4.1/alphaz/models/json/_converters.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.254191 alphaz-0.7.4.1/alphaz/models/logger/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       68 2022-01-19 15:41:22.000000 alphaz-0.7.4.1/alphaz/models/logger/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1319 2023-01-06 09:14:28.000000 alphaz-0.7.4.1/alphaz/models/logger/_colorations.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    14091 2023-04-05 11:16:09.000000 alphaz-0.7.4.1/alphaz/models/logger/_logger.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      757 2021-03-29 08:42:45.000000 alphaz-0.7.4.1/alphaz/models/logger/_utils.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.254191 alphaz-0.7.4.1/alphaz/models/logs/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1280 2021-11-12 08:53:17.000000 alphaz-0.7.4.1/alphaz/models/logs/main.log
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      160 2021-11-07 15:22:58.000000 alphaz-0.7.4.1/alphaz/models/logs/main.log.2021-11-07
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.258191 alphaz-0.7.4.1/alphaz/models/main/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      385 2023-02-06 09:05:20.000000 alphaz-0.7.4.1/alphaz/models/main/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    27277 2023-04-18 09:00:04.000000 alphaz-0.7.4.1/alphaz/models/main/_base.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.258191 alphaz-0.7.4.1/alphaz/models/main/_core/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.4.1/alphaz/models/main/_core/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    14630 2023-04-08 19:36:08.000000 alphaz-0.7.4.1/alphaz/models/main/_core/_core.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       13 2021-03-29 08:42:45.000000 alphaz-0.7.4.1/alphaz/models/main/_core/_utils.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      339 2023-02-06 09:05:20.000000 alphaz-0.7.4.1/alphaz/models/main/_enum.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1862 2023-02-17 08:49:35.000000 alphaz-0.7.4.1/alphaz/models/main/_exception.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      501 2021-03-29 08:42:45.000000 alphaz-0.7.4.1/alphaz/models/main/_file.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      477 2021-03-29 08:42:45.000000 alphaz-0.7.4.1/alphaz/models/main/_process.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1305 2021-03-29 08:42:45.000000 alphaz-0.7.4.1/alphaz/models/main/_request.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      925 2021-03-29 08:42:45.000000 alphaz-0.7.4.1/alphaz/models/main/_singleton.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2258 2023-03-16 15:41:50.000000 alphaz-0.7.4.1/alphaz/models/request.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.258191 alphaz-0.7.4.1/alphaz/models/tests/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      139 2023-03-16 15:41:50.000000 alphaz-0.7.4.1/alphaz/models/tests/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6780 2023-02-23 09:08:35.000000 alphaz-0.7.4.1/alphaz/models/tests/_category.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3095 2023-02-23 09:08:35.000000 alphaz-0.7.4.1/alphaz/models/tests/_group.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      109 2021-09-10 07:16:32.000000 alphaz-0.7.4.1/alphaz/models/tests/_levels.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4174 2023-02-23 09:08:35.000000 alphaz-0.7.4.1/alphaz/models/tests/_method.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4571 2023-04-11 14:13:25.000000 alphaz-0.7.4.1/alphaz/models/tests/_save.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    13495 2023-04-18 11:53:08.000000 alphaz-0.7.4.1/alphaz/models/tests/_test.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     7359 2023-04-18 09:00:04.000000 alphaz-0.7.4.1/alphaz/models/tests/_wrappers.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2802 2022-12-01 15:14:08.000000 alphaz-0.7.4.1/alphaz/models/user.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2367 2021-03-29 08:42:45.000000 alphaz-0.7.4.1/alphaz/models/watcher.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.258191 alphaz-0.7.4.1/alphaz/pocs/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      685 2021-03-29 08:42:45.000000 alphaz-0.7.4.1/alphaz/pocs/main.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       72 2021-03-29 08:42:45.000000 alphaz-0.7.4.1/alphaz/reload_gitignore.bat
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       67 2022-04-12 12:30:24.000000 alphaz-0.7.4.1/alphaz/req.sh
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      460 2023-04-11 14:13:25.000000 alphaz-0.7.4.1/alphaz/requirements.txt
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1345 2022-04-19 08:43:27.000000 alphaz-0.7.4.1/alphaz/run.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.258191 alphaz-0.7.4.1/alphaz/src/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.4.1/alphaz/src/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    23747 2021-03-29 08:42:45.000000 alphaz-0.7.4.1/alphaz/src/alpha.png
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.262191 alphaz-0.7.4.1/alphaz/src/configs/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      135 2022-04-19 08:43:27.000000 alphaz-0.7.4.1/alphaz/src/configs/config.json
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      674 2023-01-25 21:39:07.000000 alphaz-0.7.4.1/alphaz/src/configs/loggers.json
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      490 2022-01-13 15:32:15.000000 alphaz-0.7.4.1/alphaz/src/configs/loggers_colors.json
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.262191 alphaz-0.7.4.1/alphaz/src/database/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.4.1/alphaz/src/database/__init__.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.262191 alphaz-0.7.4.1/alphaz/stitch/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1769 2021-03-29 08:42:45.000000 alphaz-0.7.4.1/alphaz/stitch/Core.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       26 2021-03-29 08:42:45.000000 alphaz-0.7.4.1/alphaz/stitch/__init__.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.262191 alphaz-0.7.4.1/alphaz/stitch/imports/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       78 2021-03-29 08:42:45.000000 alphaz-0.7.4.1/alphaz/stitch/imports/__init__.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.262191 alphaz-0.7.4.1/alphaz/stitch/models/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.4.1/alphaz/stitch/models/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      391 2021-03-29 08:42:45.000000 alphaz-0.7.4.1/alphaz/stitch/models/element.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       46 2021-03-29 08:42:45.000000 alphaz-0.7.4.1/alphaz/stitch/run.bat
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1857 2021-03-29 08:42:45.000000 alphaz-0.7.4.1/alphaz/stitch/stitch.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.270191 alphaz-0.7.4.1/alphaz/stitch/web-drivers/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)  8738816 2021-03-29 08:42:45.000000 alphaz-0.7.4.1/alphaz/stitch/web-drivers/chromedriver.exe
--rw-rw-r--   0 aurele    (1000) aurele    (1000)  7008696 2022-04-19 08:43:27.000000 alphaz-0.7.4.1/alphaz/stitch/web-drivers/geckodriver
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.214191 alphaz-0.7.4.1/alphaz/stitch/websites/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.278191 alphaz-0.7.4.1/alphaz/stitch/websites/Test/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      204 2021-03-29 08:42:45.000000 alphaz-0.7.4.1/alphaz/stitch/websites/Test/init.json
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.278191 alphaz-0.7.4.1/alphaz/stitch/websites/stiki/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      363 2022-04-13 09:59:51.000000 alphaz-0.7.4.1/alphaz/stitch/websites/stiki/init.json
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.278191 alphaz-0.7.4.1/alphaz/templates/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.4.1/alphaz/templates/__init__.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.278191 alphaz-0.7.4.1/alphaz/templates/assets/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.4.1/alphaz/templates/assets/__init__.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.278191 alphaz-0.7.4.1/alphaz/templates/assets/css/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    95923 2021-09-10 07:16:32.000000 alphaz-0.7.4.1/alphaz/templates/assets/css/home.css
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2356 2021-08-06 18:55:11.000000 alphaz-0.7.4.1/alphaz/templates/assets/css/logs.css
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.278191 alphaz-0.7.4.1/alphaz/templates/assets/images/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.278191 alphaz-0.7.4.1/alphaz/templates/assets/images/icons/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      276 2021-08-06 18:55:11.000000 alphaz-0.7.4.1/alphaz/templates/assets/images/icons/admin.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1444 2021-08-06 18:55:11.000000 alphaz-0.7.4.1/alphaz/templates/assets/images/icons/alpha.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      142 2021-08-06 18:55:11.000000 alphaz-0.7.4.1/alphaz/templates/assets/images/icons/save.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     8889 2021-08-06 18:55:11.000000 alphaz-0.7.4.1/alphaz/templates/assets/images/icons/start-icon.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      136 2021-08-06 18:55:11.000000 alphaz-0.7.4.1/alphaz/templates/assets/images/icons/user.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    23747 2021-08-06 18:55:11.000000 alphaz-0.7.4.1/alphaz/templates/assets/images/icons/wsalpha.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1165 2021-08-06 18:55:11.000000 alphaz-0.7.4.1/alphaz/templates/assets/images/loading.gif
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.278191 alphaz-0.7.4.1/alphaz/templates/assets/js/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.278191 alphaz-0.7.4.1/alphaz/templates/assets/js/libs/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    21922 2021-08-06 18:55:11.000000 alphaz-0.7.4.1/alphaz/templates/assets/js/libs/ansi_up.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    89475 2021-08-06 18:55:11.000000 alphaz-0.7.4.1/alphaz/templates/assets/js/libs/jquery.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     7339 2022-10-26 14:51:00.000000 alphaz-0.7.4.1/alphaz/templates/assets/js/logs.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       37 2021-03-29 08:42:45.000000 alphaz-0.7.4.1/alphaz/templates/hello.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    19017 2022-01-17 10:25:20.000000 alphaz-0.7.4.1/alphaz/templates/home.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3779 2021-08-06 18:55:11.000000 alphaz-0.7.4.1/alphaz/templates/logs.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1153 2023-01-25 21:39:07.000000 alphaz-0.7.4.1/alphaz/test.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.278191 alphaz-0.7.4.1/alphaz/tests/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      119 2021-03-29 08:42:45.000000 alphaz-0.7.4.1/alphaz/tests/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    13857 2023-03-28 08:47:21.000000 alphaz-0.7.4.1/alphaz/tests/api.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      541 2023-03-16 15:41:50.000000 alphaz-0.7.4.1/alphaz/tests/basic_test.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1526 2021-11-30 22:30:57.000000 alphaz-0.7.4.1/alphaz/tests/configurations.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    22695 2023-03-16 19:44:05.000000 alphaz-0.7.4.1/alphaz/tests/database.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      397 2021-03-29 08:42:45.000000 alphaz-0.7.4.1/alphaz/tests/processes.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      555 2021-03-29 08:42:45.000000 alphaz-0.7.4.1/alphaz/tests/utils.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.278191 alphaz-0.7.4.1/alphaz/utils/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       81 2021-03-29 08:42:45.000000 alphaz-0.7.4.1/alphaz/utils/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    11552 2023-02-16 14:12:47.000000 alphaz-0.7.4.1/alphaz/utils/api.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      338 2022-04-19 08:43:27.000000 alphaz-0.7.4.1/alphaz/utils/clean.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      813 2022-05-02 08:25:25.000000 alphaz-0.7.4.1/alphaz/utils/configuration.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     5438 2022-02-24 13:20:43.000000 alphaz-0.7.4.1/alphaz/utils/database_to_dataclass.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2207 2023-03-16 15:41:50.000000 alphaz-0.7.4.1/alphaz/utils/decorators.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3112 2021-03-29 08:42:45.000000 alphaz-0.7.4.1/alphaz/utils/ensure.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4405 2022-01-13 15:32:15.000000 alphaz-0.7.4.1/alphaz/utils/mep.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     7639 2021-04-21 22:36:11.000000 alphaz-0.7.4.1/alphaz/utils/screens.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    22569 2022-01-17 10:25:20.000000 alphaz-0.7.4.1/alphaz/utils/selectionMenu.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      764 2022-01-17 10:25:20.000000 alphaz-0.7.4.1/alphaz/utils/tasks.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1535 2023-02-23 09:08:35.000000 alphaz-0.7.4.1/alphaz/utils/tests.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      628 2023-03-16 15:41:50.000000 alphaz-0.7.4.1/alphaz/utils/time.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3766 2022-01-17 10:25:20.000000 alphaz-0.7.4.1/alphaz/utils/transactions.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-19 12:08:17.222191 alphaz-0.7.4.1/alphaz.egg-info/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      589 2023-04-19 12:08:16.000000 alphaz-0.7.4.1/alphaz.egg-info/PKG-INFO
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    11189 2023-04-19 12:08:17.000000 alphaz-0.7.4.1/alphaz.egg-info/SOURCES.txt
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        1 2023-04-19 12:08:16.000000 alphaz-0.7.4.1/alphaz.egg-info/dependency_links.txt
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      458 2023-04-19 12:08:16.000000 alphaz-0.7.4.1/alphaz.egg-info/requires.txt
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        7 2023-04-19 12:08:16.000000 alphaz-0.7.4.1/alphaz.egg-info/top_level.txt
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       79 2023-04-19 12:08:17.282191 alphaz-0.7.4.1/setup.cfg
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3094 2023-04-19 12:08:06.000000 alphaz-0.7.4.1/setup.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.205110 alphaz-0.7.5/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    11144 2023-04-21 07:48:00.000000 alphaz-0.7.5/MANIFEST.in
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      585 2023-04-21 07:48:01.205110 alphaz-0.7.5/PKG-INFO
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1348 2021-07-12 18:07:51.000000 alphaz-0.7.5/README.md
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.125110 alphaz-0.7.5/alphaz/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        9 2023-04-18 09:00:04.000000 alphaz-0.7.5/alphaz/README.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      333 2023-04-13 12:43:58.000000 alphaz-0.7.5/alphaz/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      104 2021-03-29 08:42:45.000000 alphaz-0.7.5/alphaz/alphaz.bat
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       70 2021-03-29 08:42:45.000000 alphaz-0.7.5/alphaz/alphaz.code-workspace
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      208 2022-04-19 08:43:27.000000 alphaz-0.7.5/alphaz/alphaz.sh
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       48 2021-03-29 08:42:45.000000 alphaz-0.7.5/alphaz/api.bat
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      713 2023-04-18 09:00:04.000000 alphaz-0.7.5/alphaz/api.json
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      770 2022-04-13 09:59:51.000000 alphaz-0.7.5/alphaz/api.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.129110 alphaz-0.7.5/alphaz/apis/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.5/alphaz/apis/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2022-07-21 11:35:27.000000 alphaz-0.7.5/alphaz/apis/log.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2721 2023-03-17 07:06:42.000000 alphaz-0.7.5/alphaz/apis/mails.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.129110 alphaz-0.7.5/alphaz/apis/routes/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.5/alphaz/apis/routes/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1577 2023-02-23 09:08:35.000000 alphaz-0.7.5/alphaz/apis/routes/admin.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1137 2021-03-29 08:42:45.000000 alphaz-0.7.5/alphaz/apis/routes/api.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3062 2023-02-23 09:08:35.000000 alphaz-0.7.5/alphaz/apis/routes/basic_tests.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3094 2023-04-18 09:00:04.000000 alphaz-0.7.5/alphaz/apis/routes/database.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      413 2022-04-12 11:53:03.000000 alphaz-0.7.5/alphaz/apis/routes/git.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     7225 2023-02-01 13:59:24.000000 alphaz-0.7.5/alphaz/apis/routes/logs.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1810 2022-04-12 11:53:03.000000 alphaz-0.7.5/alphaz/apis/routes/mails.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6390 2023-04-21 07:47:57.000000 alphaz-0.7.5/alphaz/apis/routes/main.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1330 2023-02-23 09:08:35.000000 alphaz-0.7.5/alphaz/apis/routes/tests.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.129110 alphaz-0.7.5/alphaz/apis/routes/user_management/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      114 2022-04-27 13:24:50.000000 alphaz-0.7.5/alphaz/apis/routes/user_management/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2475 2022-05-09 13:31:06.000000 alphaz-0.7.5/alphaz/apis/routes/user_management/application_management.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2228 2022-05-09 13:31:06.000000 alphaz-0.7.5/alphaz/apis/routes/user_management/permission_management.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4058 2022-08-31 08:56:44.000000 alphaz-0.7.5/alphaz/apis/routes/user_management/role_management.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1291 2022-08-31 08:56:44.000000 alphaz-0.7.5/alphaz/apis/routes/user_management/user_management.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3324 2023-04-21 07:47:57.000000 alphaz-0.7.5/alphaz/apis/routes/users.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      584 2023-02-23 09:08:35.000000 alphaz-0.7.5/alphaz/apis/tests.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.129110 alphaz-0.7.5/alphaz/apis/users/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2022-07-21 11:35:27.000000 alphaz-0.7.5/alphaz/apis/users/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2718 2023-01-25 21:39:07.000000 alphaz-0.7.5/alphaz/apis/users/ldap.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    11543 2023-03-28 08:47:21.000000 alphaz-0.7.5/alphaz/apis/users/users.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.129110 alphaz-0.7.5/alphaz/config/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.5/alphaz/config/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      795 2021-03-29 08:42:45.000000 alphaz-0.7.5/alphaz/config/config.css
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    12602 2021-03-29 08:42:45.000000 alphaz-0.7.5/alphaz/config/config.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      707 2022-08-11 06:44:17.000000 alphaz-0.7.5/alphaz/config/main_configuration.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      823 2021-03-29 08:42:45.000000 alphaz-0.7.5/alphaz/config/page.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1700 2021-03-29 08:42:45.000000 alphaz-0.7.5/alphaz/config/source.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1564 2021-03-29 08:42:45.000000 alphaz-0.7.5/alphaz/config.json
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      238 2023-01-06 09:14:28.000000 alphaz-0.7.5/alphaz/core.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.133110 alphaz-0.7.5/alphaz/documentations/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.133110 alphaz-0.7.5/alphaz/documentations/docs/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2022-07-21 11:35:27.000000 alphaz-0.7.5/alphaz/documentations/docs/alpha_admin.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1408 2023-04-12 11:28:51.000000 alphaz-0.7.5/alphaz/documentations/docs/alpha_core.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2595 2022-07-21 11:35:27.000000 alphaz-0.7.5/alphaz/documentations/docs/alpha_screens.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2222 2023-04-12 11:28:51.000000 alphaz-0.7.5/alphaz/documentations/docs/alpha_setup.md
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.133110 alphaz-0.7.5/alphaz/documentations/docs/api/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1527 2023-04-18 09:00:04.000000 alphaz-0.7.5/alphaz/documentations/docs/api/authorizations.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       72 2023-04-18 09:00:04.000000 alphaz-0.7.5/alphaz/documentations/docs/api/cache.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2932 2023-04-18 09:00:04.000000 alphaz-0.7.5/alphaz/documentations/docs/api/configuration.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       24 2023-04-18 09:00:04.000000 alphaz-0.7.5/alphaz/documentations/docs/api/issues.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      705 2023-04-18 09:00:04.000000 alphaz-0.7.5/alphaz/documentations/docs/api/main.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      559 2023-04-18 09:00:04.000000 alphaz-0.7.5/alphaz/documentations/docs/api/methods.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1728 2023-04-18 09:00:04.000000 alphaz-0.7.5/alphaz/documentations/docs/api/parameters.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1197 2023-04-18 09:00:04.000000 alphaz-0.7.5/alphaz/documentations/docs/api/routes.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      486 2023-04-18 09:00:04.000000 alphaz-0.7.5/alphaz/documentations/docs/api/sqlalchemy.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1129 2023-04-18 09:00:04.000000 alphaz-0.7.5/alphaz/documentations/docs/api_database.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2520 2023-01-06 09:14:28.000000 alphaz-0.7.5/alphaz/documentations/docs/configuration.md
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.133110 alphaz-0.7.5/alphaz/documentations/docs/database/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2187 2023-04-18 09:00:04.000000 alphaz-0.7.5/alphaz/documentations/docs/database/init.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      442 2023-04-18 09:00:04.000000 alphaz-0.7.5/alphaz/documentations/docs/database/instantiate.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      113 2023-04-18 09:00:04.000000 alphaz-0.7.5/alphaz/documentations/docs/database/main.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1806 2023-04-18 09:00:04.000000 alphaz-0.7.5/alphaz/documentations/docs/database/model.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      373 2023-04-18 09:00:04.000000 alphaz-0.7.5/alphaz/documentations/docs/database/relations.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1087 2023-04-18 09:00:04.000000 alphaz-0.7.5/alphaz/documentations/docs/database/schema.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      615 2023-04-18 09:00:04.000000 alphaz-0.7.5/alphaz/documentations/docs/database/update.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      357 2021-04-14 08:59:25.000000 alphaz-0.7.5/alphaz/documentations/docs/documentation.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3526 2023-04-12 11:28:51.000000 alphaz-0.7.5/alphaz/documentations/docs/index.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1090 2023-04-18 09:00:04.000000 alphaz-0.7.5/alphaz/documentations/mkdocs.yml
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.137110 alphaz-0.7.5/alphaz/documentations/site/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    13156 2023-04-21 07:47:59.000000 alphaz-0.7.5/alphaz/documentations/site/404.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.137110 alphaz-0.7.5/alphaz/documentations/site/alpha_admin/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    14222 2023-04-21 07:48:00.000000 alphaz-0.7.5/alphaz/documentations/site/alpha_admin/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.137110 alphaz-0.7.5/alphaz/documentations/site/alpha_core/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    22752 2023-04-21 07:48:00.000000 alphaz-0.7.5/alphaz/documentations/site/alpha_core/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.137110 alphaz-0.7.5/alphaz/documentations/site/alpha_screens/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    21873 2023-04-21 07:48:00.000000 alphaz-0.7.5/alphaz/documentations/site/alpha_screens/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.137110 alphaz-0.7.5/alphaz/documentations/site/alpha_setup/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    24071 2023-04-21 07:48:00.000000 alphaz-0.7.5/alphaz/documentations/site/alpha_setup/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.117110 alphaz-0.7.5/alphaz/documentations/site/api/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.137110 alphaz-0.7.5/alphaz/documentations/site/api/authorizations/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    17905 2023-04-21 07:48:00.000000 alphaz-0.7.5/alphaz/documentations/site/api/authorizations/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.137110 alphaz-0.7.5/alphaz/documentations/site/api/cache/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    14918 2023-04-21 07:48:00.000000 alphaz-0.7.5/alphaz/documentations/site/api/cache/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.137110 alphaz-0.7.5/alphaz/documentations/site/api/configuration/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    27646 2023-04-21 07:48:00.000000 alphaz-0.7.5/alphaz/documentations/site/api/configuration/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.137110 alphaz-0.7.5/alphaz/documentations/site/api/issues/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    16365 2023-04-21 07:48:00.000000 alphaz-0.7.5/alphaz/documentations/site/api/issues/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.137110 alphaz-0.7.5/alphaz/documentations/site/api/main/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    17987 2023-04-21 07:48:00.000000 alphaz-0.7.5/alphaz/documentations/site/api/main/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.137110 alphaz-0.7.5/alphaz/documentations/site/api/methods/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    17722 2023-04-21 07:48:00.000000 alphaz-0.7.5/alphaz/documentations/site/api/methods/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.137110 alphaz-0.7.5/alphaz/documentations/site/api/parameters/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    20075 2023-04-21 07:48:00.000000 alphaz-0.7.5/alphaz/documentations/site/api/parameters/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.137110 alphaz-0.7.5/alphaz/documentations/site/api/routes/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    19333 2023-04-21 07:48:00.000000 alphaz-0.7.5/alphaz/documentations/site/api/routes/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.137110 alphaz-0.7.5/alphaz/documentations/site/api/sqlalchemy/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    17109 2023-04-21 07:48:00.000000 alphaz-0.7.5/alphaz/documentations/site/api/sqlalchemy/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.137110 alphaz-0.7.5/alphaz/documentations/site/api_database/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    22959 2023-04-21 07:48:00.000000 alphaz-0.7.5/alphaz/documentations/site/api_database/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.121110 alphaz-0.7.5/alphaz/documentations/site/assets/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.137110 alphaz-0.7.5/alphaz/documentations/site/assets/images/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1870 2023-04-21 07:47:59.000000 alphaz-0.7.5/alphaz/documentations/site/assets/images/favicon.png
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.137110 alphaz-0.7.5/alphaz/documentations/site/assets/javascripts/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    79520 2023-04-21 07:47:59.000000 alphaz-0.7.5/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)   384391 2023-04-21 07:47:59.000000 alphaz-0.7.5/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js.map
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.137110 alphaz-0.7.5/alphaz/documentations/site/assets/javascripts/lunr/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.141110 alphaz-0.7.5/alphaz/documentations/site/assets/javascripts/lunr/min/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    17058 2023-04-21 07:47:59.000000 alphaz-0.7.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ar.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4654 2023-04-21 07:47:59.000000 alphaz-0.7.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.da.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6119 2023-04-21 07:47:59.000000 alphaz-0.7.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.de.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6208 2023-04-21 07:47:59.000000 alphaz-0.7.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.du.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    11499 2023-04-21 07:47:59.000000 alphaz-0.7.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.es.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     9342 2023-04-21 07:47:59.000000 alphaz-0.7.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fi.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    10669 2023-04-21 07:47:59.000000 alphaz-0.7.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fr.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     9437 2023-04-21 07:47:59.000000 alphaz-0.7.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.hu.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    11232 2023-04-21 07:47:59.000000 alphaz-0.7.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.it.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2313 2023-04-21 07:47:59.000000 alphaz-0.7.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ja.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       36 2023-04-21 07:47:59.000000 alphaz-0.7.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.jp.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      817 2023-04-21 07:47:59.000000 alphaz-0.7.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.multi.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6026 2023-04-21 07:47:59.000000 alphaz-0.7.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.nl.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4754 2023-04-21 07:47:59.000000 alphaz-0.7.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.no.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    10171 2023-04-21 07:47:59.000000 alphaz-0.7.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.pt.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    10958 2023-04-21 07:47:59.000000 alphaz-0.7.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ro.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    10331 2023-04-21 07:47:59.000000 alphaz-0.7.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ru.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3647 2023-04-21 07:47:59.000000 alphaz-0.7.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4523 2023-04-21 07:47:59.000000 alphaz-0.7.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.sv.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    15009 2023-04-21 07:47:59.000000 alphaz-0.7.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.tr.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      784 2023-04-21 07:47:59.000000 alphaz-0.7.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.vi.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    22878 2023-04-21 07:47:59.000000 alphaz-0.7.5/alphaz/documentations/site/assets/javascripts/lunr/tinyseg.js
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.141110 alphaz-0.7.5/alphaz/documentations/site/assets/javascripts/workers/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    34936 2023-04-21 07:47:59.000000 alphaz-0.7.5/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)   167496 2023-04-21 07:47:59.000000 alphaz-0.7.5/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js.map
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.145110 alphaz-0.7.5/alphaz/documentations/site/assets/stylesheets/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    87332 2023-04-21 07:47:59.000000 alphaz-0.7.5/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)   319950 2023-04-21 07:47:59.000000 alphaz-0.7.5/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css.map
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    10915 2023-04-21 07:47:59.000000 alphaz-0.7.5/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    37512 2023-04-21 07:47:59.000000 alphaz-0.7.5/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css.map
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.145110 alphaz-0.7.5/alphaz/documentations/site/configuration/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    28465 2023-04-21 07:48:00.000000 alphaz-0.7.5/alphaz/documentations/site/configuration/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.121110 alphaz-0.7.5/alphaz/documentations/site/database/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.145110 alphaz-0.7.5/alphaz/documentations/site/database/init/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    23027 2023-04-21 07:48:00.000000 alphaz-0.7.5/alphaz/documentations/site/database/init/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.145110 alphaz-0.7.5/alphaz/documentations/site/database/instantiate/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    17445 2023-04-21 07:48:00.000000 alphaz-0.7.5/alphaz/documentations/site/database/instantiate/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.145110 alphaz-0.7.5/alphaz/documentations/site/database/main/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    14939 2023-04-21 07:48:00.000000 alphaz-0.7.5/alphaz/documentations/site/database/main/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.145110 alphaz-0.7.5/alphaz/documentations/site/database/model/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    24758 2023-04-21 07:48:00.000000 alphaz-0.7.5/alphaz/documentations/site/database/model/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.145110 alphaz-0.7.5/alphaz/documentations/site/database/relations/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    16511 2023-04-21 07:48:00.000000 alphaz-0.7.5/alphaz/documentations/site/database/relations/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.145110 alphaz-0.7.5/alphaz/documentations/site/database/schema/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    18704 2023-04-21 07:48:00.000000 alphaz-0.7.5/alphaz/documentations/site/database/schema/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.145110 alphaz-0.7.5/alphaz/documentations/site/database/update/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    20308 2023-04-21 07:48:00.000000 alphaz-0.7.5/alphaz/documentations/site/database/update/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.145110 alphaz-0.7.5/alphaz/documentations/site/documentation/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    17065 2023-04-21 07:48:00.000000 alphaz-0.7.5/alphaz/documentations/site/documentation/index.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    29467 2023-04-21 07:48:00.000000 alphaz-0.7.5/alphaz/documentations/site/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.145110 alphaz-0.7.5/alphaz/documentations/site/search/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    54137 2023-04-21 07:48:00.000000 alphaz-0.7.5/alphaz/documentations/site/search/search_index.json
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2809 2023-04-21 07:47:59.000000 alphaz-0.7.5/alphaz/documentations/site/sitemap.xml
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      208 2023-04-21 07:47:59.000000 alphaz-0.7.5/alphaz/documentations/site/sitemap.xml.gz
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       50 2022-04-19 08:43:27.000000 alphaz-0.7.5/alphaz/git.sh
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       45 2022-05-14 15:57:01.000000 alphaz-0.7.5/alphaz/help.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      905 2021-03-29 08:42:45.000000 alphaz-0.7.5/alphaz/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.149110 alphaz-0.7.5/alphaz/libs/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.5/alphaz/libs/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     5785 2023-04-13 20:34:53.000000 alphaz-0.7.5/alphaz/libs/api_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1901 2021-03-29 08:42:45.000000 alphaz-0.7.5/alphaz/libs/barcode_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    13999 2023-04-18 09:00:04.000000 alphaz-0.7.5/alphaz/libs/config_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2420 2023-03-29 19:04:59.000000 alphaz-0.7.5/alphaz/libs/converter_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6022 2023-04-21 07:47:57.000000 alphaz-0.7.5/alphaz/libs/database_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4223 2023-02-06 12:52:51.000000 alphaz-0.7.5/alphaz/libs/date_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6324 2023-04-18 09:00:04.000000 alphaz-0.7.5/alphaz/libs/dict_lib.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.149110 alphaz-0.7.5/alphaz/libs/emulation/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1758 2023-02-02 21:07:35.000000 alphaz-0.7.5/alphaz/libs/emulation/vt102_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1642 2021-03-29 08:42:45.000000 alphaz-0.7.5/alphaz/libs/events.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3351 2022-01-17 10:25:20.000000 alphaz-0.7.5/alphaz/libs/files_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1184 2023-04-18 09:00:04.000000 alphaz-0.7.5/alphaz/libs/flask_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       49 2021-03-29 08:42:45.000000 alphaz-0.7.5/alphaz/libs/ftp_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1093 2022-07-21 11:35:27.000000 alphaz-0.7.5/alphaz/libs/img_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6212 2023-04-11 14:13:25.000000 alphaz-0.7.5/alphaz/libs/io_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3248 2023-03-16 19:44:05.000000 alphaz-0.7.5/alphaz/libs/json_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1143 2022-07-21 11:35:27.000000 alphaz-0.7.5/alphaz/libs/logs_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    12786 2023-03-17 15:11:43.000000 alphaz-0.7.5/alphaz/libs/mail_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      508 2021-03-29 08:42:45.000000 alphaz-0.7.5/alphaz/libs/nav_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      614 2022-09-07 06:57:10.000000 alphaz-0.7.5/alphaz/libs/notifications_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1348 2021-03-29 08:42:45.000000 alphaz-0.7.5/alphaz/libs/number_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      177 2021-03-29 08:42:45.000000 alphaz-0.7.5/alphaz/libs/os_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2782 2021-03-29 08:42:45.000000 alphaz-0.7.5/alphaz/libs/process_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    11058 2023-03-16 15:41:50.000000 alphaz-0.7.5/alphaz/libs/py_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      886 2023-04-21 07:47:57.000000 alphaz-0.7.5/alphaz/libs/scp_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     8082 2022-01-17 10:25:20.000000 alphaz-0.7.5/alphaz/libs/search_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6397 2023-04-13 20:34:53.000000 alphaz-0.7.5/alphaz/libs/secure_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3018 2023-04-03 15:21:20.000000 alphaz-0.7.5/alphaz/libs/soap_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      139 2021-03-29 08:42:45.000000 alphaz-0.7.5/alphaz/libs/sql_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    18517 2023-04-21 07:47:57.000000 alphaz-0.7.5/alphaz/libs/ssh_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     9938 2023-04-21 07:47:57.000000 alphaz-0.7.5/alphaz/libs/string_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     5139 2023-02-23 09:08:35.000000 alphaz-0.7.5/alphaz/libs/test_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      703 2023-03-16 15:41:50.000000 alphaz-0.7.5/alphaz/libs/time_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4200 2022-04-12 11:53:03.000000 alphaz-0.7.5/alphaz/libs/transactions_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     7549 2023-04-21 07:47:57.000000 alphaz-0.7.5/alphaz/libs/user_lib.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.149110 alphaz-0.7.5/alphaz/libs/user_management/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2022-04-27 13:24:50.000000 alphaz-0.7.5/alphaz/libs/user_management/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1354 2022-05-09 13:31:06.000000 alphaz-0.7.5/alphaz/libs/user_management/application_management_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1621 2022-10-07 10:05:05.000000 alphaz-0.7.5/alphaz/libs/user_management/permission_management_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3367 2022-10-07 10:05:05.000000 alphaz-0.7.5/alphaz/libs/user_management/role_management_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2336 2023-01-25 21:39:07.000000 alphaz-0.7.5/alphaz/libs/user_management/user_management_lib.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.149110 alphaz-0.7.5/alphaz/mails/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.177110 alphaz-0.7.5/alphaz/mails/Images/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)   948952 2021-03-29 08:42:45.000000 alphaz-0.7.5/alphaz/mails/Images/Background.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1835 2021-03-29 08:42:45.000000 alphaz-0.7.5/alphaz/mails/Images/Facebook_logo.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2484 2021-03-29 08:42:45.000000 alphaz-0.7.5/alphaz/mails/Images/Twitter_logo.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3522 2021-03-29 08:42:45.000000 alphaz-0.7.5/alphaz/mails/Images/Web_logo.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.5/alphaz/mails/Images/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)   966605 2021-03-29 08:42:45.000000 alphaz-0.7.5/alphaz/mails/Mail.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     5097 2022-04-13 09:59:51.000000 alphaz-0.7.5/alphaz/mails/Webmail.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.5/alphaz/mails/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    22029 2023-03-17 05:42:16.000000 alphaz-0.7.5/alphaz/mails/debug.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    23078 2023-03-16 20:48:51.000000 alphaz-0.7.5/alphaz/mails/mail.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2331 2021-03-29 08:42:45.000000 alphaz-0.7.5/alphaz/mails/password_reset.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    24598 2022-04-13 09:59:51.000000 alphaz-0.7.5/alphaz/mails/stay_in_touch.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       40 2021-03-29 08:42:45.000000 alphaz-0.7.5/alphaz/mails/template.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.177110 alphaz-0.7.5/alphaz/models/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      145 2023-02-06 09:05:20.000000 alphaz-0.7.5/alphaz/models/__init__.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.181110 alphaz-0.7.5/alphaz/models/api/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      185 2022-04-12 11:53:03.000000 alphaz-0.7.5/alphaz/models/api/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      884 2023-04-12 16:11:09.000000 alphaz-0.7.5/alphaz/models/api/_answer.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2179 2021-09-13 12:55:49.000000 alphaz-0.7.5/alphaz/models/api/_colorations.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      133 2021-09-06 13:56:36.000000 alphaz-0.7.5/alphaz/models/api/_methods.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    14253 2023-02-23 09:08:35.000000 alphaz-0.7.5/alphaz/models/api/_parameter.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2240 2022-08-26 12:58:11.000000 alphaz-0.7.5/alphaz/models/api/_requests.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    18649 2023-04-13 20:07:38.000000 alphaz-0.7.5/alphaz/models/api/_route.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    21593 2023-04-21 07:47:57.000000 alphaz-0.7.5/alphaz/models/api/_structures.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      651 2022-02-01 21:43:05.000000 alphaz-0.7.5/alphaz/models/api/_utils.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      388 2022-07-22 14:00:51.000000 alphaz-0.7.5/alphaz/models/base.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.181110 alphaz-0.7.5/alphaz/models/config/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       32 2021-03-29 08:42:45.000000 alphaz-0.7.5/alphaz/models/config/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    25438 2023-01-06 09:14:28.000000 alphaz-0.7.5/alphaz/models/config/_config.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    12129 2021-08-12 12:49:09.000000 alphaz-0.7.5/alphaz/models/config/_utils.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.181110 alphaz-0.7.5/alphaz/models/database/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       53 2022-01-13 15:32:15.000000 alphaz-0.7.5/alphaz/models/database/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     5495 2023-03-17 15:16:42.000000 alphaz-0.7.5/alphaz/models/database/main_definitions.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    10028 2023-03-19 14:55:26.000000 alphaz-0.7.5/alphaz/models/database/models.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      609 2022-04-28 08:55:29.000000 alphaz-0.7.5/alphaz/models/database/operators.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1164 2023-01-25 21:39:07.000000 alphaz-0.7.5/alphaz/models/database/requests.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1087 2021-03-29 08:42:45.000000 alphaz-0.7.5/alphaz/models/database/row.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    56385 2023-04-21 07:47:57.000000 alphaz-0.7.5/alphaz/models/database/structure.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1826 2023-02-23 09:08:35.000000 alphaz-0.7.5/alphaz/models/database/tests.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4553 2023-04-21 07:47:57.000000 alphaz-0.7.5/alphaz/models/database/users_definitions.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     9285 2022-08-02 08:51:28.000000 alphaz-0.7.5/alphaz/models/database/utils.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1061 2022-04-12 11:53:03.000000 alphaz-0.7.5/alphaz/models/database/views.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1241 2021-03-29 08:42:45.000000 alphaz-0.7.5/alphaz/models/excel.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6699 2023-04-21 07:47:57.000000 alphaz-0.7.5/alphaz/models/ftp.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      150 2022-07-19 09:10:48.000000 alphaz-0.7.5/alphaz/models/img.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.181110 alphaz-0.7.5/alphaz/models/json/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       41 2021-03-29 08:42:45.000000 alphaz-0.7.5/alphaz/models/json/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2609 2023-01-06 09:14:28.000000 alphaz-0.7.5/alphaz/models/json/_converters.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.181110 alphaz-0.7.5/alphaz/models/logger/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       68 2022-01-19 15:41:22.000000 alphaz-0.7.5/alphaz/models/logger/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1319 2023-01-06 09:14:28.000000 alphaz-0.7.5/alphaz/models/logger/_colorations.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    14091 2023-04-05 11:16:09.000000 alphaz-0.7.5/alphaz/models/logger/_logger.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      757 2021-03-29 08:42:45.000000 alphaz-0.7.5/alphaz/models/logger/_utils.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.181110 alphaz-0.7.5/alphaz/models/logs/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1280 2021-11-12 08:53:17.000000 alphaz-0.7.5/alphaz/models/logs/main.log
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      160 2021-11-07 15:22:58.000000 alphaz-0.7.5/alphaz/models/logs/main.log.2021-11-07
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.181110 alphaz-0.7.5/alphaz/models/main/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      385 2023-02-06 09:05:20.000000 alphaz-0.7.5/alphaz/models/main/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    27277 2023-04-18 09:00:04.000000 alphaz-0.7.5/alphaz/models/main/_base.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.181110 alphaz-0.7.5/alphaz/models/main/_core/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.5/alphaz/models/main/_core/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    14630 2023-04-08 19:36:08.000000 alphaz-0.7.5/alphaz/models/main/_core/_core.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       13 2021-03-29 08:42:45.000000 alphaz-0.7.5/alphaz/models/main/_core/_utils.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      339 2023-02-06 09:05:20.000000 alphaz-0.7.5/alphaz/models/main/_enum.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1862 2023-02-17 08:49:35.000000 alphaz-0.7.5/alphaz/models/main/_exception.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      501 2021-03-29 08:42:45.000000 alphaz-0.7.5/alphaz/models/main/_file.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      477 2021-03-29 08:42:45.000000 alphaz-0.7.5/alphaz/models/main/_process.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1305 2021-03-29 08:42:45.000000 alphaz-0.7.5/alphaz/models/main/_request.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      925 2021-03-29 08:42:45.000000 alphaz-0.7.5/alphaz/models/main/_singleton.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2258 2023-03-16 15:41:50.000000 alphaz-0.7.5/alphaz/models/request.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.185110 alphaz-0.7.5/alphaz/models/tests/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      139 2023-03-16 15:41:50.000000 alphaz-0.7.5/alphaz/models/tests/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6780 2023-02-23 09:08:35.000000 alphaz-0.7.5/alphaz/models/tests/_category.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3095 2023-02-23 09:08:35.000000 alphaz-0.7.5/alphaz/models/tests/_group.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      109 2021-09-10 07:16:32.000000 alphaz-0.7.5/alphaz/models/tests/_levels.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4174 2023-02-23 09:08:35.000000 alphaz-0.7.5/alphaz/models/tests/_method.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4571 2023-04-11 14:13:25.000000 alphaz-0.7.5/alphaz/models/tests/_save.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    13495 2023-04-18 11:53:08.000000 alphaz-0.7.5/alphaz/models/tests/_test.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     7413 2023-04-21 07:47:57.000000 alphaz-0.7.5/alphaz/models/tests/_wrappers.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2802 2022-12-01 15:14:08.000000 alphaz-0.7.5/alphaz/models/user.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2367 2021-03-29 08:42:45.000000 alphaz-0.7.5/alphaz/models/watcher.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.185110 alphaz-0.7.5/alphaz/pocs/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      685 2021-03-29 08:42:45.000000 alphaz-0.7.5/alphaz/pocs/main.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       72 2021-03-29 08:42:45.000000 alphaz-0.7.5/alphaz/reload_gitignore.bat
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       67 2022-04-12 12:30:24.000000 alphaz-0.7.5/alphaz/req.sh
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      460 2023-04-11 14:13:25.000000 alphaz-0.7.5/alphaz/requirements.txt
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1345 2022-04-19 08:43:27.000000 alphaz-0.7.5/alphaz/run.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.185110 alphaz-0.7.5/alphaz/src/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.5/alphaz/src/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    23747 2021-03-29 08:42:45.000000 alphaz-0.7.5/alphaz/src/alpha.png
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.185110 alphaz-0.7.5/alphaz/src/configs/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      135 2022-04-19 08:43:27.000000 alphaz-0.7.5/alphaz/src/configs/config.json
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      674 2023-01-25 21:39:07.000000 alphaz-0.7.5/alphaz/src/configs/loggers.json
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      490 2022-01-13 15:32:15.000000 alphaz-0.7.5/alphaz/src/configs/loggers_colors.json
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.185110 alphaz-0.7.5/alphaz/src/database/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.5/alphaz/src/database/__init__.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.185110 alphaz-0.7.5/alphaz/stitch/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1769 2021-03-29 08:42:45.000000 alphaz-0.7.5/alphaz/stitch/Core.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       26 2021-03-29 08:42:45.000000 alphaz-0.7.5/alphaz/stitch/__init__.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.185110 alphaz-0.7.5/alphaz/stitch/imports/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       78 2021-03-29 08:42:45.000000 alphaz-0.7.5/alphaz/stitch/imports/__init__.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.185110 alphaz-0.7.5/alphaz/stitch/models/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.5/alphaz/stitch/models/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      391 2021-03-29 08:42:45.000000 alphaz-0.7.5/alphaz/stitch/models/element.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       46 2021-03-29 08:42:45.000000 alphaz-0.7.5/alphaz/stitch/run.bat
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1857 2021-03-29 08:42:45.000000 alphaz-0.7.5/alphaz/stitch/stitch.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.193110 alphaz-0.7.5/alphaz/stitch/web-drivers/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)  8738816 2021-03-29 08:42:45.000000 alphaz-0.7.5/alphaz/stitch/web-drivers/chromedriver.exe
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)  7008696 2022-04-19 08:43:27.000000 alphaz-0.7.5/alphaz/stitch/web-drivers/geckodriver
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.121110 alphaz-0.7.5/alphaz/stitch/websites/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.201110 alphaz-0.7.5/alphaz/stitch/websites/Test/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      204 2021-03-29 08:42:45.000000 alphaz-0.7.5/alphaz/stitch/websites/Test/init.json
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.201110 alphaz-0.7.5/alphaz/stitch/websites/stiki/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      363 2022-04-13 09:59:51.000000 alphaz-0.7.5/alphaz/stitch/websites/stiki/init.json
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.201110 alphaz-0.7.5/alphaz/templates/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.5/alphaz/templates/__init__.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.201110 alphaz-0.7.5/alphaz/templates/assets/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.5/alphaz/templates/assets/__init__.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.201110 alphaz-0.7.5/alphaz/templates/assets/css/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    95923 2021-09-10 07:16:32.000000 alphaz-0.7.5/alphaz/templates/assets/css/home.css
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2356 2021-08-06 18:55:11.000000 alphaz-0.7.5/alphaz/templates/assets/css/logs.css
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.201110 alphaz-0.7.5/alphaz/templates/assets/images/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.201110 alphaz-0.7.5/alphaz/templates/assets/images/icons/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      276 2021-08-06 18:55:11.000000 alphaz-0.7.5/alphaz/templates/assets/images/icons/admin.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1444 2021-08-06 18:55:11.000000 alphaz-0.7.5/alphaz/templates/assets/images/icons/alpha.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      142 2021-08-06 18:55:11.000000 alphaz-0.7.5/alphaz/templates/assets/images/icons/save.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     8889 2021-08-06 18:55:11.000000 alphaz-0.7.5/alphaz/templates/assets/images/icons/start-icon.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      136 2021-08-06 18:55:11.000000 alphaz-0.7.5/alphaz/templates/assets/images/icons/user.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    23747 2021-08-06 18:55:11.000000 alphaz-0.7.5/alphaz/templates/assets/images/icons/wsalpha.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1165 2021-08-06 18:55:11.000000 alphaz-0.7.5/alphaz/templates/assets/images/loading.gif
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.201110 alphaz-0.7.5/alphaz/templates/assets/js/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.201110 alphaz-0.7.5/alphaz/templates/assets/js/libs/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    21922 2021-08-06 18:55:11.000000 alphaz-0.7.5/alphaz/templates/assets/js/libs/ansi_up.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    89475 2021-08-06 18:55:11.000000 alphaz-0.7.5/alphaz/templates/assets/js/libs/jquery.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     7339 2022-10-26 14:51:00.000000 alphaz-0.7.5/alphaz/templates/assets/js/logs.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       37 2021-03-29 08:42:45.000000 alphaz-0.7.5/alphaz/templates/hello.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    19017 2022-01-17 10:25:20.000000 alphaz-0.7.5/alphaz/templates/home.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3779 2021-08-06 18:55:11.000000 alphaz-0.7.5/alphaz/templates/logs.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1153 2023-01-25 21:39:07.000000 alphaz-0.7.5/alphaz/test.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.205110 alphaz-0.7.5/alphaz/tests/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      119 2021-03-29 08:42:45.000000 alphaz-0.7.5/alphaz/tests/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    13857 2023-03-28 08:47:21.000000 alphaz-0.7.5/alphaz/tests/api.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      541 2023-03-16 15:41:50.000000 alphaz-0.7.5/alphaz/tests/basic_test.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1526 2021-11-30 22:30:57.000000 alphaz-0.7.5/alphaz/tests/configurations.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    25482 2023-04-21 07:47:58.000000 alphaz-0.7.5/alphaz/tests/database.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      397 2021-03-29 08:42:45.000000 alphaz-0.7.5/alphaz/tests/processes.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      555 2021-03-29 08:42:45.000000 alphaz-0.7.5/alphaz/tests/utils.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.205110 alphaz-0.7.5/alphaz/utils/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       81 2021-03-29 08:42:45.000000 alphaz-0.7.5/alphaz/utils/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    11552 2023-02-16 14:12:47.000000 alphaz-0.7.5/alphaz/utils/api.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      338 2022-04-19 08:43:27.000000 alphaz-0.7.5/alphaz/utils/clean.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      813 2022-05-02 08:25:25.000000 alphaz-0.7.5/alphaz/utils/configuration.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.205110 alphaz-0.7.5/alphaz/utils/database/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    13859 2023-04-21 07:47:58.000000 alphaz-0.7.5/alphaz/utils/database/init.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     5438 2022-02-24 13:20:43.000000 alphaz-0.7.5/alphaz/utils/database_to_dataclass.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2207 2023-03-16 15:41:50.000000 alphaz-0.7.5/alphaz/utils/decorators.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3112 2021-03-29 08:42:45.000000 alphaz-0.7.5/alphaz/utils/ensure.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4405 2022-01-13 15:32:15.000000 alphaz-0.7.5/alphaz/utils/mep.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     7639 2021-04-21 22:36:11.000000 alphaz-0.7.5/alphaz/utils/screens.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    22569 2022-01-17 10:25:20.000000 alphaz-0.7.5/alphaz/utils/selectionMenu.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      764 2022-01-17 10:25:20.000000 alphaz-0.7.5/alphaz/utils/tasks.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1535 2023-02-23 09:08:35.000000 alphaz-0.7.5/alphaz/utils/tests.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      628 2023-03-16 15:41:50.000000 alphaz-0.7.5/alphaz/utils/time.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3766 2022-01-17 10:25:20.000000 alphaz-0.7.5/alphaz/utils/transactions.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 07:48:01.125110 alphaz-0.7.5/alphaz.egg-info/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      585 2023-04-21 07:48:00.000000 alphaz-0.7.5/alphaz.egg-info/PKG-INFO
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    11219 2023-04-21 07:48:00.000000 alphaz-0.7.5/alphaz.egg-info/SOURCES.txt
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        1 2023-04-21 07:48:00.000000 alphaz-0.7.5/alphaz.egg-info/dependency_links.txt
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      458 2023-04-21 07:48:00.000000 alphaz-0.7.5/alphaz.egg-info/requires.txt
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        7 2023-04-21 07:48:00.000000 alphaz-0.7.5/alphaz.egg-info/top_level.txt
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       79 2023-04-21 07:48:01.205110 alphaz-0.7.5/setup.cfg
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3092 2023-04-21 07:46:55.000000 alphaz-0.7.5/setup.py
```

### Comparing `alphaz-0.7.4.1/MANIFEST.in` & `alphaz-0.7.5/MANIFEST.in`

 * *Files 0% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 include alphaz/mails/Webmail.html
 include alphaz/mails/Images
 include alphaz/mails/stay_in_touch.html
 include alphaz/mails/mail.html
 include alphaz/mails/password_reset.html
 include alphaz/mails/template.html
 include alphaz/utils/__pycache__
+include alphaz/utils/database
 include alphaz/tests/__pycache__
 include alphaz/stitch/websites/stiki
 include alphaz/stitch/websites/Test
 include alphaz/stitch/web-drivers/geckodriver
 include alphaz/stitch/web-drivers/chromedriver.exe
 include alphaz/stitch/websites/stiki/init.json
 include alphaz/stitch/websites/Test/init.json
```

### Comparing `alphaz-0.7.4.1/PKG-INFO` & `alphaz-0.7.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: alphaz
-Version: 0.7.4.1
+Version: 0.7.5
 Summary: A package full of very nice tools
 Home-page: https://github.com/ZAurele/alphaz
 Author: Aurèle
 Author-email: contact@aurele.eu
 License: MIT
-Download-URL: https://github.com/ZAurele/alphaz/archive/refs/tags/0.7.4.1.tar.gz
+Download-URL: https://github.com/ZAurele/alphaz/archive/refs/tags/0.7.5.tar.gz
 Description: UNKNOWN
 Keywords: Flask,Json
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `alphaz-0.7.4.1/README.md` & `alphaz-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/api.json` & `alphaz-0.7.5/alphaz/api.json`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/api.py` & `alphaz-0.7.5/alphaz/api.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/apis/mails.py` & `alphaz-0.7.5/alphaz/apis/mails.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/apis/routes/admin.py` & `alphaz-0.7.5/alphaz/apis/routes/admin.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/apis/routes/api.py` & `alphaz-0.7.5/alphaz/apis/routes/api.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/apis/routes/basic_tests.py` & `alphaz-0.7.5/alphaz/apis/routes/basic_tests.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/apis/routes/database.py` & `alphaz-0.7.5/alphaz/apis/routes/database.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/apis/routes/logs.py` & `alphaz-0.7.5/alphaz/apis/routes/logs.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/apis/routes/mails.py` & `alphaz-0.7.5/alphaz/apis/routes/mails.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/apis/routes/main.py` & `alphaz-0.7.5/alphaz/apis/routes/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,15 +154,22 @@
         return {
             "version": str(module.__version__),
             "code": str(lines),
         }
     return {"version": module.__version__}
 
 
-@route("modules", parameters=[Parameter("name"), Parameter("url"), Parameter("mode")])
+@route(
+    "modules",
+    parameters=[
+        Parameter("name"),
+        Parameter("url"),
+        Parameter("mode", default="dict", options=["dict", "requirements"]),
+    ],
+)
 def get_modules():
     return py_lib.get_modules_infos(**API.gets())
 
 
 @route("cache")
 def get_cache_infos():
     return files_lib.get_size(API.conf.get("directories/cache"), with_unit=True)
@@ -217,16 +224,23 @@
         Parameter("keys", ptype=list, required=True),
         Parameter("config"),
     ],
 )
 def get_configs_key():
     return config_lib.get_configs_key(**API.get_parameters())
 
-@route('/mail', parameters=[
-    Parameter("name", required=True),
-    Parameter("parameters", ptype=List[dict])
-],admin=True, methods=["POST"])
+
+@route(
+    "/mail",
+    parameters=[
+        Parameter("name", required=True),
+        Parameter("parameters", ptype=List[dict]),
+    ],
+    admin=True,
+    methods=["POST"],
+)
 def mail_me():
     from ...libs import mail_lib
+
     mail_lib.send_mail(
         mail_config=API["name"], parameters_list=API["parameters"], force=True
-    )
+    )
```

### Comparing `alphaz-0.7.4.1/alphaz/apis/routes/tests.py` & `alphaz-0.7.5/alphaz/apis/routes/tests.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/apis/routes/user_management/application_management.py` & `alphaz-0.7.5/alphaz/apis/routes/user_management/application_management.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/apis/routes/user_management/permission_management.py` & `alphaz-0.7.5/alphaz/apis/routes/user_management/permission_management.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/apis/routes/user_management/role_management.py` & `alphaz-0.7.5/alphaz/apis/routes/user_management/role_management.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/apis/routes/user_management/user_management.py` & `alphaz-0.7.5/alphaz/apis/routes/user_management/user_management.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/apis/routes/users.py` & `alphaz-0.7.5/alphaz/apis/routes/users.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,107 +1,133 @@
+# CORE
+from core import core
+
+API = core.api
+
+# UTILS
 from ...utils.api import ADMIN_USER_ID_PUBLIC, ADMIN_USER_NAME_PUBLIC, route, Parameter
+
+# MODELS
 from ...models.main import AlphaException
-from ..users import users
-from core import core
 
-api = core.api
+# LIBS
+from ...libs import user_lib
+
+from ..users import users
 
 
 @route("user/infos", logged=True)
 def user_infos():
-    return api.get_logged_user()
+    return API.get_logged_user()
+
+
+@route(
+    "user/data",
+    parameters=[
+        Parameter("value", required=True),
+        Parameter("column", required=True),
+        Parameter("activity", ptype=bool),
+    ],
+)
+def user_data():
+    return user_lib.get_user_data_from_database(**API.gets(), force_local=True)
 
 
 @route(
     "/register",
     methods=["POST"],
     parameters=[
         Parameter("mail", required=True),
         Parameter("username", required=True),
         Parameter("password", required=True),
         Parameter("password_confirmation", required=True),
     ],
 )
 def register():
-    if api.get_logged_user() is not None:
+    if API.get_logged_user() is not None:
         raise AlphaException("logged")
-    users.try_register_user(**api.get_parameters())
+    users.try_register_user(**API.gets())
 
 
 @route(
     "/register/validation",
     methods=["POST"],
     parameters=[Parameter("tmp_token", required=True)],
 )
 def register_validation():
-    if api.get_logged_user() is not None:
+    if API.get_logged_user() is not None:
         raise AlphaException("logged")
-    users.confirm_user_registration(**api.get_parameters())
+    users.confirm_user_registration(**API.gets())
 
 
 @route(
     "/auth",
     methods=["POST"],
     parameters=[
         Parameter("username", required=True),
         Parameter("password", required=True),
     ],
 )
 def login():
-    return users.try_login(**api.get_parameters())
+    return users.try_login(**API.gets())
 
 
 @route(
     "/auth/su",
     methods=["POST"],
     parameters=[ADMIN_USER_ID_PUBLIC, ADMIN_USER_NAME_PUBLIC],
     admin=True,
 )
 def su_login():
-    return users.try_su_login(**api.get_parameters())
+    return users.try_su_login(**API.gets())
 
 
-@route("/ldap/users", parameters=[Parameter("filters", required=True, ptype=str),])
+@route(
+    "/ldap/users",
+    parameters=[
+        Parameter("filters", required=True, ptype=str),
+    ],
+)
 def get_ldap_users():
     from ..users import users, ldap  # TODO: modify
 
-    return ldap.get_ldap_users(**api.get_parameters())
+    return ldap.get_ldap_users(**API.gets())
 
 
 @route(
     "/password/lost",
     methods=["POST"],
     parameters=[
         Parameter("username", required=False),
         Parameter("mail", required=False),
     ],
 )
 def password_lost():
-    if api.get_logged_user() is not None:
+    if API.get_logged_user() is not None:
         raise AlphaException("logged")
-    if api["username"] is None and api.get["mail"] is None:
+    if API["username"] is None and API.get["mail"] is None:
         raise AlphaException("inputs")
     users.ask_password_reset(
-        api["username"] if api.get["mail"] is None else api.get["mail"]
+        API["username"] if API.get["mail"] is None else API.get["mail"]
     )
 
 
 @route(
     "/password/reset",
     methods=["GET", "POST"],
     parameters=[
         Parameter("tmp_token", required=True),
         Parameter("password", required=True),
         Parameter("password_confirmation", required=True),
     ],
 )
 def password_reset_validation():
-    if api.get_logged_user() is not None:
+    if API.get_logged_user() is not None:
         raise AlphaException("logged")
-    users.confirm_user_password_reset(**api.get_parameters())
+    users.confirm_user_password_reset(**API.gets())
 
 
 @route("/logout", cache=False, logged=False, methods=["GET", "POST"])
 def logout():
     users.logout()
 
 
@@ -116,8 +142,8 @@
     methods=["POST"],
     parameters=[
         Parameter("password", required=True),
         Parameter("password_confirmation", required=True),
     ],
 )
 def reset_user_password():
-    users.try_reset_password(**api.get_parameters())
+    users.try_reset_password(**API.gets())
```

### Comparing `alphaz-0.7.4.1/alphaz/apis/tests.py` & `alphaz-0.7.5/alphaz/apis/tests.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/apis/users/ldap.py` & `alphaz-0.7.5/alphaz/apis/users/ldap.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/apis/users/users.py` & `alphaz-0.7.5/alphaz/apis/users/users.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/config/config.css` & `alphaz-0.7.5/alphaz/config/config.css`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/config/config.html` & `alphaz-0.7.5/alphaz/config/config.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/config/main_configuration.py` & `alphaz-0.7.5/alphaz/config/main_configuration.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/config/page.py` & `alphaz-0.7.5/alphaz/config/page.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/config/source.html` & `alphaz-0.7.5/alphaz/config/source.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/config.json` & `alphaz-0.7.5/alphaz/config.json`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/docs/alpha_core.md` & `alphaz-0.7.5/alphaz/documentations/docs/alpha_core.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/docs/alpha_screens.md` & `alphaz-0.7.5/alphaz/documentations/docs/alpha_screens.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/docs/alpha_setup.md` & `alphaz-0.7.5/alphaz/documentations/docs/alpha_setup.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/docs/api/authorizations.md` & `alphaz-0.7.5/alphaz/documentations/docs/api/authorizations.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/docs/api/configuration.md` & `alphaz-0.7.5/alphaz/documentations/docs/api/configuration.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/docs/api/main.md` & `alphaz-0.7.5/alphaz/documentations/docs/api/main.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/docs/api/methods.md` & `alphaz-0.7.5/alphaz/documentations/docs/api/methods.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/docs/api/parameters.md` & `alphaz-0.7.5/alphaz/documentations/docs/api/parameters.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/docs/api/routes.md` & `alphaz-0.7.5/alphaz/documentations/docs/api/routes.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/docs/api_database.md` & `alphaz-0.7.5/alphaz/documentations/docs/api_database.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/docs/configuration.md` & `alphaz-0.7.5/alphaz/documentations/docs/configuration.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/docs/database/init.md` & `alphaz-0.7.5/alphaz/documentations/docs/database/init.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/docs/database/model.md` & `alphaz-0.7.5/alphaz/documentations/docs/database/model.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/docs/database/schema.md` & `alphaz-0.7.5/alphaz/documentations/docs/database/schema.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/docs/database/update.md` & `alphaz-0.7.5/alphaz/documentations/docs/database/update.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/docs/index.md` & `alphaz-0.7.5/alphaz/documentations/docs/index.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/mkdocs.yml` & `alphaz-0.7.5/alphaz/documentations/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/site/404.html` & `alphaz-0.7.5/alphaz/documentations/site/404.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/site/alpha_admin/index.html` & `alphaz-0.7.5/alphaz/documentations/site/alpha_admin/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/site/alpha_core/index.html` & `alphaz-0.7.5/alphaz/documentations/site/alpha_core/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/site/alpha_screens/index.html` & `alphaz-0.7.5/alphaz/documentations/site/alpha_screens/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/site/alpha_setup/index.html` & `alphaz-0.7.5/alphaz/documentations/site/alpha_setup/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/site/api/authorizations/index.html` & `alphaz-0.7.5/alphaz/documentations/site/api/authorizations/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/site/api/cache/index.html` & `alphaz-0.7.5/alphaz/documentations/site/api/cache/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/site/api/configuration/index.html` & `alphaz-0.7.5/alphaz/documentations/site/api/configuration/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/site/api/issues/index.html` & `alphaz-0.7.5/alphaz/documentations/site/api/issues/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/site/api/main/index.html` & `alphaz-0.7.5/alphaz/documentations/site/api/main/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/site/api/methods/index.html` & `alphaz-0.7.5/alphaz/documentations/site/api/methods/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/site/api/parameters/index.html` & `alphaz-0.7.5/alphaz/documentations/site/api/parameters/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/site/api/routes/index.html` & `alphaz-0.7.5/alphaz/documentations/site/api/routes/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/site/api/sqlalchemy/index.html` & `alphaz-0.7.5/alphaz/documentations/site/api/sqlalchemy/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/site/api_database/index.html` & `alphaz-0.7.5/alphaz/documentations/site/api_database/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/site/assets/images/favicon.png` & `alphaz-0.7.5/alphaz/documentations/site/assets/images/favicon.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js` & `alphaz-0.7.5/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js.map` & `alphaz-0.7.5/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js.map`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ar.min.js` & `alphaz-0.7.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ar.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.da.min.js` & `alphaz-0.7.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.da.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.de.min.js` & `alphaz-0.7.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.de.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.du.min.js` & `alphaz-0.7.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.du.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.es.min.js` & `alphaz-0.7.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.es.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fi.min.js` & `alphaz-0.7.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fi.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fr.min.js` & `alphaz-0.7.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fr.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.hu.min.js` & `alphaz-0.7.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.hu.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.it.min.js` & `alphaz-0.7.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.it.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ja.min.js` & `alphaz-0.7.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ja.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.multi.min.js` & `alphaz-0.7.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.multi.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.nl.min.js` & `alphaz-0.7.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.nl.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.no.min.js` & `alphaz-0.7.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.no.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.pt.min.js` & `alphaz-0.7.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.pt.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ro.min.js` & `alphaz-0.7.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ro.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ru.min.js` & `alphaz-0.7.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ru.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js` & `alphaz-0.7.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.sv.min.js` & `alphaz-0.7.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.sv.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.tr.min.js` & `alphaz-0.7.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.tr.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.vi.min.js` & `alphaz-0.7.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.vi.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/site/assets/javascripts/lunr/tinyseg.js` & `alphaz-0.7.5/alphaz/documentations/site/assets/javascripts/lunr/tinyseg.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js` & `alphaz-0.7.5/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js.map` & `alphaz-0.7.5/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js.map`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css` & `alphaz-0.7.5/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css.map` & `alphaz-0.7.5/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css.map`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css` & `alphaz-0.7.5/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css.map` & `alphaz-0.7.5/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css.map`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/site/configuration/index.html` & `alphaz-0.7.5/alphaz/documentations/site/configuration/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/site/database/init/index.html` & `alphaz-0.7.5/alphaz/documentations/site/database/init/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/site/database/instantiate/index.html` & `alphaz-0.7.5/alphaz/documentations/site/database/instantiate/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/site/database/main/index.html` & `alphaz-0.7.5/alphaz/documentations/site/database/main/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/site/database/model/index.html` & `alphaz-0.7.5/alphaz/documentations/site/database/model/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/site/database/relations/index.html` & `alphaz-0.7.5/alphaz/documentations/site/database/relations/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/site/database/schema/index.html` & `alphaz-0.7.5/alphaz/documentations/site/database/schema/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/site/database/update/index.html` & `alphaz-0.7.5/alphaz/documentations/site/database/update/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/site/documentation/index.html` & `alphaz-0.7.5/alphaz/documentations/site/documentation/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/site/index.html` & `alphaz-0.7.5/alphaz/documentations/site/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/site/search/search_index.json` & `alphaz-0.7.5/alphaz/documentations/site/search/search_index.json`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/documentations/site/sitemap.xml` & `alphaz-0.7.5/alphaz/documentations/site/sitemap.xml`

 * *Files 12% similar despite different names*

#### Comparing `alphaz-0.7.4.1/alphaz/documentations/site/sitemap.xml` & `alphaz-0.7.5/alphaz/documentations/site/sitemap.xml`

```diff
@@ -1,128 +1,128 @@
 <?xml version="1.0" encoding="utf-8"?>
 <urlset xmlns="http://www.sitemaps.org/schemas/sitemap/0.9">
   <url>
     <loc>None</loc>
-    <lastmod>2023-04-19</lastmod>
+    <lastmod>2023-04-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>None</loc>
-    <lastmod>2023-04-19</lastmod>
+    <lastmod>2023-04-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>None</loc>
-    <lastmod>2023-04-19</lastmod>
+    <lastmod>2023-04-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>None</loc>
-    <lastmod>2023-04-19</lastmod>
+    <lastmod>2023-04-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>None</loc>
-    <lastmod>2023-04-19</lastmod>
+    <lastmod>2023-04-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>None</loc>
-    <lastmod>2023-04-19</lastmod>
+    <lastmod>2023-04-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>None</loc>
-    <lastmod>2023-04-19</lastmod>
+    <lastmod>2023-04-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>None</loc>
-    <lastmod>2023-04-19</lastmod>
+    <lastmod>2023-04-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>None</loc>
-    <lastmod>2023-04-19</lastmod>
+    <lastmod>2023-04-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>None</loc>
-    <lastmod>2023-04-19</lastmod>
+    <lastmod>2023-04-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>None</loc>
-    <lastmod>2023-04-19</lastmod>
+    <lastmod>2023-04-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>None</loc>
-    <lastmod>2023-04-19</lastmod>
+    <lastmod>2023-04-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>None</loc>
-    <lastmod>2023-04-19</lastmod>
+    <lastmod>2023-04-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>None</loc>
-    <lastmod>2023-04-19</lastmod>
+    <lastmod>2023-04-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>None</loc>
-    <lastmod>2023-04-19</lastmod>
+    <lastmod>2023-04-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>None</loc>
-    <lastmod>2023-04-19</lastmod>
+    <lastmod>2023-04-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>None</loc>
-    <lastmod>2023-04-19</lastmod>
+    <lastmod>2023-04-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>None</loc>
-    <lastmod>2023-04-19</lastmod>
+    <lastmod>2023-04-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>None</loc>
-    <lastmod>2023-04-19</lastmod>
+    <lastmod>2023-04-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>None</loc>
-    <lastmod>2023-04-19</lastmod>
+    <lastmod>2023-04-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>None</loc>
-    <lastmod>2023-04-19</lastmod>
+    <lastmod>2023-04-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>None</loc>
-    <lastmod>2023-04-19</lastmod>
+    <lastmod>2023-04-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>None</loc>
-    <lastmod>2023-04-19</lastmod>
+    <lastmod>2023-04-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>None</loc>
-    <lastmod>2023-04-19</lastmod>
+    <lastmod>2023-04-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>None</loc>
-    <lastmod>2023-04-19</lastmod>
+    <lastmod>2023-04-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
 </urlset>
```

### Comparing `alphaz-0.7.4.1/alphaz/index.html` & `alphaz-0.7.5/alphaz/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/libs/api_lib.py` & `alphaz-0.7.5/alphaz/libs/api_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/libs/barcode_lib.py` & `alphaz-0.7.5/alphaz/libs/barcode_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/libs/config_lib.py` & `alphaz-0.7.5/alphaz/libs/config_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/libs/converter_lib.py` & `alphaz-0.7.5/alphaz/libs/converter_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/libs/date_lib.py` & `alphaz-0.7.5/alphaz/libs/date_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/libs/dict_lib.py` & `alphaz-0.7.5/alphaz/libs/dict_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/libs/emulation/vt102_lib.py` & `alphaz-0.7.5/alphaz/libs/emulation/vt102_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/libs/events.py` & `alphaz-0.7.5/alphaz/libs/events.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/libs/files_lib.py` & `alphaz-0.7.5/alphaz/libs/files_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/libs/flask_lib.py` & `alphaz-0.7.5/alphaz/libs/flask_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/libs/img_lib.py` & `alphaz-0.7.5/alphaz/libs/img_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/libs/io_lib.py` & `alphaz-0.7.5/alphaz/libs/io_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/libs/json_lib.py` & `alphaz-0.7.5/alphaz/libs/json_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/libs/logs_lib.py` & `alphaz-0.7.5/alphaz/libs/logs_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/libs/mail_lib.py` & `alphaz-0.7.5/alphaz/libs/mail_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/libs/notifications_lib.py` & `alphaz-0.7.5/alphaz/libs/notifications_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/libs/number_lib.py` & `alphaz-0.7.5/alphaz/libs/number_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/libs/process_lib.py` & `alphaz-0.7.5/alphaz/libs/process_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/libs/py_lib.py` & `alphaz-0.7.5/alphaz/libs/py_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/libs/scp_lib.py` & `alphaz-0.7.5/alphaz/libs/scp_lib.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,25 @@
-import paramiko
+import warnings
+from cryptography.utils import CryptographyDeprecationWarning
+
+with warnings.catch_warnings():
+    warnings.filterwarnings("ignore", category=CryptographyDeprecationWarning)
+    import paramiko
+
 import scpclient
 
-def scp_to_server(file_path,host, username,password=None,copy=False):
-    """ Securely copy the file to the server. """
+
+def scp_to_server(file_path, host, username, password=None, copy=False):
+    """Securely copy the file to the server."""
     ssh_client = paramiko.SSHClient()
     ssh_client.load_system_host_keys()
-    #ssh_client.set_missing_host_key_policy(paramiko.AutoAddPolicy()) 
+    # ssh_client.set_missing_host_key_policy(paramiko.AutoAddPolicy())
     ssh_client.set_missing_host_key_policy(paramiko.WarningPolicy())
-    ssh_client.connect(host, username=username, password=password,port=22)
+    ssh_client.connect(host, username=username, password=password, port=22)
 
-    if not copy: return
+    if not copy:
+        return
 
     with scpclient.closing(scpclient.Write(ssh_client.get_transport(), "~/")) as scp:
-        scp.send_file(file_path, remote_filename="/data/elk/workstream_dbms_logs/from_ws/test.BIN")
+        scp.send_file(
+            file_path, remote_filename="/data/elk/workstream_dbms_logs/from_ws/test.BIN"
+        )
```

### Comparing `alphaz-0.7.4.1/alphaz/libs/search_lib.py` & `alphaz-0.7.5/alphaz/libs/search_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/libs/secure_lib.py` & `alphaz-0.7.5/alphaz/libs/secure_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/libs/soap_lib.py` & `alphaz-0.7.5/alphaz/libs/soap_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/libs/ssh_lib.py` & `alphaz-0.7.5/alphaz/libs/ssh_lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,23 @@
+# MODULES
 from threading import current_thread
-import paramiko, encodings, scp, re, datetime, os
+import encodings, scp, re, datetime, os
 from typing import Dict, List
 
+import warnings
+from cryptography.utils import CryptographyDeprecationWarning
+
+with warnings.catch_warnings():
+    warnings.filterwarnings("ignore", category=CryptographyDeprecationWarning)
+    import paramiko
+
+# MODELS
 from ..models.main import AlphaFile
+
+# LIBS
 from .string_lib import universal_decode
 from . import io_lib
 
 WINDOWS_LINE_ENDING = "\r\n"
 UNIX_LINE_ENDING = "\n"
```

### Comparing `alphaz-0.7.4.1/alphaz/libs/string_lib.py` & `alphaz-0.7.5/alphaz/libs/string_lib.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import re, string, chardet, unicodedata, encodings, warnings
 from typing import Any, Dict, List, Tuple
 
 import hashlib
 
+
 def is_number(txt: str) -> bool:
     """
     Check if a string is a number.
 
     Args:
         txt: The string to check.
 
@@ -92,87 +93,14 @@
             continue
         if len(x) <= 2 or is_number(x):
             continue
         words_out.append(x)
     return words_out
 
 
-black_list = [
-    "cp037",
-    "utf_16_be",
-    "cp1252",
-    "hz",
-    "ascii",
-    "utf_32",
-    "cp500",
-    "cp1140",
-    "gb2312",
-    "euc_jis_2004",
-    "cp865",
-    "ptcp154",
-    "cp860",
-    "cp437",
-    "koi8_r",
-    "cp1256",
-    "cp863",
-    "cp1125",
-    "gbk",
-    "iso8859_11",
-    "mac_iceland",
-    "mac_latin2",
-    "iso8859_8",
-    "iso2022_jp_ext",
-    "mac_greek",
-    "big5hkscs",
-    "cp949",
-    "cp866",
-    "mac_turkish",
-    "iso2022_jp_2",
-    "mac_roman",
-    "cp1250",
-    "cp950",
-    "kz1048",
-    "shift_jisx0213",
-    "cp1258",
-    "cp1253",
-    "big5",
-    "cp932",
-    "cp852",
-    "quopri_codec",
-    "bz2_codec",
-    "iso2022_jp_1",
-    "euc_kr",
-    "cp862",
-    "cp858",
-    "cp861",
-    "tis_620",
-    "cp869",
-    "cp855",
-    "shift_jis_2004",
-    "cp775",
-    "cp1026",
-    "zlib_codec",
-    "utf_16",
-    "cp1254",
-    "iso8859_7",
-    "cp850",
-    "iso8859_6",
-    "shift_jis",
-    "utf_16_le",
-    "utf_32_be",
-    "mac_cyrillic",
-    "cp273",
-    "mbcs",
-    "uu_codec",
-    "utf_32_le",
-    "cp1251",
-    "iso2022_kr",
-    "cp857",
-]
-
 """
 def universal_decode(txt, encodings_methods=[], blacklist=[]):
     encodings_methods.extend(list(set(encodings.aliases.aliases.values())))
 
     result = txt
     for encoding_method in encodings_methods:
         if encoding_method not in blacklist:
@@ -432,12 +360,13 @@
     Returns:
         A string with accent characters removed and converted to lowercase.
     """
     new = unicodedata.normalize("NFKD", old).encode("ascii", "ignore").decode("utf-8")
     new = new.lower()
     return new
 
+
 def create_hash(*args):
     hash_obj = hashlib.sha256()
     for arg in args:
-        hash_obj.update(str(arg).encode('utf-8'))
-    return hash_obj.hexdigest()
+        hash_obj.update(str(arg).encode("utf-8"))
+    return hash_obj.hexdigest()
```

### Comparing `alphaz-0.7.4.1/alphaz/libs/test_lib.py` & `alphaz-0.7.5/alphaz/libs/test_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/libs/time_lib.py` & `alphaz-0.7.5/alphaz/libs/time_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/libs/transactions_lib.py` & `alphaz-0.7.5/alphaz/libs/transactions_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/libs/user_management/application_management_lib.py` & `alphaz-0.7.5/alphaz/libs/user_management/application_management_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/libs/user_management/permission_management_lib.py` & `alphaz-0.7.5/alphaz/libs/user_management/permission_management_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/libs/user_management/role_management_lib.py` & `alphaz-0.7.5/alphaz/libs/user_management/role_management_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/libs/user_management/user_management_lib.py` & `alphaz-0.7.5/alphaz/libs/user_management/user_management_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/mails/Images/Background.png` & `alphaz-0.7.5/alphaz/mails/Images/Background.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/mails/Images/Facebook_logo.png` & `alphaz-0.7.5/alphaz/mails/Images/Facebook_logo.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/mails/Images/Twitter_logo.png` & `alphaz-0.7.5/alphaz/mails/Images/Twitter_logo.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/mails/Images/Web_logo.png` & `alphaz-0.7.5/alphaz/mails/Images/Web_logo.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/mails/Mail.png` & `alphaz-0.7.5/alphaz/mails/Mail.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/mails/Webmail.html` & `alphaz-0.7.5/alphaz/mails/Webmail.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/mails/debug.html` & `alphaz-0.7.5/alphaz/mails/debug.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/mails/mail.html` & `alphaz-0.7.5/alphaz/mails/mail.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/mails/password_reset.html` & `alphaz-0.7.5/alphaz/mails/password_reset.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/mails/stay_in_touch.html` & `alphaz-0.7.5/alphaz/mails/stay_in_touch.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/models/api/_answer.py` & `alphaz-0.7.5/alphaz/models/api/_answer.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/models/api/_colorations.py` & `alphaz-0.7.5/alphaz/models/api/_colorations.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/models/api/_parameter.py` & `alphaz-0.7.5/alphaz/models/api/_parameter.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/models/api/_requests.py` & `alphaz-0.7.5/alphaz/models/api/_requests.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/models/api/_route.py` & `alphaz-0.7.5/alphaz/models/api/_route.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/models/api/_structures.py` & `alphaz-0.7.5/alphaz/models/api/_structures.py`

 * *Files 0% similar despite different names*

```diff
@@ -457,15 +457,15 @@
                 ],
                 reloader_type=reloader_type,
             )
 
         # except SystemExit:
         #    self.info("API stopped")
 
-    def stop(self, config_path=None): # TODO: change
+    def stop(self, config_path=None):  # TODO: change
         if config_path is None:
             config_path = self.config_path
         if self.config_path is None:
             return
 
         # self.set_config(config_path=config_path, configuration=self.configuration)
 
@@ -624,16 +624,18 @@
         secret_key = self.config["JWT_SECRET_KEY"]
 
         user = None
         token = (
             AlphaRequest.get_token() if self.admin_token is None else self.admin_token
         )
 
-        su_user_id = self[ADMIN_USER_ID_PUBLIC.name]
-        su_user_name = self[ADMIN_USER_NAME_PUBLIC.name]
+        su_user_id, su_user_name = (
+            self[ADMIN_USER_ID_PUBLIC.name],
+            self[ADMIN_USER_NAME_PUBLIC.name],
+        )
 
         if (
             self.is_admin(check_logged_user=False)
             and su_user_id is not None
             or su_user_name is not None
         ):
             user = self.get_su_user(su_user_id, su_user_name)
```

### Comparing `alphaz-0.7.4.1/alphaz/models/api/_utils.py` & `alphaz-0.7.5/alphaz/models/api/_utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/models/config/_config.py` & `alphaz-0.7.5/alphaz/models/config/_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/models/config/_utils.py` & `alphaz-0.7.5/alphaz/models/config/_utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/models/database/main_definitions.py` & `alphaz-0.7.5/alphaz/models/database/main_definitions.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/models/database/models.py` & `alphaz-0.7.5/alphaz/models/database/models.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/models/database/operators.py` & `alphaz-0.7.5/alphaz/models/database/operators.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/models/database/requests.py` & `alphaz-0.7.5/alphaz/models/database/requests.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/models/database/row.py` & `alphaz-0.7.5/alphaz/models/database/row.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/models/database/structure.py` & `alphaz-0.7.5/alphaz/models/database/structure.py`

 * *Files 1% similar despite different names*

```diff
@@ -375,24 +375,25 @@
         log: AlphaLogger = None,
         config=None,
         timeout: int = None,
         main: bool = False,
         **kwargs,
     ):
         self.db_type: str = config.get("type", "oracle")
-        # cnx = config["cnx"]
+        self.user_data_url = config.get("user_data_url", None)
 
         """if type(cnx) == dict:
             cnx = py_lib.filter_kwargs(create_engine, kwargs=cnx)"""
         # engine = create_engine(cnx)
         # event.listen(engine, "before_cursor_execute", add_own_encoders)
         # self._engine = engine
 
         engine_options = config.get("engine_options", {})
         session_options = config.get("session_options", {})
+
         self.autocommit = (
             "autocommit" in session_options and session_options["autocommit"]
         )
         super().__init__(
             *args,
             engine_options=engine_options,
             session_options=session_options,
@@ -419,19 +420,21 @@
         self.query_str = None
         self.full_count = None
         self.pagination_mode = config.get("pagination_mode", "raw")
         self.mapping_mode = config.get("mapping_mode", MappingMode.AUTO1.value)
 
         self.models = []
 
-    """def get_engine(self, bind=None):
-        return self.db.get_engine(bind=self.name)
+    def get_session(self, bind: str = None):
+        return self.db.session if bind is None else self.get_engine(bind=bind)
 
-    def get_session(self):
-        return self.db.session"""
+    def get_meta(self, bind: str = None):
+        engine = self.get_engine(bind=bind)
+        meta = MetaData(engine)
+        return meta
 
     def to_json(self):
         return py_lib.get_attributes(self)
 
     def test(self, bind: str = None, close=False):
         """[Test the connection]
 
@@ -541,31 +544,33 @@
         commit: bool = True,
         bind: str = None,
         close: bool = False,
     ) -> bool:
         if self.db_type == "sqlite":
             query = query.replace("%s", "?")
 
+        engine = self.get_engine(bind=bind)
+
         # redirect to get if select
         select = query.strip().upper()[:6] == "SELECT"
         if select:
             return self.get_query_results(
                 query, values, unique=False, bind=bind, close=close
             )
         try:
             if multi:
                 for value in values:
                     if value is not None:
-                        self.get_engine(bind=bind).execute(query, value)
-                    self.get_engine(bind=bind).execute(query)
+                        engine.execute(query, value)
+                    engine.execute(query)
             else:
                 if values is not None:
-                    self.get_engine(bind=bind).execute(query, values)
+                    engine.execute(query, values)
                 else:
-                    self.get_engine(bind=bind).execute(query)
+                    engine.execute(query)
             self.query_str = get_compiled_query(query).replace("\n", "")
             if commit and not self.autocommit:
                 self.commit()
             if close:
                 self.session.close()
             return True
         except Exception as ex:
@@ -676,15 +681,15 @@
             performance_schema.threads T
         WHERE ESH.THREAD_ID = T.THREAD_ID
         AND ESH.SQL_TEXT IS NOT NULL
         AND T.PROCESSLIST_ID = %s
         ORDER BY ESH.EVENT_ID LIMIT 10;"""
 
         transaction_id = None
-        result_list = self.get_engine().execute("show engine innodb status;")
+        result_list = self.get_engine(bind=bind).execute("show engine innodb status;")
         outputs = {}
         for result in list(result_list)[0]:
             for line in result.split("\n"):
                 if transaction_id is not None:
                     matchs_thread = re.findall("thread id ([0-9]*),", line)
                     matchs_query = re.findall("query id ([0-9]*)", line)
                     if len(matchs_thread):
@@ -732,52 +737,56 @@
         )
 
     def add(
         self,
         model,
         parameters=None,
         commit: bool = True,
-        test: bool = False,
         update: bool = False,
         flush: bool = True,
         close: bool = False,
+        rollback: bool = False,
+        test: bool = False,
     ) -> object:
         if test:
-            self.log.info(f"Insert {model} with values {parameters}")
-            return None
-
+            return True
         obj = model
         if parameters is not None:
             if type(parameters) != dict:
                 self.log.error("<parameters must be of type <dict>")
                 return None
             parameters = {
                 x if not "." in str(x) else str(x).split(".")[-1]: y
                 for x, y in parameters.items()
             }
             obj = model(**parameters)
 
         if type(obj) == list:
+            session = obj[0].query.session
             if not update:
-                self.session.add_all(obj)
+                session.add_all(obj)
             else:
                 for o in obj:
-                    self.session.merge(o)
+                    session.merge(o)
         else:
+            session = obj.query.session
             if not update:
-                self.session.add(obj)
+                session.add(obj)
             else:
-                self.session.merge(obj)
+                session.merge(obj)
 
         if commit and not self.autocommit:
-            self.commit()
+            self.commit(session=session)
         elif flush:
-            self.session.flush()
+            session.flush()
+        if rollback:
+            session.rollback()
+
         if close:
-            self.session.close()
+            session.close()
         return obj
 
     def upsert(self, model, rows, bind=None):
         if type(rows) != list:
             rows = [rows]
         from sqlalchemy.dialects import postgresql
         from sqlalchemy import UniqueConstraint
@@ -833,15 +842,14 @@
         valid = True
         try:
             session.commit()
         except Exception as ex:
             self.log.error(ex=ex)
             session.rollback()
             valid = False
-
             raise ex
 
         finally:
             if close:
                 session.close()
         return valid
 
@@ -954,23 +962,24 @@
                     if hasattr(x, "__tablename__")
                 ]
             self.models = registered_models
         return self.models
 
     def ensure(self, table_name: str, bind=None, drop: bool = False):
         if not table_name.lower() in self.get_bind_tablenames(bind):
+            engine = self.get_engine(bind=bind)
             request_model = self.get_table_model(bind, table_name)
 
             self.log.info(f"Creating <{table_name}> table in <{bind}> database")
             try:
-                request_model.__table__.create(self.get_engine(bind=bind))
+                request_model.__table__.create(engine)
             except Exception as ex:
                 if drop:
                     self.log.info(f"Drop <{table_name}> table in <{bind}> database")
-                    request_model.__table__.drop(self.get_engine(bind=bind))
+                    request_model.__table__.drop(engine)
                     self.ensure(table_name)
                 else:
                     self.log.error(ex)
 
         """
         
         #if not cls.__tablename__ in cls.metadata.tables:
@@ -1408,20 +1417,24 @@
                     self.log.error(f"Cannot find any entry for model {model}")
                     return False
                 rows = self.select(model, filters=filters)
                 if len(rows) == 0:
                     self.log.error(f"Cannot find any entry for model {model}")
                     return False
 
+                values_to_update = {}
                 for row in rows:
                     for key, value in values.items():
                         if not_none and value is None:
                             continue
                         setattr(row, key if type(key) == str else key.key, value)
-                    self.session.merge(row)
+                        values_to_update[key if type(key) == str else key.key] = value
+                    # self.session.merge(row)
+                    # row.query.session.merge(row)
+                    row.query.update(values_to_update)
             else:
                 query = self._get_filtered_query(model, filters=filters)
                 values_update = self.get_values(model, values, filters)
 
                 if fetch:
                     query.update(values_update, synchronize_session="fetch")
                 else:
@@ -1443,24 +1456,27 @@
     ):
         for i, transient in enumerate(transients):
             model = transient.__class__
             filters = [] if filters is None else filters
 
             attributes = model._sa_class_manager.local_attrs
 
+            values_to_update = {}
             if len(filters) == 0:
                 for name, attribute in attributes.items():
                     val = getattr(transient, name)
 
                     if (
                         hasattr(attribute.expression, "primary_key")
                         and attribute.expression.primary_key
                         and val is not None
                     ):
                         filters.append(attribute == val)
+                    elif attribute.expression.key is not None:
+                        values_to_update[name] = val
 
             filters = get_filters(filters, model)
             if len(filters) == 0:
                 self.log.error(f"Cannot find any entry to update for model {model}")
                 return False
             rows = self.select(model, filters=filters)
             if len(rows) == 0:
@@ -1468,15 +1484,17 @@
                 return False
 
             if len(rows) != 1:
                 self.log.error(
                     f"Too much entries to update corresponding to {transient}"
                 )
                 return False
-            self.session.merge(transient)
+            # rows[0].query.update(values_to_update)
+            model.query.update(values_to_update)
+            # self.session.merge(transient)
         if commit:
             return self.commit(close)
         return True
 
     def get_values(self, model, values, filters=None):
         values_update = {}
         for key, value in values.items():
@@ -1574,15 +1592,16 @@
             if not bind in tables_by_bind:
                 tables_by_bind[bind] = [table_model]
             else:
                 tables_by_bind[bind].append(table_model)
 
         for bind, tables_models in tables_by_bind.items():
             tables = [x.__table__ for x in tables_models]
-            meta = MetaData(self.get_engine(bind=bind))
+            meta = self.get_meta(bind=bind)
+
             table_names = [x.__tablename__ for x in tables_models]
             tables_names_str = ";".join(table_names)
             if drop:
                 if log is not None:
                     log.info(f"Drop tables from bind {bind}: {tables_names_str}")
                 meta.drop_all(tables=tables)
             if create:
```

### Comparing `alphaz-0.7.4.1/alphaz/models/database/tests.py` & `alphaz-0.7.5/alphaz/models/database/tests.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/models/database/users_definitions.py` & `alphaz-0.7.5/alphaz/models/database/users_definitions.py`

 * *Files 6% similar despite different names*

```diff
@@ -70,14 +70,15 @@
     id = AlphaColumn(Integer, autoincrement=True, primary_key=True)
     username = AlphaColumn(String(30), unique=True)
     mail = AlphaColumn(String(40), default="-")
     password = AlphaColumn(String(100))
     pass_reset_token = AlphaColumn(String(100))
     pass_reset_token_exp = AlphaColumn(DateTime)
     telegram_id = AlphaColumn(String(100))
+    # icon = AlphaColumn(String(100))
     role = AlphaColumn(Integer)
 
     expire = AlphaColumn(DateTime)
     date_registred = AlphaColumn(DateTime)
     registration_token = AlphaColumn(String(100))
     registration_code = AlphaColumn(String(255))
     infos = AlphaColumn(String(500))
@@ -134,15 +135,17 @@
     __bind_key__ = BIND
     __tablename__ = "permission"
 
     key = AlphaColumn(String(200), primary_key=True)
     description = AlphaColumn(String(1000))
     activated = AlphaColumn(Boolean, default=True)
 
-    roles = relationship("Role", secondary="role_permission")
+    roles = relationship(
+        "Role", secondary="role_permission", overlaps="permissions"
+    )  # TODO: remove overlaps="permissions" and fix the warning
 
 
 class Notification(db.Model, AlphaTableUpdateDate):
     __bind_key__ = BIND
     __tablename__ = "notification"
 
     user_id = AlphaColumn(
```

### Comparing `alphaz-0.7.4.1/alphaz/models/database/utils.py` & `alphaz-0.7.5/alphaz/models/database/utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/models/database/views.py` & `alphaz-0.7.5/alphaz/models/database/views.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/models/excel.py` & `alphaz-0.7.5/alphaz/models/excel.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/models/ftp.py` & `alphaz-0.7.5/alphaz/models/ftp.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,146 +1,209 @@
 from dataclasses import field
 import pysftp, ftplib, re
 from typing import List, Dict
 
 from core import core
 
-LOG = core.get_logger('ftp')
+LOG = core.get_logger("ftp")
 
-class AlphaFtpFile():
-    def __init__(self,name,parameters=None,origin=None):
-        self.name   = name
+
+class AlphaFtpFile:
+    def __init__(self, name, parameters=None, origin=None):
+        self.name = name
         self.origin = origin
-        self.size   = 0
+        self.size = 0
         self.key = None
         self.version = 0
         self.modification_time = None
         self.type = "classic"
 
         if parameters is not None:
-            self.size   = parameters.st_size
+            self.size = parameters.st_size
             self.modification_time = parameters.st_mtime
 
-        matchs = re.findall(r"\.[A-Z]*;[0-9]*",self.name)
+        matchs = re.findall(r"\.[A-Z]*;[0-9]*", self.name)
         if len(matchs):
-            self.extension, self.version = matchs[0].replace(".","").split(';')
-            self.type = 'vms'
-            self.short_name = self.name.replace(matchs[0],'')
+            self.extension, self.version = matchs[0].replace(".", "").split(";")
+            self.type = "vms"
+            self.short_name = self.name.replace(matchs[0], "")
         else:
-            self.extension = self.name.split('.')[-1]
-            self.short_name = self.name.replace('.' + self.extension,'')
-        #print (attr.filename,attr.st_uid, attr.st_gid, attr.st_mode,attr.st_mtime,attr.st_size)
-
-class AlphaFtp():
-    cnx     = None
-    valid   = False
-    sftp    = False
-    index   = 0
-
-    def __init__(self,host,user,password=None,port=22,key=None,key_pass=None,sftp=False,log=None):
+            self.extension = self.name.split(".")[-1]
+            self.short_name = self.name.replace("." + self.extension, "")
+        # print (attr.filename,attr.st_uid, attr.st_gid, attr.st_mode,attr.st_mtime,attr.st_size)
+
+
+class AlphaFtp:
+    cnx = None
+    valid = False
+    sftp = False
+    index = 0
+
+    def __init__(
+        self,
+        host,
+        user,
+        password=None,
+        port=22,
+        key=None,
+        key_pass=None,
+        sftp=False,
+        log=None,
+    ):
         self.cnopts = pysftp.CnOpts()
         self.cnopts.hostkeys = None
 
-        self.host       = host
-        self.port       = port
-        self.user       = user
-        self.key        = key
-        self.key_pass   = key_pass
-        self.password   = password
-        self.sftp       = sftp
-        self.files:list   = []
+        self.host = host
+        self.port = port
+        self.user = user
+        self.key = key
+        self.key_pass = key_pass
+        self.password = password
+        self.sftp = sftp
+        self.files: list = []
+
+        self.log = LOG if log is None else log
 
-        self.log     = LOG if log is None else log
-    
     def connect(self):
         if self.sftp:
             if self.key is None:
-                cnx = pysftp.Connection(self.host, port=self.port, username=self.user, password=self.password, cnopts=self.cnopts)
+                cnx = pysftp.Connection(
+                    self.host,
+                    port=self.port,
+                    username=self.user,
+                    password=self.password,
+                    cnopts=self.cnopts,
+                )
             else:
-                self.log.info(f"Connecting at {self.user}@{self.host}:{self.port} using key {self.key}")
-                cnx = pysftp.Connection(self.host, port=self.port, username=self.user, password=self.password, cnopts=self.cnopts, private_key=self.key,private_key_pass=self.key_pass)
+                self.log.info(
+                    f"Connecting at {self.user}@{self.host}:{self.port} using key {self.key}"
+                )
+                cnx = pysftp.Connection(
+                    self.host,
+                    port=self.port,
+                    username=self.user,
+                    password=self.password,
+                    cnopts=self.cnopts,
+                    private_key=self.key,
+                    private_key_pass=self.key_pass,
+                )
         else:
-            cnx = ftplib.FTP(host=self.host,user=self.user,passwd=self.password)
+            cnx = ftplib.FTP(host=self.host, user=self.user, passwd=self.password)
         self.cnx = cnx
         return cnx
-    
+
     def disconnect(self):
         if self.cnx is not None:
             self.cnx.close()
 
     def test_cnx(self):
         try:
             self.connect()
-            self.log.info("Connection test to %s is valid"%self.host)
+            self.log.info("Connection test to %s is valid" % self.host)
             self.valid = True
             self.disconnect()
         except Exception as ex:
-            self.log.info("Connection test to %s failed: %s"%(self.host,ex))
+            self.log.info("Connection test to %s failed: %s" % (self.host, ex))
             self.valid = False
         return self.valid
 
     def __enter__(self):
         self.connect()
         return self
 
     def __exit__(self, exc_type, exc_value, exc_traceback):
         self.disconnect()
 
         if exc_type:
-            print(f'exc_type: {exc_type}')
-            print(f'exc_value: {exc_value}')
-            print(f'exc_traceback: {exc_traceback}')
+            print(f"exc_type: {exc_type}")
+            print(f"exc_value: {exc_value}")
+            print(f"exc_traceback: {exc_traceback}")
 
-    def list_dir(self,directory,contain=None,origin=None) -> List[AlphaFtpFile]:
+    def list_dir(self, directory, contain=None, origin=None) -> List[AlphaFtpFile]:
         files = []
 
         # Switch to a remote directory
-        self.cnx.cwd(directory) #'/home/gollnwnw'
+        self.cnx.cwd(directory)  #'/home/gollnwnw'
 
         # Obtain structure of the remote directory '/var/www/vhosts'
         if self.sftp:
             for attr in self.cnx.listdir_attr():
                 if contain is None or contain in attr.filename:
-                    ftp_file = AlphaFtpFile(attr.filename,attr,origin=origin if origin is not None else directory)
+                    ftp_file = AlphaFtpFile(
+                        attr.filename,
+                        attr,
+                        origin=origin if origin is not None else directory,
+                    )
                     files.append(ftp_file)
-                    #print (attr.filename,attr.st_uid, attr.st_gid, attr.st_mode,attr.st_mtime,attr.st_size)
+                    # print (attr.filename,attr.st_uid, attr.st_gid, attr.st_mode,attr.st_mtime,attr.st_size)
         else:
             for attr in self.cnx.nlst():
                 if contain is None or contain in attr:
-                    files.append(AlphaFtpFile(attr,None))
+                    files.append(AlphaFtpFile(attr, None))
 
         if len(files) == 0 and self.log:
-            self.log.error('No files in directory %s'%directory)
+            self.log.error("No files in directory %s" % directory)
         return files
 
-    def upload(self,sourcepath,remotepath):
-        self.cnx.put(sourcepath,remotepath)
+    def upload(self, sourcepath, remotepath):
+        self.cnx.put(sourcepath, remotepath)
 
-    def download(self,remotepath:str,localpath:str):
+    def download(self, remotepath: str, localpath: str):
         try:
             if self.sftp:
                 self.cnx.get(remotepath, localpath, callback=None)
             else:
-                with open(localpath, 'wb') as f:
-                    self.cnx.retrbinary("RETR " + remotepath ,f.write)
-            self.log.info('File %s downloaded to %s'%(remotepath,localpath))
+                with open(localpath, "wb") as f:
+                    self.cnx.retrbinary("RETR " + remotepath, f.write)
+            self.log.info("File %s downloaded to %s" % (remotepath, localpath))
             return True
         except Exception as ex:
             self.log.error(ex)
             return False
 
-    def uploads(self,files_list):
+    def uploads(self, files_list):
         for file_dict in files_list:
-            self.cnx.put(file_dict['sourcepath'],file_dict['remotepath'])
+            self.cnx.put(file_dict["sourcepath"], file_dict["remotepath"])
 
-    def makedirs(self,remote_directory):
+    def makedirs(self, remote_directory):
         self.cnx.makedirs(remote_directory)
 
-    def set_line(self,txt):
-        if not ';' in txt: return
+    def set_line(self, txt):
+        if not ";" in txt:
+            return
         try:
-            name        = txt.split()[0]
-            ftp_file    = AlphaFtpFile(name)
+            name = txt.split()[0]
+            ftp_file = AlphaFtpFile(name)
             self.files.append(ftp_file)
             self.index += 1
         except Exception as ex:
-            if self.log: self.log.error(ex)
+            if self.log:
+                self.log.error(ex)
+
+    def write_file(
+        self, file_name: str, content: str, remote_directory: str = None
+    ) -> bool:
+        if remote_directory is not None and not self.is_dir(remote_directory):
+            print(f"Go to {remote_directory}")
+            self.cnx.cwd(remote_directory)
+        with self.cnx.open(file_name, "w") as f:
+            f.write(content)
+        return True
+
+    def read_file(self, file_name: str, remote_directory: str = None) -> str:
+        if remote_directory is not None and not self.is_dir(remote_directory):
+            print(f"Go to {remote_directory}")
+            self.cnx.cwd(remote_directory)
+        with self.cnx.open(file_name, "r") as f:
+            return f.read()
+        return None
+
+    def is_dir(self, remote_directory: str):
+        current_cwd = self.cnx.pwd.lower()
+        remote_directory = (
+            remote_directory.lower()
+            .replace(":[", "/")
+            .replace(".", "/")
+            .replace("]", "")
+        )
+        print(f"CWD {current_cwd=} {remote_directory=}")
+        return current_cwd == remote_directory
```

### Comparing `alphaz-0.7.4.1/alphaz/models/json/_converters.py` & `alphaz-0.7.5/alphaz/models/json/_converters.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/models/logger/_colorations.py` & `alphaz-0.7.5/alphaz/models/logger/_colorations.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/models/logger/_logger.py` & `alphaz-0.7.5/alphaz/models/logger/_logger.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/models/logger/_utils.py` & `alphaz-0.7.5/alphaz/models/logger/_utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/models/logs/main.log` & `alphaz-0.7.5/alphaz/models/logs/main.log`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/models/main/_base.py` & `alphaz-0.7.5/alphaz/models/main/_base.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/models/main/_core/_core.py` & `alphaz-0.7.5/alphaz/models/main/_core/_core.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/models/main/_exception.py` & `alphaz-0.7.5/alphaz/models/main/_exception.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/models/main/_request.py` & `alphaz-0.7.5/alphaz/models/main/_request.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/models/main/_singleton.py` & `alphaz-0.7.5/alphaz/models/main/_singleton.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/models/request.py` & `alphaz-0.7.5/alphaz/models/request.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/models/tests/_category.py` & `alphaz-0.7.5/alphaz/models/tests/_category.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/models/tests/_group.py` & `alphaz-0.7.5/alphaz/models/tests/_group.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/models/tests/_method.py` & `alphaz-0.7.5/alphaz/models/tests/_method.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/models/tests/_save.py` & `alphaz-0.7.5/alphaz/models/tests/_save.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/models/tests/_test.py` & `alphaz-0.7.5/alphaz/models/tests/_test.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/models/tests/_wrappers.py` & `alphaz-0.7.5/alphaz/models/tests/_wrappers.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,14 +89,16 @@
 
     Returns:
         A wrapper function which performs pre- and post-processing before and after running the test function.
     """
 
     def test_alpha_in(func: Callable) -> Callable:
         def test_wrapper(*args, **kwargs):
+            if len(args) == 0:
+                return
             TestClass: AlphaTest = args[0]
             TestClass.output = None
 
             logged_output = None
             if admin_user_id is not None or admin_user_name is not None:
                 logged_output = try_su_login(
                     admin_user_id if admin_user_id is not None else admin_user_name
```

### Comparing `alphaz-0.7.4.1/alphaz/models/user.py` & `alphaz-0.7.5/alphaz/models/user.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/models/watcher.py` & `alphaz-0.7.5/alphaz/models/watcher.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/pocs/main.py` & `alphaz-0.7.5/alphaz/pocs/main.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/run.py` & `alphaz-0.7.5/alphaz/run.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/src/alpha.png` & `alphaz-0.7.5/alphaz/src/alpha.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/src/configs/loggers.json` & `alphaz-0.7.5/alphaz/src/configs/loggers.json`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/stitch/Core.py` & `alphaz-0.7.5/alphaz/stitch/Core.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/stitch/stitch.py` & `alphaz-0.7.5/alphaz/stitch/stitch.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/stitch/web-drivers/chromedriver.exe` & `alphaz-0.7.5/alphaz/stitch/web-drivers/chromedriver.exe`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/stitch/web-drivers/geckodriver` & `alphaz-0.7.5/alphaz/stitch/web-drivers/geckodriver`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/templates/assets/css/home.css` & `alphaz-0.7.5/alphaz/templates/assets/css/home.css`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/templates/assets/css/logs.css` & `alphaz-0.7.5/alphaz/templates/assets/css/logs.css`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/templates/assets/images/icons/alpha.png` & `alphaz-0.7.5/alphaz/templates/assets/images/icons/alpha.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/templates/assets/images/icons/start-icon.png` & `alphaz-0.7.5/alphaz/templates/assets/images/icons/start-icon.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/templates/assets/images/icons/wsalpha.png` & `alphaz-0.7.5/alphaz/templates/assets/images/icons/wsalpha.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/templates/assets/images/loading.gif` & `alphaz-0.7.5/alphaz/templates/assets/images/loading.gif`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/templates/assets/js/libs/ansi_up.js` & `alphaz-0.7.5/alphaz/templates/assets/js/libs/ansi_up.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/templates/assets/js/libs/jquery.min.js` & `alphaz-0.7.5/alphaz/templates/assets/js/libs/jquery.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/templates/assets/js/logs.js` & `alphaz-0.7.5/alphaz/templates/assets/js/logs.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/templates/home.html` & `alphaz-0.7.5/alphaz/templates/home.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/templates/logs.html` & `alphaz-0.7.5/alphaz/templates/logs.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/test.py` & `alphaz-0.7.5/alphaz/test.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/tests/api.py` & `alphaz-0.7.5/alphaz/tests/api.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/tests/basic_test.py` & `alphaz-0.7.5/alphaz/tests/basic_test.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/tests/configurations.py` & `alphaz-0.7.5/alphaz/tests/configurations.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/tests/database.py` & `alphaz-0.7.5/alphaz/tests/database.py`

 * *Files 7% similar despite different names*

```diff
@@ -293,21 +293,81 @@
         rows = self.db.select(Test)
         if len(rows) == 0:
             return False
         values = {x: getattr(rows[0], x) for x in self.parameters}
         return len(rows) == 1 and values == self.parameters
 
     @test(save=False)
+    def roolback(self):
+        Test.query.delete()
+        Test.query.session.commit()
+        rows = self.db.select(Test)
+        if len(rows) != 0:
+            return False
+
+        test = self.db.add(Test, self.parameters, commit=False, rollback=False)
+        rows = self.db.select(Test)
+        if len(rows) != 1:
+            return False
+        self.db.rollback(session=test.query.session)
+
+        # self.db.rollback()
+        rows = self.db.select(Test)
+
+        return len(rows) == 0
+
+    @test(save=False)
+    def roolback_update(self):
+        Test.query.delete()
+        Test.query.session.commit()
+        rows = self.db.select(Test)
+        if len(rows) != 0:
+            return False
+
+        test = self.db.add(Test, self.parameters, commit=True, rollback=False)
+
+        new_parameters = {x: y for x, y in self.parameters.items()}
+        new_parameters[Test.number.key] = 13
+        self.db.update(test, new_parameters, commit=False)
+        self.db.rollback(session=test.query.session)
+
+        rows = self.db.select(Test)
+        if len(rows) != 1:
+            return False
+        return new_parameters == rows[0]
+
+    @test(save=False)
+    def roolback_update_2(self):
+        Test.query.delete()
+        Test.query.session.commit()
+        rows = self.db.select(Test)
+        if len(rows) != 0:
+            return False
+
+        test = self.db.add(Test, self.parameters, commit=True, rollback=False)
+
+        new_parameters = {Test.number.key: 13}
+        self.db.update(
+            test, new_parameters, filters=[Test.name == "insert"], commit=False
+        )
+        self.db.rollback(session=test.query.session)
+
+        rows = self.db.select(Test)
+        if len(rows) != 1:
+            return False
+        return new_parameters == rows[0]
+
+    @test(save=False)
     def insert2(self):
         Test.query.delete()
         self.db.add(
             Test,
             {
                 Test.name: self.parameters[Test.name.key],
-                Test.number_: self.parameters[Test.number_.key],
+                Test.number: self.parameters[Test.number.key],
                 Test.text_: self.parameters[Test.text_.key],
                 Test.date_: self.parameters[Test.date_.key],
             },
         )
         rows = self.db.select(Test)
         if len(rows) == 0:
             return False
@@ -380,67 +440,93 @@
         return rows[0] == self.parameters[Test.name.key]
 
     @test(save=False)
     def add_update(self):
         Test.query.delete()
         self.db.add(Test, self.parameters)
         parameters = {x: y for x, y in self.parameters.items()}
-        parameters[Test.number_.key] += 1
+        parameters[Test.number.key] += 1
         self.db.add(Test, parameters=parameters, update=True)
         rows = self.db.select(Test)
         return len(rows) == 1 and parameters == {
             x: getattr(rows[0], x) for x in self.parameters
         }
 
     @test(save=False)
     def add_or_update(self):
         Test.query.delete()
         self.db.add(Test, self.parameters)
         parameters = {x: y for x, y in self.parameters.items()}
-        parameters[Test.number_.key] += 1
+        parameters[Test.number.key] += 1
         test2 = Test(**parameters)
         self.db.add_or_update(test2)
         rows = self.db.select(Test)
         return len(rows) == 1 and parameters == {
             x: getattr(rows[0], x) for x in self.parameters
         }
 
     @test(save=False)
     def update_with_values(self):
         Test.query.delete()
-        self.db.add(Test, self.parameters)
+        add = self.db.add(Test, self.parameters)
         parameters = {x: y for x, y in self.parameters.items()}
-        parameters[Test.number_.key] += 1
+        parameters[Test.number.key] += 1
+        parameters[Test.id.key] = add.id
         self.db.update(Test, values=parameters)
         rows = self.db.select(Test)
         return len(rows) == 1 and parameters == {
             x: getattr(rows[0], x) for x in self.parameters
         }
 
     @test(save=False, begin=delete)
     def update_with_model(self):
+        added = self.db.add(Test, self.parameters)
+        parameters = {x: y for x, y in self.parameters.items()}
+        parameters[Test.number.key] += 1
+        parameters[Test.id.key] = added.id
+        test = Test(**parameters)
+        test.query.session.commit()
+        # updated = self.db.update(Test(**parameters))
+        rows = self.db.select(Test)
+        return len(rows) == 1 and parameters == {
+            x: getattr(rows[0], x) for x in parameters
+        }
 
+    @test(save=False, begin=delete)
+    def update_with_model_update(self):
         added = self.db.add(Test, self.parameters)
         parameters = {x: y for x, y in self.parameters.items()}
-        parameters[Test.number_.key] += 1
+        parameters[Test.number.key] += 1
         parameters[Test.id.key] = added.id
-        updated = self.db.update(Test(**parameters))
+        test = Test(**parameters)
+        # test.query.session.commit()
+        updated = self.db.update(test)
+        rows = self.db.select(Test)
+        return len(rows) == 1 and parameters == {
+            x: getattr(rows[0], x) for x in parameters
+        }
+
+    @test(save=False, begin=delete)
+    def update_with_transient_model(self):
+        added = self.db.add(Test, self.parameters, commit=False)
+        added.number += 1
+        updated = self.db.update(added)
         rows = self.db.select(Test)
         return len(rows) == 1 and parameters == {
             x: getattr(rows[0], x) for x in parameters
         }
 
     @test(save=False)
     def update_last_with_model(self):
         Test.query.delete()
         added = self.db.add(Test, self.parameters)
         parameters_added = []
         for i in range(4):
             parameters = {x: y for x, y in self.parameters.items()}
-            parameters[Test.number_.key] += i + 1
+            parameters[Test.number.key] += i + 1
             parameters[Test.id.key] = added.id
             updated = self.db.update(Test(**parameters))
             parameters_added.append({**parameters})
         rows = self.db.select(Test)
         return len(rows) == 1 and parameters == {
             x: getattr(rows[0], x) for x in parameters
         }
@@ -448,21 +534,21 @@
     @test(save=False)
     def update_multiple_with_model(self):
         Test.query.delete()
 
         parameters_list = []
         for i in range(4):
             parameters = {x: y for x, y in self.parameters.items()}
-            parameters[Test.number_.key] = i
+            parameters[Test.number.key] = i
             added = self.db.add(Test, parameters)
             parameters[Test.id.key] = added.id
             parameters_list.append({**parameters})
 
         for i in range(4):
-            parameters_list[i][Test.number_.key] += 1
+            parameters_list[i][Test.number.key] += 1
             updated = self.db.update(Test(**parameters_list[i]))
 
         rows = self.db.select(Test)
         db_parameters_list = [
             {x: getattr(row, x) for x in parameters_list[i]}
             for i, row in enumerate(rows)
         ]
@@ -483,15 +569,15 @@
 
     @test(save=False)
     def add_or_update_multiple(self):
         Test.query.delete()
         tests = [Test(**self.parameters)]
         for i in range(5):
             parameters = {x: y for x, y in self.parameters.items()}
-            parameters[Test.number_.key] += i
+            parameters[Test.number.key] += i
             tests.append(Test(**parameters))
         tests.append(Test(**self.parameters))
         self.db.add_or_update(tests)
         rows = self.db.select(Test)
         return len(rows) == 1 and self.parameters == {
             x: getattr(rows[0], x) for x in self.parameters
         }
@@ -499,29 +585,29 @@
     @test(save=False)
     def add_or_update_multiple2(self):
         # take the first insert
         Test.query.delete()
         tests = [Test(**self.parameters)]
         for i in range(5):
             parameters = {x: y for x, y in self.parameters.items()}
-            parameters[Test.number_.key] += i
+            parameters[Test.number.key] += i
             tests.append(Test(**parameters))
         self.db.add_or_update(tests)
         rows = self.db.select(Test)
         return len(rows) == 1 and self.parameters == {
             x: getattr(rows[0], x) for x in self.parameters
         }
 
     @test(save=False)
     def add_or_update_multiple3(self):
         Test.query.delete()
         tests = [Test(**self.parameters)]
         for i in range(5):
             parameters = {x: y for x, y in self.parameters.items()}
-            parameters[Test.number_.key] += i
+            parameters[Test.number.key] += i
             tests.append(Test(**parameters))
         parameters2 = {x: y for x, y in self.parameters.items()}
         parameters2[Test.name.key] = "new"
         tests.append(Test(**parameters2))
         self.db.add_or_update(tests)
         rows = self.db.select(Test)
         return len(rows) == 2 and self.parameters == {
@@ -534,73 +620,73 @@
 
         rows = self.db.select(Test)
         self.assert_is_empty(rows)
 
         tests = [Test(**self.parameters)]
         for i in range(5):
             parameters = {x: y for x, y in self.parameters.items()}
-            parameters[Test.number_.key] += i
+            parameters[Test.number.key] += i
             tests.append(Test(**parameters))
         self.db.add_or_update(tests)
-        numbers = self.db.select(Test, unique=Test.number_)
+        numbers = self.db.select(Test, unique=Test.number)
         self.assert_length(numbers, 5)
         self.assert_equal(set(numbers), set([12, 13, 14, 15, 16]))
 
         rows = self.db.select(Test)
         update_data = []
         for i, row in enumerate(rows):
             p = row.to_json()
-            p[Test.number_.key] = 0
+            p[Test.number.key] = 0
             p[Test.update_date.key] = datetime.datetime.now()
             p[Test.date_.key] = datetime.datetime.strptime(
                 p[Test.date_.key], "%Y-%m-%dT%H:%M:%S"
             )
             update_data.append(p)
 
         self.db.session.bulk_update_mappings(Test, update_data)
         self.db.session.commit()
 
-        numbers = self.db.select(Test, unique=Test.number_)
+        numbers = self.db.select(Test, unique=Test.number)
         self.assert_length(numbers, 1)
         self.assert_equal(set(numbers), set([0]))
 
     @test()
     def bulk_update_2(self):
         Test.query.delete()
 
         rows = self.db.select(Test)
         self.assert_is_empty(rows)
 
         tests = [Test(**self.parameters)]
         for i in range(5):
             parameters = {x: y for x, y in self.parameters.items()}
-            parameters[Test.number_.key] += i
+            parameters[Test.number.key] += i
             tests.append(Test(**parameters))
         self.db.add_or_update(tests)
-        numbers = self.db.select(Test, unique=Test.number_)
+        numbers = self.db.select(Test, unique=Test.number)
         self.assert_length(numbers, 5)
         self.assert_equal(set(numbers), set([12, 13, 14, 15, 16]))
 
         rows = self.db.select(Test)
         for i, row in enumerate(rows):
-            row.number_ = 0
+            row.number = 0
 
         self.db.session.commit()
 
-        numbers = self.db.select(Test, unique=Test.number_)
+        numbers = self.db.select(Test, unique=Test.number)
         self.assert_length(numbers, 1)
         self.assert_equal(set(numbers), set([0]))
 
     """@test(save=False)
     def upsert(self):
         Test.query.delete()
         test = Test(**self.parameters)
         self.db.add(test)
         parameters = {x:y for x,y in self.parameters.items()}
-        parameters[Test.number_.key] += 1
+        parameters[Test.number.key] += 1
         test2 = Test(**self.parameters)
         self.db.upsert(Test,test2)
         rows    = self.db.select(Test)
         return len(rows) == 1 and parameters == {x:getattr(rows[0],x) for x in self.parameters}"""
 
     @test(save=False)
     def update_none(self):
@@ -616,33 +702,33 @@
 
     @test()
     def name(self):
         Test.query.delete()
         tests = [Test(**self.parameters)]
         for i in range(5):
             parameters = {x: y for x, y in self.parameters.items()}
-            parameters[Test.number_.key] = i
+            parameters[Test.number.key] = i
             parameters[Test.date_.key] = date_lib.str_to_datetime(
                 "2020/01/%s 10:02:03" % (i + 1)
             )
             tests.append(Test(**parameters))
         self.db.add_or_update(tests)
 
         tests = self.db.select(
             Test,
             name=[
-                {Test.number_: {Operators.IN: 1}},
+                {Test.number: {Operators.IN: 1}},
             ],
         )
         self.assert_length(tests, 1)
 
         tests = self.db.select(
             Test,
             name=[
-                {Test.number_: {Operators.IN: [1, 100]}},
+                {Test.number: {Operators.IN: [1, 100]}},
             ],
         )
         self.assert_length(tests, 1)
 
         tests = self.db.select(
             Test,
             name=[
```

### Comparing `alphaz-0.7.4.1/alphaz/tests/utils.py` & `alphaz-0.7.5/alphaz/tests/utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/utils/api.py` & `alphaz-0.7.5/alphaz/utils/api.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/utils/configuration.py` & `alphaz-0.7.5/alphaz/utils/configuration.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/utils/database_to_dataclass.py` & `alphaz-0.7.5/alphaz/utils/database_to_dataclass.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/utils/decorators.py` & `alphaz-0.7.5/alphaz/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/utils/ensure.py` & `alphaz-0.7.5/alphaz/utils/ensure.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/utils/mep.py` & `alphaz-0.7.5/alphaz/utils/mep.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/utils/screens.py` & `alphaz-0.7.5/alphaz/utils/screens.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/utils/selectionMenu.py` & `alphaz-0.7.5/alphaz/utils/selectionMenu.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/utils/tasks.py` & `alphaz-0.7.5/alphaz/utils/tasks.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/utils/tests.py` & `alphaz-0.7.5/alphaz/utils/tests.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/utils/time.py` & `alphaz-0.7.5/alphaz/utils/time.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz/utils/transactions.py` & `alphaz-0.7.5/alphaz/utils/transactions.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.4.1/alphaz.egg-info/PKG-INFO` & `alphaz-0.7.5/alphaz.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: alphaz
-Version: 0.7.4.1
+Version: 0.7.5
 Summary: A package full of very nice tools
 Home-page: https://github.com/ZAurele/alphaz
 Author: Aurèle
 Author-email: contact@aurele.eu
 License: MIT
-Download-URL: https://github.com/ZAurele/alphaz/archive/refs/tags/0.7.4.1.tar.gz
+Download-URL: https://github.com/ZAurele/alphaz/archive/refs/tags/0.7.5.tar.gz
 Description: UNKNOWN
 Keywords: Flask,Json
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `alphaz-0.7.4.1/alphaz.egg-info/SOURCES.txt` & `alphaz-0.7.5/alphaz.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -300,8 +300,9 @@
 alphaz/utils/ensure.py
 alphaz/utils/mep.py
 alphaz/utils/screens.py
 alphaz/utils/selectionMenu.py
 alphaz/utils/tasks.py
 alphaz/utils/tests.py
 alphaz/utils/time.py
-alphaz/utils/transactions.py
+alphaz/utils/transactions.py
+alphaz/utils/database/init.py
```

### Comparing `alphaz-0.7.4.1/setup.py` & `alphaz-0.7.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os, glob, re
 from datetime import date
 
 today = date.today()
 
 from setuptools import setup, find_packages
 
-version = "0.7.4.1"
+version = "0.7.5"
 
 excludes = [".git", ".vscode"]
 
 archives = glob.glob("dist/*")
 for archive in archives:
     os.remove(archive)
```

