# Comparing `tmp/djaodjin-signup-0.7.7.tar.gz` & `tmp/djaodjin-signup-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djaodjin-signup-0.7.7.tar", last modified: Wed Jan 18 22:27:27 2023, max compression
+gzip compressed data, was "djaodjin-signup-0.8.0.tar", last modified: Fri Apr 21 16:42:23 2023, max compression
```

## Comparing `djaodjin-signup-0.7.7.tar` & `djaodjin-signup-0.8.0.tar`

### file list

```diff
@@ -1,104 +1,107 @@
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-01-18 22:27:27.792976 djaodjin-signup-0.7.7/
--rw-r--r--   0 smirolo    (501) staff       (20)     1318 2022-07-26 19:09:33.000000 djaodjin-signup-0.7.7/LICENSE.txt
--rw-r--r--   0 smirolo    (501) staff       (20)       35 2022-07-26 19:09:33.000000 djaodjin-signup-0.7.7/MANIFEST.in
--rw-r--r--   0 smirolo    (501) staff       (20)     3031 2023-01-18 22:27:27.793050 djaodjin-signup-0.7.7/PKG-INFO
--rw-r--r--   0 smirolo    (501) staff       (20)     2644 2023-01-18 22:26:08.000000 djaodjin-signup-0.7.7/README.md
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-01-18 22:27:27.777486 djaodjin-signup-0.7.7/djaodjin_signup.egg-info/
--rw-r--r--   0 smirolo    (501) staff       (20)     3031 2023-01-18 22:27:27.000000 djaodjin-signup-0.7.7/djaodjin_signup.egg-info/PKG-INFO
--rw-r--r--   0 smirolo    (501) staff       (20)     2431 2023-01-18 22:27:27.000000 djaodjin-signup-0.7.7/djaodjin_signup.egg-info/SOURCES.txt
--rw-r--r--   0 smirolo    (501) staff       (20)        1 2023-01-18 22:27:27.000000 djaodjin-signup-0.7.7/djaodjin_signup.egg-info/dependency_links.txt
--rw-r--r--   0 smirolo    (501) staff       (20)      234 2023-01-18 22:27:27.000000 djaodjin-signup-0.7.7/djaodjin_signup.egg-info/requires.txt
--rw-r--r--   0 smirolo    (501) staff       (20)        7 2023-01-18 22:27:27.000000 djaodjin-signup-0.7.7/djaodjin_signup.egg-info/top_level.txt
--rw-r--r--   0 smirolo    (501) staff       (20)      536 2022-10-24 20:19:41.000000 djaodjin-signup-0.7.7/requirements.txt
--rw-r--r--   0 smirolo    (501) staff       (20)       79 2023-01-18 22:27:27.793247 djaodjin-signup-0.7.7/setup.cfg
--rw-r--r--   0 smirolo    (501) staff       (20)     2629 2022-07-26 19:09:33.000000 djaodjin-signup-0.7.7/setup.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-01-18 22:27:27.782234 djaodjin-signup-0.7.7/signup/
--rw-r--r--   0 smirolo    (501) staff       (20)     1435 2023-01-18 22:26:30.000000 djaodjin-signup-0.7.7/signup/__init__.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-01-18 22:27:27.783538 djaodjin-signup-0.7.7/signup/api/
--rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:33.000000 djaodjin-signup-0.7.7/signup/api/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)    17009 2023-01-04 15:00:55.000000 djaodjin-signup-0.7.7/signup/api/auth.py
--rw-r--r--   0 smirolo    (501) staff       (20)     5142 2022-08-24 19:36:05.000000 djaodjin-signup-0.7.7/signup/api/contacts.py
--rw-r--r--   0 smirolo    (501) staff       (20)     5964 2022-08-10 04:22:51.000000 djaodjin-signup-0.7.7/signup/api/keys.py
--rw-r--r--   0 smirolo    (501) staff       (20)     4702 2022-08-10 04:23:07.000000 djaodjin-signup-0.7.7/signup/api/tokens.py
--rw-r--r--   0 smirolo    (501) staff       (20)    29628 2022-09-12 00:55:38.000000 djaodjin-signup-0.7.7/signup/api/users.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2265 2022-07-26 19:09:33.000000 djaodjin-signup-0.7.7/signup/auth.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2798 2022-07-26 19:09:33.000000 djaodjin-signup-0.7.7/signup/authentication.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-01-18 22:27:27.784750 djaodjin-signup-0.7.7/signup/backends/
--rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:33.000000 djaodjin-signup-0.7.7/signup/backends/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     5664 2022-07-26 19:09:33.000000 djaodjin-signup-0.7.7/signup/backends/auth.py
--rw-r--r--   0 smirolo    (501) staff       (20)     5352 2022-07-26 19:09:33.000000 djaodjin-signup-0.7.7/signup/backends/auth_ldap.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1908 2022-07-26 19:09:33.000000 djaodjin-signup-0.7.7/signup/backends/mfa.py
--rw-r--r--   0 smirolo    (501) staff       (20)    10329 2022-07-26 19:09:33.000000 djaodjin-signup-0.7.7/signup/backends/sts_credentials.py
--rw-r--r--   0 smirolo    (501) staff       (20)     3680 2022-09-12 04:09:41.000000 djaodjin-signup-0.7.7/signup/compat.py
--rw-r--r--   0 smirolo    (501) staff       (20)    10563 2022-09-12 04:18:03.000000 djaodjin-signup-0.7.7/signup/decorators.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2317 2022-07-26 19:09:33.000000 djaodjin-signup-0.7.7/signup/docs.py
--rw-r--r--   0 smirolo    (501) staff       (20)    12790 2022-09-12 04:25:19.000000 djaodjin-signup-0.7.7/signup/filters.py
--rw-r--r--   0 smirolo    (501) staff       (20)    17994 2023-01-18 03:16:18.000000 djaodjin-signup-0.7.7/signup/forms.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2883 2022-09-12 04:02:07.000000 djaodjin-signup-0.7.7/signup/helpers.py
--rw-r--r--   0 smirolo    (501) staff       (20)     4463 2022-10-18 18:39:14.000000 djaodjin-signup-0.7.7/signup/middleware.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-01-18 22:27:27.786540 djaodjin-signup-0.7.7/signup/migrations/
--rw-r--r--   0 smirolo    (501) staff       (20)     2953 2022-07-26 19:09:33.000000 djaodjin-signup-0.7.7/signup/migrations/0001_v0_1_9.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1093 2022-07-26 19:09:33.000000 djaodjin-signup-0.7.7/signup/migrations/0002_0_2_0.py
--rw-r--r--   0 smirolo    (501) staff       (20)      941 2022-07-26 19:09:33.000000 djaodjin-signup-0.7.7/signup/migrations/0003_0_2_1.py
--rw-r--r--   0 smirolo    (501) staff       (20)      595 2022-07-26 19:09:33.000000 djaodjin-signup-0.7.7/signup/migrations/0004_0_2_6.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1086 2022-07-26 19:09:33.000000 djaodjin-signup-0.7.7/signup/migrations/0005_0_2_8.py
--rw-r--r--   0 smirolo    (501) staff       (20)     4900 2022-07-26 19:09:33.000000 djaodjin-signup-0.7.7/signup/migrations/0006_v0_4_7.py
--rw-r--r--   0 smirolo    (501) staff       (20)      552 2022-09-07 17:51:52.000000 djaodjin-signup-0.7.7/signup/migrations/0007_v0_4_8.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1171 2022-07-26 19:09:33.000000 djaodjin-signup-0.7.7/signup/migrations/0008_v0_6_0.py
--rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:33.000000 djaodjin-signup-0.7.7/signup/migrations/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)    19405 2023-01-04 15:01:19.000000 djaodjin-signup-0.7.7/signup/mixins.py
--rw-r--r--   0 smirolo    (501) staff       (20)    32419 2022-09-12 04:03:06.000000 djaodjin-signup-0.7.7/signup/models.py
--rw-r--r--   0 smirolo    (501) staff       (20)     8606 2022-09-12 04:11:03.000000 djaodjin-signup-0.7.7/signup/serializers.py
--rw-r--r--   0 smirolo    (501) staff       (20)     7863 2022-09-12 17:12:06.000000 djaodjin-signup-0.7.7/signup/serializers_overrides.py
--rw-r--r--   0 smirolo    (501) staff       (20)     5737 2022-08-24 19:18:51.000000 djaodjin-signup-0.7.7/signup/settings.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1887 2022-07-26 19:09:33.000000 djaodjin-signup-0.7.7/signup/signals.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-01-18 22:27:27.775566 djaodjin-signup-0.7.7/signup/static/
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-01-18 22:27:27.787567 djaodjin-signup-0.7.7/signup/static/js/
--rw-r--r--   0 smirolo    (501) staff       (20)    14494 2022-07-26 19:09:33.000000 djaodjin-signup-0.7.7/signup/static/js/djaodjin-password-strength.js
--rw-r--r--   0 smirolo    (501) staff       (20)    50139 2022-12-07 06:03:58.000000 djaodjin-signup-0.7.7/signup/static/js/djaodjin-resources-vue.js
--rw-r--r--   0 smirolo    (501) staff       (20)     5924 2022-07-26 19:09:33.000000 djaodjin-signup-0.7.7/signup/static/js/djaodjin-resources.js
--rw-r--r--   0 smirolo    (501) staff       (20)    10225 2022-07-26 19:09:33.000000 djaodjin-signup-0.7.7/signup/static/js/djaodjin-signup-angular.js
--rw-r--r--   0 smirolo    (501) staff       (20)    10199 2022-07-26 19:09:33.000000 djaodjin-signup-0.7.7/signup/static/js/djaodjin-signup-vue.js
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-01-18 22:27:27.775759 djaodjin-signup-0.7.7/signup/templates/
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-01-18 22:27:27.788310 djaodjin-signup-0.7.7/signup/templates/accounts/
--rw-r--r--   0 smirolo    (501) staff       (20)      291 2022-07-26 19:09:33.000000 djaodjin-signup-0.7.7/signup/templates/accounts/disabled.html
--rw-r--r--   0 smirolo    (501) staff       (20)      696 2022-07-26 19:09:33.000000 djaodjin-signup-0.7.7/signup/templates/accounts/login.html
--rw-r--r--   0 smirolo    (501) staff       (20)      102 2022-07-26 19:09:33.000000 djaodjin-signup-0.7.7/signup/templates/accounts/logout.html
--rw-r--r--   0 smirolo    (501) staff       (20)      796 2022-07-26 19:09:33.000000 djaodjin-signup-0.7.7/signup/templates/accounts/recover.html
--rw-r--r--   0 smirolo    (501) staff       (20)      755 2022-07-26 19:09:33.000000 djaodjin-signup-0.7.7/signup/templates/accounts/register.html
--rw-r--r--   0 smirolo    (501) staff       (20)      362 2022-07-26 19:09:33.000000 djaodjin-signup-0.7.7/signup/templates/accounts/reset.html
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-01-18 22:27:27.788986 djaodjin-signup-0.7.7/signup/templates/notification/
--rw-r--r--   0 smirolo    (501) staff       (20)      247 2022-07-26 19:09:33.000000 djaodjin-signup-0.7.7/signup/templates/notification/password_reset.eml
--rw-r--r--   0 smirolo    (501) staff       (20)      221 2022-07-26 19:09:33.000000 djaodjin-signup-0.7.7/signup/templates/notification/user_activated.eml
--rw-r--r--   0 smirolo    (501) staff       (20)      207 2022-07-26 19:09:33.000000 djaodjin-signup-0.7.7/signup/templates/notification/user_registered.eml
--rw-r--r--   0 smirolo    (501) staff       (20)      241 2022-07-26 19:09:33.000000 djaodjin-signup-0.7.7/signup/templates/notification/verification.eml
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-01-18 22:27:27.789482 djaodjin-signup-0.7.7/signup/templates/users/
--rw-r--r--   0 smirolo    (501) staff       (20)     1990 2022-07-26 19:09:33.000000 djaodjin-signup-0.7.7/signup/templates/users/index.html
--rw-r--r--   0 smirolo    (501) staff       (20)      259 2022-07-26 19:09:33.000000 djaodjin-signup-0.7.7/signup/templates/users/notifications.html
--rw-r--r--   0 smirolo    (501) staff       (20)     1273 2022-07-26 19:09:33.000000 djaodjin-signup-0.7.7/signup/templates/users/password.html
--rw-r--r--   0 smirolo    (501) staff       (20)      871 2022-07-26 19:09:33.000000 djaodjin-signup-0.7.7/signup/templates/users/pubkey.html
--rw-r--r--   0 smirolo    (501) staff       (20)     5702 2022-07-26 19:09:33.000000 djaodjin-signup-0.7.7/signup/tests.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-01-18 22:27:27.789602 djaodjin-signup-0.7.7/signup/urls/
--rw-r--r--   0 smirolo    (501) staff       (20)     1564 2022-07-26 19:09:33.000000 djaodjin-signup-0.7.7/signup/urls/__init__.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-01-18 22:27:27.790873 djaodjin-signup-0.7.7/signup/urls/api/
--rw-r--r--   0 smirolo    (501) staff       (20)     1751 2022-07-26 19:09:33.000000 djaodjin-signup-0.7.7/signup/urls/api/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1541 2022-08-10 04:42:34.000000 djaodjin-signup-0.7.7/signup/urls/api/activate.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2108 2022-09-12 04:18:56.000000 djaodjin-signup-0.7.7/signup/urls/api/auth.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1906 2022-08-10 04:14:49.000000 djaodjin-signup-0.7.7/signup/urls/api/contacts.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1651 2022-08-10 04:15:39.000000 djaodjin-signup-0.7.7/signup/urls/api/keys.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1637 2022-08-10 04:16:27.000000 djaodjin-signup-0.7.7/signup/urls/api/tokens.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2044 2022-08-10 04:52:22.000000 djaodjin-signup-0.7.7/signup/urls/api/users.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-01-18 22:27:27.791824 djaodjin-signup-0.7.7/signup/urls/views/
--rw-r--r--   0 smirolo    (501) staff       (20)     1924 2022-10-19 16:04:48.000000 djaodjin-signup-0.7.7/signup/urls/views/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2759 2022-10-11 17:39:42.000000 djaodjin-signup-0.7.7/signup/urls/views/accounts.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1697 2022-07-26 19:09:33.000000 djaodjin-signup-0.7.7/signup/urls/views/contacts.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1469 2022-10-11 17:31:10.000000 djaodjin-signup-0.7.7/signup/urls/views/saml.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2156 2022-07-26 19:09:33.000000 djaodjin-signup-0.7.7/signup/urls/views/users.py
--rw-r--r--   0 smirolo    (501) staff       (20)     9219 2022-09-12 04:01:45.000000 djaodjin-signup-0.7.7/signup/utils.py
--rw-r--r--   0 smirolo    (501) staff       (20)     4288 2022-09-12 04:10:47.000000 djaodjin-signup-0.7.7/signup/validators.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-01-18 22:27:27.792751 djaodjin-signup-0.7.7/signup/views/
--rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:33.000000 djaodjin-signup-0.7.7/signup/views/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)    24846 2023-01-04 14:26:14.000000 djaodjin-signup-0.7.7/signup/views/auth.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2553 2022-07-26 19:09:33.000000 djaodjin-signup-0.7.7/signup/views/contacts.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1841 2022-10-11 17:37:03.000000 djaodjin-signup-0.7.7/signup/views/saml.py
--rw-r--r--   0 smirolo    (501) staff       (20)    11950 2023-01-18 03:28:49.000000 djaodjin-signup-0.7.7/signup/views/users.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-21 16:42:23.631610 djaodjin-signup-0.8.0/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1318 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.0/LICENSE.txt
+-rw-r--r--   0 smirolo    (501) staff       (20)       35 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.0/MANIFEST.in
+-rw-r--r--   0 smirolo    (501) staff       (20)     3468 2023-04-21 16:42:23.631704 djaodjin-signup-0.8.0/PKG-INFO
+-rw-r--r--   0 smirolo    (501) staff       (20)     2672 2023-04-21 16:39:38.000000 djaodjin-signup-0.8.0/README.md
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-21 16:42:23.612129 djaodjin-signup-0.8.0/djaodjin_signup.egg-info/
+-rw-r--r--   0 smirolo    (501) staff       (20)     3468 2023-04-21 16:42:23.000000 djaodjin-signup-0.8.0/djaodjin_signup.egg-info/PKG-INFO
+-rw-r--r--   0 smirolo    (501) staff       (20)     2517 2023-04-21 16:42:23.000000 djaodjin-signup-0.8.0/djaodjin_signup.egg-info/SOURCES.txt
+-rw-r--r--   0 smirolo    (501) staff       (20)        1 2023-04-21 16:42:23.000000 djaodjin-signup-0.8.0/djaodjin_signup.egg-info/dependency_links.txt
+-rw-r--r--   0 smirolo    (501) staff       (20)      300 2023-04-21 16:42:23.000000 djaodjin-signup-0.8.0/djaodjin_signup.egg-info/requires.txt
+-rw-r--r--   0 smirolo    (501) staff       (20)        7 2023-04-21 16:42:23.000000 djaodjin-signup-0.8.0/djaodjin_signup.egg-info/top_level.txt
+-rw-r--r--   0 smirolo    (501) staff       (20)     1951 2023-04-18 20:03:09.000000 djaodjin-signup-0.8.0/pyproject.toml
+-rw-r--r--   0 smirolo    (501) staff       (20)       79 2023-04-21 16:42:23.631940 djaodjin-signup-0.8.0/setup.cfg
+-rw-r--r--   0 smirolo    (501) staff       (20)     1381 2023-04-18 18:47:59.000000 djaodjin-signup-0.8.0/setup.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-21 16:42:23.617423 djaodjin-signup-0.8.0/signup/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1435 2023-04-21 16:37:19.000000 djaodjin-signup-0.8.0/signup/__init__.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-21 16:42:23.619075 djaodjin-signup-0.8.0/signup/api/
+-rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.0/signup/api/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     4728 2023-03-11 21:02:26.000000 djaodjin-signup-0.8.0/signup/api/activities.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    12165 2023-04-18 21:49:58.000000 djaodjin-signup-0.8.0/signup/api/auth.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     5142 2022-08-24 19:36:05.000000 djaodjin-signup-0.8.0/signup/api/contacts.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     5964 2023-04-14 19:38:34.000000 djaodjin-signup-0.8.0/signup/api/keys.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     4702 2022-08-10 04:23:07.000000 djaodjin-signup-0.8.0/signup/api/tokens.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    32773 2023-04-18 22:37:09.000000 djaodjin-signup-0.8.0/signup/api/users.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2265 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.0/signup/auth.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2798 2023-01-21 18:23:23.000000 djaodjin-signup-0.8.0/signup/authentication.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-21 16:42:23.620889 djaodjin-signup-0.8.0/signup/backends/
+-rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.0/signup/backends/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     5598 2023-02-15 03:47:01.000000 djaodjin-signup-0.8.0/signup/backends/auth.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     5325 2023-02-15 03:47:20.000000 djaodjin-signup-0.8.0/signup/backends/auth_ldap.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2346 2023-04-14 20:11:36.000000 djaodjin-signup-0.8.0/signup/backends/mfa.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    10329 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.0/signup/backends/sts_credentials.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     3680 2022-09-12 04:09:41.000000 djaodjin-signup-0.8.0/signup/compat.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    10578 2023-03-17 20:13:09.000000 djaodjin-signup-0.8.0/signup/decorators.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2317 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.0/signup/docs.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    12836 2023-04-08 20:24:46.000000 djaodjin-signup-0.8.0/signup/filters.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    17661 2023-04-08 20:23:45.000000 djaodjin-signup-0.8.0/signup/forms.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     3472 2023-02-14 01:47:15.000000 djaodjin-signup-0.8.0/signup/helpers.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     4463 2022-10-18 18:39:14.000000 djaodjin-signup-0.8.0/signup/middleware.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-21 16:42:23.622843 djaodjin-signup-0.8.0/signup/migrations/
+-rw-r--r--   0 smirolo    (501) staff       (20)     2953 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.0/signup/migrations/0001_v0_1_9.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1093 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.0/signup/migrations/0002_0_2_0.py
+-rw-r--r--   0 smirolo    (501) staff       (20)      941 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.0/signup/migrations/0003_0_2_1.py
+-rw-r--r--   0 smirolo    (501) staff       (20)      595 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.0/signup/migrations/0004_0_2_6.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1086 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.0/signup/migrations/0005_0_2_8.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     4912 2023-04-14 19:44:41.000000 djaodjin-signup-0.8.0/signup/migrations/0006_v0_4_7.py
+-rw-r--r--   0 smirolo    (501) staff       (20)      552 2022-09-07 17:51:52.000000 djaodjin-signup-0.8.0/signup/migrations/0007_v0_4_8.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1171 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.0/signup/migrations/0008_v0_6_0.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1830 2023-04-14 20:13:48.000000 djaodjin-signup-0.8.0/signup/migrations/0009_v0_8_0.py
+-rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.0/signup/migrations/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    24697 2023-04-12 16:34:55.000000 djaodjin-signup-0.8.0/signup/mixins.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    35455 2023-04-14 20:10:39.000000 djaodjin-signup-0.8.0/signup/models.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     9177 2023-04-12 16:28:00.000000 djaodjin-signup-0.8.0/signup/serializers.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     7863 2022-09-12 17:12:06.000000 djaodjin-signup-0.8.0/signup/serializers_overrides.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     6675 2023-04-16 21:58:55.000000 djaodjin-signup-0.8.0/signup/settings.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1887 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.0/signup/signals.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-21 16:42:23.610004 djaodjin-signup-0.8.0/signup/static/
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-21 16:42:23.624086 djaodjin-signup-0.8.0/signup/static/js/
+-rw-r--r--   0 smirolo    (501) staff       (20)    14494 2023-04-12 16:40:38.000000 djaodjin-signup-0.8.0/signup/static/js/djaodjin-password-strength.js
+-rw-r--r--   0 smirolo    (501) staff       (20)    51604 2023-04-14 17:35:46.000000 djaodjin-signup-0.8.0/signup/static/js/djaodjin-resources-vue.js
+-rw-r--r--   0 smirolo    (501) staff       (20)     5924 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.0/signup/static/js/djaodjin-resources.js
+-rw-r--r--   0 smirolo    (501) staff       (20)    10225 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.0/signup/static/js/djaodjin-signup-angular.js
+-rw-r--r--   0 smirolo    (501) staff       (20)    13054 2023-04-14 19:06:38.000000 djaodjin-signup-0.8.0/signup/static/js/djaodjin-signup-vue.js
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-21 16:42:23.610246 djaodjin-signup-0.8.0/signup/templates/
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-21 16:42:23.625585 djaodjin-signup-0.8.0/signup/templates/accounts/
+-rw-r--r--   0 smirolo    (501) staff       (20)      291 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.0/signup/templates/accounts/disabled.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      775 2023-03-16 16:54:13.000000 djaodjin-signup-0.8.0/signup/templates/accounts/login.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      102 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.0/signup/templates/accounts/logout.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      796 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.0/signup/templates/accounts/recover.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      755 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.0/signup/templates/accounts/register.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      362 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.0/signup/templates/accounts/reset.html
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-21 16:42:23.626544 djaodjin-signup-0.8.0/signup/templates/notification/
+-rw-r--r--   0 smirolo    (501) staff       (20)      247 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.0/signup/templates/notification/password_reset.eml
+-rw-r--r--   0 smirolo    (501) staff       (20)      221 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.0/signup/templates/notification/user_activated.eml
+-rw-r--r--   0 smirolo    (501) staff       (20)      207 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.0/signup/templates/notification/user_registered.eml
+-rw-r--r--   0 smirolo    (501) staff       (20)      241 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.0/signup/templates/notification/verification.eml
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-21 16:42:23.627268 djaodjin-signup-0.8.0/signup/templates/users/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1465 2023-03-02 23:05:43.000000 djaodjin-signup-0.8.0/signup/templates/users/index.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      259 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.0/signup/templates/users/notifications.html
+-rw-r--r--   0 smirolo    (501) staff       (20)     2856 2023-04-14 19:13:40.000000 djaodjin-signup-0.8.0/signup/templates/users/password.html
+-rw-r--r--   0 smirolo    (501) staff       (20)     1839 2023-02-15 21:47:15.000000 djaodjin-signup-0.8.0/signup/templates/users/pubkey.html
+-rw-r--r--   0 smirolo    (501) staff       (20)     5702 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.0/signup/tests.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-21 16:42:23.627493 djaodjin-signup-0.8.0/signup/urls/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1551 2023-02-14 15:00:54.000000 djaodjin-signup-0.8.0/signup/urls/__init__.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-21 16:42:23.629182 djaodjin-signup-0.8.0/signup/urls/api/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1751 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.0/signup/urls/api/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1541 2022-08-10 04:42:34.000000 djaodjin-signup-0.8.0/signup/urls/api/activate.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1926 2023-03-08 02:03:00.000000 djaodjin-signup-0.8.0/signup/urls/api/activities.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1857 2023-03-02 05:24:17.000000 djaodjin-signup-0.8.0/signup/urls/api/auth.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1906 2022-08-10 04:14:49.000000 djaodjin-signup-0.8.0/signup/urls/api/contacts.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1651 2022-08-10 04:15:39.000000 djaodjin-signup-0.8.0/signup/urls/api/keys.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1637 2022-08-10 04:16:27.000000 djaodjin-signup-0.8.0/signup/urls/api/tokens.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2165 2023-04-05 22:33:04.000000 djaodjin-signup-0.8.0/signup/urls/api/users.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-21 16:42:23.630288 djaodjin-signup-0.8.0/signup/urls/views/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1924 2022-10-19 16:04:48.000000 djaodjin-signup-0.8.0/signup/urls/views/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2545 2023-03-02 05:23:57.000000 djaodjin-signup-0.8.0/signup/urls/views/accounts.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1649 2023-03-04 00:46:08.000000 djaodjin-signup-0.8.0/signup/urls/views/contacts.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1469 2022-10-11 17:31:10.000000 djaodjin-signup-0.8.0/signup/urls/views/saml.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2031 2023-04-05 22:31:53.000000 djaodjin-signup-0.8.0/signup/urls/views/users.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     9044 2023-04-11 21:48:35.000000 djaodjin-signup-0.8.0/signup/utils.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     4272 2023-02-15 03:45:50.000000 djaodjin-signup-0.8.0/signup/validators.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-21 16:42:23.631393 djaodjin-signup-0.8.0/signup/views/
+-rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.0/signup/views/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    16542 2023-04-14 20:11:15.000000 djaodjin-signup-0.8.0/signup/views/auth.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2739 2023-02-15 03:48:21.000000 djaodjin-signup-0.8.0/signup/views/contacts.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1903 2023-02-15 03:50:06.000000 djaodjin-signup-0.8.0/signup/views/saml.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    12714 2023-04-06 00:58:50.000000 djaodjin-signup-0.8.0/signup/views/users.py
```

### Comparing `djaodjin-signup-0.7.7/LICENSE.txt` & `djaodjin-signup-0.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.7.7/PKG-INFO` & `djaodjin-signup-0.8.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,25 @@
 Metadata-Version: 2.1
 Name: djaodjin-signup
-Version: 0.7.7
-Summary: DjaoDjin's Implementation of Frictionless Sign Up
-Home-page: https://github.com/djaodjin/djaodjin-signup/
-Download-URL: https://github.com/djaodjin/djaodjin-signup/tarball/0.7.7
-Author: The DjaoDjin Team
-Author-email: support@djaodjin.com
-License: BSD
+Version: 0.8.0
+Summary: Django app for user authentication
+Author-email: The DjaoDjin Team <help@djaodjin.com>
+Maintainer-email: The DjaoDjin Team <help@djaodjin.com>
+License: BSD-2-Clause
+Project-URL: repository, https://github.com/djaodjin/djaodjin-signup
+Project-URL: documentation, https://djaodjin-signup.readthedocs.io/
+Project-URL: changelog, https://github.com/djaodjin/djaodjin-signup/changelog
+Keywords: signup,authentication,frictionless,2fa,mfa,otp,oauth,saml
+Classifier: Framework :: Django
+Classifier: Environment :: Web Environment
+Classifier: Programming Language :: Python
+Classifier: License :: OSI Approved :: BSD License
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: ldap
 License-File: LICENSE.txt
 
 This code a frictionless signup Django app.
 
 The app will register and login a user with as little as only an email address.
 
 When the user logs out and tries to logs back in with the same email address,
@@ -19,20 +27,14 @@
 to the registered email address. Setting the password is deferred to after
 the email address has been verified.
 
 If during the first login and/or subsequent login, the email address should
 be verified before moving forward (ex: before presenting a payment view),
 you should decorate the view with an *active_required* decorator.
 
-Tested with
-
-- **Python:** 3.7, **Django:** 3.2 ([LTS](https://www.djangoproject.com/download/)), **Django Rest Framework:** 3.12
-- **Python:** 3.10, **Django:** 4.0 (latest), **Django Rest Framework:** 3.12 - see [#55](https://github.com/djaodjin/djaodjin-signup/issues/55)
-- **Python:** 2.7, **Django:** 1.11 (legacy), **Django Rest Framework:** 3.9.4
-
 This project contains bare bone templates which are compatible with Django
 and Jinja2 template engines. To see djaodjin-signup in action as part
 of a full-fledged subscription-based session proxy, take a look
 at [djaoapp](https://github.com/djaodjin/djaoapp/).
 
 
 Install
@@ -78,12 +80,20 @@
     $ python manage.py runserver
 
     # Browse http://localhost:8000/
 
 Release Notes
 =============
 
-0.7.7
+Tested with
+
+- **Python:** 3.7, **Django:** 3.2 ([LTS](https://www.djangoproject.com/download/)), **Django Rest Framework:** 3.12
+- **Python:** 3.10, **Django:** 4.2 (latest) - see [#55](https://github.com/djaodjin/djaodjin-signup/issues/55)
+- **Python:** 2.7, **Django:** 1.11 (legacy) - use testsite/requirements-legacy.txt
+
+0.8.0
 
-  * fixes showing notification summary/description on users notifications page
+  * publishes distribution using pyproject.toml
+  * enables/disables OTP 2FA through user profile
+  * moves API keys to their own page
 
 [previous release notes](changelog)
```

### Comparing `djaodjin-signup-0.7.7/README.md` & `djaodjin-signup-0.8.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -7,20 +7,14 @@
 to the registered email address. Setting the password is deferred to after
 the email address has been verified.
 
 If during the first login and/or subsequent login, the email address should
 be verified before moving forward (ex: before presenting a payment view),
 you should decorate the view with an *active_required* decorator.
 
-Tested with
-
-- **Python:** 3.7, **Django:** 3.2 ([LTS](https://www.djangoproject.com/download/)), **Django Rest Framework:** 3.12
-- **Python:** 3.10, **Django:** 4.0 (latest), **Django Rest Framework:** 3.12 - see [#55](https://github.com/djaodjin/djaodjin-signup/issues/55)
-- **Python:** 2.7, **Django:** 1.11 (legacy), **Django Rest Framework:** 3.9.4
-
 This project contains bare bone templates which are compatible with Django
 and Jinja2 template engines. To see djaodjin-signup in action as part
 of a full-fledged subscription-based session proxy, take a look
 at [djaoapp](https://github.com/djaodjin/djaoapp/).
 
 
 Install
@@ -66,12 +60,20 @@
     $ python manage.py runserver
 
     # Browse http://localhost:8000/
 
 Release Notes
 =============
 
-0.7.7
+Tested with
+
+- **Python:** 3.7, **Django:** 3.2 ([LTS](https://www.djangoproject.com/download/)), **Django Rest Framework:** 3.12
+- **Python:** 3.10, **Django:** 4.2 (latest) - see [#55](https://github.com/djaodjin/djaodjin-signup/issues/55)
+- **Python:** 2.7, **Django:** 1.11 (legacy) - use testsite/requirements-legacy.txt
+
+0.8.0
 
-  * fixes showing notification summary/description on users notifications page
+  * publishes distribution using pyproject.toml
+  * enables/disables OTP 2FA through user profile
+  * moves API keys to their own page
 
 [previous release notes](changelog)
```

### Comparing `djaodjin-signup-0.7.7/djaodjin_signup.egg-info/PKG-INFO` & `djaodjin-signup-0.8.0/djaodjin_signup.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,25 @@
 Metadata-Version: 2.1
 Name: djaodjin-signup
-Version: 0.7.7
-Summary: DjaoDjin's Implementation of Frictionless Sign Up
-Home-page: https://github.com/djaodjin/djaodjin-signup/
-Download-URL: https://github.com/djaodjin/djaodjin-signup/tarball/0.7.7
-Author: The DjaoDjin Team
-Author-email: support@djaodjin.com
-License: BSD
+Version: 0.8.0
+Summary: Django app for user authentication
+Author-email: The DjaoDjin Team <help@djaodjin.com>
+Maintainer-email: The DjaoDjin Team <help@djaodjin.com>
+License: BSD-2-Clause
+Project-URL: repository, https://github.com/djaodjin/djaodjin-signup
+Project-URL: documentation, https://djaodjin-signup.readthedocs.io/
+Project-URL: changelog, https://github.com/djaodjin/djaodjin-signup/changelog
+Keywords: signup,authentication,frictionless,2fa,mfa,otp,oauth,saml
+Classifier: Framework :: Django
+Classifier: Environment :: Web Environment
+Classifier: Programming Language :: Python
+Classifier: License :: OSI Approved :: BSD License
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: ldap
 License-File: LICENSE.txt
 
 This code a frictionless signup Django app.
 
 The app will register and login a user with as little as only an email address.
 
 When the user logs out and tries to logs back in with the same email address,
@@ -19,20 +27,14 @@
 to the registered email address. Setting the password is deferred to after
 the email address has been verified.
 
 If during the first login and/or subsequent login, the email address should
 be verified before moving forward (ex: before presenting a payment view),
 you should decorate the view with an *active_required* decorator.
 
-Tested with
-
-- **Python:** 3.7, **Django:** 3.2 ([LTS](https://www.djangoproject.com/download/)), **Django Rest Framework:** 3.12
-- **Python:** 3.10, **Django:** 4.0 (latest), **Django Rest Framework:** 3.12 - see [#55](https://github.com/djaodjin/djaodjin-signup/issues/55)
-- **Python:** 2.7, **Django:** 1.11 (legacy), **Django Rest Framework:** 3.9.4
-
 This project contains bare bone templates which are compatible with Django
 and Jinja2 template engines. To see djaodjin-signup in action as part
 of a full-fledged subscription-based session proxy, take a look
 at [djaoapp](https://github.com/djaodjin/djaoapp/).
 
 
 Install
@@ -78,12 +80,20 @@
     $ python manage.py runserver
 
     # Browse http://localhost:8000/
 
 Release Notes
 =============
 
-0.7.7
+Tested with
+
+- **Python:** 3.7, **Django:** 3.2 ([LTS](https://www.djangoproject.com/download/)), **Django Rest Framework:** 3.12
+- **Python:** 3.10, **Django:** 4.2 (latest) - see [#55](https://github.com/djaodjin/djaodjin-signup/issues/55)
+- **Python:** 2.7, **Django:** 1.11 (legacy) - use testsite/requirements-legacy.txt
+
+0.8.0
 
-  * fixes showing notification summary/description on users notifications page
+  * publishes distribution using pyproject.toml
+  * enables/disables OTP 2FA through user profile
+  * moves API keys to their own page
 
 [previous release notes](changelog)
```

### Comparing `djaodjin-signup-0.7.7/djaodjin_signup.egg-info/SOURCES.txt` & `djaodjin-signup-0.8.0/djaodjin_signup.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 LICENSE.txt
 MANIFEST.in
 README.md
-requirements.txt
+pyproject.toml
 setup.cfg
 setup.py
 djaodjin_signup.egg-info/PKG-INFO
 djaodjin_signup.egg-info/SOURCES.txt
 djaodjin_signup.egg-info/dependency_links.txt
 djaodjin_signup.egg-info/requires.txt
 djaodjin_signup.egg-info/top_level.txt
@@ -25,14 +25,15 @@
 signup/serializers_overrides.py
 signup/settings.py
 signup/signals.py
 signup/tests.py
 signup/utils.py
 signup/validators.py
 signup/api/__init__.py
+signup/api/activities.py
 signup/api/auth.py
 signup/api/contacts.py
 signup/api/keys.py
 signup/api/tokens.py
 signup/api/users.py
 signup/backends/__init__.py
 signup/backends/auth.py
@@ -43,14 +44,15 @@
 signup/migrations/0002_0_2_0.py
 signup/migrations/0003_0_2_1.py
 signup/migrations/0004_0_2_6.py
 signup/migrations/0005_0_2_8.py
 signup/migrations/0006_v0_4_7.py
 signup/migrations/0007_v0_4_8.py
 signup/migrations/0008_v0_6_0.py
+signup/migrations/0009_v0_8_0.py
 signup/migrations/__init__.py
 signup/static/js/djaodjin-password-strength.js
 signup/static/js/djaodjin-resources-vue.js
 signup/static/js/djaodjin-resources.js
 signup/static/js/djaodjin-signup-angular.js
 signup/static/js/djaodjin-signup-vue.js
 signup/templates/accounts/disabled.html
@@ -66,14 +68,15 @@
 signup/templates/users/index.html
 signup/templates/users/notifications.html
 signup/templates/users/password.html
 signup/templates/users/pubkey.html
 signup/urls/__init__.py
 signup/urls/api/__init__.py
 signup/urls/api/activate.py
+signup/urls/api/activities.py
 signup/urls/api/auth.py
 signup/urls/api/contacts.py
 signup/urls/api/keys.py
 signup/urls/api/tokens.py
 signup/urls/api/users.py
 signup/urls/views/__init__.py
 signup/urls/views/accounts.py
```

### Comparing `djaodjin-signup-0.7.7/signup/__init__.py` & `djaodjin-signup-0.8.0/signup/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 # ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 """
 PEP 386-compliant version number for the signup django app.
 """
 
-__version__ = '0.7.7'
+__version__ = '0.8.0'
```

### Comparing `djaodjin-signup-0.7.7/signup/api/auth.py` & `djaodjin-signup-0.8.0/signup/api/auth.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022, DjaoDjin inc.
+# Copyright (c) 2023, DjaoDjin inc.
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice,
 #    this list of conditions and the following disclaimer.
@@ -20,64 +20,51 @@
 # OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
 # OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 # ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import logging
 
-from django.contrib.auth import (get_user_model,
-    authenticate, login as auth_login, logout as auth_logout)
+from django.contrib.auth import get_user_model, logout as auth_logout
 from django.contrib.auth.tokens import default_token_generator
-from django.utils.http import urlsafe_base64_decode
 import jwt
 from rest_framework import exceptions, permissions, status, serializers
-from rest_framework.generics import GenericAPIView, CreateAPIView
+from rest_framework.generics import GenericAPIView
 from rest_framework.response import Response
 
 
 from .. import settings
-from ..compat import gettext_lazy as _, six
+from ..compat import gettext_lazy as _
 from ..docs import OpenAPIResponse, no_body, swagger_auto_schema
 from ..helpers import as_timestamp, datetime_or_now
-from ..mixins import (ActivateMixin, LoginMixin, RecoverMixin, RegisterMixin,
-    SSORequired)
+from ..mixins import (LoginMixin, RegisterMixin, VerifyMixin,
+    VerifyCompleteMixin, SSORequired)
 from ..models import Contact
 from ..serializers_overrides import UserDetailSerializer
-from ..serializers import (ActivateSerializer, CredentialsSerializer,
-    PasswordResetSerializer, PasswordResetConfirmSerializer,
-    TokenSerializer, UserCreateSerializer, ValidationErrorSerializer)
-from ..utils import get_disabled_authentication, get_disabled_registration
+from ..serializers import (CredentialsSerializer,
+    RecoverSerializer, TokenSerializer, UserActivateSerializer,
+    UserCreateSerializer, ValidationErrorSerializer)
+from ..utils import get_disabled_registration
 
 
 LOGGER = logging.getLogger(__name__)
 
 
-class AllowAuthenticationEnabled(permissions.BasePermission):
-    """
-    Allows access only authentication is not disabled.
-    """
-    message = _("authentication has been temporarly disabled.")
-
-    def has_permission(self, request, view):
-        return not get_disabled_authentication(request)
-
-
 class AllowRegistrationEnabled(permissions.BasePermission):
     """
     Allows access only when registration is not disabled.
     """
     message = _("registration is disabled.")
 
     def has_permission(self, request, view):
         return not get_disabled_registration(request)
 
 
 class JWTBase(GenericAPIView):
 
-    permission_classes = [AllowAuthenticationEnabled]
     serializer_class = TokenSerializer
 
     def create_token(self, user, expires_at=None):
         if not expires_at:
             exp = (as_timestamp(datetime_or_now())
                 + self.request.session.get_expiry_age())
         else:
@@ -87,133 +74,24 @@
         token = jwt.encode(payload, settings.JWT_SECRET_KEY,
             settings.JWT_ALGORITHM)
         try:
             token = token.decode('utf-8')
         except AttributeError:
             # PyJWT==2.0.1 already returns an oject of type `str`.
             pass
-        LOGGER.info("%s signed in.", user,
-            extra={'event': 'login', 'request': self.request})
         return Response(TokenSerializer().to_representation({'token': token}),
             status=status.HTTP_201_CREATED)
 
-    @staticmethod
-    def optional_session_cookie(request, user):
-        if request.query_params.get('cookie', False):
-            auth_login(request, user)
-
     def permission_denied(self, request, message=None, code=None):
         # We override this function from `APIView`. The request will never
         # be authenticated by definition since we are dealing with login
         # and register APIs.
         raise exceptions.PermissionDenied(detail=message)
 
 
-class JWTActivate(ActivateMixin, JWTBase):
-    """
-    Retrieves an activation key
-
-    This API is typically used to pre-populate a registration form
-    when a user was invited to the site by another user.
-
-    The response is usually presented in an HTML
-    `activate page </docs/guides/themes/#workflow_activate>`_
-    as present in the default theme.
-
-    **Tags: auth, visitor, usermodel
-
-    **Example
-
-    .. code-block:: http
-
-        GET /api/auth/activate/16793aa72a4c7ae94b50b20c2eca52df5b0fe2c6\
- HTTP/1.1
-
-    responds
-
-    .. code-block:: json
-
-        {
-          "slug": "joe1",
-          "username": "joe1",
-          "email": "joe1@localhost.localdomain",
-          "full_name": "Joe Act",
-          "printable_name": "Joe Act",
-          "created_at": "2020-05-30T00:00:00Z"
-        }
-    """
-    model = get_user_model()
-    serializer_class = ActivateSerializer
-
-    def get_serializer_class(self):
-        if self.request.method.lower() == 'get':
-            return UserDetailSerializer
-        return super(JWTActivate, self).get_serializer_class()
-
-    def get(self, request, *args, **kwargs):#pylint:disable=unused-argument
-        verification_key = self.kwargs.get(self.key_url_kwarg)
-        token = Contact.objects.get_token(verification_key=verification_key)
-        if not token:
-            raise serializers.ValidationError({'detail': "invalid request"})
-        serializer = self.get_serializer(token.user)
-        return Response(serializer.data)
-
-    @swagger_auto_schema(responses={
-        201: OpenAPIResponse("", TokenSerializer),
-        400: OpenAPIResponse("parameters error", ValidationErrorSerializer)})
-    def post(self, request, *args, **kwargs):#pylint:disable=unused-argument
-        """
-        Activates a user
-
-        Activates a new user and returns a JSON Web Token that can subsequently
-        be used to authenticate the new user in HTTP requests.
-
-        **Tags: auth, visitor, usermodel
-
-        **Example
-
-        .. code-block:: http
-
-            POST /api/auth/activate/16793aa72a4c7ae94b50b20c2eca52df5b0fe2c6\
- HTTP/1.1
-
-        .. code-block:: json
-
-            {
-              "username": "joe1",
-              "new_password": "yoyo",
-              "full_name": "Joe Card1"
-            }
-
-        responds
-
-        .. code-block:: json
-
-            {
-                "token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJ1c2VybmFtZSI6\
-    ImpvZTEiLCJlbWFpbCI6ImpvZSsxQGRqYW9kamluLmNvbSIsImZ1bGxfbmFtZ\
-    SI6IkpvZSAgQ2FyZDEiLCJleHAiOjE1Mjk2NTUyMjR9.GFxjU5AvcCQbVylF1P\
-    JwcBUUMECj8AKxsHtRHUSypco"
-            }
-        """
-        serializer = self.get_serializer(data=request.data)
-        if serializer.is_valid():
-            # We are not using `is_valid(raise_exception=True)` here
-            # because we do not want to give clues on the reasons for failure.
-            user = self.activate_user(**serializer.validated_data)
-            if user:
-                # Okay, security check complete. Log the user in.
-                user_with_backend = authenticate(
-                    request, username=user.username,
-                    password=serializer.validated_data.get('new_password'))
-                self.optional_session_cookie(request, user_with_backend)
-                return self.create_token(user_with_backend)
-        raise serializers.ValidationError({'detail': "invalid request"})
-
-
 class JWTLogin(LoginMixin, JWTBase):
     """
     Authenticates a user
 
     Returns a JSON Web Token that can be used in HTTP requests that require
     authentication.
 
@@ -249,164 +127,175 @@
     model = get_user_model()
     serializer_class = CredentialsSerializer
 
     @swagger_auto_schema(responses={
         201: OpenAPIResponse("", TokenSerializer),
         400: OpenAPIResponse("parameters error", ValidationErrorSerializer)})
     def post(self, request, *args, **kwargs):
-        #pylint:disable=unused-argument,too-many-nested-blocks
-        serializer = self.get_serializer(data=request.data)
-        if serializer.is_valid():
-            try:
-                user = self.login_user(**serializer.validated_data)
-                if user:
-                    self.optional_session_cookie(request, user)
-                    return self.create_token(user)
-            except SSORequired as err:
-                raise serializers.ValidationError({'detail': _(
-                    "SSO required through %(provider)s") % {
-                        'provider': err.printable_name},
+        try:
+            user_with_backend = self.run_pipeline()
+            return self.create_token(user_with_backend)
+        except SSORequired as err:
+            raise serializers.ValidationError({'detail': _(
+                "SSO required through %(provider)s") % {
+                    'provider': err.printable_name},
                     'provider': err.delegate_auth.provider,
                     'url': self.request.build_absolute_uri(err.url)})
 
         raise exceptions.PermissionDenied()
 
 
-class JWTPasswordResetConfirm(JWTBase):
+class JWTRegister(RegisterMixin, JWTBase):
     """
-    Confirms a password reset
+    Registers a user
 
-    Sets a new password after a recover password was triggered
-    and returns a JSON Web Token that can subsequently
+    Creates a new user and returns a JSON Web Token that can subsequently
     be used to authenticate the new user in HTTP requests.
 
     The API is typically used within an HTML
-    `reset password page </docs/guides/themes/#workflow_reset>`_
+    `register page </docs/guides/themes/#workflow_register>`_
     as present in the default theme.
 
     **Tags: auth, visitor, usermodel
 
     **Example
 
     .. code-block:: http
 
-        POST /api/auth/reset/0123456789abcef0123456789abcef/abc123 HTTP/1.1
+        POST /api/auth/register HTTP/1.1
 
     .. code-block:: json
 
         {
-          "new_password": "yoyo"
+          "email": "joe+1@example.com",
+          "full_name": "Joe Card1",
+          "new_password": "yoyo",
+          "username": "joe1"
         }
 
     responds
 
     .. code-block:: json
 
         {
             "token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJ1c2VybmFtZSI6\
 ImpvZTEiLCJlbWFpbCI6ImpvZSsxQGRqYW9kamluLmNvbSIsImZ1bGxfbmFtZ\
 SI6IkpvZSAgQ2FyZDEiLCJleHAiOjE1Mjk2NTUyMjR9.GFxjU5AvcCQbVylF1P\
 JwcBUUMECj8AKxsHtRHUSypco"
         }
     """
     model = get_user_model()
-    serializer_class = PasswordResetConfirmSerializer
-    token_generator = default_token_generator
+    permission_classes = [AllowRegistrationEnabled]
+    serializer_class = UserCreateSerializer
 
     @swagger_auto_schema(responses={
         201: OpenAPIResponse("", TokenSerializer),
         400: OpenAPIResponse("parameters error", ValidationErrorSerializer)})
     def post(self, request, *args, **kwargs):#pylint:disable=unused-argument
-        serializer = self.get_serializer(data=request.data)
-        if serializer.is_valid():
-            # We are not using `is_valid(raise_exception=True)` here
-            # because we do not want to give clues on the reasons for failure.
-            try:
-                uid = urlsafe_base64_decode(self.kwargs.get('uidb64'))
-                if not isinstance(uid, six.string_types):
-                    # See Django2.2 release notes
-                    uid = uid.decode()
-                user = self.model.objects.get(pk=uid)
-            except (TypeError, ValueError, OverflowError,
-                    self.model.DoesNotExist):
-                user = None
-            if user is not None and self.token_generator.check_token(
-                                        user, self.kwargs.get('token')):
-                new_password = serializer.validated_data['new_password']
-                user.set_password(new_password)
-                user.save()
-                LOGGER.info("%s reset her/his password.", user,
-                    extra={'event': 'resetpassword', 'request': request})
-                user_with_backend = authenticate(
-                    request, username=user.username, password=new_password)
-                self.optional_session_cookie(request, user_with_backend)
-                return self.create_token(user_with_backend)
+        try:
+            user_with_backend = self.run_pipeline()
+            return self.create_token(user_with_backend)
+        except SSORequired as err:
+            raise serializers.ValidationError({'detail': _(
+                "SSO required through %(provider)s") % {
+                    'provider': err.printable_name},
+                    'provider': err.delegate_auth.provider,
+                    'url': self.request.build_absolute_uri(err.url)})
+
         raise serializers.ValidationError({'detail': "invalid request"})
 
 
-class JWTRegister(RegisterMixin, JWTBase):
+class JWTActivate(VerifyCompleteMixin, JWTRegister):
     """
-    Registers a user
+    Retrieves an activation key
 
-    Creates a new user and returns a JSON Web Token that can subsequently
-    be used to authenticate the new user in HTTP requests.
+    This API is typically used to pre-populate a registration form
+    when a user was invited to the site by another user.
 
-    The API is typically used within an HTML
-    `register page </docs/guides/themes/#workflow_register>`_
+    The response is usually presented in an HTML
+    `activate page </docs/guides/themes/#workflow_activate>`_
     as present in the default theme.
 
     **Tags: auth, visitor, usermodel
 
     **Example
 
     .. code-block:: http
 
-        POST /api/auth/register HTTP/1.1
-
-    .. code-block:: json
-
-        {
-          "username": "joe1",
-          "password": "yoyo",
-          "email": "joe+1@example.com",
-          "full_name": "Joe Card1"
-        }
+        GET /api/auth/activate/16793aa72a4c7ae94b50b20c2eca52df5b0fe2c6\
+ HTTP/1.1
 
     responds
 
     .. code-block:: json
 
         {
-            "token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJ1c2VybmFtZSI6\
-ImpvZTEiLCJlbWFpbCI6ImpvZSsxQGRqYW9kamluLmNvbSIsImZ1bGxfbmFtZ\
-SI6IkpvZSAgQ2FyZDEiLCJleHAiOjE1Mjk2NTUyMjR9.GFxjU5AvcCQbVylF1P\
-JwcBUUMECj8AKxsHtRHUSypco"
+          "slug": "joe1",
+          "username": "joe1",
+          "email": "joe1@localhost.localdomain",
+          "full_name": "Joe Act",
+          "printable_name": "Joe Act",
+          "created_at": "2020-05-30T00:00:00Z"
         }
     """
-    model = get_user_model()
-    permission_classes = [AllowAuthenticationEnabled, AllowRegistrationEnabled]
-    serializer_class = UserCreateSerializer
+    serializer_class = UserActivateSerializer
 
-    def register(self, serializer):
-        return self.register_user(**serializer.validated_data)
+    def get_serializer_class(self):
+        if self.request.method.lower() == 'get':
+            return  UserDetailSerializer
+        return super(JWTActivate, self).get_serializer_class()
+
+    def get(self, request, *args, **kwargs):#pylint:disable=unused-argument
+        verification_key = self.kwargs.get(self.key_url_kwarg)
+        token = Contact.objects.get_token(verification_key=verification_key)
+        if not token:
+            raise serializers.ValidationError({'detail': "invalid request"})
+        serializer = self.get_serializer(token.user)
+        return Response(serializer.data)
 
     @swagger_auto_schema(responses={
         201: OpenAPIResponse("", TokenSerializer),
         400: OpenAPIResponse("parameters error", ValidationErrorSerializer)})
     def post(self, request, *args, **kwargs):#pylint:disable=unused-argument
-        serializer = self.get_serializer(data=request.data)
-        if serializer.is_valid(raise_exception=True):
-            # It is OK to use `raise_exception=True` because the serializer
-            # purely does field validation (i.e. no checks of values
-            # in database).
-            user = self.register(serializer)
-            if user:
-                self.optional_session_cookie(request, user)
-                return self.create_token(user)
-        raise serializers.ValidationError({'detail': "invalid request"})
+        """
+        Activates a user
+
+        Activates a new user and returns a JSON Web Token that can subsequently
+        be used to authenticate the new user in HTTP requests.
+
+        **Tags: auth, visitor, usermodel
+
+        **Example
+
+        .. code-block:: http
+
+            POST /api/auth/activate/16793aa72a4c7ae94b50b20c2eca52df5b0fe2c6\
+ HTTP/1.1
+
+        .. code-block:: json
+
+            {
+              "username": "joe1",
+              "email": "joe1@locahost.localdomain",
+              "new_password": "yoyo",
+              "full_name": "Joe Card1"
+            }
+
+        responds
+
+        .. code-block:: json
+
+            {
+                "token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJ1c2VybmFtZSI6\
+    ImpvZTEiLCJlbWFpbCI6ImpvZSsxQGRqYW9kamluLmNvbSIsImZ1bGxfbmFtZ\
+    SI6IkpvZSAgQ2FyZDEiLCJleHAiOjE1Mjk2NTUyMjR9.GFxjU5AvcCQbVylF1P\
+    JwcBUUMECj8AKxsHtRHUSypco"
+            }
+        """
+        return super(JWTActivate, self).post(request, *args, **kwargs)
 
 
 class JWTLogout(JWTBase):
     """
     Logs a user out
 
     Removes all cookies associated with the session.
@@ -431,17 +320,17 @@
         response = Response(status=status.HTTP_200_OK)
         if settings.LOGOUT_CLEAR_COOKIES:
             for cookie in settings.LOGOUT_CLEAR_COOKIES:
                 response.delete_cookie(cookie)
         return response
 
 
-class PasswordResetAPIView(RecoverMixin, CreateAPIView):
+class RecoverAPIView(VerifyMixin, JWTBase):
     """
-    Sends a password reset link
+    Sends a one-time link or code
 
     The user is uniquely identified by her email address.
 
     The API is typically used within an HTML
     `recover credentials page </docs/guides/themes/#workflow_recover>`_
     as present in the default theme.
 
@@ -464,26 +353,22 @@
     .. code-block:: json
 
         {
             "email": "xia@localhost.localdomain"
         }
     """
     model = get_user_model()
-    permission_classes = [AllowAuthenticationEnabled]
-    serializer_class = PasswordResetSerializer
+    serializer_class = RecoverSerializer
     token_generator = default_token_generator
 
-    def perform_create(self, serializer):
+    def post(self, request, *args, **kwargs):#pylint:disable=unused-argument
         try:
-            self.recover_user(**serializer.validated_data)
+            user_with_backend = self.run_pipeline()
+            return self.create_token(user_with_backend)
         except SSORequired as err:
             raise serializers.ValidationError({'detail': _(
                 "SSO required through %(provider)s") % {
                     'provider': err.printable_name},
-                'provider': err.delegate_auth.provider,
-                'url': self.request.build_absolute_uri(err.url)})
+                    'provider': err.delegate_auth.provider,
+                    'url': self.request.build_absolute_uri(err.url)})
 
-    def permission_denied(self, request, message=None, code=None):
-        # We override this function from `APIView`. The request will never
-        # be authenticated by definition since we are dealing with login
-        # and register APIs.
-        raise exceptions.PermissionDenied(detail=message)
+        raise exceptions.PermissionDenied()
```

### Comparing `djaodjin-signup-0.7.7/signup/api/contacts.py` & `djaodjin-signup-0.8.0/signup/api/contacts.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.7.7/signup/api/keys.py` & `djaodjin-signup-0.8.0/signup/api/keys.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022, Djaodjin Inc.
+# Copyright (c) 2023, Djaodjin Inc.
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice,
 #    this list of conditions and the following disclaimer.
@@ -94,25 +94,25 @@
             raise PermissionDenied(_("Incorrect credentials"))
         allowed_chars = 'abcdefghjkmnpqrstuvwxyz'\
             'ABCDEFGHJKLMNPQRSTUVWXYZ'\
             '23456789'
         api_pub_key = generate_random_slug(
             length=Credentials.API_PUB_KEY_LENGTH,
             allowed_chars=allowed_chars)
-        api_priv_key = generate_random_slug(
-            length=Credentials.API_PRIV_KEY_LENGTH,
+        api_password = generate_random_slug(
+            length=Credentials.API_PASSWORD_LENGTH,
             allowed_chars=allowed_chars)
         Credentials.objects.update_or_create(
             user=self.user,
             defaults={
                 'api_pub_key': api_pub_key,
-                'api_priv_key': make_password(api_priv_key)
+                'api_password': make_password(api_password)
             })
         return Response(APIKeysSerializer().to_representation({
-            'secret': api_pub_key + api_priv_key
+            'secret': api_pub_key + api_password
         }), status=status.HTTP_201_CREATED)
 
 
 class PublicKeyAPIView(UserMixin, GenericAPIView):
     """
     Updates a user public RSA key
     """
```

### Comparing `djaodjin-signup-0.7.7/signup/api/tokens.py` & `djaodjin-signup-0.8.0/signup/api/tokens.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.7.7/signup/api/users.py` & `djaodjin-signup-0.8.0/signup/api/users.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022, DjaoDjin inc.
+# Copyright (c) 2023, DjaoDjin inc.
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice,
 #    this list of conditions and the following disclaimer.
@@ -20,37 +20,37 @@
 # OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
 # OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 # ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import hashlib, logging, os, re
 
+import pyotp
 from django.contrib.auth import logout as auth_logout
 from django.db import transaction, IntegrityError
 from django.core.exceptions import PermissionDenied
 from django.contrib.auth import update_session_auth_hash, get_user_model
-from rest_framework import parsers, status
+from rest_framework import generics, parsers, status
 from rest_framework.exceptions import ValidationError
-from rest_framework.generics import (CreateAPIView, ListCreateAPIView,
-    RetrieveUpdateDestroyAPIView, GenericAPIView, RetrieveUpdateAPIView)
 from rest_framework.response import Response
 from rest_framework.settings import api_settings
 
 
 from .. import filters, settings
 from ..compat import (force_str, gettext_lazy as _, reverse, six,
     urlparse, urlunparse)
 from ..decorators import check_has_credentials
 from ..docs import OpenAPIResponse, no_body, swagger_auto_schema
 from ..helpers import full_name_natural_split
 from ..mixins import ContactMixin, UserMixin
-from ..models import Contact, Credentials, Notification
+from ..models import Contact, Credentials, Notification, OTPGenerator
 from ..serializers_overrides import UserSerializer, UserDetailSerializer
-from ..serializers import (PasswordChangeSerializer, NotificationsSerializer,
-    UploadBlobSerializer, UserCreateSerializer, ValidationErrorSerializer)
+from ..serializers import (OTPSerializer, OTPUpdateSerializer,
+    PasswordChangeSerializer, NotificationsSerializer, UploadBlobSerializer,
+    UserCreateSerializer, ValidationErrorSerializer)
 from ..utils import generate_random_code, get_picture_storage, handle_uniq_error
 
 
 LOGGER = logging.getLogger(__name__)
 
 
 def get_order_func(fields):
@@ -75,15 +75,15 @@
             get_order_func(fields[1:])(left, right))
     field_name = fields[0]
     return lambda left, right: (
         getattr(left, field_name) < getattr(right, field_name) or
         get_order_func(fields[1:])(left, right))
 
 
-class UserActivateAPIView(ContactMixin, GenericAPIView):
+class UserActivateAPIView(ContactMixin, generics.GenericAPIView):
     """
     Sends an activation link
 
     Re-sends an activation e-mail if the user is not already activated.
 
     The template for the e-mail sent to the user can be found in
     notification/verification.eml.
@@ -125,15 +125,15 @@
         resp_data.update({
             'detail': _("Activation e-mail successfuly sent to %(email)s") % {
                 'email': instance.email}
         })
         return Response(resp_data)
 
 
-class UserDetailAPIView(UserMixin, RetrieveUpdateDestroyAPIView):
+class UserDetailAPIView(UserMixin, generics.RetrieveUpdateDestroyAPIView):
     """
     Retrieves a user account
 
     Retrieves details on one single user account with slug ``{user}``.
 
     The API is typically used within an HTML
     `contact information page </docs/guides/themes/#dashboard_profile>`_
@@ -306,20 +306,20 @@
                     contact.picture = ""
                     contact.email_verification_key = None
                     contact.email_verification_at = None
                     contact.email_verified_at = None
                     contact.phone_verification_key = None
                     contact.phone_verification_at = None
                     contact.phone_verified_at = None
-                    contact.mfa_priv_key = None
+                    contact.one_time_code = None
                 Contact.objects.bulk_update(contacts, [
                     'email', 'phone', 'full_name', 'nick_name', 'picture',
                     'email_verification_key', 'email_verification_at',
                     'email_verified_at', 'phone_verification_key',
-                    'phone_verification_at', 'mfa_priv_key'])
+                    'phone_verification_at', 'one_time_code'])
             if user.pk:
                 self.delete_records(user)
                 requires_logout = (self.request.user == user)
                 user.username = slug
                 user.email = email
                 user.password = '!'
                 user.is_active = False
@@ -386,52 +386,16 @@
         # A little patchy but it works. Otherwise we would need to override
         # `update` as well.
         #pylint:disable=pointless-statement,protected-access
         serializer.data
         serializer._data.update({'detail': _("Profile updated.")})
 
 
-class UserListCreateAPIView(ListCreateAPIView):
-    """
-    Lists user accounts
-
-    Returns a list of {{PAGE_SIZE}} profile and user accounts.
-
-    The queryset can be filtered for at least one field to match a search
-    term (``q``).
-
-    The queryset can be ordered by a field by adding an HTTP query parameter
-    ``o=`` followed by the field name. A sequence of fields can be used
-    to create a complete ordering by adding a sequence of ``o`` HTTP query
-    parameters. To reverse the natural order of a field, prefix the field
-    name by a minus (-) sign.
-
-    **Tags: profile, broker, usermodel
+class UserListMixin(object):
 
-    **Example
-
-    .. code-block:: http
-
-        GET /api/users?q=xia HTTP/1.1
-
-    responds
-
-    .. code-block:: json
-
-        {
-            "count": 1,
-            "next": null,
-            "previous": null,
-            "results": [{
-              "slug": "xia",
-              "username": "xia",
-              "printable_name": "Xia"
-            }]
-        }
-    """
     search_fields = (
         'email',
         # fields in User model:
         'username',
     )
     ordering_fields = (
         ('full_name', 'full_name'),
@@ -442,58 +406,14 @@
     alternate_ordering = ('first_name', 'last_name')
 
     filter_backends = (filters.SearchFilter, filters.OrderingFilter)
     serializer_class = UserSerializer
     queryset = Contact.objects.all().select_related('user')
     user_queryset = get_user_model().objects.filter(is_active=True)
 
-    def get_serializer_class(self):
-        if self.request.method.lower() == 'post':
-            return UserCreateSerializer
-        return super(UserListCreateAPIView, self).get_serializer_class()
-
-    @swagger_auto_schema(responses={
-        201: OpenAPIResponse("success", UserDetailSerializer),
-        400: OpenAPIResponse("parameters error", ValidationErrorSerializer)})
-    def post(self, request, *args, **kwargs):
-        """
-        Creates a user account
-
-        **Tags: profile, broker, usermodel
-
-        **Examples
-
-        .. code-block:: http
-
-            POST /api/users HTTP/1.1
-
-        .. code-block:: json
-
-            {
-              "full_name": "Xia Lee",
-              "nick_name": "Xia",
-              "email": "xia@locahost.localdomain"
-            }
-
-        responds
-
-        .. code-block:: json
-
-            {
-              "slug": "xia",
-              "username": "xia",
-              "created_at": "2018-01-01T00:00:00Z",
-              "printable_name": "Xia",
-              "full_name": "Xia Lee",
-              "nick_name": "Xia",
-              "email": "xia@locahost.localdomain"
-            }
-        """
-        return self.create(request, *args, **kwargs)
-
     def as_user(self, contact):
         user_model = self.user_queryset.model
         first_name, unused, last_name = full_name_natural_split(
             contact.full_name)
         return user_model(username=contact.slug, email=contact.email,
             first_name=first_name, last_name=last_name)
 
@@ -573,15 +493,99 @@
         # XXX It could be faster to stop previous loops early but it is not
         # clear. The extra check at each iteration might in fact be slower.
         page = page[:api_settings.PAGE_SIZE]
 
         serializer = self.get_serializer(page, many=True)
         return self.get_paginated_response(serializer.data)
 
+
+class UserListCreateAPIView(UserListMixin, generics.ListCreateAPIView):
+    """
+    Lists user accounts
+
+    Returns a list of {{PAGE_SIZE}} profile and user accounts.
+
+    The queryset can be filtered for at least one field to match a search
+    term (``q``).
+
+    The queryset can be ordered by a field by adding an HTTP query parameter
+    ``o=`` followed by the field name. A sequence of fields can be used
+    to create a complete ordering by adding a sequence of ``o`` HTTP query
+    parameters. To reverse the natural order of a field, prefix the field
+    name by a minus (-) sign.
+
+    **Tags: profile, broker, usermodel
+
+    **Example
+
+    .. code-block:: http
+
+        GET /api/users?q=xia HTTP/1.1
+
+    responds
+
+    .. code-block:: json
+
+        {
+            "count": 1,
+            "next": null,
+            "previous": null,
+            "results": [{
+              "slug": "xia",
+              "username": "xia",
+              "printable_name": "Xia"
+            }]
+        }
+    """
+    def get_serializer_class(self):
+        if self.request.method.lower() == 'post':
+            return UserCreateSerializer
+        return super(UserListCreateAPIView, self).get_serializer_class()
+
+    @swagger_auto_schema(responses={
+        201: OpenAPIResponse("success", UserDetailSerializer),
+        400: OpenAPIResponse("parameters error", ValidationErrorSerializer)})
+    def post(self, request, *args, **kwargs):
+        """
+        Creates a user account
+
+        **Tags: profile, broker, usermodel
+
+        **Examples
+
+        .. code-block:: http
+
+            POST /api/users HTTP/1.1
+
+        .. code-block:: json
+
+            {
+              "full_name": "Xia Lee",
+              "nick_name": "Xia",
+              "email": "xia@locahost.localdomain"
+            }
+
+        responds
+
+        .. code-block:: json
+
+            {
+              "slug": "xia",
+              "username": "xia",
+              "created_at": "2018-01-01T00:00:00Z",
+              "printable_name": "Xia",
+              "full_name": "Xia Lee",
+              "nick_name": "Xia",
+              "email": "xia@locahost.localdomain"
+            }
+        """
+        return self.create(request, *args, **kwargs)
+
     def create(self, request, *args, **kwargs):
+        #pylint:disable=too-many-locals
         serializer = self.get_serializer(data=request.data)
         serializer.is_valid(raise_exception=True)
 
         user_model = self.user_queryset.model
         slug = serializer.validated_data.get('slug',
             serializer.validated_data.get('username'))
         full_name = serializer.validated_data.get('full_name',
@@ -616,15 +620,124 @@
 
         location = self.request.build_absolute_uri(
             reverse('api_user_profile', args=(user,)))
         return Response(UserDetailSerializer().to_representation(user),
             status=status.HTTP_201_CREATED, headers={'Location': location})
 
 
-class PasswordChangeAPIView(GenericAPIView):
+class ActivityByAccountContactAPIView(UserListMixin, generics.ListAPIView):
+    """
+    Lists contacts for activities on an account
+
+    Returns a list of {{PAGE_SIZE}} contacts for activities on {account}.
+
+    **Tags: profile, broker, usermodel
+
+    **Example
+
+    .. code-block:: http
+
+        GET /api/activities/xia/contacts HTTP/1.1
+
+    responds
+
+    .. code-block:: json
+
+        {
+            "count": 1,
+            "next": null,
+            "previous": null,
+            "results": [{
+              "slug": "xia",
+              "username": "xia",
+              "printable_name": "Xia"
+            }]
+        }
+    """
+    def get_queryset(self):
+        return Contact.objects.filter(activities__account__slug=self.kwargs.get(
+            self.account_url_kwarg)).select_related('user')
+
+
+class OTPChangeAPIView(UserMixin, generics.GenericAPIView):
+
+    serializer_class = OTPUpdateSerializer
+
+    def get_issuer_name(self):
+        return None
+
+    def get_queryset(self):
+        return OTPGenerator.objects.filter(user=self.user)
+
+    @swagger_auto_schema(responses={
+        200: OpenAPIResponse("success", OTPSerializer),
+        201: OpenAPIResponse("success", OTPSerializer),
+        400: OpenAPIResponse("parameters error", ValidationErrorSerializer)})
+    def put(self, request, *args, **kwargs):
+        """
+        Enables or disables OTP
+
+        The API is typically used within an HTML
+        `update password page </docs/guides/themes/#dashboard_users_password>`_
+        as present in the default theme.
+
+        **Tags: auth, user, usermodel
+
+        **Example
+
+        .. code-block:: http
+
+            POST /api/users/xia/otp HTTP/1.1
+
+        .. code-block:: json
+
+            {
+              "password": "yoyo",
+              "enable": true
+            }
+
+        responds
+
+        .. code-block:: json
+
+            {
+              "priv_key": "**********************",
+              "provisioning_uri": "https://localhost:8020/"
+            }
+        """
+        #pylint:disable=unused-argument
+        serializer = self.get_serializer(data=request.data)
+        serializer.is_valid(raise_exception=True)
+
+        password = serializer.validated_data['password']
+        if not self.request.user.check_password(password):
+            raise PermissionDenied(_("Incorrect credentials"))
+
+        if serializer.validated_data.get('enable'):
+            otp, created = OTPGenerator.objects.get_or_create(
+                user=self.user, defaults={
+                    'priv_key': pyotp.random_base32()
+                })
+
+            return Response(OTPSerializer().to_representation({
+                'priv_key': otp.priv_key,
+                'provisioning_uri': otp.provisioning_uri(
+                    issuer_name=self.get_issuer_name())
+            }), status=(status.HTTP_201_CREATED
+                if created else status.HTTP_200_OK))
+
+        try:
+            OTPGenerator.objects.get(user=self.user).delete()
+        except OTPGenerator.DoesNotExist:
+            pass
+
+        return Response(status=status.HTTP_204_NO_CONTENT)
+
+
+class PasswordChangeAPIView(generics.GenericAPIView):
     """
     Updates a user password
     """
     lookup_field = 'username'
     lookup_url_kwarg = 'user'
     serializer_class = PasswordChangeSerializer
     queryset = get_user_model().objects.filter(is_active=True)
@@ -679,15 +792,15 @@
             # django.contrib.auth.middleware.SessionAuthenticationMiddleware
             # is enabled.
             update_session_auth_hash(self.request, serializer.instance)
 
         return Response({'detail': _("Password updated successfully.")})
 
 
-class UserNotificationsAPIView(UserMixin, RetrieveUpdateAPIView):
+class UserNotificationsAPIView(UserMixin, generics.RetrieveUpdateAPIView):
     """
     Lists a user notifications preferences
 
     The API is typically used within an HTML
     `notifications page </docs/guides/themes/#dashboard_users_notifications>`_
     as present in the default theme.
 
@@ -785,15 +898,15 @@
                     if not enabled:
                         self.user.notifications.add(notification)
                 else:
                     if enabled:
                         self.user.notifications.add(notification)
 
 
-class UserPictureAPIView(ContactMixin, CreateAPIView):
+class UserPictureAPIView(ContactMixin, generics.CreateAPIView):
     """
     Uploads a picture for a user account
 
     The API is typically used within an HTML
     `contact information page </docs/guides/themes/#dashboard_profile>`_
     as present in the default theme.
```

### Comparing `djaodjin-signup-0.7.7/signup/auth.py` & `djaodjin-signup-0.8.0/signup/auth.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.7.7/signup/authentication.py` & `djaodjin-signup-0.8.0/signup/authentication.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.7.7/signup/backends/auth.py` & `djaodjin-signup-0.8.0/signup/backends/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,14 @@
 
 
 class UsernameOrEmailModelBackend(object):
     """
     Backend to authenticate a user through either her username
     or email address.
     """
-    #pylint: disable=no-self-use
     model = get_user_model()
 
     def find_user(self, username):
         try:
             validate_email_base(username)
             kwargs = {'email__iexact': username}
         except ValidationError:
@@ -91,15 +90,14 @@
 
 
 class UsernameOrEmailPhoneModelBackend(object):
     """
     Backend to authenticate a user through either her username,
     email address or phone number.
     """
-    #pylint: disable=no-self-use
     model = get_user_model()
 
     def find_user(self, username):
         user_kwargs = {}
         contact_kwargs = {}
         username = str(username) # We could have a ``PhoneNumber`` here.
         try:
```

### Comparing `djaodjin-signup-0.7.7/signup/backends/auth_ldap.py` & `djaodjin-signup-0.8.0/signup/backends/auth_ldap.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,12 +141,12 @@
         except ldap.LDAPError:
             user = None
         finally:
             ldap_connection.unbind_s()
 
         return user
 
-    def get_user(self, user_id):#pylint:disable=no-self-use
+    def get_user(self, user_id):
         try:
             return LDAPUser(self, db_user=self.model.objects.get(pk=user_id))
         except self.model.DoesNotExist:
             return None
```

### Comparing `djaodjin-signup-0.7.7/signup/backends/mfa.py` & `djaodjin-signup-0.8.0/signup/urls/views/saml.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2019, Djaodjin Inc.
+# Copyright (c) 2022, Djaodjin Inc.
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice,
 #    this list of conditions and the following disclaimer.
@@ -18,28 +18,14 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
 # OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
 # OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 # ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-"""
-Backends to send one-time authentication codes
-"""
-from __future__ import unicode_literals
+from ...compat import path
+from ...views.saml import saml_metadata_view
 
-from .. import signals
-from ..utils import generate_random_code
 
-
-class EmailMFABackend(object):
-    """
-    Backend to authenticate a user through either her username
-    or email address.
-    """
-    #pylint: disable=no-self-use
-
-    def create_token(self, user, request=None):
-        user.mfa_priv_key = generate_random_code()
-        user.save()
-        signals.user_mfa_code.send(
-            sender=__name__, user=user, code=user.mfa_priv_key, request=request)
+urlpatterns = [
+    path('', saml_metadata_view)
+]
```

### Comparing `djaodjin-signup-0.7.7/signup/backends/sts_credentials.py` & `djaodjin-signup-0.8.0/signup/backends/sts_credentials.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.7.7/signup/compat.py` & `djaodjin-signup-0.8.0/signup/compat.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.7.7/signup/decorators.py` & `djaodjin-signup-0.8.0/signup/decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 
     The email embed a link to a verification url and a redirect to the page
     the verification email was sent from so that the user stays on her
     workflow once verification is completed.
     """
     # XXX needs to send phone text message instead of e-mail!!!
     back_url = request.build_absolute_uri(reverse('registration_activate',
-        args=(contact.email_verification_key,)))
+        args=(contact.phone_verification_key,)))
     if next_url:
         back_url += '?%s=%s' % (redirect_field_name, next_url)
     signals.user_verification.send(
         sender=__name__, user=contact.user, request=request,
         back_url=back_url, expiration_days=settings.KEY_EXPIRATION)
 
 
@@ -120,15 +120,15 @@
     """
     Checks that a *user* has set login credentials (i.e. password).
     """
     if has_invalid_password(user):
         # Let's send e-mail again.
         #pylint:disable=unused-variable
         contact, created = Contact.objects.prepare_email_verification(
-            user, user.email)
+            user.email, user=user)
         if not next_url:
             next_url = validate_redirect(request)
         send_verification_email(
             contact, request, next_url=next_url,
             redirect_field_name=redirect_field_name)
         return False
     return True
@@ -141,15 +141,15 @@
     Checks that a *user*'s e-mail has been verified.
     """
     #pylint:disable=unused-variable
     if Contact.objects.is_reachable_by_email(user):
         return True
 
     contact, created = Contact.objects.prepare_email_verification(
-        user, user.email)
+        user.email, user=user)
     # Let's send e-mail again.
     if not next_url:
         next_url = validate_redirect(request)
     send_verification_email(
         contact, request, next_url=next_url,
         redirect_field_name=redirect_field_name)
     return False
@@ -162,15 +162,15 @@
     Checks that a *user*'s e-mail has been verified.
     """
     #pylint:disable=unused-variable
     if Contact.objects.is_reachable_by_phone(user):
         return True
 
     contact, created = Contact.objects.prepare_phone_verification(
-        user, user.phone) # XXX
+        user.phone, user=user) # XXX
     # Let's send e-mail again.
     if not next_url:
         next_url = validate_redirect(request)
     send_verification_phone(
         contact, request, next_url=next_url,
         redirect_field_name=redirect_field_name)
     return False
```

### Comparing `djaodjin-signup-0.7.7/signup/docs.py` & `djaodjin-signup-0.8.0/signup/docs.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.7.7/signup/filters.py` & `djaodjin-signup-0.8.0/signup/filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 # ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 from __future__ import unicode_literals
 
 import operator
 from functools import reduce
 import logging
 
+from django.core.exceptions import FieldDoesNotExist
 from django.db import models
 from rest_framework.compat import distinct
 from rest_framework.filters import (OrderingFilter as BaseOrderingFilter,
     SearchFilter as BaseSearchFilter)
 
 from . import settings
 from .compat import force_str, six
@@ -76,16 +77,16 @@
             queryset = distinct(queryset, base)
         return queryset
 
 
     @staticmethod
     def filter_valid_fields(queryset, fields, view):
         #pylint:disable=protected-access
-        model_fields = set([
-            field.name for field in queryset.model._meta.get_fields()])
+        model_fields = {
+            field.name for field in queryset.model._meta.get_fields()}
         # We add all the fields that could be aliases then filter out the ones
         # which are not present in the model.
         alternate_fields = getattr(view, 'alternate_fields', {})
         for field in fields:
             alternate_field = alternate_fields.get(field, None)
             if alternate_field:
                 if isinstance(alternate_field, (list, tuple)):
@@ -199,16 +200,16 @@
 
     def get_valid_fields(self, queryset, view, context=None):
         #pylint:disable=protected-access
         model_fields = {
             field.name for field in queryset.model._meta.get_fields()}
         base_fields = super(OrderingFilter, self).get_valid_fields(
             queryset, view, context=context if context else {})
-        valid_fields = tuple([
-            field for field in base_fields if field[0] in model_fields])
+        valid_fields = tuple(
+            field for field in base_fields if field[0] in model_fields)
         return valid_fields
 
     def get_ordering(self, request, queryset, view):
         #pylint:disable=protected-access
         ordering = None
         params = request.query_params.get(self.ordering_param)
         if params:
```

### Comparing `djaodjin-signup-0.7.7/signup/forms.py` & `djaodjin-signup-0.8.0/signup/forms.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,22 +27,20 @@
 """
 
 from django import forms
 from django.conf import locale
 from django.core import validators
 from django.contrib.auth import password_validation, get_user_model
 from django.contrib.auth.forms import (
-    AuthenticationForm as AuthenticationBaseForm,
-    PasswordResetForm as PasswordResetBaseForm)
+    AuthenticationForm as AuthenticationBaseForm)
 from phonenumber_field.formfields import PhoneNumberField
 
 from . import settings, validators
 from .compat import gettext_lazy as _, six
 from .helpers import full_name_natural_split
-from .models import Contact
 from .utils import get_recaptcha_form_field
 
 
 class EmailField(forms.EmailField):
 
     default_validators = [validators.validate_email]
 
@@ -247,37 +245,35 @@
             attrs={'placeholder': _("Your password")}))
 
     class Meta:
         model = get_user_model()
         fields = ['password', 'new_password', 'new_password2']
 
 
-class PasswordResetForm(PasswordResetBaseForm):
+class RecoverForm(forms.Form):
     """
-    Form displayed to recover password.
+    Form displayed to authenticate through a verification link.
     """
-    email = CommField()
+    username = UsernameOrCommField()
 
 
 class ActivationForm(PasswordConfirmMixin, forms.Form):
     """
     Form to set password, and optionally user's profile information
     in an activation view.
     """
     submit_title = _("Activate")
 
     error_messages = {
         'password_mismatch': _("Password and password confirmation"\
         " do not match."),
     }
 
-    email = EmailField(label=_("E-mail address"),
-        disabled=True, required=False)
-    phone = PhoneField(label=_("Phone number"),
-        disabled=True, required=False)
+    email = EmailField(label=_("E-mail address"), required=False)
+    phone = PhoneField(label=_("Phone number"), required=False)
     full_name = forms.RegexField(
         regex=r'^[\w\s]+$', max_length=60,
         widget=forms.TextInput(attrs={'placeholder':'Full name'}),
         label=_("Full name"),
         error_messages={'invalid':
             _("Sorry we do not recognize some characters in your full name.")})
     username = forms.SlugField(widget=forms.TextInput(
@@ -291,35 +287,26 @@
         help_text=password_validation.password_validators_help_text_html())
     new_password2 = forms.CharField(strip=False,
         label=_("Confirm password"),
         widget=forms.PasswordInput(attrs={
             'placeholder': _("Confirm password")}))
 
     def __init__(self, *args, **kwargs):
-        self.user = kwargs.pop('instance')
+        initial = kwargs.get('initial')
+        email_verification = initial.pop('email_verification', False)
+        phone_verification = initial.pop('phone_verification', False)
         super(ActivationForm, self).__init__(*args, **kwargs)
+        if email_verification:
+            self.fields['email'].disabled = True
+        if phone_verification:
+            self.fields['phone'].disabled = True
         if settings.REQUIRES_RECAPTCHA:
             self.fields['captcha'] = get_recaptcha_form_field()
 
 
-class UserActivateForm(forms.Form):
-    """
-    Verfication of an e-mail address
-    """
-    password = forms.CharField(
-        label=_("Password"),
-        widget=forms.PasswordInput(attrs={'placeholder': _("Password")}),
-        strip=False,
-        help_text=password_validation.password_validators_help_text_html())
-
-    def __init__(self, *args, **kwargs):
-        self.user = kwargs.pop('instance')
-        super(UserActivateForm, self).__init__(*args, **kwargs)
-
-
 class PublicKeyForm(forms.Form):
 
     submit_title = _("Update")
 
     pubkey = forms.CharField(widget=forms.Textarea)
     password = forms.CharField(
         label=_("Password"),
@@ -348,15 +335,15 @@
         max_length=254, label=_("Full name"))
     nick_name = forms.CharField(required=False, widget=forms.TextInput(
         attrs={'placeholder': _("Short casual name used to address the user")}),
         max_length=254, label=_("Nick name"))
 
     class Meta:
         model = get_user_model()
-        fields = ['username', 'email', 'full_name']
+        fields = ['username', 'full_name', 'email']
 
     def __init__(self, instance=None, **kwargs):
         super(UserForm, self).__init__(instance=instance, **kwargs)
         if instance:
             # define other fields dynamically
             self.fields['phone'] = PhoneField(required=False)
             lang_code = settings.LANGUAGE_CODE
@@ -407,26 +394,14 @@
         for item, initial in six.iteritems(self.initial.get('notifications')):
             self.fields[item] = forms.BooleanField(
                 label=initial[0].get('summary', ""),
                 help_text=initial[0].get('description', ""),
                 required=False, initial=initial[1])
 
 
-class StartAuthenticationForm(forms.Form):
-    """
-    Form to present a user who may or may not have an account yet.
-    """
-    username = UsernameOrCommField()
-    submit_title = _("Submit")
-
-    def __init__(self, *args, **kwargs):
-        kwargs.pop('request')
-        super(StartAuthenticationForm, self).__init__(*args, **kwargs)
-
-
 class AuthenticationForm(AuthenticationBaseForm):
 
     # The field is called `username`, yet it is technically
     # a username, e-mail or phone.
     username = UsernameOrCommField()
     password = forms.CharField(widget=forms.PasswordInput(
         attrs={'placeholder': _("Password")}), label=_("Password"))
@@ -438,26 +413,39 @@
             placeholder_label = _('%(username)s, e-mail or phone' % {
                 'username': username_label})
             self.fields['username'].label = placeholder_label
             self.fields['username'].widget.attrs['placeholder'] \
                 = placeholder_label
 
 
-class MFACodeForm(AuthenticationForm):
+class StartAuthenticationForm(forms.Form):
+    """
+    Form to present a user who may or may not have an account yet.
+    """
+    username = UsernameOrCommField()
+    submit_title = _("Submit")
+
+    def __init__(self, *args, **kwargs):
+        kwargs.pop('request')
+        super(StartAuthenticationForm, self).__init__(*args, **kwargs)
+
+
+class PasswordAuthForm(StartAuthenticationForm):
+
+    password = forms.CharField(widget=forms.PasswordInput(
+        attrs={'placeholder': _("Password")}), label=_("Password"))
+
+    def __init__(self, *args, **kwargs):
+        super(PasswordAuthForm, self).__init__(*args, **kwargs)
+        self.fields['username'].widget = forms.HiddenInput()
+
+
+class MFACodeForm(PasswordAuthForm):
 
     code = forms.IntegerField(widget=forms.TextInput(
         attrs={'placeholder': _("One-time authentication code"),
             'autofocus': True}),
         label=_("One-time authentication code"))
 
     def __init__(self, *args, **kwargs):
         super(MFACodeForm, self).__init__(*args, **kwargs)
-        self.fields['username'].widget = forms.HiddenInput()
         self.fields['password'].widget = forms.HiddenInput()
-
-    def clean(self):
-        super(MFACodeForm, self).clean()
-        code = self.cleaned_data.get('code')
-        contact = Contact.objects.filter(user=self.user_cache).first()
-        if not contact or code != contact.mfa_priv_key:
-            raise forms.ValidationError(_("MFA code does not match."))
-        return self.cleaned_data
```

### Comparing `djaodjin-signup-0.7.7/signup/helpers.py` & `djaodjin-signup-0.8.0/signup/helpers.py`

 * *Files 18% similar despite different names*

```diff
@@ -72,7 +72,24 @@
     else:
         mid_name = " ".join(parts)
     return first_name, mid_name, last_name
 
 
 def has_invalid_password(user):
     return not user.password or user.password.startswith('!')
+
+
+def update_context_urls(context, urls):
+    if 'urls' in context:
+        for key, val in six.iteritems(urls):
+            if key in context['urls']:
+                if isinstance(val, dict):
+                    context['urls'][key].update(val)
+                else:
+                    # Because organization_create url is added in this mixin
+                    # and in ``OrganizationRedirectView``.
+                    context['urls'][key] = val
+            else:
+                context['urls'].update({key: val})
+    else:
+        context.update({'urls': urls})
+    return context
```

### Comparing `djaodjin-signup-0.7.7/signup/middleware.py` & `djaodjin-signup-0.8.0/signup/middleware.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.7.7/signup/migrations/0001_v0_1_9.py` & `djaodjin-signup-0.8.0/signup/migrations/0001_v0_1_9.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.7.7/signup/migrations/0002_0_2_0.py` & `djaodjin-signup-0.8.0/signup/migrations/0002_0_2_0.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.7.7/signup/migrations/0003_0_2_1.py` & `djaodjin-signup-0.8.0/signup/migrations/0003_0_2_1.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.7.7/signup/migrations/0004_0_2_6.py` & `djaodjin-signup-0.8.0/signup/migrations/0004_0_2_6.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.7.7/signup/migrations/0005_0_2_8.py` & `djaodjin-signup-0.8.0/signup/migrations/0005_0_2_8.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.7.7/signup/migrations/0006_v0_4_7.py` & `djaodjin-signup-0.8.0/signup/migrations/0006_v0_4_7.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,10 +106,10 @@
             model_name='contact',
             name='user',
             field=models.ForeignKey(null=True, on_delete=django.db.models.deletion.CASCADE, related_name='contacts', to=settings.AUTH_USER_MODEL),
         ),
         migrations.AlterField(
             model_name='notification',
             name='slug',
-            field=models.SlugField(help_text='Unique identifier shown in the URL bar', unique=True),
+            field=models.SlugField(choices=[], help_text='Unique identifier shown in the URL bar', unique=True),
         ),
     ]
```

### Comparing `djaodjin-signup-0.7.7/signup/migrations/0007_v0_4_8.py` & `djaodjin-signup-0.8.0/signup/migrations/0007_v0_4_8.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.7.7/signup/migrations/0008_v0_6_0.py` & `djaodjin-signup-0.8.0/signup/migrations/0008_v0_6_0.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.7.7/signup/mixins.py` & `djaodjin-signup-0.8.0/signup/mixins.py`

 * *Files 26% similar despite different names*

```diff
@@ -18,36 +18,33 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
 # OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
 # OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 # ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-import logging
+import logging, re
 
 from django.http import Http404
-from django.contrib.auth import (REDIRECT_FIELD_NAME, authenticate,
-    get_user_model)
+from django.contrib.auth import (authenticate,
+    get_user_model, login as auth_login)
 from django.db import IntegrityError
 from django.utils import translation
-from django.utils.encoding import force_bytes
-from django.utils.http import urlencode, urlsafe_base64_encode
-from django.utils.safestring import mark_safe
+from django.utils.http import urlencode
 from rest_framework import exceptions, serializers
 from rest_framework.generics import get_object_or_404
-from rest_framework.settings import api_settings
 
 from . import signals, settings
-from .auth import validate_redirect
 from .compat import gettext_lazy as _, is_authenticated, reverse, six
-from .decorators import check_has_credentials
-from .helpers import full_name_natural_split
-from .models import Contact, DelegateAuth
-from .utils import (get_login_throttle, get_password_reset_throttle,
-    handle_uniq_error)
+from .decorators import send_verification_email, send_verification_phone
+from .helpers import (full_name_natural_split, has_invalid_password,
+    update_context_urls)
+from .models import Contact, DelegateAuth, OTPGenerator
+from .utils import (get_disabled_authentication, get_disabled_registration,
+    get_email_dynamic_validator, get_login_throttle, handle_uniq_error)
 from .validators import as_email_or_phone
 
 LOGGER = logging.getLogger(__name__)
 
 
 class SSORequired(exceptions.AuthenticationFailed):
 
@@ -74,205 +71,336 @@
         })
 
     @property
     def printable_name(self):
         return self.provider_info.get('name', str(self.delegate_auth.provider))
 
 
-class ChecksMixin(object):
+class IncorrectPath(exceptions.AuthenticationFailed):
+    """
+    Incorrect path
+    """
 
-    @staticmethod
-    def check_sso_required(email):
-        domain = email.split('@')[-1]
-        try:
-            delegate_auth = DelegateAuth.objects.get(domain=domain)
-            raise SSORequired(delegate_auth)
-        except DelegateAuth.DoesNotExist:
-            pass
+class IncorrectUser(exceptions.AuthenticationFailed):
+    """
+    Cannot find user or contact
+    """
 
 
-class ActivateMixin(ChecksMixin):
+class VerifyRequired(exceptions.AuthenticationFailed):
+    """
+    break workflow because we are waiting for a link/code to continue.
+    """
 
-    key_url_kwarg = 'verification_key'
+class OTPRequired(exceptions.AuthenticationFailed):
+    """
+    break workflow because we require the user to enter an OTP
+    """
 
-    def activate_user(self, **cleaned_data):
-        verification_key = self.kwargs.get(self.key_url_kwarg)
-        full_name = cleaned_data.get('full_name', None)
-        if not full_name:
-            first_name = cleaned_data.get('first_name', "")
-            last_name = cleaned_data.get('last_name', "")
-            full_name = (first_name + ' ' + last_name).strip()
-        # If we don't save the ``User`` model here,
-        # we won't be able to authenticate later.
-        try:
-            user, previously_inactive = Contact.objects.activate_user(
-                verification_key,
-                username=cleaned_data.get('username'),
-                password=cleaned_data.get('new_password'),
-                full_name=full_name)
-        except IntegrityError as err:
-            handle_uniq_error(err)
+class PasswordRequired(exceptions.AuthenticationFailed):
+    """
+    break workflow because we require the user to enter a password
+    """
 
-        if user:
-            if not user.last_login:
-                # XXX copy/paste from models.ActivatedUserManager.create_user
-                LOGGER.info("'%s %s <%s>' registered with username '%s'",
-                    user.first_name, user.last_name, user.email, user,
-                    extra={'event': 'register', 'user': user})
-                signals.user_registered.send(sender=__name__, user=user)
-            elif previously_inactive:
-                LOGGER.info("'%s %s <%s>' activated with username '%s'",
-                    user.first_name, user.last_name, user.email, user,
-                    extra={'event': 'activate', 'user': user})
-                signals.user_activated.send(sender=__name__, user=user,
-                    verification_key=self.kwargs.get(self.key_url_kwarg),
-                    request=self.request)
-        return user
+class AuthDisabled(exceptions.PermissionDenied):
+    """
+    Authentication is disabled
+    """
 
+class RegistrationDisabled(exceptions.PermissionDenied):
+    """
+    Registration is disabled
+    """
 
-class AuthMixin(ChecksMixin):
+
+class AuthMixin(object):
     """
     Steps used in authentiction workflows, either login through a password
     or through an e-mail link.
     """
-    def check_user_throttles(self, request, user):
-        throttle = get_login_throttle()
-        if throttle:
-            throttle(request, self, user)
+    backend_path = 'signup.backends.auth.UsernameOrEmailPhoneModelBackend'
+    model = get_user_model()
+    form_class = None
+    serializer_class = None
 
-    def candidate_user(self, username):
-        """
-        Login through an e-mail link.
-        """
-        email, phone = as_email_or_phone(username)
+    def prefetch_contact_info(self):
+        return {}
+
+    def validate_inputs(self, initial_data=None):
+        # The authentication URLs are anonymously accessible, hence
+        # prime candidates for bots. These will POST to '/login/.' for
+        # example because there is a `action="."` in the <form> tag
+        # in login.html.
+        # We cannot catch these by restricting the match pattern.
+        # 1. '^login/$' will not match 'login/.' hence trigger the catch
+        #    all pattern that might forward the HTTP request.
+        # 2. 'login/(?P<extra>.*)' will through a missing argument
+        #    exception in `reverse` calls.
+        try:
+            pat = (r'(?P<expected_path>%s)(?P<extra>.*)' %
+                self.request.resolver_match.route)
+            look = re.match(pat, self.request.path.lstrip('/'))
+            if look:
+                expected_path = '/' + look.group('expected_path')
+                extra =  look.group('extra')
+                if extra:
+                    raise IncorrectPath(
+                        self.request.build_absolute_uri(expected_path))
+        except AttributeError:
+            pass # Django<=1.11 ResolverMatch does not have
+                 # a route attribute.
+
+        cleaned_data = {}
+        if initial_data:
+            cleaned_data = initial_data.copy()
+        if self.form_class is not None:
+            form = self.get_form()
+            if self.request.method.lower() in ('post',):
+                if not form.is_valid():
+                    raise serializers.ValidationError()
+                for field_name in six.iterkeys(form.data):
+                    cleaned_data.update({
+                        field_name: form.cleaned_data.get(
+                            field_name, form.data[field_name])})
+            cleaned_data.update({'next_url': self.get_success_url()})
+        elif self.serializer_class is not None:
+            data = initial_data.copy()
+            data.update(self.request.data)
+            serializer = self.get_serializer(data=data)
+            serializer.is_valid(raise_exception=True)
+            for field_name in six.iterkeys(data):
+                if field_name == 'phone':
+                    # See serializers_overrides.py:UserDetailSerializer
+                    field_value = serializer.validated_data.get('get_phone',
+                        serializer.validated_data.get(
+                            field_name, data[field_name]))
+                else:
+                    field_value = serializer.validated_data.get(
+                        field_name, data[field_name])
+                cleaned_data.update({field_name: field_value})
+
+        if 'email' not in cleaned_data and 'phone' not in cleaned_data:
+            username = cleaned_data.get('username')
+            email, phone = as_email_or_phone(username)
+            cleaned_data.update({'email': email, 'phone': phone})
+        if 'phone' not in cleaned_data:
+            email = cleaned_data.get('email')
+            email, phone = as_email_or_phone(email)
+            cleaned_data.update({'email': email, 'phone': phone})
+
+        return cleaned_data
+
+    def register_check_disabled(self):
+        pass
+
+    def register_check_data(self, **cleaned_data):
+        pass
+
+    def find_candidate(self, **cleaned_data):
+        username = cleaned_data.get('username')
+        email = cleaned_data.get('email')
+        phone = cleaned_data.get('phone')
+        if not username:
+            username = email
+        if not username:
+            username = phone
         try:
             user = self.model.objects.find_user(username)
 
-            # Rate-limit based on the user.
-            self.check_user_throttles(self.request, user)
             if not email:
                 email = user.email
 
         except self.model.DoesNotExist:
             user = None
 
+        return user, email
+
+    def auth_check_disabled(self, user):
+        auth_disabled = get_disabled_authentication(self.request, user)
+        if auth_disabled:
+            raise AuthDisabled()
+
+    def check_user_throttles(self, request, user):
+        """
+        Rate-limit based on the user.
+        """
+        throttle = get_login_throttle()
+        if throttle:
+            throttle(request, self, user)
+
+    def check_sso_required(self, email):
         # If the user cannot be found and we are not login
         # with an e-mail address, we cannot tell if we should
         # redirect to an SSO provider or not.
         if email:
-            self.check_sso_required(email)
+            domain = email.split('@')[-1]
+            try:
+                delegate_auth = DelegateAuth.objects.get(domain=domain)
+                raise SSORequired(delegate_auth)
+            except DelegateAuth.DoesNotExist:
+                pass
+
+    def auth_check_mfa(self, user, **cleaned_data):
+        code = cleaned_data.get('code')
+        if OTPGenerator.objects.filter(user=user).exists():
+            if not code:
+                raise OTPRequired({
+                    'code': _("OTP code is required.")})
+            if not user.otp.verify(code):
+                if user.otp.nb_attempts >= settings.MFA_MAX_ATTEMPTS:
+                    user.otp.clear_attempts()
+                    raise exceptions.PermissionDenied({'detail': _(
+            "You have exceeded the number of attempts to enter the OTP code."\
+                        " Please start again.")})
+                user.otp.nb_attempts += 1
+                user.otp.save()
+                raise serializers.ValidationError({
+                    'code': _("OTP code does not match.")})
+            user.otp.clear_attempts()
 
-        if not user:
-            if phone:
-                raise serializers.ValidationError({'detail': _(
-                    "We cannot find an account"\
-                    " for this phone number. Please verify the spelling.")})
-            if email:
-                raise serializers.ValidationError({'detail': _(
-                    "We cannot find an account"\
-                    " for this e-mail address. Please verify the spelling.")})
-            raise serializers.ValidationError({'detail': _(
-                "We cannot find an account"\
-                " for this username. Please verify the spelling.")})
-
-        next_url = validate_redirect(self.request)
-        if not check_has_credentials(self.request, user,
-                    next_url=next_url):
-            if phone:
-                raise serializers.ValidationError({'detail':
-                    _("You should now secure and activate"\
-                      " your account following the instructions"\
-                      " we just phoned you. Thank you.")})
-            if email:
-                raise serializers.ValidationError({'detail':
-                    _("You should now secure and activate"\
-                      " your account following the instructions"\
-                      " we just emailed you. Thank you.")})
+    def create_user(self, **cleaned_data):
+        #pylint:disable=unused-argument
+        return None
+
+    def check_password(self, user, **cleaned_data):
+        #pylint:disable=unused-argument
+        return None
 
-        return user
+    def create_session(self, user_with_backend):
+        """
+        Attaches a session cookie to the request and
+        generates an login event in the audit logs.
+        """
+        if self.form_class or self.request.query_params.get('cookie', False):
+            auth_login(self.request, user_with_backend)
+        LOGGER.info("%s signed in.", user_with_backend,
+            extra={'event': 'login', 'request': self.request})
+
+    def run_pipeline(self):
+        # Register: Check if registration or auth is disabled
+        self.register_check_disabled()
+        # Login, Verify, Register:
+        # Bot prevention
+        # - no extra characters on URL path
+        # - validate fields through regex
+        # - optional Captcha
+
+        # `ActivationView` will run the pipeline in GET HTTP requests
+        # (uses `verification_key` in URL path), while other views will
+        # solely do so in POST HTTP requests.
+        initial_data = self.prefetch_contact_info()
+        LOGGER.debug("[run_pipeline] initial_data=%s", str(initial_data))
+        cleaned_data = self.validate_inputs(initial_data)
+        LOGGER.debug("[run_pipeline] cleaned_data=%s", str(cleaned_data))
+        # Login, Verify: Find candidate User or Contact
+        user, email = self.find_candidate(**cleaned_data)
+        LOGGER.debug("[run_pipeline] found_candidate user=%s, email=%s" % (
+            user, email))
+        # Login, Verify: Check if auth is disabled for User, or
+        # auth disabled globally if we only have a Contact
+        self.auth_check_disabled(user)
+        # Login, Verify: Auth rate-limiter
+        self.check_user_throttles(self.request, user)
+        # Login, Verify, Register:
+        # Redirects if email requires SSO
+        self.check_sso_required(email)
+        # Login: If login by verifying e-mail or phone, send code
+        #        Else check password
+        user_with_backend = self.check_password(user, **cleaned_data)
+
+        # Login, Verify: If required, check 2FA
+        self.auth_check_mfa(user, **cleaned_data)
+
+        # Register: Bot prevention verify e-mail if it looks suspicious.
+        self.register_check_data(**cleaned_data)
+        # Verify: If does not exist, create User from Contact
+        # Register: Create User
+        if not user_with_backend:
+            user_with_backend = self.create_user(**cleaned_data)
+        # Login, Verify, Register: Create session
+        LOGGER.debug("[run_pipeline] create session for user_with_backend=%s",
+            user_with_backend)
+
+        self.create_session(user_with_backend)
+        return user_with_backend
 
 
 class LoginMixin(AuthMixin):
     """
     Workflow for authentication (login/sign-in) either through an HTML page
     view or an API call.
     """
-    def login_user(self, **cleaned_data):
-        """
-        Login through a password.
-        """
-        username = cleaned_data.get('username', None)
-        self.candidate_user(username)
-
+    def check_password(self, user, **cleaned_data):
+        user_with_backend = None
+        username = cleaned_data.get('username')
         password = cleaned_data.get('password')
-        if not password:
-            raise serializers.ValidationError({
-                'password': _("password is required.")})
-
         user_with_backend = authenticate(self.request,
             username=username, password=password)
+        if user_with_backend:
+            return user_with_backend
 
-        contact = getattr(user_with_backend, '_contact', None)
-        if contact and contact.mfa_backend:
-            if not contact.mfa_priv_key:
-                contact.create_mfa_token()
-                raise serializers.ValidationError({
-                    'code': _("MFA code is required.")})
+        disabled_registration = get_disabled_registration(self.request)
+        if not disabled_registration:
+            if not user:
+                phone = email = None # XXX call find_candidate again?
+                if phone:
+                    raise IncorrectUser({'phone': _("Not found.")})
+                if email:
+                    raise IncorrectUser({'email': _("Not found.")})
+                raise IncorrectUser({'username': _("Not found.")})
+        if not password:
+            raise PasswordRequired({
+                'password': _("Password is required.")})
 
-            code = cleaned_data.get('code')
-            if code != contact.mfa_priv_key:
-                if contact.mfa_nb_attempts >= settings.MFA_MAX_ATTEMPTS:
-                    contact.clear_mfa_token()
-                    raise exceptions.PermissionDenied({'detail': _(
-            "You have exceeded the number of attempts to enter the MFA code."\
-                        " Please start again.")})
-                contact.mfa_nb_attempts += 1
-                contact.save()
-                raise serializers.ValidationError({
-                    'code': _("MFA code does not match.")})
+        raise serializers.ValidationError({
+            'detail': _("Credentials do not match.")})
 
-            contact.clear_mfa_token()
 
-        return user_with_backend
+class VerifyMixin(AuthMixin):
+    """
+    Authenticate by verifying e-mail or phone
+    """
+    def check_password(self, user, **cleaned_data):
+        next_url = cleaned_data.get('next_url')
+        email = cleaned_data.get('email')
+        if not email:
+            email = user.email
+        # send link through e-mail
+        if email:
+            contact, unused = Contact.objects.prepare_email_verification(
+                email, user=user)
+            send_verification_email(contact, self.request, next_url=next_url)
+            raise VerifyRequired({'detail': _(
+                    "We sent a one-time link to your e-mail address.")})
 
+        raise serializers.ValidationError({
+            'detail': _("Credentials do not match.")})
 
-class RecoverMixin(AuthMixin):
 
-    def check_user_throttles(self, request, user):
-        throttle = get_password_reset_throttle()
-        if throttle:
-            throttle(request, self, user)
+class VerifyPhoneMixin(AuthMixin):
+    """
+    Authenticate by verifying phone
+    """
+    def check_password(self, user, **cleaned_data):
+        next_url = cleaned_data.get('next_url')
 
-    def recover_user(self, **cleaned_data):
-        """
-        Login through an e-mail link.
-        """
-        username = cleaned_data.get('email', None)
-        user = self.candidate_user(username)
+        phone = cleaned_data.get('phone')
+        # send link through phone
+        if phone:
+            contact, unused = Contact.objects.prepare_phone_verification(
+                phone, user=user)
+            send_verification_phone(contact, self.request, next_url=next_url)
+            raise VerifyRequired({'detail': _(
+                    "We sent a one-time code to your phone.")})
 
-        # Make sure that a reset password email is sent to a user
-        # that actually has an activated account.
-        uid = urlsafe_base64_encode(force_bytes(user.pk))
-        if not isinstance(uid, six.string_types):
-            # See Django2.2 release notes
-            uid = uid.decode()
-        token = self.token_generator.make_token(user)
-        next_url = validate_redirect(self.request)
-        back_url = self.request.build_absolute_uri(
-            reverse('password_reset_confirm', args=(uid, token)))
-        if next_url:
-            back_url += '?%s=%s' % (REDIRECT_FIELD_NAME, next_url)
-        signals.user_reset_password.send(
-            sender=__name__, user=user, request=self.request,
-            back_url=back_url, expiration_days=settings.KEY_EXPIRATION)
+        raise serializers.ValidationError({
+            'detail': _("Credentials do not match.")})
 
 
-class RegisterMixin(ChecksMixin):
-
-    backend_path = 'signup.backends.auth.UsernameOrEmailPhoneModelBackend'
+class RegisterMixin(AuthMixin):
 
     registration_fields = (
         'country',
         'email',
         'full_name',
         'first_name',
         'last_name',
@@ -288,84 +416,45 @@
         'phone',
         'get_phone',
         'region',
         'street_address',
         'username',
     )
 
+    def register_check_disabled(self):
+        disabled_registration = get_disabled_registration(self.request)
+        if disabled_registration:
+            raise RegistrationDisabled()
+
+    def register_check_data(self, **cleaned_data):
+        email = cleaned_data.get('email')
+        if email:
+            dynamic_validator = get_email_dynamic_validator()
+            if dynamic_validator:
+                dynamic_validator(email)
+
     @staticmethod
     def first_and_last_names(**cleaned_data):
         first_name = cleaned_data.get('first_name', None)
         last_name = cleaned_data.get('last_name', None)
         if not first_name:
             # If the form does not contain a first_name/last_name pair,
             # we assume a full_name was passed instead.
             full_name = cleaned_data.get(
                 'user_full_name', cleaned_data.get('full_name', None))
             first_name, _, last_name = full_name_natural_split(full_name)
         return first_name, last_name
 
-    def register_user(self, next_url=None, **cleaned_data):
-        email = cleaned_data.get('email', None)
-        if email:
-            self.check_sso_required(email)
-            try:
-                user = self.model.objects.find_user(email)
-                if check_has_credentials(self.request, user, next_url=next_url):
-                    raise serializers.ValidationError(
-                        {'email':
-                         _("A user with that e-mail address already exists."),
-                         api_settings.NON_FIELD_ERRORS_KEY:
-                         mark_safe(_(
-                             "This email address has already been registered!"\
-    " Please <a href=\"%s\">login</a> with your credentials. Thank you.")
-                            % reverse('login'))})
-                raise serializers.ValidationError(
-                    {'email':
-                     _("A user with that e-mail address already exists."),
-                     api_settings.NON_FIELD_ERRORS_KEY:
-                     mark_safe(_(
-                         "This email address has already been registered!"\
-    " You should now secure and activate your account following "\
-    " the instructions we just emailed you. Thank you."))})
-            except self.model.DoesNotExist:
-                # OK to continue. We will have raised an exception in all other
-                # cases.
-                pass
-
-        phone = cleaned_data.get('phone', cleaned_data.get('get_phone'))
-        if phone:
-            try:
-                user = self.model.objects.find_user(phone)
-                if check_has_credentials(self.request, user, next_url=next_url):
-                    raise serializers.ValidationError(
-                        {'phone':
-                         _("A user with that phone number already exists."),
-                         api_settings.NON_FIELD_ERRORS_KEY:
-                         mark_safe(_(
-                             "This phone number has already been registered!"\
-    " Please <a href=\"%s\">login</a> with your credentials. Thank you.")
-                            % reverse('login'))})
-                raise serializers.ValidationError(
-                    {'phone':
-                     _("A user with that phone number already exists."),
-                     api_settings.NON_FIELD_ERRORS_KEY:
-                     mark_safe(_(
-                         "This phone number has already been registered!"\
-    " You should now secure and activate your account following "\
-    " the instructions we just messaged you. Thank you."))})
-            except self.model.DoesNotExist:
-                # OK to continue. We will have raised an exception in all other
-                # cases.
-                pass
-
+    def create_user(self, **cleaned_data):
         first_name, last_name = self.first_and_last_names(**cleaned_data)
-        username = cleaned_data.get('username', None)
+        email = cleaned_data.get('email')
+        phone = cleaned_data.get('phone')
+        username = cleaned_data.get('username')
         password = cleaned_data.get('new_password',
-            cleaned_data.get('password', None))
+            cleaned_data.get('password'))
         lang = cleaned_data.get('lang', cleaned_data.get('get_lang',
             translation.get_language_from_request(self.request)))
         user_extra = {}
         for field_name, field_value in six.iteritems(cleaned_data):
             if field_name not in self.registration_fields:
                 if field_name.startswith('user_'):
                     user_extra.update({field_name[5:]: field_value})
@@ -377,35 +466,98 @@
             lang=lang, extra=user_extra)
         # Bypassing authentication here, we are doing frictionless registration
         # the first time around.
         user.backend = self.backend_path
         return user
 
 
-class UrlsMixin(object):
+class VerifyCompleteMixin(AuthMixin):
 
-    @staticmethod
-    def update_context_urls(context, urls):
-        if 'urls' in context:
-            for key, val in six.iteritems(urls):
-                if key in context['urls']:
-                    if isinstance(val, dict):
-                        context['urls'][key].update(val)
-                    else:
-                        # Because organization_create url is added in this mixin
-                        # and in ``OrganizationRedirectView``.
-                        context['urls'][key] = val
-                else:
-                    context['urls'].update({key: val})
+    key_url_kwarg = 'verification_key'
+
+    def prefetch_contact_info(self):
+        data = {}
+        verification_key = self.kwargs.get(self.key_url_kwarg)
+        contact = Contact.objects.get_token(verification_key)
+        if contact:
+            fields = []
+            if self.form_class is not None:
+                fields = six.iterkeys(self.get_initial())
+            elif self.serializer_class is not None:
+                fields = self.serializer_class.Meta.fields
+            for field_name in fields:
+                field_value = getattr(contact, field_name, None)
+                if not field_value and contact.user:
+                    field_value = getattr(contact.user, field_name, None)
+                if field_value:
+                    data.update({field_name: field_value})
+        return data
+
+    def find_candidate(self, **cleaned_data):
+        verification_key = self.kwargs.get(self.key_url_kwarg)
+        contact = Contact.objects.get_token(verification_key)
+        if not contact:
+            raise serializers.ValidationError({
+                'detail': _("verification key not found")})
+
+        if contact.user:
+            email = contact.user.email
         else:
-            context.update({'urls': urls})
-        return context
+            email = contact.email
+
+        return contact.user, email
+
+
+    def check_password(self, user, **cleaned_data):
+        #pylint:disable=unused-argument
+        if (self.request.method.lower() == 'get' and
+            (not user or has_invalid_password(user))):
+            raise IncorrectUser({'email': _("Not found.")})
+        return None
+
+    def create_user(self, **cleaned_data):
+        verification_key = self.kwargs.get(self.key_url_kwarg)
+        full_name = cleaned_data.get('full_name', None)
+        if not full_name:
+            first_name = cleaned_data.get('first_name', "")
+            last_name = cleaned_data.get('last_name', "")
+            full_name = (first_name + ' ' + last_name).strip()
+        # If we don't save the ``User`` model here,
+        # we won't be able to authenticate later.
+        try:
+            user, previously_inactive = Contact.objects.activate_user(
+                verification_key,
+                username=cleaned_data.get('username'),
+                password=cleaned_data.get('new_password'),
+                full_name=full_name)
+        except IntegrityError as err:
+            handle_uniq_error(err)
+
+        if user:
+            if not user.last_login:
+                # XXX copy/paste from models.ActivatedUserManager.create_user
+                LOGGER.info("'%s %s <%s>' registered with username '%s'",
+                    user.first_name, user.last_name, user.email, user,
+                    extra={'event': 'register', 'user': user})
+                signals.user_registered.send(sender=__name__, user=user)
+            elif previously_inactive:
+                LOGGER.info("'%s %s <%s>' activated with username '%s'",
+                    user.first_name, user.last_name, user.email, user,
+                    extra={'event': 'activate', 'user': user})
+                signals.user_activated.send(sender=__name__, user=user,
+                    verification_key=self.kwargs.get(self.key_url_kwarg),
+                    request=self.request)
+
+        # Bypassing authentication here, we are doing frictionless registration
+        # the first time around.
+        user.backend = self.backend_path
+        return user
 
 
-class ContactMixin(UrlsMixin):
+class ContactMixin(settings.EXTRA_MIXIN):
 
     lookup_field = 'slug'
     lookup_url_kwarg = 'user'
     user_queryset = get_user_model().objects.filter(is_active=True)
 
     @property
     def contact(self):
@@ -428,15 +580,15 @@
             lookup_url_kwarg = self.lookup_url_kwarg or self.lookup_field
             filter_kwargs = {'username': self.kwargs[lookup_url_kwarg]}
             user = get_object_or_404(self.user_queryset, **filter_kwargs)
             obj = self.as_contact(user)
         return obj
 
 
-class UserMixin(UrlsMixin):
+class UserMixin(settings.EXTRA_MIXIN):
 
     user_field = 'username'
     user_url_kwarg = 'user'
     user_queryset = get_user_model().objects.filter(is_active=True)
     user_model = get_user_model()
 
     # django-restframework
@@ -468,15 +620,15 @@
         return self.queryset.model(username=contact.slug, email=contact.email,
             first_name=first_name, last_name=last_name)
 
     def get_context_data(self, **kwargs):
         context = super(UserMixin, self).get_context_data(**kwargs)
         # URLs for user
         if is_authenticated(self.request):
-            self.update_context_urls(context, {
+            update_context_urls(context, {
                 'profile_redirect': reverse('accounts_profile'),
                 'user': {
                     'notifications': reverse(
                         'users_notifications', args=(self.user,)),
                     'profile': reverse('users_profile', args=(self.user,)),
                 }
             })
```

### Comparing `djaodjin-signup-0.7.7/signup/models.py` & `djaodjin-signup-0.8.0/signup/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022, Djaodjin Inc.
+# Copyright (c) 2023, Djaodjin Inc.
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice,
 #    this list of conditions and the following disclaimer.
@@ -26,27 +26,28 @@
 User Model for the signup app
 """
 from __future__ import absolute_import
 from __future__ import unicode_literals
 
 import datetime, hashlib, logging, random, re, string
 
+import pyotp
 from django.core.exceptions import ValidationError
 from django.core.validators import (RegexValidator, URLValidator,
     validate_email as validate_email_base)
 from django.contrib.auth import get_user_model
 from django.contrib.auth.models import UserManager
 from django.db import models, transaction, IntegrityError
 from django.template.defaultfilters import slugify
 from django.contrib.auth.hashers import check_password, make_password
 from phonenumber_field.modelfields import PhoneNumberField
 from rest_framework.exceptions import ValidationError as DRFValidationError
 
 from . import settings, signals
-from .backends.mfa import EmailMFABackend
+from .backends.mfa import EmailOTCBackend, PhoneOTCBackend
 from .compat import (gettext_lazy as _, import_string,
     python_2_unicode_compatible, six)
 from .helpers import (datetime_or_now, full_name_natural_split,
     has_invalid_password)
 from .utils import generate_random_slug, handle_uniq_error
 from .validators import validate_phone
 
@@ -59,14 +60,22 @@
     extra_class = settings.EXTRA_FIELD
     if extra_class is None:
         extra_class = models.TextField
     elif isinstance(extra_class, str):
         extra_class = import_string(extra_class)
     return extra_class
 
+def _get_encrypted_field_class():
+    encrypted_class = settings.ENCRYPTED_FIELD
+    if encrypted_class is None:
+        encrypted_class = models.CharField
+    elif isinstance(encrypted_class, str):
+        encrypted_class = import_string(encrypted_class)
+    return encrypted_class
+
 
 def domain_name_validator(value):
     """
     Validates that the given value contains no whitespaces to prevent common
     typos.
     """
     if not value:
@@ -191,34 +200,35 @@
                 # Force is_active to True and create an email verification key
                 # (see above definition of active user).
                 # In case we delegate auth to a SSO provider, we assume
                 # the e-mail address has already been verified.
                 if uses_sso_provider:
                     at_time = datetime_or_now()
                     try:
-                        contact = Contact.objects.get(user=user, email=email)
+                        contact = Contact.objects.get(user=user,
+                            email__iexact=email)
                         contact.email_verified_at = at_time
                         contact.save()
                     except Contact.DoesNotExist:
                         create_kwargs = {
                             'user': user,
                             'email': email,
                             'full_name': user.get_full_name(),
                             'nick_name': user.first_name,
                             'email_verified_at': at_time
                         }
                         Contact.objects.create(**create_kwargs)
                 else:
-                    Contact.objects.prepare_email_verification(user, email,
-                        phone=phone, lang=lang, extra=extra)
+                    Contact.objects.prepare_email_verification(email,
+                        user=user, phone=phone, lang=lang, extra=extra)
             elif phone:
                 # Force is_active to True and create an email verification key
                 # (see above definition of active user).
-                Contact.objects.prepare_phone_verification(user, phone,
-                    email=email, lang=lang, extra=extra)
+                Contact.objects.prepare_phone_verification(phone,
+                    user=user, email=email, lang=lang, extra=extra)
             user.is_active = True
             user.save()
             LOGGER.info("'%s <%s>' registered with username '%s'%s%s",
                 user.get_full_name(), user.email, user,
                 (" and phone %s" % str(phone)) if phone else "",
                 (" and preferred language %s" % str(lang)) if lang else "",
                 extra={'event': 'register', 'user': user})
@@ -293,117 +303,149 @@
                         - datetime.timedelta(days=settings.KEY_EXPIRATION))
                 return self.filter(email_filter | phone_filter).select_related(
                     'user').get()
             except Contact.DoesNotExist:
                 pass # We return None instead here.
         return None
 
-    def prepare_email_verification(self, user, email, at_time=None,
+    def prepare_email_verification(self, email, user=None, at_time=None,
                                    verification_key=None, reason=None,
                                    **kwargs):
         #pylint:disable=too-many-arguments
         at_time = datetime_or_now(at_time)
         if verification_key is None:
             random_key = str(random.random()).encode('utf-8')
             salt = hashlib.sha1(random_key).hexdigest()[:5]
             verification_key = hashlib.sha1(
-                (salt+user.username).encode('utf-8')).hexdigest()
+                (salt+email).encode('utf-8')).hexdigest()
         # XXX The get() needs to be targeted at the write database in order
         # to avoid potential transaction consistency problems.
+        contact = None
         try:
+            if user:
+                contact = self.get(email=email, user=user)
+            else:
+                contact = self.get(email=email, user__isnull=True)
+        except self.model.DoesNotExist:
+            pass
+        if not contact and user:
+            contact = self.filter(email__isnull=True, user=user).first()
+
+        if contact:
+            created = False
             with transaction.atomic():
                 # We have to wrap in a transaction.atomic here, otherwise
                 # we end-up with a TransactionManager error when Contact.slug
                 # already exists in db and we generate new one.
-                contact = self.get(user=user, email=email)
                 if not contact.email_verification_key:
                     # If we already have a verification key, let's keep it.
                     # We want to avoid users clicking multiple times on a link
                     # that will trigger an activate url, then filling the first
                     # form that showed up.
                     contact.email_verification_key = verification_key
                 contact.email_verification_at = at_time
                 # XXX It is possible a 'reason' field would be a better
                 # implementation.
                 if reason:
                     contact.extra = reason
                 contact.save()
-                return contact, False
-        except self.model.DoesNotExist:
+        else:
+            created = True
             kwargs.update({
                 'user': user,
                 'email': email,
-                'full_name': user.get_full_name(),
-                'nick_name': user.first_name,
                 'email_verification_key': verification_key,
                 'email_verification_at': at_time
             })
+            if user:
+                kwargs.update({
+                    'full_name': user.get_full_name(),
+                    'nick_name': user.first_name,
+                })
             if reason:
                 # XXX It is possible a 'reason' field would be a better
                 # implementation.
                 kwargs.update({'extra': reason})
-        return self.create(**kwargs), True
+            contact = self.create(**kwargs)
 
-    def prepare_phone_verification(self, user, phone, at_time=None,
+        return contact, created
+
+
+    def prepare_phone_verification(self, phone, user=None, at_time=None,
                                    verification_key=None, reason=None,
                                    **kwargs):
         #pylint:disable=too-many-arguments
         at_time = datetime_or_now(at_time)
         if verification_key is None:
             random_key = str(random.random()).encode('utf-8')
             salt = hashlib.sha1(random_key).hexdigest()[:5]
             verification_key = hashlib.sha1(
-                (salt+user.username).encode('utf-8')).hexdigest()
+                (salt+phone).encode('utf-8')).hexdigest()
         # XXX The get() needs to be targeted at the write database in order
         # to avoid potential transaction consistency problems.
+        contact = None
         try:
+            if user:
+                contact = self.get(phone=phone, user=user)
+            else:
+                contact = self.get(phone=phone, user__isnull=True)
+        except self.model.DoesNotExist:
+            pass
+        if not contact and user:
+            contact = self.filter(phone__isnull=True, user=user).first()
+
+        if contact:
+            created = False
             with transaction.atomic():
                 # We have to wrap in a transaction.atomic here, otherwise
                 # we end-up with a TransactionManager error when Contact.slug
                 # already exists in db and we generate new one.
-                contact = self.get(user=user, phone=phone)
                 if not contact.phone_verification_key:
                     # If we already have a verification key, let's keep it.
                     # We want to avoid users clicking multiple times on a link
                     # that will trigger an activate url, then filling the first
                     # form that showed up.
                     contact.phone_verification_key = verification_key
                 contact.phone_verification_at = at_time
                 # XXX It is possible a 'reason' field would be a better
                 # implementation.
                 if reason:
                     contact.extra = reason
                 contact.save()
-                return contact, False
-        except self.model.DoesNotExist:
+        else:
+            created = True
             kwargs.update({
                 'user': user,
                 'phone': phone,
-                'full_name': user.get_full_name(),
-                'nick_name': user.first_name,
                 'phone_verification_key': verification_key,
                 'phone_verification_at': at_time
             })
+            if user:
+                kwargs.update({
+                    'full_name': user.get_full_name(),
+                    'nick_name': user.first_name,
+                })
             if reason:
                 # XXX It is possible a 'reason' field would be a better
                 # implementation.
                 kwargs.update({'extra': reason})
-        return self.create(**kwargs), True
+            contact = self.create(**kwargs)
+        return contact, created
 
     def activate_user(self, verification_key,
                       username=None, password=None, full_name=None):
         """
         Activate a user whose email address has been verified.
         """
         #pylint:disable=too-many-arguments
         at_time = datetime_or_now()
         try:
             token = self.get_token(verification_key=verification_key)
             if token:
-                LOGGER.info('user %s activated through code: %s',
+                LOGGER.info('active user %s through code: %s ...',
                     token.user, verification_key,
                     extra={'event': 'activate', 'username': token.user.username,
                         'verification_key': verification_key,
                         'email_verification_key': token.email_verification_key,
                         'phone_verification_key': token.phone_verification_key})
                 previously_inactive = has_invalid_password(token.user)
                 with transaction.atomic():
@@ -418,23 +460,32 @@
                     if full_name:
                         token.full_name = full_name
                         #pylint:disable=unused-variable
                         first_name, mid_name, last_name = \
                             full_name_natural_split(full_name)
                         token.user.first_name = first_name
                         token.user.last_name = last_name
+                        LOGGER.info('%s (first_name, last_name) needs '\
+                            'to be saved as ("%s", "%s")', verification_key,
+                            token.user.first_name, token.user.last_name)
                         needs_save = True
                     if username:
                         token.user.username = username
+                        LOGGER.info('%s username needs to be saved as "%s"',
+                            verification_key, token.user.username)
                         needs_save = True
                     if password:
                         token.user.set_password(password)
+                        LOGGER.info('%s password needs to be saved',
+                            verification_key)
                         needs_save = True
                     if not token.user.is_active:
                         token.user.is_active = True
+                        LOGGER.info('%s user needs to be activated',
+                            verification_key)
                         needs_save = True
                     if needs_save:
                         token.user.save()
                 return token.user, previously_inactive
         except Contact.DoesNotExist:
             pass # We return None instead here.
         return None, None
@@ -455,20 +506,22 @@
 
 
 @python_2_unicode_compatible
 class Contact(models.Model):
     """
     Used in workflow to verify the email address of a ``User``.
     """
-    NO_MFA = 0
+    NO_OTC = 0
     EMAIL_BACKEND = 1
+    PHONE_BACKEND = 2
 
-    MFA_BACKEND_TYPE = (
-        (NO_MFA, "password only"),
+    OTC_BACKEND_TYPE = (
+        (NO_OTC, "send link instead of one-time code"),
         (EMAIL_BACKEND, "send one-time authentication code through email"),
+        (PHONE_BACKEND, "send one-time authentication code through phone"),
     )
 
     objects = ContactManager()
 
     slug = models.SlugField(unique=True,
         help_text=_("Unique identifier shown in the URL bar, effectively"\
             " the username for profiles with login credentials."))
@@ -485,15 +538,15 @@
     # 2083 number is used because it is a safe option to choose based
     # on some older browsers behavior
     # https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=4&cad=rja&uact=8&ved=2ahUKEwi2hbjPwIPgAhULXCsKHQ-lAj4QFjADegQIBhAL&url=https%3A%2F%2Fstackoverflow.com%2Fquestions%2F417142%2Fwhat-is-the-maximum-length-of-a-url-in-different-browsers&usg=AOvVaw0QgMo_L7jjK0YsXchrJgOQ
     picture = models.URLField(_("URL to a profile picture"), max_length=2083,
         null=True, blank=True,
         help_text=_("URL location of the profile picture"))
     user = models.ForeignKey(settings.AUTH_USER_MODEL,
-        null=True, on_delete=models.CASCADE, related_name='contacts')
+        null=True, on_delete=models.SET_NULL, related_name='contacts')
     # key must be unique when used in URLs. IF we use a code,
     # then it shouldn't be.
     email_verification_key = models.CharField(_(
         "Email verification key"),
          null=True, max_length=40)
     email_verification_at = models.DateTimeField(null=True,
         help_text=_("Date/time when the e-mail verification key was sent"))
@@ -506,21 +559,21 @@
         help_text=_("Date/time when the phone verification key was sent"))
     phone_verified_at = models.DateTimeField(null=True,
         help_text=_("Date/time when the phone number was last verified"))
     lang = models.CharField(_("Preferred communication language"),
          default=settings.LANGUAGE_CODE, max_length=8,
         help_text=_("Two-letter ISO 639 code for the preferred"\
         " communication language (ex: en)"))
-    mfa_backend = models.PositiveSmallIntegerField(
-        choices=MFA_BACKEND_TYPE, default=NO_MFA,
+    otc_backend = models.PositiveSmallIntegerField(
+        choices=OTC_BACKEND_TYPE, default=NO_OTC,
         help_text=_("Backend to use for multi-factor authentication"))
-    mfa_priv_key = models.IntegerField(
+    one_time_code = models.IntegerField(
         _("One-time authentication code"), null=True)
-    mfa_nb_attempts = models.IntegerField(
-        _("Number of attempts to pass the MFA code"), default=0)
+    otc_nb_attempts = models.IntegerField(
+        _("Number of attempts to pass the one-time code"), default=0)
     extra = _get_extra_field_class()(null=True,
         help_text=_("Extra meta data (can be stringify JSON)"))
 
     def __str__(self):
         return str(self.slug)
 
     @property
@@ -531,48 +584,53 @@
     def printable_name(self):
         if self.nick_name:
             return self.nick_name
         if self.full_name:
             return self.full_name
         return self.username
 
-    def get_mfa_backend(self):
-        if self.mfa_backend == self.EMAIL_BACKEND:
-            return EmailMFABackend()
+    def get_otc_backend(self):
+        if self.otc_backend == self.EMAIL_BACKEND:
+            return EmailOTCBackend()
+        if self.otc_backend == self.PHONE_BACKEND:
+            return PhoneOTCBackend()
         return None
 
-    def create_mfa_token(self):
-        return self.get_mfa_backend().create_token(self)
+    def create_otc_token(self):
+        return self.get_otc_backend().create_token(self)
 
-    def clear_mfa_token(self):
-        self.mfa_priv_key = None
-        self.mfa_nb_attempts = 0
+    def clear_otc_token(self):
+        self.one_time_code = None
+        self.otc_nb_attempts = 0
         self.save()
 
     def save(self, force_insert=False, force_update=False,
              using=None, update_fields=None):
         if not self.lang:
             self.lang = settings.LANGUAGE_CODE
         if self.slug: # serializer will set created slug to '' instead of None.
             return super(Contact, self).save(
                 force_insert=force_insert, force_update=force_update,
                 using=using, update_fields=update_fields)
         max_length = self._meta.get_field('slug').max_length
-        slug_base = (self.user.username
-            if self.user else slugify(self.email.split('@')[0]))
-        if not slug_base:
+        slug_base = None
+        if self.user:
+            slug_base = self.user.username
+        if not slug_base and self.email:
             # email might be empty
+            slug_base = slugify(self.email.split('@', maxsplit=1)[0])
+        if not slug_base:
             slug_base = generate_random_slug(15)
         elif len(slug_base) > max_length:
             slug_base = slug_base[:max_length]
         self.slug = slug_base
         for idx in range(1, 10): #pylint:disable=unused-variable
             try:
                 try:
-                    with transaction.atomic():
+                    with transaction.atomic(using=using):
                         if self.user:
                             # pylint:disable=unused-variable
                             save_user = False
                             first_name, mid_name, last_name = \
                                 full_name_natural_split(self.full_name)
                             if not self.user.first_name:
                                 self.user.first_name = first_name
@@ -651,40 +709,67 @@
 
 @python_2_unicode_compatible
 class Credentials(models.Model):
     """
     API Credentials to authenticate a `User`.
     """
     API_PUB_KEY_LENGTH = 32
-    API_PRIV_KEY_LENGTH = 32
+    API_PASSWORD_LENGTH = 32
 
     api_pub_key = models.SlugField(unique=True, max_length=API_PUB_KEY_LENGTH)
-    api_priv_key = models.CharField(max_length=128)
+    api_password = models.CharField(max_length=128)
     user = models.OneToOneField(settings.AUTH_USER_MODEL,
         on_delete=models.CASCADE, related_name='credentials')
     extra = _get_extra_field_class()(null=True)
 
     def __str__(self):
         return str(self.api_pub_key)
 
-    def set_priv_key(self, api_priv_key):
-        self.api_priv_key = make_password(api_priv_key)
-        self._api_priv_key = api_priv_key
+    def set_priv_key(self, api_password):
+        #pylint:disable=attribute-defined-outside-init
+        self.api_password = make_password(api_password)
+        self._api_password = api_password
 
-    def check_priv_key(self, raw_api_priv_key):
+    def check_priv_key(self, raw_api_password):
         """
-        Return a boolean of whether the raw api_priv_key was correct. Handles
+        Return a boolean of whether the raw api_password was correct. Handles
         hashing formats behind the scenes.
         """
-        def setter(raw_api_priv_key):
-            self.set_priv_key(raw_api_priv_key)
+        def setter(raw_api_password):
+            #pylint:disable=attribute-defined-outside-init
+            self.set_priv_key(raw_api_password)
             # Password hash upgrades shouldn't be considered password changes.
-            self._api_priv_key = None
-            self.save(update_fields=["api_priv_key"])
-        return check_password(raw_api_priv_key, self.api_priv_key, setter)
+            self._api_password = None
+            self.save(update_fields=["api_password"])
+        return check_password(raw_api_password, self.api_password, setter)
+
+
+class OTPGenerator(models.Model):
+    """
+    Generates OTP one-time code for authentication
+    """
+
+    user = models.OneToOneField(settings.AUTH_USER_MODEL,
+        on_delete=models.CASCADE, related_name='otp')
+    priv_key = _get_encrypted_field_class()(
+        _("Private key for the OTP generator"), max_length=40, null=True)
+    nb_attempts = models.IntegerField(
+        _("Number of attempts to pass the OTP code"), default=0)
+
+    def verify(self, code):
+        totp = pyotp.TOTP(self.priv_key)
+        return totp.verify(code)
+
+    def clear_attempts(self):
+        self.nb_attempts = 0
+        self.save()
+
+    def provisioning_uri(self, issuer_name=None):
+        return pyotp.totp.TOTP(self.priv_key).provisioning_uri(
+            name=self.user.email, issuer_name=issuer_name)
 
 
 @python_2_unicode_compatible
 class DelegateAuth(models.Model):
     """
     Authentication for users with e-mail addresses in these domains must be
     delegated to a SSO provider.
@@ -703,16 +788,16 @@
 
 
 def get_user_contact(user):
     if isinstance(settings.USER_CONTACT_CALLABLE, six.string_types):
         return import_string(settings.USER_CONTACT_CALLABLE)(user)
     if user:
         return Contact.objects.filter(
-            models.Q(slug=user.username)
-            | models.Q(email=user.email)).order_by(
+            models.Q(slug__iexact=user.username)
+            | models.Q(email__iexact=user.email)).order_by(
             'slug', 'email').first()
     return None
 
 
 def get_nick_name(obj):
     if hasattr(obj, 'nick_name'):
         return obj.nick_name
```

### Comparing `djaodjin-signup-0.7.7/signup/serializers.py` & `djaodjin-signup-0.8.0/signup/serializers.py`

 * *Files 7% similar despite different names*

```diff
@@ -71,29 +71,14 @@
     def create(self, validated_data):
         raise RuntimeError('`create()` should not be called.')
 
     def update(self, instance, validated_data):
         raise RuntimeError('`update()` should not be called.')
 
 
-class ActivateSerializer(serializers.ModelSerializer):
-
-    username = serializers.CharField(required=False,
-        help_text=_("Username to identify the account"))
-    new_password = serializers.CharField(required=False, write_only=True,
-        style={'input_type': 'password'}, help_text=_("Password with which"\
-            " a user can authenticate with the service"))
-    full_name = serializers.CharField(required=False,
-        help_text=_("Full name (effectively first name followed by last name)"))
-
-    class Meta:
-        model = get_user_model()
-        fields = ('username', 'new_password', 'full_name')
-
-
 class ActivitySerializer(serializers.ModelSerializer):
 
     account = get_account_serializer()(allow_null=True,
         help_text=_("Account the activity is associated to"))
     created_by = get_user_serializer()(read_only=True,
         help_text=_("User that created the activity"))
 
@@ -132,23 +117,14 @@
         help_text=_("Secret API Key used to authenticate user on every HTTP"\
         " request"))
 
     class Meta:
         fields = ('secret',)
 
 
-class PublicKeySerializer(AuthenticatedUserPasswordSerializer):
-    """
-    Updates a user public key
-    """
-    pubkey = serializers.CharField(max_length=500,
-        style={'input_type': 'password'},
-        help_text=_("New public key for the user referenced in the URL"))
-
-
 class StringListField(serializers.ListField):
     child = serializers.CharField()
 
 
 class NotificationsSerializer(serializers.ModelSerializer):
 
     notifications = StringListField(allow_empty=True,
@@ -173,29 +149,64 @@
     code = serializers.IntegerField(required=False, write_only=True,
         style={'input_type': 'password'},
         help_text=_("One-time code. This field will be checked against"\
             " an expected code when multi-factor authentication (MFA)"\
             " is enabled."))
 
 
+class OTPUpdateSerializer(AuthenticatedUserPasswordSerializer):
+    """
+    Returns sensitive information to setup OTP generator
+    """
+    enable = serializers.BooleanField(write_only=True,
+        help_text=_("Enables/disables OTP"))
+
+    class Meta(AuthenticatedUserPasswordSerializer.Meta):
+        fields = AuthenticatedUserPasswordSerializer.Meta.fields + (
+            'enable',)
+
+
+class OTPSerializer(NoModelSerializer):
+    """
+    Returns sensitive information to setup OTP generator
+    """
+    priv_key = serializers.CharField(
+        help_text=_("Private key"))
+    provisioning_uri = serializers.URLField(
+        help_text=_("Provisioning URI"))
+
+    class Meta:
+        fields = ('priv_key', 'provisioning_uri')
+        read_only_fields = ('priv_key', 'provisioning_uri')
+
+
+class PublicKeySerializer(AuthenticatedUserPasswordSerializer):
+    """
+    Updates a user public key
+    """
+    pubkey = serializers.CharField(max_length=500,
+        style={'input_type': 'password'},
+        help_text=_("New public key for the user referenced in the URL"))
+
+
 class PasswordResetConfirmSerializer(NoModelSerializer):
 
     new_password = serializers.CharField(write_only=True,
         style={'input_type': 'password'},
         help_text=_("New password for the user referenced in the URL"))
 
 
 class PasswordChangeSerializer(PasswordResetConfirmSerializer):
 
     password = serializers.CharField(write_only=True,
         style={'input_type': 'password'},
         help_text=_("Password of the user making the HTTP request"))
 
 
-class PasswordResetSerializer(NoModelSerializer):
+class RecoverSerializer(NoModelSerializer):
     """
     Serializer to send an e-mail to a user in order to recover her account.
     """
     email = CommField(
         help_text=_("Email or phone number to recover the account"))
 
 
@@ -223,23 +234,32 @@
         help_text=_("URL to uploaded content"))
 
 
 class UserCreateSerializer(UserDetailSerializer):
 
     username = serializers.CharField(required=False,
         help_text=_("Unique identifier for the user, typically used in URLs"))
-    password = serializers.CharField(required=False, write_only=True,
+    new_password = serializers.CharField(required=False, write_only=True,
         style={'input_type': 'password'}, help_text=_("Password with which"\
             " a user can authenticate with the service"))
     full_name = serializers.CharField(
         help_text=_("Full name (effectively first name followed by last name)"))
 
     class Meta(UserDetailSerializer.Meta):
-        fields = UserDetailSerializer.Meta.fields + ('password',)
+        fields = UserDetailSerializer.Meta.fields + ('new_password',)
 
     def validate(self, attrs):
         if not (attrs.get('email') or
             attrs.get('phone', attrs.get('get_phone'))):
             raise ValidationError(
                 {'email': _("Either email or phone must be valid."),
                  'phone': _("Either email or phone must be valid.")})
         return super(UserCreateSerializer, self).validate(attrs)
+
+
+class UserActivateSerializer(UserCreateSerializer):
+
+    new_password = serializers.CharField(required=True, write_only=True,
+        style={'input_type': 'password'}, help_text=_("Password with which"\
+            " a user can authenticate with the service"))
+    full_name = serializers.CharField(required=False,
+        help_text=_("Full name (effectively first name followed by last name)"))
```

### Comparing `djaodjin-signup-0.7.7/signup/serializers_overrides.py` & `djaodjin-signup-0.8.0/signup/serializers_overrides.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.7.7/signup/settings.py` & `djaodjin-signup-0.8.0/signup/settings.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2021, Djaodjin Inc.
+# Copyright (c) 2023, Djaodjin Inc.
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice,
 #    this list of conditions and the following disclaimer.
@@ -38,14 +38,15 @@
 DISABLED_REGISTRATION
    prevent new users from registering
 
 REQUIRE_RECAPTCHA
    Requires to answer a recaptcha in registration
 """
 
+import django
 from django.conf import settings
 
 _SETTINGS = {
     'ACCOUNT_ACTIVATION_DAYS': getattr(settings, 'ACCOUNT_ACTIVATION_DAYS', 2),
     'ACCOUNT_MODEL': getattr(settings, 'AUTH_USER_MODEL', None),
     'ACCOUNT_SERIALIZER': 'signup.serializers_overrides.UserSerializer',
     'AUTH_USER_MODEL': getattr(settings, 'AUTH_USER_MODEL'),
@@ -55,37 +56,40 @@
     'AWS_UPLOAD_ROLE': None,
     'AWS_S3_BUCKET_NAME': getattr(settings, 'AWS_S3_BUCKET_NAME', None),
     'BYPASS_VERIFICATION_KEY_EXPIRED_CHECK': False,
     'DEFAULT_FROM_EMAIL': getattr(settings, 'DEFAULT_FROM_EMAIL'),
     'DISABLED_AUTHENTICATION': False,
     'DISABLED_REGISTRATION': False,
     'EMAIL_DYNAMIC_VALIDATOR': None,
+    'ENCRYPTED_FIELD': (
+        # django-fernet==0.6 is not compatible with Django4+ (``force_text``)
+        'fernet_fields.EncryptedCharField' if django.VERSION[0] < 4 else None),
     'EXTRA_FIELD': None,
+    'EXTRA_MIXIN': object,
     'JWT_ALGORITHM': 'HS256',
     'JWT_SECRET_KEY': getattr(settings, 'SECRET_KEY'),
     'LDAP': {
         'SERVER_URI': None,
         'USER_SERCH_DN': None
     },
     'LOGIN_THROTTLE': None,
     'LOGOUT_CLEAR_COOKIES' : None,
     'MFA_MAX_ATTEMPTS': 3,
     'NOTIFICATION_TYPE': tuple([]),
     'NOTIFICATIONS_OPT_OUT': True,
-    'PASSWORD_RESET_THROTTLE': None,
     'PICTURE_STORAGE_CALLABLE': None,
     'RANDOM_SEQUENCE': [],
     'REQUIRES_RECAPTCHA': False,
     'SEARCH_FIELDS_PARAM': 'q_f',
     'SSO_PROVIDERS': {
         'azuread-oauth2': {'name': 'Microsoft'},
         'github': {'name': 'GitHub'},
         'google-oauth2': {'name': 'Google'},
     },
-    'USER_CONTACT_CALLABLE': None,
+    'USER_CONTACT_CALLABLE': None,  # XXX deprecated?
     'USER_SERIALIZER': 'signup.serializers_overrides.UserSerializer',
 }
 _SETTINGS.update(getattr(settings, 'SIGNUP', {}))
 
 ACCOUNT_MODEL = _SETTINGS.get('ACCOUNT_MODEL')
 ACCOUNT_SERIALIZER = _SETTINGS.get('ACCOUNT_SERIALIZER')
 AUTH_USER_MODEL = _SETTINGS.get('AUTH_USER_MODEL')
@@ -93,30 +97,50 @@
 AWS_UPLOAD_ROLE = _SETTINGS.get('AWS_UPLOAD_ROLE')
 AWS_ACCOUNT_ID = _SETTINGS.get('AWS_ACCOUNT_ID')
 AWS_EXTERNAL_ID = _SETTINGS.get('AWS_EXTERNAL_ID')
 AWS_S3_BUCKET_NAME = _SETTINGS.get('AWS_S3_BUCKET_NAME')
 BYPASS_VERIFICATION_KEY_EXPIRED_CHECK = _SETTINGS.get(
     'BYPASS_VERIFICATION_KEY_EXPIRED_CHECK')
 DEFAULT_FROM_EMAIL = _SETTINGS.get('DEFAULT_FROM_EMAIL')
+
+#: When `True`, authentication on the site is disabled.
+#: This settings can either be a boolean value or a callable function.
 DISABLED_AUTHENTICATION = _SETTINGS.get('DISABLED_AUTHENTICATION')
+
+#: When `True`, registration of new users on the site is disabled.
+#: This settings can either be a boolean value or a callable function.
 DISABLED_REGISTRATION = _SETTINGS.get('DISABLED_REGISTRATION')
+
+#: A callable function which is passed an email address and that returns `False`
+#: when the email suspiciously looks like it belongs to a bot.
 EMAIL_DYNAMIC_VALIDATOR = _SETTINGS.get('EMAIL_DYNAMIC_VALIDATOR')
+
+ENCRYPTED_FIELD = _SETTINGS.get('ENCRYPTED_FIELD')
 EXTRA_FIELD = _SETTINGS.get('EXTRA_FIELD')
+EXTRA_MIXIN = _SETTINGS.get('EXTRA_MIXIN')
 JWT_SECRET_KEY = _SETTINGS.get('JWT_SECRET_KEY')
 JWT_ALGORITHM = _SETTINGS.get('JWT_ALGORITHM')
 KEY_EXPIRATION = _SETTINGS.get('ACCOUNT_ACTIVATION_DAYS')
 LDAP_SERVER_URI = _SETTINGS.get('LDAP', {}).get('SERVER_URI', None)
 LDAP_USER_SEARCH_DN = _SETTINGS.get('LDAP', {}).get('USER_SERCH_DN', None)
+
+#: A callable function, which is passed a triplet (request, view, user), and
+#: that throttles the HTTP request when there are too many attempts for that
+#: particular user to login.
 LOGIN_THROTTLE = _SETTINGS.get('LOGIN_THROTTLE')
+
 LOGOUT_CLEAR_COOKIES = _SETTINGS.get('LOGOUT_CLEAR_COOKIES')
 MFA_MAX_ATTEMPTS = _SETTINGS.get('MFA_MAX_ATTEMPTS')
 NOTIFICATION_TYPE = _SETTINGS.get('NOTIFICATION_TYPE')
 NOTIFICATIONS_OPT_OUT = _SETTINGS.get('NOTIFICATIONS_OPT_OUT')
-PASSWORD_RESET_THROTTLE = _SETTINGS.get('PASSWORD_RESET_THROTTLE')
+
+#: A callable function which returns a `Storage` object that will be used
+#: to upload a contact picture
 PICTURE_STORAGE_CALLABLE = _SETTINGS.get('PICTURE_STORAGE_CALLABLE')
+
 RANDOM_SEQUENCE = _SETTINGS.get('RANDOM_SEQUENCE')
 REQUIRES_RECAPTCHA = _SETTINGS.get('REQUIRES_RECAPTCHA')
 SEARCH_FIELDS_PARAM = _SETTINGS.get('SEARCH_FIELDS_PARAM')
 SSO_PROVIDERS = _SETTINGS.get('SSO_PROVIDERS')
 USER_CONTACT_CALLABLE = _SETTINGS.get('USER_CONTACT_CALLABLE')
 USER_SERIALIZER = _SETTINGS.get('USER_SERIALIZER')
```

### Comparing `djaodjin-signup-0.7.7/signup/signals.py` & `djaodjin-signup-0.8.0/signup/signals.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.7.7/signup/static/js/djaodjin-password-strength.js` & `djaodjin-signup-0.8.0/signup/static/js/djaodjin-password-strength.js`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.7.7/signup/static/js/djaodjin-resources-vue.js` & `djaodjin-signup-0.8.0/signup/static/js/djaodjin-resources-vue.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -153,22 +153,151 @@
                     }
                 }
                 vm.showMessages(messages, "error");
             },
         }
     };
 
+
+    /** compute outdated based on `params`.
+
+        `params = {start_at, ends_at}` must exist in either the `props` or `data`
+        of the component.
+
+        A subclass of this mixin must define either the function `autoReload`
+        or `reload` in order to make updates as a user is typing in input fields
+        or when a button is pressed respectively.
+     */
+    var paramsMixin = {
+        data: function() {
+            var data = {
+                lastGetParams: {},
+            }
+            return data;
+        },
+        methods: {
+            asDateInputField: function(dateISOString) {
+                const dateValue = moment(dateISOString);
+                return dateValue.isValid() ? dateValue.format("YYYY-MM-DD") : null;
+            },
+            asDateISOString: function(dateInputField) {
+                const dateValue = moment(dateInputField, "YYYY-MM-DD");
+                return dateValue.isValid() ? dateValue.toISOString() : null;
+            },
+            autoReload: function() {},
+            reload: function() {},
+            getParams: function(excludes) {
+                var vm = this;
+                var params = {};
+                for (var key in vm.params) {
+                    if (vm.params.hasOwnProperty(key) && vm.params[key]) {
+                        if (excludes && key in excludes) continue;
+                        params[key] = vm.params[key];
+                    }
+                }
+                return params;
+            },
+            getQueryString: function(excludes) {
+                var vm = this;
+                var sep = "";
+                var result = "";
+                var params = vm.getParams(excludes);
+                for (var key in params) {
+                    if (params.hasOwnProperty(key)) {
+                        result += sep + key + '=' + encodeURIComponent(
+                            params[key].toString());
+                        sep = "&";
+                    }
+                }
+                if (result) {
+                    result = '?' + result;
+                }
+                return result;
+            },
+        },
+        computed: {
+            _start_at: {
+                get: function() {
+                    return this.asDateInputField(this.params.start_at);
+                },
+                set: function(newVal) {
+                    if (newVal) {
+                        // The setter might be call with `newVal === null`
+                        // when the date is incorrect (ex: 09/31/2022).
+                        this.$set(this.params, 'start_at',
+                            this.asDateISOString(newVal));
+                        if (this.outdated) this.debouncedAutoReload();
+                    }
+                }
+            },
+            _ends_at: {
+                get: function() {
+                    // form field input="date" will expect ends_at as a String
+                    // but will literally cut the hour part regardless of timezone.
+                    // We don't want an empty list as a result.
+                    // If we use moment `endOfDay` we get 23:59:59 so we
+                    // add a full day instead. It seemed clever to run the following
+                    // code but that prevented entering the year part in the input
+                    // field (as oppossed to use the widget).
+                    //
+                    // const dateValue = moment(this.params.ends_at).add(1,'days');
+                    // return dateValue.isValid() ? dateValue.format("YYYY-MM-DD") : null;
+                    return this.asDateInputField(this.params.ends_at);
+                },
+                set: function(newVal) {
+                    if (newVal) {
+                        // The setter might be call with `newVal === null`
+                        // when the date is incorrect (ex: 09/31/2022).
+                        this.$set(this.params, 'ends_at',
+                            this.asDateISOString(newVal));
+                        if (this.outdated) this.debouncedAutoReload();
+                    }
+                }
+            },
+            outdated: function() {
+                var vm = this;
+                const params = vm.getParams();
+                for (var key in vm.lastGetParams) {
+                    if (vm.lastGetParams.hasOwnProperty(key)) {
+                        if (vm.lastGetParams[key] !== params[key]) {
+                            return true;
+                        }
+                    }
+                }
+                for (var key in params) {
+                    if (params.hasOwnProperty(key)) {
+                        if (params[key] !== vm.lastGetParams[key]) {
+                            return true;
+                        }
+                    }
+                }
+                return false;
+            }
+        },
+        created: function() {
+            // _.debounce is a function provided by lodash to limit how
+            // often a particularly expensive operation can be run.
+            if (typeof _ != 'undefined' && typeof _.debounce != 'undefined') {
+                this.debouncedAutoReload = _.debounce(this.autoReload, 500);
+            } else {
+                this.debouncedAutoReload = this.autoReload;
+            }
+        }
+    };
+
+
     /** A wrapper around jQuery ajax functions that adds authentication
         parameters as necessary.
 
         requires `jQuery`
     */
     var httpRequestMixin = {
         mixins: [
-            messagesMixin
+            messagesMixin,
+            paramsMixin
         ],
         // XXX conflitcs when params defined as props
         //    data: function() {
         //        return {
         //            params: {}
         //        }
         //    },
@@ -213,52 +342,41 @@
                 }
                 return "";
             },
 
             _safeUrl: function(base, path) {
                 if (!path) return base;
 
-                if (base && base[base.length - 1] == '/') {
-                    if (path && path[0] == '/') {
-                        return base + path.substring(1);
+                const parts = [base].concat(
+                    (typeof path === 'string') ? [path] : path);
+                var cleanParts = [];
+                var start, end;
+                for (var idx = 0; idx < parts.length; ++idx) {
+                    const part = parts[idx];
+                    for (start = 0; start < part.length; ++start) {
+                        if (part[start] !== '/') {
+                            break;
+                        }
                     }
-                    return base + path;
-                }
-                if (path && path[0] == '/') {
-                    return base + path;
-                }
-                return base + '/' + path;
-            },
-
-            getParams: function(excludes) {
-                var vm = this;
-                var params = {};
-                for (var key in vm.params) {
-                    if (vm.params.hasOwnProperty(key) && vm.params[key]) {
-                        if (excludes && key in excludes) continue;
-                        params[key] = vm.params[key];
+                    for (end = part.length - 1; end >= 0; --end) {
+                        if (part[end] !== '/') {
+                            break;
+                        }
                     }
-                }
-                return params;
-            },
-            getQueryString: function(excludes) {
-                var vm = this;
-                var sep = "";
-                var result = "";
-                var params = vm.getParams(excludes);
-                for (var key in params) {
-                    if (params.hasOwnProperty(key)) {
-                        result += sep + key + '=' + params[key].toString();
-                        sep = "&";
+                    if (start < end) {
+                        cleanParts.push(part.slice(start, end + 1));
+                    } else {
+                        cleanParts.push(part);
                     }
                 }
-                if (result) {
-                    result = '?' + result;
+                var cleanUrl = cleanParts[0];
+                for (idx = 1; idx < cleanParts.length; ++idx) {
+                    cleanUrl += '/' + cleanParts[idx];
                 }
-                return result;
+                return cleanUrl.startsWith('http') ? cleanUrl[0] : '/' + cleanUrl;
             },
 
             /** This method generates a GET HTTP request to `url` with a query
                 string built of a `queryParams` dictionnary.
 
                 It supports the following prototypes:
 
@@ -709,38 +827,37 @@
                 if (!successCallback) {
                     successCallback = function() {};
                 }
                 if (!failureCallback) {
                     failureCallback = vm.showErrorMessages;
                 }
                 for (var idx = 0; idx < queryArray.length; ++idx) {
-                    ajaxCalls.push(function() {
-                        return $.ajax({
-                            method: queryArray[idx].method,
-                            url: queryArray[idx].url,
-                            data: JSON.stringify(queryArray[idx].data),
-                            beforeSend: function(xhr, settings) {
-                                var authToken = vm._getAuthToken();
-                                if (authToken) {
-                                    xhr.setRequestHeader("Authorization",
-                                        "Bearer " + authToken);
-                                } else {
-                                    if (!vm._csrfSafeMethod(settings.type)) {
-                                        var csrfToken = vm._getCSRFToken();
-                                        if (csrfToken) {
-                                            xhr.setRequestHeader("X-CSRFToken", csrfToken);
-                                        }
+                    ajaxCalls.push($.ajax({
+                        method: queryArray[idx].method,
+                        url: queryArray[idx].url,
+                        data: JSON.stringify(queryArray[idx].data),
+                        beforeSend: function(xhr, settings) {
+                            var authToken = vm._getAuthToken();
+                            if (authToken) {
+                                xhr.setRequestHeader("Authorization",
+                                    "Bearer " + authToken);
+                            } else {
+                                if (!vm._csrfSafeMethod(settings.type)) {
+                                    var csrfToken = vm._getCSRFToken();
+                                    if (csrfToken) {
+                                        xhr.setRequestHeader("X-CSRFToken", csrfToken);
                                     }
                                 }
-                            },
-                            contentType: 'application/json',
-                        });
-                    }());
+                            }
+                        },
+                        contentType: 'application/json',
+                    }));
                 }
-                jQuery.when(ajaxCalls).done(successCallback).fail(failureCallback);
+                jQuery.when.apply(jQuery, ajaxCalls).done(successCallback).fail(
+                    failureCallback);
             },
         }
     }
 
 
     var itemMixin = {
         mixins: [
@@ -791,83 +908,56 @@
                 }
                 return !isEmpty;
             },
         },
     }
 
 
-    var filterableMixin = {
-        data: function() {
-            return {
-                params: {
-                    q: '',
-                },
-                mixinFilterCb: 'get',
-            }
-        },
-        methods: {
-            filterList: function() {
-                if (this.params.q) {
-                    if ("page" in this.params) {
-                        this.params.page = 1;
-                    }
-                }
-                if (this[this.mixinFilterCb]) {
-                    this[this.mixinFilterCb]();
-                }
-            },
-        },
-    }
-
-
     var paginationMixin = {
         data: function() {
             return {
                 params: {
                     page: 1,
                 },
+                mergeResults: false,
                 itemsPerPage: this.$itemsPerPage,
                 ellipsisThreshold: 4,
+                preReload: ['resetPage'],
                 getCompleteCb: 'getCompleted',
                 getBeforeCb: 'resetPage',
-                qsCache: null,
-                isInfiniteScroll: false,
             }
         },
         methods: {
             resetPage: function() {
                 var vm = this;
-                if (!vm.ISState) return;
-                if (vm.qsCache && vm.qsCache !== vm.qs) {
-                    vm.params.page = 1;
-                    vm.ISState.reset();
-                }
-                vm.qsCache = vm.qs;
+                vm.params.page = 1;
             },
             getCompleted: function() {
                 var vm = this;
-                if (!vm.ISState) return;
                 vm.mergeResults = false;
-                if (vm.pageCount > 0) {
-                    vm.ISState.loaded();
-                }
-                if (vm.params.page >= vm.pageCount) {
-                    vm.ISState.complete();
+            },
+            handleScroll: function(evt) {
+                var vm = this;
+                let element = this.$el;
+                if (element.getBoundingClientRect().bottom < window.innerHeight) {
+                    let menubar = vm.$el.querySelector('[role="pagination"]');
+                    var style = window.getComputedStyle(menubar);
+                    if (style.display == 'none') {
+                        // We are not displaying the pagination menubar,
+                        // so let's scroll!
+                        vm.paginationHandler();
+                    }
                 }
             },
             paginationHandler: function($state) {
                 var vm = this;
-                if (!vm.ISState) return;
-                if (!vm.itemsLoaded) {
-                    // this handler is triggered on initial get too
+                if (!vm.itemsLoaded || vm.mergeResults) {
+                    // this handler is triggered on initial get() too.
                     return;
                 }
-                // rudimentary way to detect which type of pagination
-                // is active. ideally need to monitor resolution changes
-                vm.isInfiniteScroll = true;
                 var nxt = vm.params.page + 1;
                 if (nxt <= vm.pageCount) {
                     vm.$set(vm.params, 'page', nxt);
                     vm.mergeResults = true;
                     vm.get();
                 }
             },
@@ -923,23 +1013,21 @@
                 var vm = this;
                 var pages = [];
                 for (var idx = vm.minDirectPageLink; idx <= vm.maxDirectPageLink; ++idx) {
                     pages.push(idx);
                 }
                 return pages;
             },
-            ISState: function() {
-                if (!this.$refs.infiniteLoading) return;
-                return this.$refs.infiniteLoading.stateChanger;
-            },
-            qs: function() {
-                return this.getQueryString({
-                    page: null
-                });
-            },
+        },
+        mounted: function() {
+            var vm = this;
+            window.addEventListener("scroll", vm.handleScroll);
+        },
+        unmounted: function() {
+            window.removeEventListener("scroll", vm.handleScroll);
         }
     }
 
 
     var sortableMixin = {
         data: function() {
             var defaultDir = this.$sortDirection || 'desc';
@@ -1034,41 +1122,39 @@
     }
 
 
     var itemListMixin = {
         mixins: [
             httpRequestMixin,
             paginationMixin,
-            filterableMixin,
             sortableMixin
         ],
         data: function() {
             return this.getInitData();
         },
         methods: {
             getInitData: function() {
                 var data = {
                     url: null,
-                    itemsLoaded: false,
-                    items: {
-                        results: [],
-                        count: 0
-                    },
-                    mergeResults: false,
                     params: {
                         // The following dates will be stored as `String` objects
                         // as oppossed to `moment` or `Date` objects because this
                         // is how form fields input="date" will update them.
                         start_at: null,
                         ends_at: null,
                         // The timezone for both start_at and ends_at.
-                        timezone: 'local'
+                        timezone: 'local',
+                        q: '',
+                    },
+                    itemsLoaded: false,
+                    items: {
+                        results: [],
+                        count: 0
                     },
-                    lastGetParams: {},
-                    autoreload: true,
+                    mergeResults: false,
                     getCb: null,
                     getCompleteCb: null,
                     getBeforeCb: null,
                 }
                 if (this.$dateRange) {
                     if (this.$dateRange.start_at) {
                         data.params['start_at'] = this.$dateRange.start_at;
@@ -1118,89 +1204,33 @@
                             vm[vm.getCompleteCb]();
                         }
                     }
                 }
                 if (vm[vm.getBeforeCb]) {
                     vm[vm.getBeforeCb]();
                 }
+                vm.fetch(cb);
+            },
+            fetch: function(cb) {
+                let vm = this;
                 vm.lastGetParams = vm.getParams();
                 vm.reqGet(vm.url, vm.lastGetParams, cb);
             },
-            asDateInputField: function(dateISOString) {
-                const dateValue = moment(dateISOString);
-                return dateValue.isValid() ? dateValue.format("YYYY-MM-DD") : null;
-            },
-            asDateISOString: function(dateInputField) {
-                const dateValue = moment(dateInputField, "YYYY-MM-DD");
-                return dateValue.isValid() ? dateValue.toISOString() : null;
-            }
-        },
-        computed: {
-            _start_at: {
-                get: function() {
-                    return this.asDateInputField(this.params.start_at);
-                },
-                set: function(newVal) {
-                    if (newVal) {
-                        // The setter might be call with `newVal === null`
-                        // when the date is incorrect (ex: 09/31/2022).
-                        this.$set(this.params, 'start_at',
-                            this.asDateISOString(newVal));
-                        if (this.autoreload && this.outdated) this.get();
-                    }
-                }
-            },
-            _ends_at: {
-                get: function() {
-                    // form field input="date" will expect ends_at as a String
-                    // but will literally cut the hour part regardless of timezone.
-                    // We don't want an empty list as a result.
-                    // If we use moment `endOfDay` we get 23:59:59 so we
-                    // add a full day instead. It seemed clever to run the following
-                    // code but that prevented entering the year part in the input
-                    // field (as oppossed to use the widget).
-                    //
-                    // const dateValue = moment(this.params.ends_at).add(1,'days');
-                    // return dateValue.isValid() ? dateValue.format("YYYY-MM-DD") : null;
-                    return this.asDateInputField(this.params.ends_at);
-                },
-                set: function(newVal) {
-                    if (newVal) {
-                        // The setter might be call with `newVal === null`
-                        // when the date is incorrect (ex: 09/31/2022).
-                        this.$set(this.params, 'ends_at',
-                            this.asDateISOString(newVal));
-                        if (this.autoreload && this.outdated) this.get();
-                    }
+            reload: function() {
+                let vm = this;
+                for (let idx = 0; idx < vm.preReload.length; ++idx) {
+                    vm[vm.preReload[idx]]();
                 }
+                vm.get();
             },
-            outdated: function() {
-                var vm = this;
-                const params = vm.getParams();
-                for (var key in vm.lastGetParams) {
-                    if (vm.lastGetParams.hasOwnProperty(key)) {
-                        if (vm.lastGetParams[key] !== params[key]) {
-                            return true;
-                        }
-                    }
-                }
-                for (var key in params) {
-                    if (params.hasOwnProperty(key)) {
-                        if (params[key] !== vm.lastGetParams[key]) {
-                            return true;
-                        }
-                    }
-                }
-                return false;
-            }
-        }
+        },
     };
 
 
-    var TypeAhead = Vue.extend({
+    var typeAheadMixin = {
         mixins: [
             httpRequestMixin
         ],
         data: function data() {
             return {
                 url: null,
                 items: [],
@@ -1238,22 +1268,21 @@
                 var vm = this;
                 if (vm.current !== -1) {
                     vm.onHit(vm.items[vm.current]);
                 }
             },
 
             onHit: function onHit() {
-                Vue.util.warn('You need to implement the `onHit` method', this);
+                console.warn('You need to implement the `onHit` method', this);
             },
 
             reset: function() {
                 var vm = this;
-                vm.items = [];
+                vm.clear();
                 vm.query = '';
-                vm.loading = false;
             },
 
             setActive: function(index) {
                 var vm = this;
                 vm.current = index;
             },
 
@@ -1309,19 +1338,22 @@
                 return !this.query;
             },
             isDirty: function isDirty() {
                 return !!this.query;
             }
         },
         mounted: function() {
-            // do nothing.
+            if (this.$el.dataset && this.$el.dataset.url) {
+                this.url = this.$el.dataset.url;
+            }
         }
-    });
+    };
 
     // attach properties to the exports object to define
     // the exported module properties.
-    exports.messagesMixin = messagesMixin;
     exports.httpRequestMixin = httpRequestMixin;
-    exports.itemMixin = itemMixin;
     exports.itemListMixin = itemListMixin;
-    exports.TypeAhead = TypeAhead;
+    exports.itemMixin = itemMixin;
+    exports.messagesMixin = messagesMixin;
+    exports.paramsMixin = paramsMixin;
+    exports.typeAheadMixin = typeAheadMixin;
 }));
```

### Comparing `djaodjin-signup-0.7.7/signup/static/js/djaodjin-resources.js` & `djaodjin-signup-0.8.0/signup/static/js/djaodjin-resources.js`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.7.7/signup/static/js/djaodjin-signup-angular.js` & `djaodjin-signup-0.8.0/signup/static/js/djaodjin-signup-angular.js`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.7.7/signup/static/js/djaodjin-signup-vue.js` & `djaodjin-signup-0.8.0/signup/static/js/djaodjin-signup-vue.js`

 * *Files 21% similar despite different names*

#### js-beautify {}

```diff
@@ -28,21 +28,21 @@
         failCb: function(res) {
             var vm = this;
             if (res.status === 403) {
                 // incorrect password
                 vm.passwordIncorrect = true;
             } else {
                 vm.modalHide();
-                showErrorMessages(res);
+                vm.showErrorMessages(res);
             }
         },
     },
     computed: {
         dialog: function() { // XXX depends on jQuery / bootstrap.js
-            var dialog = $(this.modalSelector);
+            var dialog = $(this.$el).find(this.modalSelector);
             if (dialog && jQuery().modal) {
                 return dialog;
             }
         },
     },
 }
 
@@ -64,17 +64,14 @@
     },
     methods: {
         createContact: function() {
             var vm = this;
             vm.reqPost(vm.url, this.contact,
                 function(resp) {
                     window.location = vm.redirectUrl(resp.slug);
-                },
-                function(resp) {
-                    showErrorMessages(resp);
                 });
         },
         redirectUrl: function(contact) {
             var vm = this;
             return vm.redirect_url + contact + '/';
         }
     },
@@ -107,16 +104,14 @@
                 account: vm.itemSelected.slug
             }
             vm.reqPost(vm.url, {
                 text: vm.activityText,
                 account: vm.itemSelected.slug
             }, function(resp) {
                 vm.get();
-            }, function(resp) {
-                showErrorMessages(resp);
             });
         },
         getCandidates: function(query, done) {
             var vm = this;
             vm.searching = true;
             vm.reqGet(vm.typeaheadUrl, {
                     q: query
@@ -135,67 +130,38 @@
 
 Vue.component('user-update', {
     mixins: [httpRequestMixin],
     data: function() {
         return {
             url: this.$urls.user.api_profile,
             picture_url: this.$urls.user.api_user_picture,
+            verify_url: this.$urls.user.api_recover,
             redirect_url: this.$urls.profile_redirect,
             api_activate_url: this.$urls.user.api_activate,
-            api_generate_keys_url: this.$urls.user.api_generate_keys,
             formFields: {},
             userModalOpen: false,
-            apiModalOpen: false,
-            apiKey: "Generating ...",
             picture: null,
-            password: '',
+            codeSent: false
         };
     },
     methods: {
         activate: function() {
             var vm = this;
             vm.reqPost(vm.api_activate_url,
                 function(resp) {
                     if (resp.detail) {
-                        showMessages([resp.detail], "info");
-                    }
-                },
-                function(resp) {
-                    showErrorMessages(resp);
-                });
-        },
-        resetKey: function() {
-            this.apiModalOpen = true;
-        },
-        generateKey: function() {
-            var vm = this;
-            vm.reqPost(vm.api_generate_keys_url, {
-                    password: vm.password
-                },
-                function(resp) {
-                    vm.apiKey = resp.secret;
-                },
-                function(resp) {
-                    if (resp.responseJSON && resp.responseJSON.length > 0) {
-                        // this most likely tells that the password
-                        // is incorrect
-                        vm.apiKey = resp.responseJSON[0];
-                        return;
+                        vm.showMessages([resp.detail], "info");
                     }
-                    showErrorMessages(resp);
                 });
         },
         deleteProfile: function() {
             var vm = this;
             vm.reqDelete(vm.url,
                 function() {
                     window.location = vm.redirect_url;
-                },
-                function(resp) {
-                    showErrorMessages(resp);
                 });
         },
         get: function() {
             var vm = this;
             vm.reqGet(vm.url,
                 function(resp) {
                     vm.formFields = resp;
@@ -215,15 +181,15 @@
                 }
             }
             vm.reqPatch(vm.url, data,
                 function(resp) {
                     // XXX should really be success but then it needs to be changed
                     // in Django views as well.
                     if (resp.detail) {
-                        showMessages([resp.detail], "info");
+                        vm.showMessages([resp.detail], "info");
                     }
                 });
             if (vm.imageSelected) {
                 vm.uploadProfilePicture();
             }
         },
         uploadProfilePicture: function() {
@@ -233,15 +199,15 @@
                 var form = new FormData();
                 form.append('file', blob, vm.picture.getChosenFile().name);
                 vm.reqPostBlob(vm.picture_url, form,
                     function(resp) {
                         vm.formFields.picture = resp.location;
                         vm.picture.remove();
                         vm.$forceUpdate();
-                        showMessages(["Profile was updated."], "success");
+                        vm.showMessages(["Profile was updated."], "success");
                     });
             }, 'image/jpeg');
         },
         validateForm: function() { // XXX depends on jQuery
             var vm = this;
             var isEmpty = true;
             var fields = $(vm.$el).find('[name]').not(
@@ -256,14 +222,64 @@
                     // We have at least one piece of information
                     // about the plan already available.
                     isEmpty = false;
                 }
             }
             return !isEmpty;
         },
+        verifyEmail: function() {
+            var vm = this;
+            vm.reqPost(vm.verify_url, {
+                    email: vm.$refs.email.value
+                },
+                function(resp) {
+                    vm.modalHide();
+                    if (resp.detail) {
+                        vm.showMessages([resp.detail], "success");
+                    }
+                },
+                function(resp) {
+                    vm.codeSent = true;
+                    if (resp.detail) {
+                        vm.showMessages([resp.detail], "success");
+                    }
+                });
+        },
+        verifyPhone: function() {
+            var vm = this;
+            vm.reqPost(vm.verify_url, {
+                    email: vm.$refs.phone.value
+                },
+                function(resp) {
+                    vm.codeSent = true;
+                    if (resp.detail) {
+                        vm.showMessages([resp.detail], "success");
+                    }
+                },
+                function(resp) {
+                    vm.codeSent = true;
+                    if (resp.detail) {
+                        vm.showMessages([resp.detail], "success");
+                    }
+                });
+        },
+        submitCode: function() {
+            // submit the one-time code that was e-mailed
+            // or sent by text message.
+            var vm = this;
+            vm.reqPost(vm.verify_url, {
+                    code: vm.$refs.code.value
+                },
+                function(resp) {
+                    vm.modalHide();
+                    if (resp.detail) {
+                        vm.showMessages([resp.detail], "success");
+                    }
+                });
+        }
     },
     computed: {
         imageSelected: function() {
             return this.picture && this.picture.hasImage();
         }
     },
     mounted: function() {
@@ -281,45 +297,127 @@
     mixins: [
         httpRequestMixin,
         userPasswordModalMixin
     ],
     data: function() {
         return {
             url: this.$urls.user.api_password_change,
+            otp_url: this.$urls.user.api_otp_change,
             modalSelector: '.user-password-modal',
             newPassword: '',
             newPassword2: '',
+            otpEnabled: true,
+            otpPrivKey: '',
+            nextCb: null
         };
     },
     methods: {
-        modalShowAndValidate: function() {
+        modalShowAndValidate: function(nextCb) {
             var vm = this;
+            vm.nextCb = nextCb ? nextCb : null;
             vm.modalShow();
         },
         updatePassword: function() {
             var vm = this;
             // We are using the view (and not the API) so that the redirect
             // to the profile page is done correctly and a success message
             // shows up.
             vm.reqPut(vm.url, {
                 password: vm.password,
                 new_password: vm.newPassword,
                 new_password2: vm.newPassword2
             }, function(resp) {
-                vm.modalHide();
                 vm.newPassword = '';
                 vm.newPassword2 = '';
                 if (resp.detail) {
-                    showMessages([resp.detail], "success");
+                    vm.showMessages([resp.detail], "success");
                 }
             }, vm.failCb);
         },
         submitPassword: function() {
             var vm = this;
-            vm.updatePassword();
+            vm.modalHide();
+            if (vm.nextCb) {
+                vm[vm.nextCb]();
+            } else {
+                vm.updatePassword();
+            }
+        },
+        enableOTP: function() {
+            var vm = this;
+            vm.reqPut(vm.otp_url, {
+                password: vm.password,
+                enable: true
+            }, function(resp) {
+                vm.otpEnabled = true;
+                vm.otpPrivKey = resp.priv_key
+                QRCode.toCanvas(
+                    document.getElementById('otp-qr-canvas'),
+                    resp.provisioning_uri,
+                    function(error) {
+                        if (error) vm.showErrorMessages(error);
+                    })
+            })
+        },
+        disableOTP: function() {
+            var vm = this;
+            vm.reqPut(vm.otp_url, {
+                password: vm.password,
+                enable: false
+            }, function(resp) {
+                vm.otpEnabled = false;
+            })
+        },
+    },
+    mounted: function() {
+        if (this.$el.dataset) {
+            this.otpEnabled = !!this.$el.dataset.otpEnabled;
+        }
+    }
+});
+
+
+Vue.component('user-rotate-api-keys', {
+    mixins: [
+        httpRequestMixin,
+        userPasswordModalMixin
+    ],
+    data: function() {
+        return {
+            url: this.$urls.user.api_generate_keys,
+            modalSelector: '.user-password-modal',
+            apiKey: '',
+        };
+    },
+    methods: {
+        generateKey: function() {
+            var vm = this;
+            vm.reqPost(vm.url, {
+                    password: vm.password
+                },
+                function(resp) {
+                    vm.apiKey = resp.secret;
+                    vm.modalHide();
+                    if (resp.detail) {
+                        vm.showMessages([resp.detail], "success");
+                    }
+                },
+                function(resp) {
+                    if (resp.responseJSON && resp.responseJSON.length > 0) {
+                        // this most likely tells that the password
+                        // is incorrect
+                        vm.apiKey = resp.responseJSON[0];
+                        return;
+                    }
+                    vm.showErrorMessages(resp);
+                });
+        },
+        submitPassword: function() {
+            var vm = this;
+            vm.generateKey();
         },
     },
 });
 
 
 Vue.component('user-update-pubkey', {
     mixins: [
@@ -338,15 +436,15 @@
             var vm = this;
             vm.reqPut(vm.url, {
                 pubkey: vm.pubkey,
                 password: vm.password,
             }, function(resp) {
                 vm.modalHide();
                 if (resp.detail) {
-                    showMessages([resp.detail], "success");
+                    vm.showMessages([resp.detail], "success");
                 }
             }, vm.failCb);
         },
         submitPassword: function() {
             var vm = this;
             vm.updatePubkey();
         },
```

### Comparing `djaodjin-signup-0.7.7/signup/templates/accounts/login.html` & `djaodjin-signup-0.8.0/signup/templates/accounts/recover.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 {% extends "base.html" %}
 
-{% block localheader_title %}Sign In{% endblock %}
+{% block localheader_title %}Recover Password{% endblock %}
 
 {% block content %}
 <div>
-  {% if sso_required %}
-  <p>
-You are required to login through the following Single Sign On (SSO) provider:
-  </p>
-  <a href="{{sso_required.url}}">{{sso_required.printable_name}}</a>
-  {% else %}
-  <form method="post" action=".{% if next %}/?next={{next}}{% endif %}">
+  <h1>Recover Password</h1>
+  <div>
+    {% if sso_required %}
+    <p>
+        You are required to login through the following Single Sign On (SSO) provider:
+    </p>
+    <a href="{{sso_required.url}}">{{sso_required.printable_name}}</a>
+    {% else %}
+    <p>
+Please enter your e-mail or phone.
+Your password will be reset and you will get a chance to choose a new password.
+    </p>
+    <form method="post" action=".">
       {% csrf_token %}
-      {{form}}
+      {{ form }}
       <button type="submit" name="submit">Submit</button>
-  </form>
-  <p>
-      <a href="{% url 'password_reset' %}">Forgot password?</a>
-  </p>
-  <p>
+    </form>
+    <p>
       Don't have an account? -- <a href="{% url 'registration_register' %}">Sign up</a>
-  </p>
-  {% endif %}
+    </p>
+    {% endif %}
+  </div>
 </div>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,10 +1,12 @@
-{% extends "base.html" %} {% block localheader_title %}Sign In{% endblock %} {%
-block content %}
+{% extends "base.html" %} {% block localheader_title %}Recover Password{%
+endblock %} {% block content %}
+****** Recover Password ******
 {% if sso_required %}
 You are required to login through the following Single Sign On (SSO) provider:
 {{sso_required.printable_name}} {% else %}
-{% csrf_token %} {{form}} Submit
-Forgot_password?
+Please enter your e-mail or phone. Your password will be reset and you will get
+a chance to choose a new password.
+{% csrf_token %} {{ form }} Submit
 Don't have an account? -- Sign_up
 {% endif %}
 {% endblock %}
```

### Comparing `djaodjin-signup-0.7.7/signup/templates/accounts/register.html` & `djaodjin-signup-0.8.0/signup/templates/accounts/register.html`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.7.7/signup/templates/users/index.html` & `djaodjin-signup-0.8.0/signup/templates/users/index.html`

 * *Files 22% similar despite different names*

```diff
@@ -16,40 +16,27 @@
       {{form.as_p}}
       <button type="submit">Update</button>
     </form>
     <div>
       <a id="change-password" href="{% url 'password_change' user %}">Change Password</a>
     </div>
     <div>
+      <a id="keys-update" href="{% url 'pubkey_update' user %}">Programmatic Keys</a>
+    </div>
+    <div>
       <a href="{% url 'users_notifications' user %}">Notifications</a>
     </div>
     {% if urls.user.api_activate %}
     <div>
       <button id="activate-user" @click="activate">Activate</button>
       <span>
         Send an activation e-mail to the user.
       </span>
     </div>
     {% endif %}
-    {% if urls.user.api_generate_keys %}
-    <div id="generate-key">
-      <h5 id="generate-key-open">Reset API Key</h5>
-      <form method="POST" ng-submit="generateKey($event)"
-            @submit.prevent="generateKey">
-        <input name="key" maxlength="128" type="text" disabled
-               ng-model="api_key"
-               v-model="apiKey" />
-        <input name="password" maxlength="128" type="text"
-               placeholder="Password"
-               ng-model="password"
-               v-model="password" />
-        <button id="regenerate-key" type="submit">Generate</button>
-      </form>
-    </div>
-    {% endif %}
     <hr />
     <button id="delete-profile-btn"
             type="button"
             @click="deleteProfile">Delete</button>
   </div><!-- userProfileCtrl -->
 </user-update><!-- signupApp -->
 {% endblock %}
```

#### html2text {}

```diff
@@ -3,18 +3,15 @@
 submit.prevent="updateProfile">
 
 src="formFields.picture" width="100" height="100">
 width="100" :height="100">
 click.prevent="uploadProfilePicture">Save picture
 {{form.as_p}} Update
 Change_Password
+Programmatic_Keys
 Notifications
 {% if urls.user.api_activate %}
 click="activate">Activate  Send an activation e-mail to the user.
-{% endif %} {% if urls.user.api_generate_keys %}
-** Reset API Key **
-submit.prevent="generateKey"> [key                 ] [password            ]
-Generate
 {% endif %}
 ===============================================================================
 click="deleteProfile">Delete
  {% endblock %}
```

### Comparing `djaodjin-signup-0.7.7/signup/tests.py` & `djaodjin-signup-0.8.0/signup/tests.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.7.7/signup/urls/__init__.py` & `djaodjin-signup-0.8.0/signup/urls/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022, Djaodjin Inc.
+# Copyright (c) 2023, Djaodjin Inc.
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice,
 #    this list of conditions and the following disclaimer.
@@ -22,13 +22,13 @@
 # OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 # ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 """
 URLconf for frictionless signup (API and HTML pages).
 """
 
-from ..compat import include, re_path
+from ..compat import include, path
 
 urlpatterns = [
-    re_path(r'^api/', include('signup.urls.api')),
-    re_path(r'^', include('signup.urls.views')),
+    path('api/', include('signup.urls.api')),
+    path('', include('signup.urls.views')),
 ]
```

### Comparing `djaodjin-signup-0.7.7/signup/urls/api/__init__.py` & `djaodjin-signup-0.8.0/signup/urls/api/__init__.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.7.7/signup/urls/api/activate.py` & `djaodjin-signup-0.8.0/signup/urls/api/activate.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.7.7/signup/urls/api/auth.py` & `djaodjin-signup-0.8.0/signup/urls/api/auth.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022, Djaodjin Inc.
+# Copyright (c) 2023, Djaodjin Inc.
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice,
 #    this list of conditions and the following disclaimer.
@@ -20,21 +20,19 @@
 # OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
 # OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 # ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from ... import settings
 from ...compat import path, re_path
-from ...api.auth import (JWTActivate, JWTLogin, JWTPasswordResetConfirm,
-    JWTRegister, PasswordResetAPIView)
+from ...api.auth import (JWTActivate, JWTLogin, JWTRegister,
+    RecoverAPIView)
 
 
 urlpatterns = [
     re_path(r'^auth/activate/(?P<verification_key>%s)$'
         % settings.EMAIL_VERIFICATION_PAT,
         JWTActivate.as_view(), name='api_activate'),
     path('auth/register', JWTRegister.as_view(), name='api_register'),
-    path('auth/recover', PasswordResetAPIView.as_view(), name='api_recover'),
-    re_path(r'^auth/reset/(?P<uidb64>[0-9A-Za-z_\-]+)/(?P<token>[0-9A-Za-z]{1,13}-[0-9A-Za-z]{1,20})$', #pylint: disable=line-too-long
-        JWTPasswordResetConfirm.as_view(), name='api_password_reset_confirm'),
+    path('auth/recover', RecoverAPIView.as_view(), name='api_recover'),
     path('auth', JWTLogin.as_view(), name='api_login'),
 ]
```

### Comparing `djaodjin-signup-0.7.7/signup/urls/api/contacts.py` & `djaodjin-signup-0.8.0/signup/urls/api/contacts.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.7.7/signup/urls/api/keys.py` & `djaodjin-signup-0.8.0/signup/urls/api/keys.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.7.7/signup/urls/api/tokens.py` & `djaodjin-signup-0.8.0/signup/urls/api/tokens.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.7.7/signup/urls/api/users.py` & `djaodjin-signup-0.8.0/signup/urls/api/users.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022, Djaodjin Inc.
+# Copyright (c) 2023, Djaodjin Inc.
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice,
 #    this list of conditions and the following disclaimer.
@@ -19,22 +19,25 @@
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
 # OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
 # OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 # ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from ...compat import path
-from ...api.users import (PasswordChangeAPIView, UserDetailAPIView,
-    UserListCreateAPIView, UserNotificationsAPIView, UserPictureAPIView)
+from ...api.users import (OTPChangeAPIView, PasswordChangeAPIView,
+    UserDetailAPIView, UserListCreateAPIView, UserNotificationsAPIView,
+    UserPictureAPIView)
 
 urlpatterns = [
     path('users/<slug:user>/notifications',
         UserNotificationsAPIView.as_view(), name='api_user_notifications'),
     path('users/<slug:user>/picture',
         UserPictureAPIView.as_view(), name='api_user_picture'),
+    path('users/<slug:user>/otp',
+        OTPChangeAPIView.as_view(), name='api_user_otp_change'),
     path('users/<slug:user>/password',
         PasswordChangeAPIView.as_view(), name='api_user_password_change'),
     path('users/<slug:user>',
         UserDetailAPIView.as_view(), name='api_user_profile'),
     path(r'users',
         UserListCreateAPIView.as_view(), name='saas_api_users'),
 ]
```

### Comparing `djaodjin-signup-0.7.7/signup/urls/views/__init__.py` & `djaodjin-signup-0.8.0/signup/urls/views/__init__.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.7.7/signup/urls/views/accounts.py` & `djaodjin-signup-0.8.0/signup/urls/views/users.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022, Djaodjin Inc.
+# Copyright (c) 2023, Djaodjin Inc.
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice,
 #    this list of conditions and the following disclaimer.
@@ -18,39 +18,24 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
 # OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
 # OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 # ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-from ... import settings
-from ...compat import include, re_path
-from ...forms import StartAuthenticationForm
-from ...views.auth import (ActivationView, PasswordResetView,
-    PasswordResetConfirmView, SigninView, SignoutView, SignupView)
-from ...views.saml import saml_metadata_view
+from ...compat import path
+from ...views.users import (PasswordChangeView,
+    UserPublicKeyUpdateView, UserProfileView, UserNotificationsView,
+    redirect_to_user_profile)
 
 urlpatterns = [
-    # When the key and/or token are wrong we don't want to give any clue
-    # as to why that is so. Less information communicated to an attacker,
-    # the better.
-    re_path(r'^activate/(?P<verification_key>%s)/'
-        % settings.EMAIL_VERIFICATION_PAT,
-        ActivationView.as_view(), name='registration_activate'),
-    re_path(r'^activate/',
-        SigninView.as_view(
-            form_class=StartAuthenticationForm,
-            template_name='accounts/activate/index.html'),
-        name='registration_activate_start'),
-    re_path('', include('social_django.urls', namespace='social')),
-    re_path(r'^login/',
-        SigninView.as_view(), name='login'),
-    re_path(r'^logout/',
-        SignoutView.as_view(), name='logout'),
-    re_path(r'^recover/',
-        PasswordResetView.as_view(), name='password_reset'),
-    re_path(r'^register/',
-        SignupView.as_view(), name='registration_register'),
-    re_path(r'^reset/(?P<uidb64>[0-9A-Za-z_\-]+)/(?P<token>[0-9A-Za-z\-]+)/$',
-        PasswordResetConfirmView.as_view(), name='password_reset_confirm'),
-    re_path('^saml/', saml_metadata_view),
+    # These three URLs must be protected.
+    path('<slug:user>/password/',
+        PasswordChangeView.as_view(), name='password_change'),
+    path('<slug:user>/pubkey/',
+        UserPublicKeyUpdateView.as_view(), name='pubkey_update'),
+    path('<slug:user>/notifications/',
+        UserNotificationsView.as_view(), name='users_notifications'),
+    path('<slug:user>/',
+        UserProfileView.as_view(), name='users_profile'),
+    path('', redirect_to_user_profile, name='accounts_profile'),
 ]
```

### Comparing `djaodjin-signup-0.7.7/signup/urls/views/contacts.py` & `djaodjin-signup-0.8.0/signup/urls/views/contacts.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022, Djaodjin Inc.
+# Copyright (c) 2023, Djaodjin Inc.
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice,
 #    this list of conditions and the following disclaimer.
@@ -18,17 +18,16 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
 # OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
 # OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 # ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-from ... import settings
-from ...compat import re_path
+from ...compat import path
 from ...views.contacts import ContactListView, ContactDetailView
 
 urlpatterns = [
     # These three URLs must be protected.
-    re_path(r'^(?P<user>%s)/' % settings.USERNAME_PAT,
-        ContactDetailView.as_view(), name='contact'),
-    re_path(r'^', ContactListView.as_view(), name='contacts'),
+    path('<slug:user>/',
+        ContactDetailView.as_view(), name='signup_contact'),
+    path(r'', ContactListView.as_view(), name='signup_contacts'),
 ]
```

### Comparing `djaodjin-signup-0.7.7/signup/urls/views/saml.py` & `djaodjin-signup-0.8.0/signup/views/saml.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022, Djaodjin Inc.
+# Copyright (c) 2023, Djaodjin Inc.
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice,
 #    this list of conditions and the following disclaimer.
@@ -18,14 +18,24 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
 # OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
 # OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 # ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-from ...compat import path
-from ...views.saml import saml_metadata_view
+from django.http import HttpResponse, HttpResponseBadRequest
+from social_django.utils import load_strategy, load_backend
 
+from ..compat import reverse
 
-urlpatterns = [
-    path('', saml_metadata_view)
-]
+
+def saml_metadata_view(request):
+    complete_url = reverse('social:complete', args=("saml", ))
+    saml_backend = load_backend(
+        load_strategy(request),
+        "saml",
+        redirect_uri=complete_url,
+    )
+    metadata, errors = saml_backend.generate_metadata_xml()
+    if errors:
+        return HttpResponseBadRequest(errors)
+    return HttpResponse(content=metadata, content_type='text/xml')
```

### Comparing `djaodjin-signup-0.7.7/signup/urls/views/users.py` & `djaodjin-signup-0.8.0/signup/urls/api/activities.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022, Djaodjin Inc.
+# Copyright (c) 2023, Djaodjin Inc.
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice,
 #    this list of conditions and the following disclaimer.
@@ -18,24 +18,23 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
 # OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
 # OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 # ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-from ...settings import USERNAME_PAT
-from ...compat import re_path
-from ...views.users import (PasswordChangeView, UserPublicKeyUpdateView,
-    UserProfileView, UserNotificationsView, redirect_to_user_profile)
+from ...compat import path
+from ...api.activities import (ActivityByAccountAPIView,
+    ActivityByAccountIndexAPIView)
+from ...api.users import ActivityByAccountContactAPIView
 
 urlpatterns = [
-    # These three URLs must be protected.
-    re_path(r'^(?P<user>%s)/password/' % USERNAME_PAT,
-        PasswordChangeView.as_view(), name='password_change'),
-    re_path(r'^(?P<user>%s)/pubkey/' % USERNAME_PAT,
-        UserPublicKeyUpdateView.as_view(), name='pubkey_update'),
-    re_path(r'^(?P<user>%s)/notifications/' % USERNAME_PAT,
-        UserNotificationsView.as_view(), name='users_notifications'),
-    re_path(r'^(?P<user>%s)/' % USERNAME_PAT,
-        UserProfileView.as_view(), name='users_profile'),
-    re_path(r'^', redirect_to_user_profile, name='accounts_profile'),
+    path('activities/<slug:profile>/contacts',
+        ActivityByAccountContactAPIView.as_view(),
+        name='api_profile_activities_contacts'),
+    path('activities/<slug:profile>',
+        ActivityByAccountAPIView.as_view(),
+        name='api_profile_activities'),
+    path('activities',
+        ActivityByAccountIndexAPIView.as_view(),
+        name='api_profile_activities_index'),
 ]
```

### Comparing `djaodjin-signup-0.7.7/signup/utils.py` & `djaodjin-signup-0.8.0/signup/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -219,17 +219,17 @@
     try:
         user = user_model.objects.get(username=username)
     except user_model.DoesNotExist:
         raise serializers.ValidationError(_("User does not exist."))
     return user
 
 
-def get_disabled_authentication(request):
+def get_disabled_authentication(request, user):
     if isinstance(settings.DISABLED_AUTHENTICATION, six.string_types):
-        return import_string(settings.DISABLED_AUTHENTICATION)(request)
+        return import_string(settings.DISABLED_AUTHENTICATION)(request, user)
     return bool(settings.DISABLED_AUTHENTICATION)
 
 
 def get_disabled_registration(request):
     if isinstance(settings.DISABLED_REGISTRATION, six.string_types):
         return import_string(settings.DISABLED_REGISTRATION)(request)
     return bool(settings.DISABLED_REGISTRATION)
@@ -243,20 +243,14 @@
 
 def get_login_throttle():
     if isinstance(settings.LOGIN_THROTTLE, six.string_types):
         return import_string(settings.LOGIN_THROTTLE)
     return None
 
 
-def get_password_reset_throttle():
-    if isinstance(settings.PASSWORD_RESET_THROTTLE, six.string_types):
-        return import_string(settings.PASSWORD_RESET_THROTTLE)
-    return None
-
-
 def get_picture_storage(request, account=None, **kwargs):
     if settings.PICTURE_STORAGE_CALLABLE:
         try:
             return import_string(settings.PICTURE_STORAGE_CALLABLE)(
                 request, account=account, **kwargs)
         except ImportError:
             pass
```

### Comparing `djaodjin-signup-0.7.7/signup/validators.py` & `djaodjin-signup-0.8.0/signup/validators.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
 # OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 # ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from django.utils.deconstruct import deconstructible
 from django.core.exceptions import ValidationError
 from django.core.validators import (EmailValidator as EmailValidatorBase,
-    RegexValidator, validate_email as validate_email_base, validate_slug)
+    validate_email as validate_email_base, validate_slug)
 from django.utils.translation import gettext_lazy as _
 from phonenumber_field import phonenumber
 
 from .utils import get_email_dynamic_validator
 
 
 @deconstructible
```

### Comparing `djaodjin-signup-0.7.7/signup/views/contacts.py` & `djaodjin-signup-0.8.0/signup/views/contacts.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2019, Djaodjin Inc.
+# Copyright (c) 2023, Djaodjin Inc.
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice,
 #    this list of conditions and the following disclaimer.
@@ -22,42 +22,50 @@
 # OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 # ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 """Views about contact activities"""
 
 from django.views.generic import DetailView, TemplateView
 
+from .. import settings
 from ..compat import reverse
-from ..mixins import ContactMixin, UrlsMixin
+from ..helpers import update_context_urls
+from ..mixins import ContactMixin
 from ..models import Contact
 
 
 class ContactDetailView(ContactMixin, DetailView):
 
     template_name = 'contacts/contact.html'
     model = Contact
 
     def get_object(self):
         return self.contact
 
     def get_context_data(self, **kwargs):
         context = super(ContactDetailView, self).get_context_data(**kwargs)
         context.update({'contact': self.contact})
-        self.update_context_urls(context, {
+        update_context_urls(context, {
             'api_activities': reverse('api_activities', args=(self.contact,)),
             'api_contact': reverse('api_contact', args=(self.contact,)),
             'api_contacts': reverse('api_contacts')
         })
         return context
 
 
-class ContactListView(UrlsMixin, TemplateView):
+class ContactListMixin(settings.EXTRA_MIXIN):
+    """
+    Mixin such that EXTRA_MIXIN can defaults to `object`.
+    """
+
+
+class ContactListView(ContactListMixin, TemplateView):
 
     template_name = 'contacts/index.html'
 
     def get_context_data(self, **kwargs):
         context = super(ContactListView, self).get_context_data(**kwargs)
         self.update_context_urls(context, {
             'api_contacts': reverse('api_contacts'),
-            'contacts': reverse('contacts')
+            'contacts': reverse('signup_contacts')
         })
         return context
```

### Comparing `djaodjin-signup-0.7.7/signup/views/saml.py` & `djaodjin-signup-0.8.0/signup/backends/mfa.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022, Djaodjin Inc.
+# Copyright (c) 2023, Djaodjin Inc.
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice,
 #    this list of conditions and the following disclaimer.
@@ -18,23 +18,42 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
 # OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
 # OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 # ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-from django.http import HttpResponse
-from social_django.utils import load_strategy, load_backend
+"""
+Backends to send one-time authentication codes
+"""
+from __future__ import unicode_literals
 
-from ..compat import reverse
+from .. import signals
+from ..utils import generate_random_code
 
 
-def saml_metadata_view(request):
-    complete_url = reverse('social:complete', args=("saml", ))
-    saml_backend = load_backend(
-        load_strategy(request),
-        "saml",
-        redirect_uri=complete_url,
-    )
-    metadata, errors = saml_backend.generate_metadata_xml()
-    if not errors:
-        return HttpResponse(content=metadata, content_type='text/xml')
+class EmailOTCBackend(object):
+    """
+    Backend to authenticate a user through a code sent to an email address.
+    """
+
+    def create_token(self, user, request=None):
+        user.one_time_code = generate_random_code()
+        user.otc_backend = user.EMAIL_BACKEND
+        user.save()
+        signals.user_mfa_code.send(
+            sender=__name__, user=user, code=user.one_time_code,
+            request=request)
+
+
+class PhoneOTCBackend(object):
+    """
+    Backend to authenticate a user through a code sent to a phone number.
+    """
+
+    def create_token(self, user, request=None):
+        user.one_time_code = generate_random_code()
+        user.otc_backend = user.PHONE_BACKEND
+        user.save()
+        signals.user_mfa_code.send(
+            sender=__name__, user=user, code=user.one_time_code,
+            request=request)
```

### Comparing `djaodjin-signup-0.7.7/signup/views/users.py` & `djaodjin-signup-0.8.0/signup/views/users.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022, Djaodjin Inc.
+# Copyright (c) 2023, Djaodjin Inc.
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice,
 #    this list of conditions and the following disclaimer.
@@ -37,17 +37,17 @@
 from django.views.decorators.csrf import csrf_protect
 from django.views.generic.edit import UpdateView
 
 from .. import settings
 from ..compat import gettext_lazy as _, is_authenticated, reverse, six
 from ..forms import (PasswordChangeForm, PublicKeyForm, UserForm,
     UserNotificationsForm)
-from ..helpers import has_invalid_password
+from ..helpers import has_invalid_password, update_context_urls
 from ..mixins import UserMixin
-from ..models import Contact, Notification
+from ..models import Contact, Notification, OTPGenerator
 from ..utils import update_db_row
 
 
 LOGGER = logging.getLogger(__name__)
 
 
 class UserProfileView(UserMixin, UpdateView):
@@ -104,44 +104,60 @@
 
     def get_initial(self):
         initial = super(UserProfileView, self).get_initial()
         if self.object:
             initial.update({'full_name': self.object.get_full_name()})
         return initial
 
+
     def get_context_data(self, **kwargs):
         context = super(UserProfileView, self).get_context_data(**kwargs)
         setattr(context['user'], 'full_name', context['user'].get_full_name())
         contact = context['user'].contacts.filter(
             picture__isnull=False).order_by('created_at').first()
         if contact:
             setattr(context['user'], 'picture', contact.picture)
         # URLs for user
         if is_authenticated(self.request):
-            self.update_context_urls(context, {'user': {
+            update_context_urls(context, {'user': {
+                'api_recover': reverse('api_recover'),
                 'api_generate_keys': reverse(
                     'api_generate_keys', args=(self.object,)),
                 'api_profile': reverse(
                     'api_user_profile', args=(self.object,)),
                 'api_password_change': reverse(
                     'api_user_password_change', args=(self.object,)),
+                'api_otp_change': reverse(
+                    'api_user_otp_change', args=(self.object,)),
                 'api_user_picture': reverse(
                     'api_user_picture', args=(self.object,)),
                 'api_contact': reverse(
                     'api_contact', args=(self.object.username,)), #XXX
                 'api_pubkey': reverse(
                     'api_pubkey', args=(self.object,)),
                 'password_change': reverse(
                     'password_change', args=(self.object,)),
+                'keys_update': reverse(
+                    'pubkey_update', args=(self.object,)),
             }})
             if has_invalid_password(self.object):
-                self.update_context_urls(context, {'user': {
+                update_context_urls(context, {'user': {
                     'api_activate': reverse(
                         'api_user_activate', args=(self.object,)),
                 }})
+            contact = context['user'].contacts.filter(
+                email=self.object.email).order_by('created_at').first()
+            if contact:
+                context.update({
+                    'email_verified_at': contact.email_verified_at,
+                    'phone_verified_at': contact.phone_verified_at
+                })
+            context.update({
+                'otp_enabled': OTPGenerator.objects.filter(
+                    user=self.object).exists()})
         return context
 
     def get_success_url(self):
         messages.info(self.request, _("Profile updated."))
         return reverse('users_profile', args=(self.object,))
```

