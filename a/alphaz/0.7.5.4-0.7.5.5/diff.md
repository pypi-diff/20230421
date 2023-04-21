# Comparing `tmp/alphaz-0.7.5.4.tar.gz` & `tmp/alphaz-0.7.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alphaz-0.7.5.4.tar", last modified: Fri Apr 21 16:00:30 2023, max compression
+gzip compressed data, was "dist/alphaz-0.7.5.5.tar", last modified: Fri Apr 21 17:50:44 2023, max compression
```

## Comparing `alphaz-0.7.5.4.tar` & `alphaz-0.7.5.5.tar`

### file list

```diff
@@ -1,394 +1,394 @@
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.587209 alphaz-0.7.5.4/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    11211 2023-04-21 16:00:30.000000 alphaz-0.7.5.4/MANIFEST.in
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      589 2023-04-21 16:00:30.587209 alphaz-0.7.5.4/PKG-INFO
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1348 2021-07-12 18:07:51.000000 alphaz-0.7.5.4/README.md
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.535209 alphaz-0.7.5.4/alphaz/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        9 2023-04-18 09:00:04.000000 alphaz-0.7.5.4/alphaz/README.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      333 2023-04-13 12:43:58.000000 alphaz-0.7.5.4/alphaz/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      104 2021-03-29 08:42:45.000000 alphaz-0.7.5.4/alphaz/alphaz.bat
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       70 2021-03-29 08:42:45.000000 alphaz-0.7.5.4/alphaz/alphaz.code-workspace
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      208 2022-04-19 08:43:27.000000 alphaz-0.7.5.4/alphaz/alphaz.sh
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       48 2021-03-29 08:42:45.000000 alphaz-0.7.5.4/alphaz/api.bat
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      713 2023-04-18 09:00:04.000000 alphaz-0.7.5.4/alphaz/api.json
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      770 2022-04-13 09:59:51.000000 alphaz-0.7.5.4/alphaz/api.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.535209 alphaz-0.7.5.4/alphaz/apis/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.5.4/alphaz/apis/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2022-07-21 11:35:27.000000 alphaz-0.7.5.4/alphaz/apis/log.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2721 2023-03-17 07:06:42.000000 alphaz-0.7.5.4/alphaz/apis/mails.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.535209 alphaz-0.7.5.4/alphaz/apis/routes/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.5.4/alphaz/apis/routes/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1577 2023-02-23 09:08:35.000000 alphaz-0.7.5.4/alphaz/apis/routes/admin.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1137 2021-03-29 08:42:45.000000 alphaz-0.7.5.4/alphaz/apis/routes/api.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3062 2023-02-23 09:08:35.000000 alphaz-0.7.5.4/alphaz/apis/routes/basic_tests.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3094 2023-04-18 09:00:04.000000 alphaz-0.7.5.4/alphaz/apis/routes/database.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      413 2022-04-12 11:53:03.000000 alphaz-0.7.5.4/alphaz/apis/routes/git.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     7225 2023-02-01 13:59:24.000000 alphaz-0.7.5.4/alphaz/apis/routes/logs.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1810 2022-04-12 11:53:03.000000 alphaz-0.7.5.4/alphaz/apis/routes/mails.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6390 2023-04-21 07:47:57.000000 alphaz-0.7.5.4/alphaz/apis/routes/main.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1330 2023-02-23 09:08:35.000000 alphaz-0.7.5.4/alphaz/apis/routes/tests.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.535209 alphaz-0.7.5.4/alphaz/apis/routes/user_management/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      114 2022-04-27 13:24:50.000000 alphaz-0.7.5.4/alphaz/apis/routes/user_management/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2475 2022-05-09 13:31:06.000000 alphaz-0.7.5.4/alphaz/apis/routes/user_management/application_management.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2228 2022-05-09 13:31:06.000000 alphaz-0.7.5.4/alphaz/apis/routes/user_management/permission_management.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4058 2022-08-31 08:56:44.000000 alphaz-0.7.5.4/alphaz/apis/routes/user_management/role_management.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1291 2022-08-31 08:56:44.000000 alphaz-0.7.5.4/alphaz/apis/routes/user_management/user_management.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3324 2023-04-21 07:47:57.000000 alphaz-0.7.5.4/alphaz/apis/routes/users.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      584 2023-02-23 09:08:35.000000 alphaz-0.7.5.4/alphaz/apis/tests.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.535209 alphaz-0.7.5.4/alphaz/apis/users/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2022-07-21 11:35:27.000000 alphaz-0.7.5.4/alphaz/apis/users/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2718 2023-01-25 21:39:07.000000 alphaz-0.7.5.4/alphaz/apis/users/ldap.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    11543 2023-03-28 08:47:21.000000 alphaz-0.7.5.4/alphaz/apis/users/users.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.539209 alphaz-0.7.5.4/alphaz/config/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.5.4/alphaz/config/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      795 2021-03-29 08:42:45.000000 alphaz-0.7.5.4/alphaz/config/config.css
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    12602 2021-03-29 08:42:45.000000 alphaz-0.7.5.4/alphaz/config/config.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      707 2022-08-11 06:44:17.000000 alphaz-0.7.5.4/alphaz/config/main_configuration.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      823 2021-03-29 08:42:45.000000 alphaz-0.7.5.4/alphaz/config/page.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1700 2021-03-29 08:42:45.000000 alphaz-0.7.5.4/alphaz/config/source.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1564 2021-03-29 08:42:45.000000 alphaz-0.7.5.4/alphaz/config.json
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      238 2023-01-06 09:14:28.000000 alphaz-0.7.5.4/alphaz/core.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.539209 alphaz-0.7.5.4/alphaz/documentations/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.539209 alphaz-0.7.5.4/alphaz/documentations/docs/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2022-07-21 11:35:27.000000 alphaz-0.7.5.4/alphaz/documentations/docs/alpha_admin.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1408 2023-04-12 11:28:51.000000 alphaz-0.7.5.4/alphaz/documentations/docs/alpha_core.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2595 2022-07-21 11:35:27.000000 alphaz-0.7.5.4/alphaz/documentations/docs/alpha_screens.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2222 2023-04-12 11:28:51.000000 alphaz-0.7.5.4/alphaz/documentations/docs/alpha_setup.md
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.539209 alphaz-0.7.5.4/alphaz/documentations/docs/api/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1527 2023-04-18 09:00:04.000000 alphaz-0.7.5.4/alphaz/documentations/docs/api/authorizations.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       72 2023-04-18 09:00:04.000000 alphaz-0.7.5.4/alphaz/documentations/docs/api/cache.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2932 2023-04-18 09:00:04.000000 alphaz-0.7.5.4/alphaz/documentations/docs/api/configuration.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       24 2023-04-18 09:00:04.000000 alphaz-0.7.5.4/alphaz/documentations/docs/api/issues.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      705 2023-04-18 09:00:04.000000 alphaz-0.7.5.4/alphaz/documentations/docs/api/main.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      559 2023-04-18 09:00:04.000000 alphaz-0.7.5.4/alphaz/documentations/docs/api/methods.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1728 2023-04-18 09:00:04.000000 alphaz-0.7.5.4/alphaz/documentations/docs/api/parameters.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1197 2023-04-18 09:00:04.000000 alphaz-0.7.5.4/alphaz/documentations/docs/api/routes.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      486 2023-04-18 09:00:04.000000 alphaz-0.7.5.4/alphaz/documentations/docs/api/sqlalchemy.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1129 2023-04-18 09:00:04.000000 alphaz-0.7.5.4/alphaz/documentations/docs/api_database.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2520 2023-01-06 09:14:28.000000 alphaz-0.7.5.4/alphaz/documentations/docs/configuration.md
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.539209 alphaz-0.7.5.4/alphaz/documentations/docs/database/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2187 2023-04-18 09:00:04.000000 alphaz-0.7.5.4/alphaz/documentations/docs/database/init.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      442 2023-04-18 09:00:04.000000 alphaz-0.7.5.4/alphaz/documentations/docs/database/instantiate.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      113 2023-04-18 09:00:04.000000 alphaz-0.7.5.4/alphaz/documentations/docs/database/main.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1806 2023-04-18 09:00:04.000000 alphaz-0.7.5.4/alphaz/documentations/docs/database/model.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      373 2023-04-18 09:00:04.000000 alphaz-0.7.5.4/alphaz/documentations/docs/database/relations.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1087 2023-04-18 09:00:04.000000 alphaz-0.7.5.4/alphaz/documentations/docs/database/schema.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      615 2023-04-18 09:00:04.000000 alphaz-0.7.5.4/alphaz/documentations/docs/database/update.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      357 2021-04-14 08:59:25.000000 alphaz-0.7.5.4/alphaz/documentations/docs/documentation.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3526 2023-04-12 11:28:51.000000 alphaz-0.7.5.4/alphaz/documentations/docs/index.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1090 2023-04-18 09:00:04.000000 alphaz-0.7.5.4/alphaz/documentations/mkdocs.yml
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.539209 alphaz-0.7.5.4/alphaz/documentations/site/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    13156 2023-04-21 16:00:29.000000 alphaz-0.7.5.4/alphaz/documentations/site/404.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.539209 alphaz-0.7.5.4/alphaz/documentations/site/alpha_admin/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    14222 2023-04-21 16:00:29.000000 alphaz-0.7.5.4/alphaz/documentations/site/alpha_admin/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.543209 alphaz-0.7.5.4/alphaz/documentations/site/alpha_core/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    22752 2023-04-21 16:00:29.000000 alphaz-0.7.5.4/alphaz/documentations/site/alpha_core/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.543209 alphaz-0.7.5.4/alphaz/documentations/site/alpha_screens/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    21873 2023-04-21 16:00:29.000000 alphaz-0.7.5.4/alphaz/documentations/site/alpha_screens/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.543209 alphaz-0.7.5.4/alphaz/documentations/site/alpha_setup/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    24071 2023-04-21 16:00:29.000000 alphaz-0.7.5.4/alphaz/documentations/site/alpha_setup/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.527209 alphaz-0.7.5.4/alphaz/documentations/site/api/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.543209 alphaz-0.7.5.4/alphaz/documentations/site/api/authorizations/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    17905 2023-04-21 16:00:29.000000 alphaz-0.7.5.4/alphaz/documentations/site/api/authorizations/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.543209 alphaz-0.7.5.4/alphaz/documentations/site/api/cache/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    14918 2023-04-21 16:00:29.000000 alphaz-0.7.5.4/alphaz/documentations/site/api/cache/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.543209 alphaz-0.7.5.4/alphaz/documentations/site/api/configuration/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    27646 2023-04-21 16:00:29.000000 alphaz-0.7.5.4/alphaz/documentations/site/api/configuration/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.543209 alphaz-0.7.5.4/alphaz/documentations/site/api/issues/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    16365 2023-04-21 16:00:29.000000 alphaz-0.7.5.4/alphaz/documentations/site/api/issues/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.543209 alphaz-0.7.5.4/alphaz/documentations/site/api/main/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    17987 2023-04-21 16:00:29.000000 alphaz-0.7.5.4/alphaz/documentations/site/api/main/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.543209 alphaz-0.7.5.4/alphaz/documentations/site/api/methods/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    17722 2023-04-21 16:00:29.000000 alphaz-0.7.5.4/alphaz/documentations/site/api/methods/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.543209 alphaz-0.7.5.4/alphaz/documentations/site/api/parameters/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    20075 2023-04-21 16:00:29.000000 alphaz-0.7.5.4/alphaz/documentations/site/api/parameters/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.543209 alphaz-0.7.5.4/alphaz/documentations/site/api/routes/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    19333 2023-04-21 16:00:29.000000 alphaz-0.7.5.4/alphaz/documentations/site/api/routes/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.543209 alphaz-0.7.5.4/alphaz/documentations/site/api/sqlalchemy/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    17109 2023-04-21 16:00:29.000000 alphaz-0.7.5.4/alphaz/documentations/site/api/sqlalchemy/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.543209 alphaz-0.7.5.4/alphaz/documentations/site/api_database/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    22959 2023-04-21 16:00:29.000000 alphaz-0.7.5.4/alphaz/documentations/site/api_database/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.527209 alphaz-0.7.5.4/alphaz/documentations/site/assets/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.543209 alphaz-0.7.5.4/alphaz/documentations/site/assets/images/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1870 2023-04-21 16:00:29.000000 alphaz-0.7.5.4/alphaz/documentations/site/assets/images/favicon.png
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.543209 alphaz-0.7.5.4/alphaz/documentations/site/assets/javascripts/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    79520 2023-04-21 16:00:29.000000 alphaz-0.7.5.4/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)   384391 2023-04-21 16:00:29.000000 alphaz-0.7.5.4/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js.map
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.543209 alphaz-0.7.5.4/alphaz/documentations/site/assets/javascripts/lunr/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.547209 alphaz-0.7.5.4/alphaz/documentations/site/assets/javascripts/lunr/min/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    17058 2023-04-21 16:00:29.000000 alphaz-0.7.5.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ar.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4654 2023-04-21 16:00:29.000000 alphaz-0.7.5.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.da.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6119 2023-04-21 16:00:29.000000 alphaz-0.7.5.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.de.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6208 2023-04-21 16:00:29.000000 alphaz-0.7.5.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.du.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    11499 2023-04-21 16:00:29.000000 alphaz-0.7.5.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.es.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     9342 2023-04-21 16:00:29.000000 alphaz-0.7.5.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fi.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    10669 2023-04-21 16:00:29.000000 alphaz-0.7.5.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fr.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     9437 2023-04-21 16:00:29.000000 alphaz-0.7.5.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.hu.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    11232 2023-04-21 16:00:29.000000 alphaz-0.7.5.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.it.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2313 2023-04-21 16:00:29.000000 alphaz-0.7.5.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ja.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       36 2023-04-21 16:00:29.000000 alphaz-0.7.5.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.jp.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      817 2023-04-21 16:00:29.000000 alphaz-0.7.5.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.multi.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6026 2023-04-21 16:00:29.000000 alphaz-0.7.5.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.nl.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4754 2023-04-21 16:00:29.000000 alphaz-0.7.5.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.no.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    10171 2023-04-21 16:00:29.000000 alphaz-0.7.5.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.pt.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    10958 2023-04-21 16:00:29.000000 alphaz-0.7.5.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ro.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    10331 2023-04-21 16:00:29.000000 alphaz-0.7.5.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ru.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3647 2023-04-21 16:00:29.000000 alphaz-0.7.5.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4523 2023-04-21 16:00:29.000000 alphaz-0.7.5.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.sv.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    15009 2023-04-21 16:00:29.000000 alphaz-0.7.5.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.tr.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      784 2023-04-21 16:00:29.000000 alphaz-0.7.5.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.vi.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    22878 2023-04-21 16:00:29.000000 alphaz-0.7.5.4/alphaz/documentations/site/assets/javascripts/lunr/tinyseg.js
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.547209 alphaz-0.7.5.4/alphaz/documentations/site/assets/javascripts/workers/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    34936 2023-04-21 16:00:29.000000 alphaz-0.7.5.4/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)   167496 2023-04-21 16:00:29.000000 alphaz-0.7.5.4/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js.map
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.547209 alphaz-0.7.5.4/alphaz/documentations/site/assets/stylesheets/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    87332 2023-04-21 16:00:29.000000 alphaz-0.7.5.4/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css
--rw-rw-r--   0 aurele    (1000) aurele    (1000)   319950 2023-04-21 16:00:29.000000 alphaz-0.7.5.4/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css.map
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    10915 2023-04-21 16:00:29.000000 alphaz-0.7.5.4/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    37512 2023-04-21 16:00:29.000000 alphaz-0.7.5.4/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css.map
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.547209 alphaz-0.7.5.4/alphaz/documentations/site/configuration/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    28465 2023-04-21 16:00:29.000000 alphaz-0.7.5.4/alphaz/documentations/site/configuration/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.527209 alphaz-0.7.5.4/alphaz/documentations/site/database/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.547209 alphaz-0.7.5.4/alphaz/documentations/site/database/init/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    23027 2023-04-21 16:00:29.000000 alphaz-0.7.5.4/alphaz/documentations/site/database/init/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.547209 alphaz-0.7.5.4/alphaz/documentations/site/database/instantiate/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    17445 2023-04-21 16:00:29.000000 alphaz-0.7.5.4/alphaz/documentations/site/database/instantiate/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.547209 alphaz-0.7.5.4/alphaz/documentations/site/database/main/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    14939 2023-04-21 16:00:29.000000 alphaz-0.7.5.4/alphaz/documentations/site/database/main/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.547209 alphaz-0.7.5.4/alphaz/documentations/site/database/model/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    24758 2023-04-21 16:00:29.000000 alphaz-0.7.5.4/alphaz/documentations/site/database/model/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.551209 alphaz-0.7.5.4/alphaz/documentations/site/database/relations/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    16511 2023-04-21 16:00:29.000000 alphaz-0.7.5.4/alphaz/documentations/site/database/relations/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.551209 alphaz-0.7.5.4/alphaz/documentations/site/database/schema/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    18704 2023-04-21 16:00:29.000000 alphaz-0.7.5.4/alphaz/documentations/site/database/schema/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.551209 alphaz-0.7.5.4/alphaz/documentations/site/database/update/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    20308 2023-04-21 16:00:29.000000 alphaz-0.7.5.4/alphaz/documentations/site/database/update/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.551209 alphaz-0.7.5.4/alphaz/documentations/site/documentation/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    17065 2023-04-21 16:00:29.000000 alphaz-0.7.5.4/alphaz/documentations/site/documentation/index.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    29467 2023-04-21 16:00:29.000000 alphaz-0.7.5.4/alphaz/documentations/site/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.551209 alphaz-0.7.5.4/alphaz/documentations/site/search/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    54137 2023-04-21 16:00:29.000000 alphaz-0.7.5.4/alphaz/documentations/site/search/search_index.json
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2809 2023-04-21 16:00:29.000000 alphaz-0.7.5.4/alphaz/documentations/site/sitemap.xml
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      208 2023-04-21 16:00:29.000000 alphaz-0.7.5.4/alphaz/documentations/site/sitemap.xml.gz
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       50 2022-04-19 08:43:27.000000 alphaz-0.7.5.4/alphaz/git.sh
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       45 2022-05-14 15:57:01.000000 alphaz-0.7.5.4/alphaz/help.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      905 2021-03-29 08:42:45.000000 alphaz-0.7.5.4/alphaz/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.555209 alphaz-0.7.5.4/alphaz/libs/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.5.4/alphaz/libs/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     5785 2023-04-13 20:34:53.000000 alphaz-0.7.5.4/alphaz/libs/api_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1901 2021-03-29 08:42:45.000000 alphaz-0.7.5.4/alphaz/libs/barcode_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    13999 2023-04-18 09:00:04.000000 alphaz-0.7.5.4/alphaz/libs/config_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2420 2023-03-29 19:04:59.000000 alphaz-0.7.5.4/alphaz/libs/converter_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6022 2023-04-21 07:47:57.000000 alphaz-0.7.5.4/alphaz/libs/database_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4223 2023-02-06 12:52:51.000000 alphaz-0.7.5.4/alphaz/libs/date_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6324 2023-04-18 09:00:04.000000 alphaz-0.7.5.4/alphaz/libs/dict_lib.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.555209 alphaz-0.7.5.4/alphaz/libs/emulation/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1758 2023-02-02 21:07:35.000000 alphaz-0.7.5.4/alphaz/libs/emulation/vt102_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1642 2021-03-29 08:42:45.000000 alphaz-0.7.5.4/alphaz/libs/events.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3351 2022-01-17 10:25:20.000000 alphaz-0.7.5.4/alphaz/libs/files_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1184 2023-04-18 09:00:04.000000 alphaz-0.7.5.4/alphaz/libs/flask_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       49 2021-03-29 08:42:45.000000 alphaz-0.7.5.4/alphaz/libs/ftp_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1093 2022-07-21 11:35:27.000000 alphaz-0.7.5.4/alphaz/libs/img_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6212 2023-04-11 14:13:25.000000 alphaz-0.7.5.4/alphaz/libs/io_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3248 2023-03-16 19:44:05.000000 alphaz-0.7.5.4/alphaz/libs/json_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1143 2022-07-21 11:35:27.000000 alphaz-0.7.5.4/alphaz/libs/logs_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    12786 2023-03-17 15:11:43.000000 alphaz-0.7.5.4/alphaz/libs/mail_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      508 2021-03-29 08:42:45.000000 alphaz-0.7.5.4/alphaz/libs/nav_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      614 2022-09-07 06:57:10.000000 alphaz-0.7.5.4/alphaz/libs/notifications_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1348 2021-03-29 08:42:45.000000 alphaz-0.7.5.4/alphaz/libs/number_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      177 2021-03-29 08:42:45.000000 alphaz-0.7.5.4/alphaz/libs/os_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2782 2021-03-29 08:42:45.000000 alphaz-0.7.5.4/alphaz/libs/process_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    11058 2023-03-16 15:41:50.000000 alphaz-0.7.5.4/alphaz/libs/py_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      886 2023-04-21 07:47:57.000000 alphaz-0.7.5.4/alphaz/libs/scp_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     8082 2022-01-17 10:25:20.000000 alphaz-0.7.5.4/alphaz/libs/search_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6397 2023-04-13 20:34:53.000000 alphaz-0.7.5.4/alphaz/libs/secure_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3018 2023-04-03 15:21:20.000000 alphaz-0.7.5.4/alphaz/libs/soap_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      139 2021-03-29 08:42:45.000000 alphaz-0.7.5.4/alphaz/libs/sql_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    18517 2023-04-21 07:47:57.000000 alphaz-0.7.5.4/alphaz/libs/ssh_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     9938 2023-04-21 07:47:57.000000 alphaz-0.7.5.4/alphaz/libs/string_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     5139 2023-02-23 09:08:35.000000 alphaz-0.7.5.4/alphaz/libs/test_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      703 2023-03-16 15:41:50.000000 alphaz-0.7.5.4/alphaz/libs/time_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4200 2022-04-12 11:53:03.000000 alphaz-0.7.5.4/alphaz/libs/transactions_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     7595 2023-04-21 08:56:00.000000 alphaz-0.7.5.4/alphaz/libs/user_lib.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.555209 alphaz-0.7.5.4/alphaz/libs/user_management/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2022-04-27 13:24:50.000000 alphaz-0.7.5.4/alphaz/libs/user_management/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1354 2022-05-09 13:31:06.000000 alphaz-0.7.5.4/alphaz/libs/user_management/application_management_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1621 2022-10-07 10:05:05.000000 alphaz-0.7.5.4/alphaz/libs/user_management/permission_management_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3367 2022-10-07 10:05:05.000000 alphaz-0.7.5.4/alphaz/libs/user_management/role_management_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2336 2023-01-25 21:39:07.000000 alphaz-0.7.5.4/alphaz/libs/user_management/user_management_lib.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.555209 alphaz-0.7.5.4/alphaz/mails/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.559209 alphaz-0.7.5.4/alphaz/mails/Images/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)   948952 2021-03-29 08:42:45.000000 alphaz-0.7.5.4/alphaz/mails/Images/Background.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1835 2021-03-29 08:42:45.000000 alphaz-0.7.5.4/alphaz/mails/Images/Facebook_logo.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2484 2021-03-29 08:42:45.000000 alphaz-0.7.5.4/alphaz/mails/Images/Twitter_logo.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3522 2021-03-29 08:42:45.000000 alphaz-0.7.5.4/alphaz/mails/Images/Web_logo.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.5.4/alphaz/mails/Images/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)   966605 2021-03-29 08:42:45.000000 alphaz-0.7.5.4/alphaz/mails/Mail.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     5097 2022-04-13 09:59:51.000000 alphaz-0.7.5.4/alphaz/mails/Webmail.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.5.4/alphaz/mails/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    22029 2023-03-17 05:42:16.000000 alphaz-0.7.5.4/alphaz/mails/debug.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    23078 2023-03-16 20:48:51.000000 alphaz-0.7.5.4/alphaz/mails/mail.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2331 2021-03-29 08:42:45.000000 alphaz-0.7.5.4/alphaz/mails/password_reset.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    24598 2022-04-13 09:59:51.000000 alphaz-0.7.5.4/alphaz/mails/stay_in_touch.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       40 2021-03-29 08:42:45.000000 alphaz-0.7.5.4/alphaz/mails/template.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.559209 alphaz-0.7.5.4/alphaz/models/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      145 2023-02-06 09:05:20.000000 alphaz-0.7.5.4/alphaz/models/__init__.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.559209 alphaz-0.7.5.4/alphaz/models/api/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      185 2022-04-12 11:53:03.000000 alphaz-0.7.5.4/alphaz/models/api/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      884 2023-04-12 16:11:09.000000 alphaz-0.7.5.4/alphaz/models/api/_answer.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2179 2021-09-13 12:55:49.000000 alphaz-0.7.5.4/alphaz/models/api/_colorations.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      133 2021-09-06 13:56:36.000000 alphaz-0.7.5.4/alphaz/models/api/_methods.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    14253 2023-02-23 09:08:35.000000 alphaz-0.7.5.4/alphaz/models/api/_parameter.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2240 2022-08-26 12:58:11.000000 alphaz-0.7.5.4/alphaz/models/api/_requests.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    18649 2023-04-13 20:07:38.000000 alphaz-0.7.5.4/alphaz/models/api/_route.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    21593 2023-04-21 07:47:57.000000 alphaz-0.7.5.4/alphaz/models/api/_structures.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      651 2022-02-01 21:43:05.000000 alphaz-0.7.5.4/alphaz/models/api/_utils.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      388 2022-07-22 14:00:51.000000 alphaz-0.7.5.4/alphaz/models/base.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.559209 alphaz-0.7.5.4/alphaz/models/config/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       32 2021-03-29 08:42:45.000000 alphaz-0.7.5.4/alphaz/models/config/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    25438 2023-01-06 09:14:28.000000 alphaz-0.7.5.4/alphaz/models/config/_config.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    12129 2021-08-12 12:49:09.000000 alphaz-0.7.5.4/alphaz/models/config/_utils.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.563209 alphaz-0.7.5.4/alphaz/models/database/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       53 2022-01-13 15:32:15.000000 alphaz-0.7.5.4/alphaz/models/database/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     5495 2023-03-17 15:16:42.000000 alphaz-0.7.5.4/alphaz/models/database/main_definitions.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    10028 2023-03-19 14:55:26.000000 alphaz-0.7.5.4/alphaz/models/database/models.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      609 2022-04-28 08:55:29.000000 alphaz-0.7.5.4/alphaz/models/database/operators.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1164 2023-01-25 21:39:07.000000 alphaz-0.7.5.4/alphaz/models/database/requests.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1087 2021-03-29 08:42:45.000000 alphaz-0.7.5.4/alphaz/models/database/row.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    56108 2023-04-21 08:56:00.000000 alphaz-0.7.5.4/alphaz/models/database/structure.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1826 2023-02-23 09:08:35.000000 alphaz-0.7.5.4/alphaz/models/database/tests.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4529 2023-04-21 13:36:09.000000 alphaz-0.7.5.4/alphaz/models/database/users_definitions.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     9285 2022-08-02 08:51:28.000000 alphaz-0.7.5.4/alphaz/models/database/utils.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1061 2022-04-12 11:53:03.000000 alphaz-0.7.5.4/alphaz/models/database/views.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1241 2021-03-29 08:42:45.000000 alphaz-0.7.5.4/alphaz/models/excel.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6699 2023-04-21 07:47:57.000000 alphaz-0.7.5.4/alphaz/models/ftp.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      150 2022-07-19 09:10:48.000000 alphaz-0.7.5.4/alphaz/models/img.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.563209 alphaz-0.7.5.4/alphaz/models/json/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       41 2021-03-29 08:42:45.000000 alphaz-0.7.5.4/alphaz/models/json/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2609 2023-01-06 09:14:28.000000 alphaz-0.7.5.4/alphaz/models/json/_converters.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.563209 alphaz-0.7.5.4/alphaz/models/logger/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       68 2022-01-19 15:41:22.000000 alphaz-0.7.5.4/alphaz/models/logger/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1319 2023-01-06 09:14:28.000000 alphaz-0.7.5.4/alphaz/models/logger/_colorations.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    14091 2023-04-05 11:16:09.000000 alphaz-0.7.5.4/alphaz/models/logger/_logger.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      757 2021-03-29 08:42:45.000000 alphaz-0.7.5.4/alphaz/models/logger/_utils.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.563209 alphaz-0.7.5.4/alphaz/models/logs/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1280 2021-11-12 08:53:17.000000 alphaz-0.7.5.4/alphaz/models/logs/main.log
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      160 2021-11-07 15:22:58.000000 alphaz-0.7.5.4/alphaz/models/logs/main.log.2021-11-07
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.563209 alphaz-0.7.5.4/alphaz/models/main/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      385 2023-02-06 09:05:20.000000 alphaz-0.7.5.4/alphaz/models/main/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    27277 2023-04-18 09:00:04.000000 alphaz-0.7.5.4/alphaz/models/main/_base.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.563209 alphaz-0.7.5.4/alphaz/models/main/_core/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.5.4/alphaz/models/main/_core/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    15047 2023-04-21 16:00:27.000000 alphaz-0.7.5.4/alphaz/models/main/_core/_core.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       13 2021-03-29 08:42:45.000000 alphaz-0.7.5.4/alphaz/models/main/_core/_utils.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      339 2023-02-06 09:05:20.000000 alphaz-0.7.5.4/alphaz/models/main/_enum.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1862 2023-02-17 08:49:35.000000 alphaz-0.7.5.4/alphaz/models/main/_exception.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      501 2021-03-29 08:42:45.000000 alphaz-0.7.5.4/alphaz/models/main/_file.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      477 2021-03-29 08:42:45.000000 alphaz-0.7.5.4/alphaz/models/main/_process.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1305 2021-03-29 08:42:45.000000 alphaz-0.7.5.4/alphaz/models/main/_request.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      925 2021-03-29 08:42:45.000000 alphaz-0.7.5.4/alphaz/models/main/_singleton.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2258 2023-03-16 15:41:50.000000 alphaz-0.7.5.4/alphaz/models/request.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.567209 alphaz-0.7.5.4/alphaz/models/tests/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      139 2023-03-16 15:41:50.000000 alphaz-0.7.5.4/alphaz/models/tests/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6780 2023-02-23 09:08:35.000000 alphaz-0.7.5.4/alphaz/models/tests/_category.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3095 2023-02-23 09:08:35.000000 alphaz-0.7.5.4/alphaz/models/tests/_group.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      109 2021-09-10 07:16:32.000000 alphaz-0.7.5.4/alphaz/models/tests/_levels.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4174 2023-02-23 09:08:35.000000 alphaz-0.7.5.4/alphaz/models/tests/_method.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4571 2023-04-11 14:13:25.000000 alphaz-0.7.5.4/alphaz/models/tests/_save.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    13495 2023-04-18 11:53:08.000000 alphaz-0.7.5.4/alphaz/models/tests/_test.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     7413 2023-04-21 07:47:57.000000 alphaz-0.7.5.4/alphaz/models/tests/_wrappers.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2802 2022-12-01 15:14:08.000000 alphaz-0.7.5.4/alphaz/models/user.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2367 2021-03-29 08:42:45.000000 alphaz-0.7.5.4/alphaz/models/watcher.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.567209 alphaz-0.7.5.4/alphaz/pocs/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      685 2021-03-29 08:42:45.000000 alphaz-0.7.5.4/alphaz/pocs/main.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       72 2021-03-29 08:42:45.000000 alphaz-0.7.5.4/alphaz/reload_gitignore.bat
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       67 2022-04-12 12:30:24.000000 alphaz-0.7.5.4/alphaz/req.sh
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      460 2023-04-11 14:13:25.000000 alphaz-0.7.5.4/alphaz/requirements.txt
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1345 2022-04-19 08:43:27.000000 alphaz-0.7.5.4/alphaz/run.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.567209 alphaz-0.7.5.4/alphaz/src/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.5.4/alphaz/src/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    23747 2021-03-29 08:42:45.000000 alphaz-0.7.5.4/alphaz/src/alpha.png
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.567209 alphaz-0.7.5.4/alphaz/src/configs/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      135 2022-04-19 08:43:27.000000 alphaz-0.7.5.4/alphaz/src/configs/config.json
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      674 2023-01-25 21:39:07.000000 alphaz-0.7.5.4/alphaz/src/configs/loggers.json
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      490 2022-01-13 15:32:15.000000 alphaz-0.7.5.4/alphaz/src/configs/loggers_colors.json
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.567209 alphaz-0.7.5.4/alphaz/src/database/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.5.4/alphaz/src/database/__init__.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.567209 alphaz-0.7.5.4/alphaz/stitch/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1769 2021-03-29 08:42:45.000000 alphaz-0.7.5.4/alphaz/stitch/Core.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       26 2021-03-29 08:42:45.000000 alphaz-0.7.5.4/alphaz/stitch/__init__.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.567209 alphaz-0.7.5.4/alphaz/stitch/imports/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       78 2021-03-29 08:42:45.000000 alphaz-0.7.5.4/alphaz/stitch/imports/__init__.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.567209 alphaz-0.7.5.4/alphaz/stitch/models/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.5.4/alphaz/stitch/models/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      391 2021-03-29 08:42:45.000000 alphaz-0.7.5.4/alphaz/stitch/models/element.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       46 2021-03-29 08:42:45.000000 alphaz-0.7.5.4/alphaz/stitch/run.bat
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1857 2021-03-29 08:42:45.000000 alphaz-0.7.5.4/alphaz/stitch/stitch.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.575209 alphaz-0.7.5.4/alphaz/stitch/web-drivers/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)  8738816 2021-03-29 08:42:45.000000 alphaz-0.7.5.4/alphaz/stitch/web-drivers/chromedriver.exe
--rw-rw-r--   0 aurele    (1000) aurele    (1000)  7008696 2022-04-19 08:43:27.000000 alphaz-0.7.5.4/alphaz/stitch/web-drivers/geckodriver
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.531209 alphaz-0.7.5.4/alphaz/stitch/websites/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.583209 alphaz-0.7.5.4/alphaz/stitch/websites/Test/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      204 2021-03-29 08:42:45.000000 alphaz-0.7.5.4/alphaz/stitch/websites/Test/init.json
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.583209 alphaz-0.7.5.4/alphaz/stitch/websites/stiki/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      363 2022-04-13 09:59:51.000000 alphaz-0.7.5.4/alphaz/stitch/websites/stiki/init.json
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.583209 alphaz-0.7.5.4/alphaz/templates/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.5.4/alphaz/templates/__init__.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.583209 alphaz-0.7.5.4/alphaz/templates/assets/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.5.4/alphaz/templates/assets/__init__.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.583209 alphaz-0.7.5.4/alphaz/templates/assets/css/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    95923 2021-09-10 07:16:32.000000 alphaz-0.7.5.4/alphaz/templates/assets/css/home.css
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2356 2021-08-06 18:55:11.000000 alphaz-0.7.5.4/alphaz/templates/assets/css/logs.css
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.583209 alphaz-0.7.5.4/alphaz/templates/assets/images/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.583209 alphaz-0.7.5.4/alphaz/templates/assets/images/icons/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      276 2021-08-06 18:55:11.000000 alphaz-0.7.5.4/alphaz/templates/assets/images/icons/admin.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1444 2021-08-06 18:55:11.000000 alphaz-0.7.5.4/alphaz/templates/assets/images/icons/alpha.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      142 2021-08-06 18:55:11.000000 alphaz-0.7.5.4/alphaz/templates/assets/images/icons/save.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     8889 2021-08-06 18:55:11.000000 alphaz-0.7.5.4/alphaz/templates/assets/images/icons/start-icon.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      136 2021-08-06 18:55:11.000000 alphaz-0.7.5.4/alphaz/templates/assets/images/icons/user.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    23747 2021-08-06 18:55:11.000000 alphaz-0.7.5.4/alphaz/templates/assets/images/icons/wsalpha.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1165 2021-08-06 18:55:11.000000 alphaz-0.7.5.4/alphaz/templates/assets/images/loading.gif
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.583209 alphaz-0.7.5.4/alphaz/templates/assets/js/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.583209 alphaz-0.7.5.4/alphaz/templates/assets/js/libs/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    21922 2021-08-06 18:55:11.000000 alphaz-0.7.5.4/alphaz/templates/assets/js/libs/ansi_up.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    89475 2021-08-06 18:55:11.000000 alphaz-0.7.5.4/alphaz/templates/assets/js/libs/jquery.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     7339 2022-10-26 14:51:00.000000 alphaz-0.7.5.4/alphaz/templates/assets/js/logs.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       37 2021-03-29 08:42:45.000000 alphaz-0.7.5.4/alphaz/templates/hello.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    19017 2022-01-17 10:25:20.000000 alphaz-0.7.5.4/alphaz/templates/home.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3779 2021-08-06 18:55:11.000000 alphaz-0.7.5.4/alphaz/templates/logs.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1153 2023-01-25 21:39:07.000000 alphaz-0.7.5.4/alphaz/test.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.587209 alphaz-0.7.5.4/alphaz/tests/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      119 2021-03-29 08:42:45.000000 alphaz-0.7.5.4/alphaz/tests/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    13857 2023-03-28 08:47:21.000000 alphaz-0.7.5.4/alphaz/tests/api.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      541 2023-03-16 15:41:50.000000 alphaz-0.7.5.4/alphaz/tests/basic_test.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1526 2021-11-30 22:30:57.000000 alphaz-0.7.5.4/alphaz/tests/configurations.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    25075 2023-04-21 08:56:00.000000 alphaz-0.7.5.4/alphaz/tests/database.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      397 2021-03-29 08:42:45.000000 alphaz-0.7.5.4/alphaz/tests/processes.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      555 2021-03-29 08:42:45.000000 alphaz-0.7.5.4/alphaz/tests/utils.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.587209 alphaz-0.7.5.4/alphaz/utils/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       81 2021-03-29 08:42:45.000000 alphaz-0.7.5.4/alphaz/utils/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    11552 2023-02-16 14:12:47.000000 alphaz-0.7.5.4/alphaz/utils/api.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.587209 alphaz-0.7.5.4/alphaz/utils/apm/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2023-04-21 13:36:09.000000 alphaz-0.7.5.4/alphaz/utils/apm/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1438 2023-04-21 16:00:27.000000 alphaz-0.7.5.4/alphaz/utils/apm/ora.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      338 2022-04-19 08:43:27.000000 alphaz-0.7.5.4/alphaz/utils/clean.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      813 2022-05-02 08:25:25.000000 alphaz-0.7.5.4/alphaz/utils/configuration.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.587209 alphaz-0.7.5.4/alphaz/utils/database/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    13859 2023-04-21 07:47:58.000000 alphaz-0.7.5.4/alphaz/utils/database/init.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     5438 2022-02-24 13:20:43.000000 alphaz-0.7.5.4/alphaz/utils/database_to_dataclass.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2207 2023-03-16 15:41:50.000000 alphaz-0.7.5.4/alphaz/utils/decorators.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3112 2021-03-29 08:42:45.000000 alphaz-0.7.5.4/alphaz/utils/ensure.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4405 2022-01-13 15:32:15.000000 alphaz-0.7.5.4/alphaz/utils/mep.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     7639 2021-04-21 22:36:11.000000 alphaz-0.7.5.4/alphaz/utils/screens.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    22569 2022-01-17 10:25:20.000000 alphaz-0.7.5.4/alphaz/utils/selectionMenu.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      764 2022-01-17 10:25:20.000000 alphaz-0.7.5.4/alphaz/utils/tasks.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1535 2023-02-23 09:08:35.000000 alphaz-0.7.5.4/alphaz/utils/tests.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      628 2023-03-16 15:41:50.000000 alphaz-0.7.5.4/alphaz/utils/time.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3766 2022-01-17 10:25:20.000000 alphaz-0.7.5.4/alphaz/utils/transactions.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 16:00:30.535209 alphaz-0.7.5.4/alphaz.egg-info/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      589 2023-04-21 16:00:30.000000 alphaz-0.7.5.4/alphaz.egg-info/PKG-INFO
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    11272 2023-04-21 16:00:30.000000 alphaz-0.7.5.4/alphaz.egg-info/SOURCES.txt
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        1 2023-04-21 16:00:30.000000 alphaz-0.7.5.4/alphaz.egg-info/dependency_links.txt
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      458 2023-04-21 16:00:30.000000 alphaz-0.7.5.4/alphaz.egg-info/requires.txt
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        7 2023-04-21 16:00:30.000000 alphaz-0.7.5.4/alphaz.egg-info/top_level.txt
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       79 2023-04-21 16:00:30.591209 alphaz-0.7.5.4/setup.cfg
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3094 2023-04-21 15:59:32.000000 alphaz-0.7.5.4/setup.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.188132 alphaz-0.7.5.5/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    11211 2023-04-21 17:50:43.000000 alphaz-0.7.5.5/MANIFEST.in
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      589 2023-04-21 17:50:44.188132 alphaz-0.7.5.5/PKG-INFO
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1348 2021-07-12 18:07:51.000000 alphaz-0.7.5.5/README.md
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.124132 alphaz-0.7.5.5/alphaz/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        9 2023-04-18 09:00:04.000000 alphaz-0.7.5.5/alphaz/README.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      333 2023-04-13 12:43:58.000000 alphaz-0.7.5.5/alphaz/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      104 2021-03-29 08:42:45.000000 alphaz-0.7.5.5/alphaz/alphaz.bat
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       70 2021-03-29 08:42:45.000000 alphaz-0.7.5.5/alphaz/alphaz.code-workspace
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      208 2022-04-19 08:43:27.000000 alphaz-0.7.5.5/alphaz/alphaz.sh
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       48 2021-03-29 08:42:45.000000 alphaz-0.7.5.5/alphaz/api.bat
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      713 2023-04-18 09:00:04.000000 alphaz-0.7.5.5/alphaz/api.json
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      770 2022-04-13 09:59:51.000000 alphaz-0.7.5.5/alphaz/api.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.124132 alphaz-0.7.5.5/alphaz/apis/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.5.5/alphaz/apis/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2022-07-21 11:35:27.000000 alphaz-0.7.5.5/alphaz/apis/log.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2721 2023-03-17 07:06:42.000000 alphaz-0.7.5.5/alphaz/apis/mails.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.128132 alphaz-0.7.5.5/alphaz/apis/routes/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.5.5/alphaz/apis/routes/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1577 2023-02-23 09:08:35.000000 alphaz-0.7.5.5/alphaz/apis/routes/admin.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1137 2021-03-29 08:42:45.000000 alphaz-0.7.5.5/alphaz/apis/routes/api.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3062 2023-02-23 09:08:35.000000 alphaz-0.7.5.5/alphaz/apis/routes/basic_tests.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3094 2023-04-18 09:00:04.000000 alphaz-0.7.5.5/alphaz/apis/routes/database.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      413 2022-04-12 11:53:03.000000 alphaz-0.7.5.5/alphaz/apis/routes/git.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     7225 2023-02-01 13:59:24.000000 alphaz-0.7.5.5/alphaz/apis/routes/logs.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1810 2022-04-12 11:53:03.000000 alphaz-0.7.5.5/alphaz/apis/routes/mails.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6390 2023-04-21 07:47:57.000000 alphaz-0.7.5.5/alphaz/apis/routes/main.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1330 2023-02-23 09:08:35.000000 alphaz-0.7.5.5/alphaz/apis/routes/tests.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.128132 alphaz-0.7.5.5/alphaz/apis/routes/user_management/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      114 2022-04-27 13:24:50.000000 alphaz-0.7.5.5/alphaz/apis/routes/user_management/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2475 2022-05-09 13:31:06.000000 alphaz-0.7.5.5/alphaz/apis/routes/user_management/application_management.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2228 2022-05-09 13:31:06.000000 alphaz-0.7.5.5/alphaz/apis/routes/user_management/permission_management.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4058 2022-08-31 08:56:44.000000 alphaz-0.7.5.5/alphaz/apis/routes/user_management/role_management.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1291 2022-08-31 08:56:44.000000 alphaz-0.7.5.5/alphaz/apis/routes/user_management/user_management.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3324 2023-04-21 07:47:57.000000 alphaz-0.7.5.5/alphaz/apis/routes/users.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      584 2023-02-23 09:08:35.000000 alphaz-0.7.5.5/alphaz/apis/tests.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.128132 alphaz-0.7.5.5/alphaz/apis/users/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2022-07-21 11:35:27.000000 alphaz-0.7.5.5/alphaz/apis/users/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2718 2023-01-25 21:39:07.000000 alphaz-0.7.5.5/alphaz/apis/users/ldap.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    11543 2023-03-28 08:47:21.000000 alphaz-0.7.5.5/alphaz/apis/users/users.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.128132 alphaz-0.7.5.5/alphaz/config/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.5.5/alphaz/config/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      795 2021-03-29 08:42:45.000000 alphaz-0.7.5.5/alphaz/config/config.css
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    12602 2021-03-29 08:42:45.000000 alphaz-0.7.5.5/alphaz/config/config.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      707 2022-08-11 06:44:17.000000 alphaz-0.7.5.5/alphaz/config/main_configuration.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      823 2021-03-29 08:42:45.000000 alphaz-0.7.5.5/alphaz/config/page.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1700 2021-03-29 08:42:45.000000 alphaz-0.7.5.5/alphaz/config/source.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1564 2021-03-29 08:42:45.000000 alphaz-0.7.5.5/alphaz/config.json
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      238 2023-01-06 09:14:28.000000 alphaz-0.7.5.5/alphaz/core.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.128132 alphaz-0.7.5.5/alphaz/documentations/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.128132 alphaz-0.7.5.5/alphaz/documentations/docs/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2022-07-21 11:35:27.000000 alphaz-0.7.5.5/alphaz/documentations/docs/alpha_admin.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1408 2023-04-12 11:28:51.000000 alphaz-0.7.5.5/alphaz/documentations/docs/alpha_core.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2595 2022-07-21 11:35:27.000000 alphaz-0.7.5.5/alphaz/documentations/docs/alpha_screens.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2222 2023-04-12 11:28:51.000000 alphaz-0.7.5.5/alphaz/documentations/docs/alpha_setup.md
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.132132 alphaz-0.7.5.5/alphaz/documentations/docs/api/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1527 2023-04-18 09:00:04.000000 alphaz-0.7.5.5/alphaz/documentations/docs/api/authorizations.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       72 2023-04-18 09:00:04.000000 alphaz-0.7.5.5/alphaz/documentations/docs/api/cache.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2932 2023-04-18 09:00:04.000000 alphaz-0.7.5.5/alphaz/documentations/docs/api/configuration.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       24 2023-04-18 09:00:04.000000 alphaz-0.7.5.5/alphaz/documentations/docs/api/issues.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      705 2023-04-18 09:00:04.000000 alphaz-0.7.5.5/alphaz/documentations/docs/api/main.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      559 2023-04-18 09:00:04.000000 alphaz-0.7.5.5/alphaz/documentations/docs/api/methods.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1728 2023-04-18 09:00:04.000000 alphaz-0.7.5.5/alphaz/documentations/docs/api/parameters.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1197 2023-04-18 09:00:04.000000 alphaz-0.7.5.5/alphaz/documentations/docs/api/routes.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      486 2023-04-18 09:00:04.000000 alphaz-0.7.5.5/alphaz/documentations/docs/api/sqlalchemy.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1129 2023-04-18 09:00:04.000000 alphaz-0.7.5.5/alphaz/documentations/docs/api_database.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2520 2023-01-06 09:14:28.000000 alphaz-0.7.5.5/alphaz/documentations/docs/configuration.md
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.132132 alphaz-0.7.5.5/alphaz/documentations/docs/database/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2187 2023-04-18 09:00:04.000000 alphaz-0.7.5.5/alphaz/documentations/docs/database/init.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      442 2023-04-18 09:00:04.000000 alphaz-0.7.5.5/alphaz/documentations/docs/database/instantiate.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      113 2023-04-18 09:00:04.000000 alphaz-0.7.5.5/alphaz/documentations/docs/database/main.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1806 2023-04-18 09:00:04.000000 alphaz-0.7.5.5/alphaz/documentations/docs/database/model.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      373 2023-04-18 09:00:04.000000 alphaz-0.7.5.5/alphaz/documentations/docs/database/relations.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1087 2023-04-18 09:00:04.000000 alphaz-0.7.5.5/alphaz/documentations/docs/database/schema.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      615 2023-04-18 09:00:04.000000 alphaz-0.7.5.5/alphaz/documentations/docs/database/update.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      357 2021-04-14 08:59:25.000000 alphaz-0.7.5.5/alphaz/documentations/docs/documentation.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3526 2023-04-12 11:28:51.000000 alphaz-0.7.5.5/alphaz/documentations/docs/index.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1090 2023-04-18 09:00:04.000000 alphaz-0.7.5.5/alphaz/documentations/mkdocs.yml
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.132132 alphaz-0.7.5.5/alphaz/documentations/site/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    13156 2023-04-21 17:50:43.000000 alphaz-0.7.5.5/alphaz/documentations/site/404.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.132132 alphaz-0.7.5.5/alphaz/documentations/site/alpha_admin/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    14222 2023-04-21 17:50:43.000000 alphaz-0.7.5.5/alphaz/documentations/site/alpha_admin/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.132132 alphaz-0.7.5.5/alphaz/documentations/site/alpha_core/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    22752 2023-04-21 17:50:43.000000 alphaz-0.7.5.5/alphaz/documentations/site/alpha_core/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.132132 alphaz-0.7.5.5/alphaz/documentations/site/alpha_screens/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    21873 2023-04-21 17:50:43.000000 alphaz-0.7.5.5/alphaz/documentations/site/alpha_screens/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.132132 alphaz-0.7.5.5/alphaz/documentations/site/alpha_setup/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    24071 2023-04-21 17:50:43.000000 alphaz-0.7.5.5/alphaz/documentations/site/alpha_setup/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.116132 alphaz-0.7.5.5/alphaz/documentations/site/api/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.132132 alphaz-0.7.5.5/alphaz/documentations/site/api/authorizations/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    17905 2023-04-21 17:50:43.000000 alphaz-0.7.5.5/alphaz/documentations/site/api/authorizations/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.132132 alphaz-0.7.5.5/alphaz/documentations/site/api/cache/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    14918 2023-04-21 17:50:43.000000 alphaz-0.7.5.5/alphaz/documentations/site/api/cache/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.132132 alphaz-0.7.5.5/alphaz/documentations/site/api/configuration/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    27646 2023-04-21 17:50:43.000000 alphaz-0.7.5.5/alphaz/documentations/site/api/configuration/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.136132 alphaz-0.7.5.5/alphaz/documentations/site/api/issues/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    16365 2023-04-21 17:50:43.000000 alphaz-0.7.5.5/alphaz/documentations/site/api/issues/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.136132 alphaz-0.7.5.5/alphaz/documentations/site/api/main/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    17987 2023-04-21 17:50:43.000000 alphaz-0.7.5.5/alphaz/documentations/site/api/main/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.136132 alphaz-0.7.5.5/alphaz/documentations/site/api/methods/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    17722 2023-04-21 17:50:43.000000 alphaz-0.7.5.5/alphaz/documentations/site/api/methods/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.136132 alphaz-0.7.5.5/alphaz/documentations/site/api/parameters/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    20075 2023-04-21 17:50:43.000000 alphaz-0.7.5.5/alphaz/documentations/site/api/parameters/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.136132 alphaz-0.7.5.5/alphaz/documentations/site/api/routes/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    19333 2023-04-21 17:50:43.000000 alphaz-0.7.5.5/alphaz/documentations/site/api/routes/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.136132 alphaz-0.7.5.5/alphaz/documentations/site/api/sqlalchemy/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    17109 2023-04-21 17:50:43.000000 alphaz-0.7.5.5/alphaz/documentations/site/api/sqlalchemy/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.136132 alphaz-0.7.5.5/alphaz/documentations/site/api_database/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    22959 2023-04-21 17:50:43.000000 alphaz-0.7.5.5/alphaz/documentations/site/api_database/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.116132 alphaz-0.7.5.5/alphaz/documentations/site/assets/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.136132 alphaz-0.7.5.5/alphaz/documentations/site/assets/images/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1870 2023-04-21 17:50:42.000000 alphaz-0.7.5.5/alphaz/documentations/site/assets/images/favicon.png
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.136132 alphaz-0.7.5.5/alphaz/documentations/site/assets/javascripts/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    79520 2023-04-21 17:50:42.000000 alphaz-0.7.5.5/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)   384391 2023-04-21 17:50:42.000000 alphaz-0.7.5.5/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js.map
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.136132 alphaz-0.7.5.5/alphaz/documentations/site/assets/javascripts/lunr/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.140132 alphaz-0.7.5.5/alphaz/documentations/site/assets/javascripts/lunr/min/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    17058 2023-04-21 17:50:42.000000 alphaz-0.7.5.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ar.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4654 2023-04-21 17:50:42.000000 alphaz-0.7.5.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.da.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6119 2023-04-21 17:50:42.000000 alphaz-0.7.5.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.de.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6208 2023-04-21 17:50:42.000000 alphaz-0.7.5.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.du.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    11499 2023-04-21 17:50:42.000000 alphaz-0.7.5.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.es.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     9342 2023-04-21 17:50:42.000000 alphaz-0.7.5.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fi.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    10669 2023-04-21 17:50:42.000000 alphaz-0.7.5.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fr.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     9437 2023-04-21 17:50:42.000000 alphaz-0.7.5.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.hu.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    11232 2023-04-21 17:50:42.000000 alphaz-0.7.5.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.it.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2313 2023-04-21 17:50:42.000000 alphaz-0.7.5.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ja.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       36 2023-04-21 17:50:42.000000 alphaz-0.7.5.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.jp.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      817 2023-04-21 17:50:42.000000 alphaz-0.7.5.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.multi.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6026 2023-04-21 17:50:42.000000 alphaz-0.7.5.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.nl.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4754 2023-04-21 17:50:42.000000 alphaz-0.7.5.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.no.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    10171 2023-04-21 17:50:42.000000 alphaz-0.7.5.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.pt.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    10958 2023-04-21 17:50:42.000000 alphaz-0.7.5.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ro.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    10331 2023-04-21 17:50:42.000000 alphaz-0.7.5.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ru.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3647 2023-04-21 17:50:42.000000 alphaz-0.7.5.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4523 2023-04-21 17:50:42.000000 alphaz-0.7.5.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.sv.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    15009 2023-04-21 17:50:42.000000 alphaz-0.7.5.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.tr.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      784 2023-04-21 17:50:42.000000 alphaz-0.7.5.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.vi.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    22878 2023-04-21 17:50:42.000000 alphaz-0.7.5.5/alphaz/documentations/site/assets/javascripts/lunr/tinyseg.js
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.140132 alphaz-0.7.5.5/alphaz/documentations/site/assets/javascripts/workers/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    34936 2023-04-21 17:50:42.000000 alphaz-0.7.5.5/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)   167496 2023-04-21 17:50:42.000000 alphaz-0.7.5.5/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js.map
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.140132 alphaz-0.7.5.5/alphaz/documentations/site/assets/stylesheets/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    87332 2023-04-21 17:50:42.000000 alphaz-0.7.5.5/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)   319950 2023-04-21 17:50:42.000000 alphaz-0.7.5.5/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css.map
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    10915 2023-04-21 17:50:42.000000 alphaz-0.7.5.5/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    37512 2023-04-21 17:50:42.000000 alphaz-0.7.5.5/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css.map
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.140132 alphaz-0.7.5.5/alphaz/documentations/site/configuration/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    28465 2023-04-21 17:50:43.000000 alphaz-0.7.5.5/alphaz/documentations/site/configuration/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.116132 alphaz-0.7.5.5/alphaz/documentations/site/database/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.140132 alphaz-0.7.5.5/alphaz/documentations/site/database/init/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    23027 2023-04-21 17:50:43.000000 alphaz-0.7.5.5/alphaz/documentations/site/database/init/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.140132 alphaz-0.7.5.5/alphaz/documentations/site/database/instantiate/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    17445 2023-04-21 17:50:43.000000 alphaz-0.7.5.5/alphaz/documentations/site/database/instantiate/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.140132 alphaz-0.7.5.5/alphaz/documentations/site/database/main/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    14939 2023-04-21 17:50:43.000000 alphaz-0.7.5.5/alphaz/documentations/site/database/main/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.140132 alphaz-0.7.5.5/alphaz/documentations/site/database/model/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    24758 2023-04-21 17:50:43.000000 alphaz-0.7.5.5/alphaz/documentations/site/database/model/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.140132 alphaz-0.7.5.5/alphaz/documentations/site/database/relations/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    16511 2023-04-21 17:50:43.000000 alphaz-0.7.5.5/alphaz/documentations/site/database/relations/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.144132 alphaz-0.7.5.5/alphaz/documentations/site/database/schema/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    18704 2023-04-21 17:50:43.000000 alphaz-0.7.5.5/alphaz/documentations/site/database/schema/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.144132 alphaz-0.7.5.5/alphaz/documentations/site/database/update/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    20308 2023-04-21 17:50:43.000000 alphaz-0.7.5.5/alphaz/documentations/site/database/update/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.144132 alphaz-0.7.5.5/alphaz/documentations/site/documentation/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    17065 2023-04-21 17:50:43.000000 alphaz-0.7.5.5/alphaz/documentations/site/documentation/index.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    29467 2023-04-21 17:50:43.000000 alphaz-0.7.5.5/alphaz/documentations/site/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.144132 alphaz-0.7.5.5/alphaz/documentations/site/search/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    54137 2023-04-21 17:50:43.000000 alphaz-0.7.5.5/alphaz/documentations/site/search/search_index.json
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2809 2023-04-21 17:50:42.000000 alphaz-0.7.5.5/alphaz/documentations/site/sitemap.xml
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      208 2023-04-21 17:50:42.000000 alphaz-0.7.5.5/alphaz/documentations/site/sitemap.xml.gz
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       50 2022-04-19 08:43:27.000000 alphaz-0.7.5.5/alphaz/git.sh
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       45 2022-05-14 15:57:01.000000 alphaz-0.7.5.5/alphaz/help.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      905 2021-03-29 08:42:45.000000 alphaz-0.7.5.5/alphaz/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.148132 alphaz-0.7.5.5/alphaz/libs/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.5.5/alphaz/libs/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     5785 2023-04-13 20:34:53.000000 alphaz-0.7.5.5/alphaz/libs/api_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1901 2021-03-29 08:42:45.000000 alphaz-0.7.5.5/alphaz/libs/barcode_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    13999 2023-04-18 09:00:04.000000 alphaz-0.7.5.5/alphaz/libs/config_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2420 2023-03-29 19:04:59.000000 alphaz-0.7.5.5/alphaz/libs/converter_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6022 2023-04-21 07:47:57.000000 alphaz-0.7.5.5/alphaz/libs/database_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4223 2023-02-06 12:52:51.000000 alphaz-0.7.5.5/alphaz/libs/date_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6324 2023-04-18 09:00:04.000000 alphaz-0.7.5.5/alphaz/libs/dict_lib.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.148132 alphaz-0.7.5.5/alphaz/libs/emulation/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1758 2023-02-02 21:07:35.000000 alphaz-0.7.5.5/alphaz/libs/emulation/vt102_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1642 2021-03-29 08:42:45.000000 alphaz-0.7.5.5/alphaz/libs/events.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3351 2022-01-17 10:25:20.000000 alphaz-0.7.5.5/alphaz/libs/files_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1184 2023-04-18 09:00:04.000000 alphaz-0.7.5.5/alphaz/libs/flask_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       49 2021-03-29 08:42:45.000000 alphaz-0.7.5.5/alphaz/libs/ftp_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1093 2022-07-21 11:35:27.000000 alphaz-0.7.5.5/alphaz/libs/img_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6212 2023-04-11 14:13:25.000000 alphaz-0.7.5.5/alphaz/libs/io_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3248 2023-03-16 19:44:05.000000 alphaz-0.7.5.5/alphaz/libs/json_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1143 2022-07-21 11:35:27.000000 alphaz-0.7.5.5/alphaz/libs/logs_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    12786 2023-03-17 15:11:43.000000 alphaz-0.7.5.5/alphaz/libs/mail_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      508 2021-03-29 08:42:45.000000 alphaz-0.7.5.5/alphaz/libs/nav_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      614 2022-09-07 06:57:10.000000 alphaz-0.7.5.5/alphaz/libs/notifications_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1348 2021-03-29 08:42:45.000000 alphaz-0.7.5.5/alphaz/libs/number_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      177 2021-03-29 08:42:45.000000 alphaz-0.7.5.5/alphaz/libs/os_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2782 2021-03-29 08:42:45.000000 alphaz-0.7.5.5/alphaz/libs/process_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    11058 2023-03-16 15:41:50.000000 alphaz-0.7.5.5/alphaz/libs/py_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      886 2023-04-21 07:47:57.000000 alphaz-0.7.5.5/alphaz/libs/scp_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     8082 2022-01-17 10:25:20.000000 alphaz-0.7.5.5/alphaz/libs/search_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6397 2023-04-13 20:34:53.000000 alphaz-0.7.5.5/alphaz/libs/secure_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3018 2023-04-03 15:21:20.000000 alphaz-0.7.5.5/alphaz/libs/soap_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      139 2021-03-29 08:42:45.000000 alphaz-0.7.5.5/alphaz/libs/sql_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    18517 2023-04-21 07:47:57.000000 alphaz-0.7.5.5/alphaz/libs/ssh_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     9938 2023-04-21 07:47:57.000000 alphaz-0.7.5.5/alphaz/libs/string_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     5139 2023-02-23 09:08:35.000000 alphaz-0.7.5.5/alphaz/libs/test_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      703 2023-03-16 15:41:50.000000 alphaz-0.7.5.5/alphaz/libs/time_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4200 2022-04-12 11:53:03.000000 alphaz-0.7.5.5/alphaz/libs/transactions_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     7595 2023-04-21 08:56:00.000000 alphaz-0.7.5.5/alphaz/libs/user_lib.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.148132 alphaz-0.7.5.5/alphaz/libs/user_management/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2022-04-27 13:24:50.000000 alphaz-0.7.5.5/alphaz/libs/user_management/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1354 2022-05-09 13:31:06.000000 alphaz-0.7.5.5/alphaz/libs/user_management/application_management_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1621 2022-10-07 10:05:05.000000 alphaz-0.7.5.5/alphaz/libs/user_management/permission_management_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3367 2022-10-07 10:05:05.000000 alphaz-0.7.5.5/alphaz/libs/user_management/role_management_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2336 2023-01-25 21:39:07.000000 alphaz-0.7.5.5/alphaz/libs/user_management/user_management_lib.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.152132 alphaz-0.7.5.5/alphaz/mails/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.152132 alphaz-0.7.5.5/alphaz/mails/Images/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)   948952 2021-03-29 08:42:45.000000 alphaz-0.7.5.5/alphaz/mails/Images/Background.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1835 2021-03-29 08:42:45.000000 alphaz-0.7.5.5/alphaz/mails/Images/Facebook_logo.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2484 2021-03-29 08:42:45.000000 alphaz-0.7.5.5/alphaz/mails/Images/Twitter_logo.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3522 2021-03-29 08:42:45.000000 alphaz-0.7.5.5/alphaz/mails/Images/Web_logo.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.5.5/alphaz/mails/Images/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)   966605 2021-03-29 08:42:45.000000 alphaz-0.7.5.5/alphaz/mails/Mail.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     5097 2022-04-13 09:59:51.000000 alphaz-0.7.5.5/alphaz/mails/Webmail.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.5.5/alphaz/mails/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    22029 2023-03-17 05:42:16.000000 alphaz-0.7.5.5/alphaz/mails/debug.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    23078 2023-03-16 20:48:51.000000 alphaz-0.7.5.5/alphaz/mails/mail.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2331 2021-03-29 08:42:45.000000 alphaz-0.7.5.5/alphaz/mails/password_reset.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    24598 2022-04-13 09:59:51.000000 alphaz-0.7.5.5/alphaz/mails/stay_in_touch.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       40 2021-03-29 08:42:45.000000 alphaz-0.7.5.5/alphaz/mails/template.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.152132 alphaz-0.7.5.5/alphaz/models/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      145 2023-02-06 09:05:20.000000 alphaz-0.7.5.5/alphaz/models/__init__.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.156132 alphaz-0.7.5.5/alphaz/models/api/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      185 2022-04-12 11:53:03.000000 alphaz-0.7.5.5/alphaz/models/api/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      884 2023-04-12 16:11:09.000000 alphaz-0.7.5.5/alphaz/models/api/_answer.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2179 2021-09-13 12:55:49.000000 alphaz-0.7.5.5/alphaz/models/api/_colorations.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      133 2021-09-06 13:56:36.000000 alphaz-0.7.5.5/alphaz/models/api/_methods.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    14253 2023-02-23 09:08:35.000000 alphaz-0.7.5.5/alphaz/models/api/_parameter.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2240 2022-08-26 12:58:11.000000 alphaz-0.7.5.5/alphaz/models/api/_requests.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    18649 2023-04-13 20:07:38.000000 alphaz-0.7.5.5/alphaz/models/api/_route.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    21593 2023-04-21 07:47:57.000000 alphaz-0.7.5.5/alphaz/models/api/_structures.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      651 2022-02-01 21:43:05.000000 alphaz-0.7.5.5/alphaz/models/api/_utils.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      388 2022-07-22 14:00:51.000000 alphaz-0.7.5.5/alphaz/models/base.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.156132 alphaz-0.7.5.5/alphaz/models/config/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       32 2021-03-29 08:42:45.000000 alphaz-0.7.5.5/alphaz/models/config/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    25438 2023-01-06 09:14:28.000000 alphaz-0.7.5.5/alphaz/models/config/_config.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    12129 2021-08-12 12:49:09.000000 alphaz-0.7.5.5/alphaz/models/config/_utils.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.156132 alphaz-0.7.5.5/alphaz/models/database/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       53 2022-01-13 15:32:15.000000 alphaz-0.7.5.5/alphaz/models/database/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     5495 2023-03-17 15:16:42.000000 alphaz-0.7.5.5/alphaz/models/database/main_definitions.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    10028 2023-03-19 14:55:26.000000 alphaz-0.7.5.5/alphaz/models/database/models.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      609 2022-04-28 08:55:29.000000 alphaz-0.7.5.5/alphaz/models/database/operators.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1164 2023-01-25 21:39:07.000000 alphaz-0.7.5.5/alphaz/models/database/requests.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1087 2021-03-29 08:42:45.000000 alphaz-0.7.5.5/alphaz/models/database/row.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    56108 2023-04-21 08:56:00.000000 alphaz-0.7.5.5/alphaz/models/database/structure.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1826 2023-02-23 09:08:35.000000 alphaz-0.7.5.5/alphaz/models/database/tests.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4529 2023-04-21 13:36:09.000000 alphaz-0.7.5.5/alphaz/models/database/users_definitions.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     9285 2022-08-02 08:51:28.000000 alphaz-0.7.5.5/alphaz/models/database/utils.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1061 2022-04-12 11:53:03.000000 alphaz-0.7.5.5/alphaz/models/database/views.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1241 2021-03-29 08:42:45.000000 alphaz-0.7.5.5/alphaz/models/excel.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6699 2023-04-21 07:47:57.000000 alphaz-0.7.5.5/alphaz/models/ftp.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      150 2022-07-19 09:10:48.000000 alphaz-0.7.5.5/alphaz/models/img.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.156132 alphaz-0.7.5.5/alphaz/models/json/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       41 2021-03-29 08:42:45.000000 alphaz-0.7.5.5/alphaz/models/json/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2609 2023-01-06 09:14:28.000000 alphaz-0.7.5.5/alphaz/models/json/_converters.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.156132 alphaz-0.7.5.5/alphaz/models/logger/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       68 2022-01-19 15:41:22.000000 alphaz-0.7.5.5/alphaz/models/logger/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1319 2023-01-06 09:14:28.000000 alphaz-0.7.5.5/alphaz/models/logger/_colorations.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    14091 2023-04-05 11:16:09.000000 alphaz-0.7.5.5/alphaz/models/logger/_logger.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      757 2021-03-29 08:42:45.000000 alphaz-0.7.5.5/alphaz/models/logger/_utils.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.160132 alphaz-0.7.5.5/alphaz/models/logs/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1280 2021-11-12 08:53:17.000000 alphaz-0.7.5.5/alphaz/models/logs/main.log
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      160 2021-11-07 15:22:58.000000 alphaz-0.7.5.5/alphaz/models/logs/main.log.2021-11-07
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.160132 alphaz-0.7.5.5/alphaz/models/main/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      385 2023-02-06 09:05:20.000000 alphaz-0.7.5.5/alphaz/models/main/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    27277 2023-04-18 09:00:04.000000 alphaz-0.7.5.5/alphaz/models/main/_base.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.160132 alphaz-0.7.5.5/alphaz/models/main/_core/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.5.5/alphaz/models/main/_core/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    15112 2023-04-21 17:50:41.000000 alphaz-0.7.5.5/alphaz/models/main/_core/_core.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       13 2021-03-29 08:42:45.000000 alphaz-0.7.5.5/alphaz/models/main/_core/_utils.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      339 2023-02-06 09:05:20.000000 alphaz-0.7.5.5/alphaz/models/main/_enum.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1862 2023-02-17 08:49:35.000000 alphaz-0.7.5.5/alphaz/models/main/_exception.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      501 2021-03-29 08:42:45.000000 alphaz-0.7.5.5/alphaz/models/main/_file.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      477 2021-03-29 08:42:45.000000 alphaz-0.7.5.5/alphaz/models/main/_process.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1305 2021-03-29 08:42:45.000000 alphaz-0.7.5.5/alphaz/models/main/_request.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      925 2021-03-29 08:42:45.000000 alphaz-0.7.5.5/alphaz/models/main/_singleton.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2258 2023-03-16 15:41:50.000000 alphaz-0.7.5.5/alphaz/models/request.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.160132 alphaz-0.7.5.5/alphaz/models/tests/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      139 2023-03-16 15:41:50.000000 alphaz-0.7.5.5/alphaz/models/tests/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6780 2023-02-23 09:08:35.000000 alphaz-0.7.5.5/alphaz/models/tests/_category.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3095 2023-02-23 09:08:35.000000 alphaz-0.7.5.5/alphaz/models/tests/_group.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      109 2021-09-10 07:16:32.000000 alphaz-0.7.5.5/alphaz/models/tests/_levels.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4174 2023-02-23 09:08:35.000000 alphaz-0.7.5.5/alphaz/models/tests/_method.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4571 2023-04-11 14:13:25.000000 alphaz-0.7.5.5/alphaz/models/tests/_save.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    13495 2023-04-18 11:53:08.000000 alphaz-0.7.5.5/alphaz/models/tests/_test.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     7413 2023-04-21 07:47:57.000000 alphaz-0.7.5.5/alphaz/models/tests/_wrappers.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2802 2022-12-01 15:14:08.000000 alphaz-0.7.5.5/alphaz/models/user.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2367 2021-03-29 08:42:45.000000 alphaz-0.7.5.5/alphaz/models/watcher.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.160132 alphaz-0.7.5.5/alphaz/pocs/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      685 2021-03-29 08:42:45.000000 alphaz-0.7.5.5/alphaz/pocs/main.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       72 2021-03-29 08:42:45.000000 alphaz-0.7.5.5/alphaz/reload_gitignore.bat
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       67 2022-04-12 12:30:24.000000 alphaz-0.7.5.5/alphaz/req.sh
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      460 2023-04-11 14:13:25.000000 alphaz-0.7.5.5/alphaz/requirements.txt
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1345 2022-04-19 08:43:27.000000 alphaz-0.7.5.5/alphaz/run.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.160132 alphaz-0.7.5.5/alphaz/src/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.5.5/alphaz/src/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    23747 2021-03-29 08:42:45.000000 alphaz-0.7.5.5/alphaz/src/alpha.png
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.164132 alphaz-0.7.5.5/alphaz/src/configs/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      135 2022-04-19 08:43:27.000000 alphaz-0.7.5.5/alphaz/src/configs/config.json
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      674 2023-01-25 21:39:07.000000 alphaz-0.7.5.5/alphaz/src/configs/loggers.json
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      490 2022-01-13 15:32:15.000000 alphaz-0.7.5.5/alphaz/src/configs/loggers_colors.json
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.164132 alphaz-0.7.5.5/alphaz/src/database/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.5.5/alphaz/src/database/__init__.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.164132 alphaz-0.7.5.5/alphaz/stitch/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1769 2021-03-29 08:42:45.000000 alphaz-0.7.5.5/alphaz/stitch/Core.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       26 2021-03-29 08:42:45.000000 alphaz-0.7.5.5/alphaz/stitch/__init__.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.164132 alphaz-0.7.5.5/alphaz/stitch/imports/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       78 2021-03-29 08:42:45.000000 alphaz-0.7.5.5/alphaz/stitch/imports/__init__.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.164132 alphaz-0.7.5.5/alphaz/stitch/models/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.5.5/alphaz/stitch/models/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      391 2021-03-29 08:42:45.000000 alphaz-0.7.5.5/alphaz/stitch/models/element.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       46 2021-03-29 08:42:45.000000 alphaz-0.7.5.5/alphaz/stitch/run.bat
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1857 2021-03-29 08:42:45.000000 alphaz-0.7.5.5/alphaz/stitch/stitch.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.172132 alphaz-0.7.5.5/alphaz/stitch/web-drivers/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)  8738816 2021-03-29 08:42:45.000000 alphaz-0.7.5.5/alphaz/stitch/web-drivers/chromedriver.exe
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)  7008696 2022-04-19 08:43:27.000000 alphaz-0.7.5.5/alphaz/stitch/web-drivers/geckodriver
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.120132 alphaz-0.7.5.5/alphaz/stitch/websites/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.180132 alphaz-0.7.5.5/alphaz/stitch/websites/Test/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      204 2021-03-29 08:42:45.000000 alphaz-0.7.5.5/alphaz/stitch/websites/Test/init.json
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.180132 alphaz-0.7.5.5/alphaz/stitch/websites/stiki/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      363 2022-04-13 09:59:51.000000 alphaz-0.7.5.5/alphaz/stitch/websites/stiki/init.json
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.180132 alphaz-0.7.5.5/alphaz/templates/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.5.5/alphaz/templates/__init__.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.180132 alphaz-0.7.5.5/alphaz/templates/assets/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.5.5/alphaz/templates/assets/__init__.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.180132 alphaz-0.7.5.5/alphaz/templates/assets/css/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    95923 2021-09-10 07:16:32.000000 alphaz-0.7.5.5/alphaz/templates/assets/css/home.css
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2356 2021-08-06 18:55:11.000000 alphaz-0.7.5.5/alphaz/templates/assets/css/logs.css
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.180132 alphaz-0.7.5.5/alphaz/templates/assets/images/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.184132 alphaz-0.7.5.5/alphaz/templates/assets/images/icons/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      276 2021-08-06 18:55:11.000000 alphaz-0.7.5.5/alphaz/templates/assets/images/icons/admin.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1444 2021-08-06 18:55:11.000000 alphaz-0.7.5.5/alphaz/templates/assets/images/icons/alpha.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      142 2021-08-06 18:55:11.000000 alphaz-0.7.5.5/alphaz/templates/assets/images/icons/save.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     8889 2021-08-06 18:55:11.000000 alphaz-0.7.5.5/alphaz/templates/assets/images/icons/start-icon.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      136 2021-08-06 18:55:11.000000 alphaz-0.7.5.5/alphaz/templates/assets/images/icons/user.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    23747 2021-08-06 18:55:11.000000 alphaz-0.7.5.5/alphaz/templates/assets/images/icons/wsalpha.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1165 2021-08-06 18:55:11.000000 alphaz-0.7.5.5/alphaz/templates/assets/images/loading.gif
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.184132 alphaz-0.7.5.5/alphaz/templates/assets/js/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.184132 alphaz-0.7.5.5/alphaz/templates/assets/js/libs/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    21922 2021-08-06 18:55:11.000000 alphaz-0.7.5.5/alphaz/templates/assets/js/libs/ansi_up.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    89475 2021-08-06 18:55:11.000000 alphaz-0.7.5.5/alphaz/templates/assets/js/libs/jquery.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     7339 2022-10-26 14:51:00.000000 alphaz-0.7.5.5/alphaz/templates/assets/js/logs.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       37 2021-03-29 08:42:45.000000 alphaz-0.7.5.5/alphaz/templates/hello.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    19017 2022-01-17 10:25:20.000000 alphaz-0.7.5.5/alphaz/templates/home.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3779 2021-08-06 18:55:11.000000 alphaz-0.7.5.5/alphaz/templates/logs.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1153 2023-01-25 21:39:07.000000 alphaz-0.7.5.5/alphaz/test.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.184132 alphaz-0.7.5.5/alphaz/tests/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      119 2021-03-29 08:42:45.000000 alphaz-0.7.5.5/alphaz/tests/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    13857 2023-03-28 08:47:21.000000 alphaz-0.7.5.5/alphaz/tests/api.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      541 2023-03-16 15:41:50.000000 alphaz-0.7.5.5/alphaz/tests/basic_test.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1526 2021-11-30 22:30:57.000000 alphaz-0.7.5.5/alphaz/tests/configurations.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    25075 2023-04-21 08:56:00.000000 alphaz-0.7.5.5/alphaz/tests/database.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      397 2021-03-29 08:42:45.000000 alphaz-0.7.5.5/alphaz/tests/processes.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      555 2021-03-29 08:42:45.000000 alphaz-0.7.5.5/alphaz/tests/utils.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.188132 alphaz-0.7.5.5/alphaz/utils/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       81 2021-03-29 08:42:45.000000 alphaz-0.7.5.5/alphaz/utils/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    11552 2023-02-16 14:12:47.000000 alphaz-0.7.5.5/alphaz/utils/api.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.188132 alphaz-0.7.5.5/alphaz/utils/apm/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2023-04-21 13:36:09.000000 alphaz-0.7.5.5/alphaz/utils/apm/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1671 2023-04-21 17:50:41.000000 alphaz-0.7.5.5/alphaz/utils/apm/ora.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      338 2022-04-19 08:43:27.000000 alphaz-0.7.5.5/alphaz/utils/clean.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      813 2022-05-02 08:25:25.000000 alphaz-0.7.5.5/alphaz/utils/configuration.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.188132 alphaz-0.7.5.5/alphaz/utils/database/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    13859 2023-04-21 07:47:58.000000 alphaz-0.7.5.5/alphaz/utils/database/init.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     5438 2022-02-24 13:20:43.000000 alphaz-0.7.5.5/alphaz/utils/database_to_dataclass.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2207 2023-03-16 15:41:50.000000 alphaz-0.7.5.5/alphaz/utils/decorators.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3112 2021-03-29 08:42:45.000000 alphaz-0.7.5.5/alphaz/utils/ensure.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4405 2022-01-13 15:32:15.000000 alphaz-0.7.5.5/alphaz/utils/mep.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     7639 2021-04-21 22:36:11.000000 alphaz-0.7.5.5/alphaz/utils/screens.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    22569 2022-01-17 10:25:20.000000 alphaz-0.7.5.5/alphaz/utils/selectionMenu.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      764 2022-01-17 10:25:20.000000 alphaz-0.7.5.5/alphaz/utils/tasks.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1535 2023-02-23 09:08:35.000000 alphaz-0.7.5.5/alphaz/utils/tests.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      628 2023-03-16 15:41:50.000000 alphaz-0.7.5.5/alphaz/utils/time.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3766 2022-01-17 10:25:20.000000 alphaz-0.7.5.5/alphaz/utils/transactions.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-21 17:50:44.124132 alphaz-0.7.5.5/alphaz.egg-info/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      589 2023-04-21 17:50:43.000000 alphaz-0.7.5.5/alphaz.egg-info/PKG-INFO
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    11272 2023-04-21 17:50:43.000000 alphaz-0.7.5.5/alphaz.egg-info/SOURCES.txt
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        1 2023-04-21 17:50:43.000000 alphaz-0.7.5.5/alphaz.egg-info/dependency_links.txt
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      458 2023-04-21 17:50:43.000000 alphaz-0.7.5.5/alphaz.egg-info/requires.txt
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        7 2023-04-21 17:50:43.000000 alphaz-0.7.5.5/alphaz.egg-info/top_level.txt
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       79 2023-04-21 17:50:44.188132 alphaz-0.7.5.5/setup.cfg
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3094 2023-04-21 17:41:33.000000 alphaz-0.7.5.5/setup.py
```

### Comparing `alphaz-0.7.5.4/MANIFEST.in` & `alphaz-0.7.5.5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/PKG-INFO` & `alphaz-0.7.5.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: alphaz
-Version: 0.7.5.4
+Version: 0.7.5.5
 Summary: A package full of very nice tools
 Home-page: https://github.com/ZAurele/alphaz
 Author: Aurèle
 Author-email: contact@aurele.eu
 License: MIT
-Download-URL: https://github.com/ZAurele/alphaz/archive/refs/tags/0.7.5.4.tar.gz
+Download-URL: https://github.com/ZAurele/alphaz/archive/refs/tags/0.7.5.5.tar.gz
 Description: UNKNOWN
 Keywords: Flask,Json
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `alphaz-0.7.5.4/README.md` & `alphaz-0.7.5.5/README.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/api.json` & `alphaz-0.7.5.5/alphaz/api.json`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/api.py` & `alphaz-0.7.5.5/alphaz/api.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/apis/mails.py` & `alphaz-0.7.5.5/alphaz/apis/mails.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/apis/routes/admin.py` & `alphaz-0.7.5.5/alphaz/apis/routes/admin.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/apis/routes/api.py` & `alphaz-0.7.5.5/alphaz/apis/routes/api.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/apis/routes/basic_tests.py` & `alphaz-0.7.5.5/alphaz/apis/routes/basic_tests.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/apis/routes/database.py` & `alphaz-0.7.5.5/alphaz/apis/routes/database.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/apis/routes/logs.py` & `alphaz-0.7.5.5/alphaz/apis/routes/logs.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/apis/routes/mails.py` & `alphaz-0.7.5.5/alphaz/apis/routes/mails.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/apis/routes/main.py` & `alphaz-0.7.5.5/alphaz/apis/routes/main.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/apis/routes/tests.py` & `alphaz-0.7.5.5/alphaz/apis/routes/tests.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/apis/routes/user_management/application_management.py` & `alphaz-0.7.5.5/alphaz/apis/routes/user_management/application_management.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/apis/routes/user_management/permission_management.py` & `alphaz-0.7.5.5/alphaz/apis/routes/user_management/permission_management.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/apis/routes/user_management/role_management.py` & `alphaz-0.7.5.5/alphaz/apis/routes/user_management/role_management.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/apis/routes/user_management/user_management.py` & `alphaz-0.7.5.5/alphaz/apis/routes/user_management/user_management.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/apis/routes/users.py` & `alphaz-0.7.5.5/alphaz/apis/routes/users.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/apis/tests.py` & `alphaz-0.7.5.5/alphaz/apis/tests.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/apis/users/ldap.py` & `alphaz-0.7.5.5/alphaz/apis/users/ldap.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/apis/users/users.py` & `alphaz-0.7.5.5/alphaz/apis/users/users.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/config/config.css` & `alphaz-0.7.5.5/alphaz/config/config.css`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/config/config.html` & `alphaz-0.7.5.5/alphaz/config/config.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/config/main_configuration.py` & `alphaz-0.7.5.5/alphaz/config/main_configuration.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/config/page.py` & `alphaz-0.7.5.5/alphaz/config/page.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/config/source.html` & `alphaz-0.7.5.5/alphaz/config/source.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/config.json` & `alphaz-0.7.5.5/alphaz/config.json`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/docs/alpha_core.md` & `alphaz-0.7.5.5/alphaz/documentations/docs/alpha_core.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/docs/alpha_screens.md` & `alphaz-0.7.5.5/alphaz/documentations/docs/alpha_screens.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/docs/alpha_setup.md` & `alphaz-0.7.5.5/alphaz/documentations/docs/alpha_setup.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/docs/api/authorizations.md` & `alphaz-0.7.5.5/alphaz/documentations/docs/api/authorizations.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/docs/api/configuration.md` & `alphaz-0.7.5.5/alphaz/documentations/docs/api/configuration.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/docs/api/main.md` & `alphaz-0.7.5.5/alphaz/documentations/docs/api/main.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/docs/api/methods.md` & `alphaz-0.7.5.5/alphaz/documentations/docs/api/methods.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/docs/api/parameters.md` & `alphaz-0.7.5.5/alphaz/documentations/docs/api/parameters.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/docs/api/routes.md` & `alphaz-0.7.5.5/alphaz/documentations/docs/api/routes.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/docs/api_database.md` & `alphaz-0.7.5.5/alphaz/documentations/docs/api_database.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/docs/configuration.md` & `alphaz-0.7.5.5/alphaz/documentations/docs/configuration.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/docs/database/init.md` & `alphaz-0.7.5.5/alphaz/documentations/docs/database/init.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/docs/database/model.md` & `alphaz-0.7.5.5/alphaz/documentations/docs/database/model.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/docs/database/schema.md` & `alphaz-0.7.5.5/alphaz/documentations/docs/database/schema.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/docs/database/update.md` & `alphaz-0.7.5.5/alphaz/documentations/docs/database/update.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/docs/index.md` & `alphaz-0.7.5.5/alphaz/documentations/docs/index.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/mkdocs.yml` & `alphaz-0.7.5.5/alphaz/documentations/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/site/404.html` & `alphaz-0.7.5.5/alphaz/documentations/site/404.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/site/alpha_admin/index.html` & `alphaz-0.7.5.5/alphaz/documentations/site/alpha_admin/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/site/alpha_core/index.html` & `alphaz-0.7.5.5/alphaz/documentations/site/alpha_core/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/site/alpha_screens/index.html` & `alphaz-0.7.5.5/alphaz/documentations/site/alpha_screens/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/site/alpha_setup/index.html` & `alphaz-0.7.5.5/alphaz/documentations/site/alpha_setup/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/site/api/authorizations/index.html` & `alphaz-0.7.5.5/alphaz/documentations/site/api/authorizations/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/site/api/cache/index.html` & `alphaz-0.7.5.5/alphaz/documentations/site/api/cache/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/site/api/configuration/index.html` & `alphaz-0.7.5.5/alphaz/documentations/site/api/configuration/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/site/api/issues/index.html` & `alphaz-0.7.5.5/alphaz/documentations/site/api/issues/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/site/api/main/index.html` & `alphaz-0.7.5.5/alphaz/documentations/site/api/main/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/site/api/methods/index.html` & `alphaz-0.7.5.5/alphaz/documentations/site/api/methods/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/site/api/parameters/index.html` & `alphaz-0.7.5.5/alphaz/documentations/site/api/parameters/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/site/api/routes/index.html` & `alphaz-0.7.5.5/alphaz/documentations/site/api/routes/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/site/api/sqlalchemy/index.html` & `alphaz-0.7.5.5/alphaz/documentations/site/api/sqlalchemy/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/site/api_database/index.html` & `alphaz-0.7.5.5/alphaz/documentations/site/api_database/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/site/assets/images/favicon.png` & `alphaz-0.7.5.5/alphaz/documentations/site/assets/images/favicon.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js` & `alphaz-0.7.5.5/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js.map` & `alphaz-0.7.5.5/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js.map`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ar.min.js` & `alphaz-0.7.5.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ar.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.da.min.js` & `alphaz-0.7.5.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.da.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.de.min.js` & `alphaz-0.7.5.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.de.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.du.min.js` & `alphaz-0.7.5.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.du.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.es.min.js` & `alphaz-0.7.5.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.es.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fi.min.js` & `alphaz-0.7.5.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fi.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fr.min.js` & `alphaz-0.7.5.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fr.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.hu.min.js` & `alphaz-0.7.5.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.hu.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.it.min.js` & `alphaz-0.7.5.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.it.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ja.min.js` & `alphaz-0.7.5.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ja.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.multi.min.js` & `alphaz-0.7.5.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.multi.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.nl.min.js` & `alphaz-0.7.5.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.nl.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.no.min.js` & `alphaz-0.7.5.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.no.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.pt.min.js` & `alphaz-0.7.5.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.pt.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ro.min.js` & `alphaz-0.7.5.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ro.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ru.min.js` & `alphaz-0.7.5.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ru.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js` & `alphaz-0.7.5.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.sv.min.js` & `alphaz-0.7.5.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.sv.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.tr.min.js` & `alphaz-0.7.5.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.tr.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.vi.min.js` & `alphaz-0.7.5.5/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.vi.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/site/assets/javascripts/lunr/tinyseg.js` & `alphaz-0.7.5.5/alphaz/documentations/site/assets/javascripts/lunr/tinyseg.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js` & `alphaz-0.7.5.5/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js.map` & `alphaz-0.7.5.5/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js.map`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css` & `alphaz-0.7.5.5/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css.map` & `alphaz-0.7.5.5/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css.map`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css` & `alphaz-0.7.5.5/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css.map` & `alphaz-0.7.5.5/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css.map`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/site/configuration/index.html` & `alphaz-0.7.5.5/alphaz/documentations/site/configuration/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/site/database/init/index.html` & `alphaz-0.7.5.5/alphaz/documentations/site/database/init/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/site/database/instantiate/index.html` & `alphaz-0.7.5.5/alphaz/documentations/site/database/instantiate/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/site/database/main/index.html` & `alphaz-0.7.5.5/alphaz/documentations/site/database/main/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/site/database/model/index.html` & `alphaz-0.7.5.5/alphaz/documentations/site/database/model/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/site/database/relations/index.html` & `alphaz-0.7.5.5/alphaz/documentations/site/database/relations/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/site/database/schema/index.html` & `alphaz-0.7.5.5/alphaz/documentations/site/database/schema/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/site/database/update/index.html` & `alphaz-0.7.5.5/alphaz/documentations/site/database/update/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/site/documentation/index.html` & `alphaz-0.7.5.5/alphaz/documentations/site/documentation/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/site/index.html` & `alphaz-0.7.5.5/alphaz/documentations/site/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/site/search/search_index.json` & `alphaz-0.7.5.5/alphaz/documentations/site/search/search_index.json`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/documentations/site/sitemap.xml` & `alphaz-0.7.5.5/alphaz/documentations/site/sitemap.xml`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/index.html` & `alphaz-0.7.5.5/alphaz/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/libs/api_lib.py` & `alphaz-0.7.5.5/alphaz/libs/api_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/libs/barcode_lib.py` & `alphaz-0.7.5.5/alphaz/libs/barcode_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/libs/config_lib.py` & `alphaz-0.7.5.5/alphaz/libs/config_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/libs/converter_lib.py` & `alphaz-0.7.5.5/alphaz/libs/converter_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/libs/database_lib.py` & `alphaz-0.7.5.5/alphaz/libs/database_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/libs/date_lib.py` & `alphaz-0.7.5.5/alphaz/libs/date_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/libs/dict_lib.py` & `alphaz-0.7.5.5/alphaz/libs/dict_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/libs/emulation/vt102_lib.py` & `alphaz-0.7.5.5/alphaz/libs/emulation/vt102_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/libs/events.py` & `alphaz-0.7.5.5/alphaz/libs/events.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/libs/files_lib.py` & `alphaz-0.7.5.5/alphaz/libs/files_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/libs/flask_lib.py` & `alphaz-0.7.5.5/alphaz/libs/flask_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/libs/img_lib.py` & `alphaz-0.7.5.5/alphaz/libs/img_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/libs/io_lib.py` & `alphaz-0.7.5.5/alphaz/libs/io_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/libs/json_lib.py` & `alphaz-0.7.5.5/alphaz/libs/json_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/libs/logs_lib.py` & `alphaz-0.7.5.5/alphaz/libs/logs_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/libs/mail_lib.py` & `alphaz-0.7.5.5/alphaz/libs/mail_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/libs/notifications_lib.py` & `alphaz-0.7.5.5/alphaz/libs/notifications_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/libs/number_lib.py` & `alphaz-0.7.5.5/alphaz/libs/number_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/libs/process_lib.py` & `alphaz-0.7.5.5/alphaz/libs/process_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/libs/py_lib.py` & `alphaz-0.7.5.5/alphaz/libs/py_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/libs/scp_lib.py` & `alphaz-0.7.5.5/alphaz/libs/scp_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/libs/search_lib.py` & `alphaz-0.7.5.5/alphaz/libs/search_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/libs/secure_lib.py` & `alphaz-0.7.5.5/alphaz/libs/secure_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/libs/soap_lib.py` & `alphaz-0.7.5.5/alphaz/libs/soap_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/libs/ssh_lib.py` & `alphaz-0.7.5.5/alphaz/libs/ssh_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/libs/string_lib.py` & `alphaz-0.7.5.5/alphaz/libs/string_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/libs/test_lib.py` & `alphaz-0.7.5.5/alphaz/libs/test_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/libs/time_lib.py` & `alphaz-0.7.5.5/alphaz/libs/time_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/libs/transactions_lib.py` & `alphaz-0.7.5.5/alphaz/libs/transactions_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/libs/user_lib.py` & `alphaz-0.7.5.5/alphaz/libs/user_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/libs/user_management/application_management_lib.py` & `alphaz-0.7.5.5/alphaz/libs/user_management/application_management_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/libs/user_management/permission_management_lib.py` & `alphaz-0.7.5.5/alphaz/libs/user_management/permission_management_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/libs/user_management/role_management_lib.py` & `alphaz-0.7.5.5/alphaz/libs/user_management/role_management_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/libs/user_management/user_management_lib.py` & `alphaz-0.7.5.5/alphaz/libs/user_management/user_management_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/mails/Images/Background.png` & `alphaz-0.7.5.5/alphaz/mails/Images/Background.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/mails/Images/Facebook_logo.png` & `alphaz-0.7.5.5/alphaz/mails/Images/Facebook_logo.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/mails/Images/Twitter_logo.png` & `alphaz-0.7.5.5/alphaz/mails/Images/Twitter_logo.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/mails/Images/Web_logo.png` & `alphaz-0.7.5.5/alphaz/mails/Images/Web_logo.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/mails/Mail.png` & `alphaz-0.7.5.5/alphaz/mails/Mail.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/mails/Webmail.html` & `alphaz-0.7.5.5/alphaz/mails/Webmail.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/mails/debug.html` & `alphaz-0.7.5.5/alphaz/mails/debug.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/mails/mail.html` & `alphaz-0.7.5.5/alphaz/mails/mail.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/mails/password_reset.html` & `alphaz-0.7.5.5/alphaz/mails/password_reset.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/mails/stay_in_touch.html` & `alphaz-0.7.5.5/alphaz/mails/stay_in_touch.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/models/api/_answer.py` & `alphaz-0.7.5.5/alphaz/models/api/_answer.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/models/api/_colorations.py` & `alphaz-0.7.5.5/alphaz/models/api/_colorations.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/models/api/_parameter.py` & `alphaz-0.7.5.5/alphaz/models/api/_parameter.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/models/api/_requests.py` & `alphaz-0.7.5.5/alphaz/models/api/_requests.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/models/api/_route.py` & `alphaz-0.7.5.5/alphaz/models/api/_route.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/models/api/_structures.py` & `alphaz-0.7.5.5/alphaz/models/api/_structures.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/models/api/_utils.py` & `alphaz-0.7.5.5/alphaz/models/api/_utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/models/config/_config.py` & `alphaz-0.7.5.5/alphaz/models/config/_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/models/config/_utils.py` & `alphaz-0.7.5.5/alphaz/models/config/_utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/models/database/main_definitions.py` & `alphaz-0.7.5.5/alphaz/models/database/main_definitions.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/models/database/models.py` & `alphaz-0.7.5.5/alphaz/models/database/models.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/models/database/operators.py` & `alphaz-0.7.5.5/alphaz/models/database/operators.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/models/database/requests.py` & `alphaz-0.7.5.5/alphaz/models/database/requests.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/models/database/row.py` & `alphaz-0.7.5.5/alphaz/models/database/row.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/models/database/structure.py` & `alphaz-0.7.5.5/alphaz/models/database/structure.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/models/database/tests.py` & `alphaz-0.7.5.5/alphaz/models/database/tests.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/models/database/users_definitions.py` & `alphaz-0.7.5.5/alphaz/models/database/users_definitions.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/models/database/utils.py` & `alphaz-0.7.5.5/alphaz/models/database/utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/models/database/views.py` & `alphaz-0.7.5.5/alphaz/models/database/views.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/models/excel.py` & `alphaz-0.7.5.5/alphaz/models/excel.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/models/ftp.py` & `alphaz-0.7.5.5/alphaz/models/ftp.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/models/json/_converters.py` & `alphaz-0.7.5.5/alphaz/models/json/_converters.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/models/logger/_colorations.py` & `alphaz-0.7.5.5/alphaz/models/logger/_colorations.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/models/logger/_logger.py` & `alphaz-0.7.5.5/alphaz/models/logger/_logger.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/models/logger/_utils.py` & `alphaz-0.7.5.5/alphaz/models/logger/_utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/models/logs/main.log` & `alphaz-0.7.5.5/alphaz/models/logs/main.log`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/models/main/_base.py` & `alphaz-0.7.5.5/alphaz/models/main/_base.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/models/main/_core/_core.py` & `alphaz-0.7.5.5/alphaz/models/main/_core/_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -325,15 +325,17 @@
 
         # APM
         apm_config = self.config.get("apm", None)
         if apm_config is not None and apm_config.get("active", False):
             from alphaz.utils.apm import ora
             from elasticapm.contrib.flask import ElasticAPM
 
-            self.api.config["ELASTIC_APM"] = apm_config
+            self.api.config["ELASTIC_APM"] = {
+                x.upper(): y for x, y in apm_config.items()
+            }
             self.info(f"Starting apm with configuration {apm_config}...")
             self.apm = ElasticAPM(self.api)
 
         # if self.config.get("cors"):
         # CORS(self.api, resources={r"*": {"origins": "*"}}, supports_credentials=True)
         # logging.getLogger("flask_cors").level = logging.DEBUG
         self.api.config["CORS_HEADERS"] = "Content-Type"
```

### Comparing `alphaz-0.7.5.4/alphaz/models/main/_exception.py` & `alphaz-0.7.5.5/alphaz/models/main/_exception.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/models/main/_request.py` & `alphaz-0.7.5.5/alphaz/models/main/_request.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/models/main/_singleton.py` & `alphaz-0.7.5.5/alphaz/models/main/_singleton.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/models/request.py` & `alphaz-0.7.5.5/alphaz/models/request.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/models/tests/_category.py` & `alphaz-0.7.5.5/alphaz/models/tests/_category.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/models/tests/_group.py` & `alphaz-0.7.5.5/alphaz/models/tests/_group.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/models/tests/_method.py` & `alphaz-0.7.5.5/alphaz/models/tests/_method.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/models/tests/_save.py` & `alphaz-0.7.5.5/alphaz/models/tests/_save.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/models/tests/_test.py` & `alphaz-0.7.5.5/alphaz/models/tests/_test.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/models/tests/_wrappers.py` & `alphaz-0.7.5.5/alphaz/models/tests/_wrappers.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/models/user.py` & `alphaz-0.7.5.5/alphaz/models/user.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/models/watcher.py` & `alphaz-0.7.5.5/alphaz/models/watcher.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/pocs/main.py` & `alphaz-0.7.5.5/alphaz/pocs/main.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/run.py` & `alphaz-0.7.5.5/alphaz/run.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/src/alpha.png` & `alphaz-0.7.5.5/alphaz/src/alpha.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/src/configs/loggers.json` & `alphaz-0.7.5.5/alphaz/src/configs/loggers.json`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/stitch/Core.py` & `alphaz-0.7.5.5/alphaz/stitch/Core.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/stitch/stitch.py` & `alphaz-0.7.5.5/alphaz/stitch/stitch.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/stitch/web-drivers/chromedriver.exe` & `alphaz-0.7.5.5/alphaz/stitch/web-drivers/chromedriver.exe`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/stitch/web-drivers/geckodriver` & `alphaz-0.7.5.5/alphaz/stitch/web-drivers/geckodriver`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/templates/assets/css/home.css` & `alphaz-0.7.5.5/alphaz/templates/assets/css/home.css`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/templates/assets/css/logs.css` & `alphaz-0.7.5.5/alphaz/templates/assets/css/logs.css`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/templates/assets/images/icons/alpha.png` & `alphaz-0.7.5.5/alphaz/templates/assets/images/icons/alpha.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/templates/assets/images/icons/start-icon.png` & `alphaz-0.7.5.5/alphaz/templates/assets/images/icons/start-icon.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/templates/assets/images/icons/wsalpha.png` & `alphaz-0.7.5.5/alphaz/templates/assets/images/icons/wsalpha.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/templates/assets/images/loading.gif` & `alphaz-0.7.5.5/alphaz/templates/assets/images/loading.gif`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/templates/assets/js/libs/ansi_up.js` & `alphaz-0.7.5.5/alphaz/templates/assets/js/libs/ansi_up.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/templates/assets/js/libs/jquery.min.js` & `alphaz-0.7.5.5/alphaz/templates/assets/js/libs/jquery.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/templates/assets/js/logs.js` & `alphaz-0.7.5.5/alphaz/templates/assets/js/logs.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/templates/home.html` & `alphaz-0.7.5.5/alphaz/templates/home.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/templates/logs.html` & `alphaz-0.7.5.5/alphaz/templates/logs.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/test.py` & `alphaz-0.7.5.5/alphaz/test.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/tests/api.py` & `alphaz-0.7.5.5/alphaz/tests/api.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/tests/basic_test.py` & `alphaz-0.7.5.5/alphaz/tests/basic_test.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/tests/configurations.py` & `alphaz-0.7.5.5/alphaz/tests/configurations.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/tests/database.py` & `alphaz-0.7.5.5/alphaz/tests/database.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/tests/utils.py` & `alphaz-0.7.5.5/alphaz/tests/utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/utils/api.py` & `alphaz-0.7.5.5/alphaz/utils/api.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/utils/apm/ora.py` & `alphaz-0.7.5.5/alphaz/utils/apm/ora.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,45 +1,53 @@
+import re
 from elasticapm.instrumentation.packages.dbapi2 import (
     ConnectionProxy,
     CursorProxy,
     DbApi2Instrumentation,
     extract_signature,
 )
 from elasticapm.instrumentation import register
 from elasticapm.utils import default_ports
 
 
+def get_dsn_match(dsn: str, name: str, default=None) -> str:
+    matchs = re.findall(f"{name}\s+=\s+([^\)]*)\)", dsn)
+    return matchs[0] if len(matchs) != 0 else default
+
+
 class OracleCursorProxy(CursorProxy):
     provider_name = "oracle"
 
     def extract_signature(self, sql):
         return extract_signature(sql)
 
     @property
     def _self_database(self) -> str:
         # for unknown reasons, the connection is available as the `_connection` attribute on Python 3.6,
         # and as `_cnx` on later Python versions
-        return self.connection.dsn.split("SID=")[1].split(")")[0]
+        dsn = self.connection.dsn if hasattr(self, "connection") else ""
+        return get_dsn_match(dsn, "SID")
         # connection = getattr(self, "_cnx") or getattr(self, "_connection")
         # return connection.database if connection else ""
 
 
 class OracleConnectionProxy(ConnectionProxy):
     cursor_proxy = OracleCursorProxy
 
 
 class OracleInstrumentation(DbApi2Instrumentation):
     name = "oracle"
 
     instrument_list = [("cx_Oracle", "connect")]
 
     def call(self, module, method, wrapped, instance, args, kwargs):
+        dsn = kwargs.get("dsn", "")
         destination_info = {
-            "address": kwargs["dsn"].split("HOST=")[1].split(")")[0],
-            "port": int(kwargs["dsn"].split("PORT=")[1].split(")")[0]),
+            "address": get_dsn_match(dsn, "HOST"),
+            "port": int(get_dsn_match(dsn, "PORT", 0)),
         }
         return OracleConnectionProxy(
             wrapped(*args, **kwargs), destination_info=destination_info
         )
 
 
 register.register("alphaz.utils.apm.ora.OracleInstrumentation")
```

### Comparing `alphaz-0.7.5.4/alphaz/utils/configuration.py` & `alphaz-0.7.5.5/alphaz/utils/configuration.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/utils/database/init.py` & `alphaz-0.7.5.5/alphaz/utils/database/init.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/utils/database_to_dataclass.py` & `alphaz-0.7.5.5/alphaz/utils/database_to_dataclass.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/utils/decorators.py` & `alphaz-0.7.5.5/alphaz/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/utils/ensure.py` & `alphaz-0.7.5.5/alphaz/utils/ensure.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/utils/mep.py` & `alphaz-0.7.5.5/alphaz/utils/mep.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/utils/screens.py` & `alphaz-0.7.5.5/alphaz/utils/screens.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/utils/selectionMenu.py` & `alphaz-0.7.5.5/alphaz/utils/selectionMenu.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/utils/tasks.py` & `alphaz-0.7.5.5/alphaz/utils/tasks.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/utils/tests.py` & `alphaz-0.7.5.5/alphaz/utils/tests.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/utils/time.py` & `alphaz-0.7.5.5/alphaz/utils/time.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz/utils/transactions.py` & `alphaz-0.7.5.5/alphaz/utils/transactions.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/alphaz.egg-info/PKG-INFO` & `alphaz-0.7.5.5/alphaz.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: alphaz
-Version: 0.7.5.4
+Version: 0.7.5.5
 Summary: A package full of very nice tools
 Home-page: https://github.com/ZAurele/alphaz
 Author: Aurèle
 Author-email: contact@aurele.eu
 License: MIT
-Download-URL: https://github.com/ZAurele/alphaz/archive/refs/tags/0.7.5.4.tar.gz
+Download-URL: https://github.com/ZAurele/alphaz/archive/refs/tags/0.7.5.5.tar.gz
 Description: UNKNOWN
 Keywords: Flask,Json
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `alphaz-0.7.5.4/alphaz.egg-info/SOURCES.txt` & `alphaz-0.7.5.5/alphaz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.5.4/setup.py` & `alphaz-0.7.5.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os, glob, re
 from datetime import date
 
 today = date.today()
 
 from setuptools import setup, find_packages
 
-version = "0.7.5.4"
+version = "0.7.5.5"
 
 excludes = [".git", ".vscode"]
 
 archives = glob.glob("dist/*")
 for archive in archives:
     os.remove(archive)
```

