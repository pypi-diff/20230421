# Comparing `tmp/moodle-dl-2.3.1.7.tar.gz` & `tmp/moodle-dl-2.3.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moodle-dl-2.3.1.7.tar", last modified: Wed Mar 29 16:46:16 2023, max compression
+gzip compressed data, was "moodle-dl-2.3.1.8.tar", last modified: Fri Apr 21 09:10:32 2023, max compression
```

## Comparing `moodle-dl-2.3.1.7.tar` & `moodle-dl-2.3.1.8.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 16:46:16.935193 moodle-dl-2.3.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9972 2023-03-29 16:46:16.935193 moodle-dl-2.3.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8861 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 16:46:16.931193 moodle-dl-2.3.1.7/moodle_dl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/moodle_dl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 16:46:16.931193 moodle-dl-2.3.1.7/moodle_dl/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/moodle_dl/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25830 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/moodle_dl/cli/config_wizard.py
--rw-r--r--   0 runner    (1001) docker     (123)     8153 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/moodle_dl/cli/database_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/moodle_dl/cli/moodle_wizard.py
--rw-r--r--   0 runner    (1001) docker     (123)     7747 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/moodle_dl/cli/notifications_wizard.py
--rw-r--r--   0 runner    (1001) docker     (123)    11176 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/moodle_dl/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    27295 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/moodle_dl/database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 16:46:16.931193 moodle-dl-2.3.1.7/moodle_dl/downloader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/moodle_dl/downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/moodle_dl/downloader/download_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 16:46:16.931193 moodle-dl-2.3.1.7/moodle_dl/downloader/extractors/
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/moodle_dl/downloader/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/moodle_dl/downloader/extractors/echo360.py
--rw-r--r--   0 runner    (1001) docker     (123)    12660 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/moodle_dl/downloader/extractors/googledrive.py
--rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/moodle_dl/downloader/extractors/helixmedia_lti.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/moodle_dl/downloader/extractors/kalvidres_lti.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/moodle_dl/downloader/extractors/opencast_lti.py
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/moodle_dl/downloader/extractors/owncloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/moodle_dl/downloader/extractors/sharepoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/moodle_dl/downloader/extractors/sharepointfiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/moodle_dl/downloader/fake_download_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    41144 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/moodle_dl/downloader/task.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17435 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/moodle_dl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 16:46:16.931193 moodle-dl-2.3.1.7/moodle_dl/moodle/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/moodle_dl/moodle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/moodle_dl/moodle/cookie_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/moodle_dl/moodle/core_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 16:46:16.935193 moodle-dl-2.3.1.7/moodle_dl/moodle/mods/
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/moodle_dl/moodle/mods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10225 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/moodle_dl/moodle/mods/assign.py
--rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/moodle_dl/moodle/mods/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/moodle_dl/moodle/mods/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/moodle_dl/moodle/mods/folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/moodle_dl/moodle/mods/forum.py
--rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/moodle_dl/moodle/mods/lesson.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/moodle_dl/moodle/mods/page.py
--rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/moodle_dl/moodle/mods/quiz.py
--rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/moodle_dl/moodle/mods/workshop.py
--rw-r--r--   0 runner    (1001) docker     (123)    29312 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/moodle_dl/moodle/moodle_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12184 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/moodle_dl/moodle/moodle_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    15710 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/moodle_dl/moodle/request_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    18485 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/moodle_dl/moodle/result_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 16:46:16.935193 moodle-dl-2.3.1.7/moodle_dl/notifications/
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/moodle_dl/notifications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 16:46:16.935193 moodle-dl-2.3.1.7/moodle_dl/notifications/console/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/moodle_dl/notifications/console/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/moodle_dl/notifications/console/console_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 16:46:16.935193 moodle-dl-2.3.1.7/moodle_dl/notifications/mail/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/moodle_dl/notifications/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36960 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/moodle_dl/notifications/mail/header.png
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/moodle_dl/notifications/mail/header_extender.png
--rw-r--r--   0 runner    (1001) docker     (123)    10237 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/moodle_dl/notifications/mail/mail_formater.py
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/moodle_dl/notifications/mail/mail_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/moodle_dl/notifications/mail/mail_shooter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/moodle_dl/notifications/notification_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 16:46:16.935193 moodle-dl-2.3.1.7/moodle_dl/notifications/telegram/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/moodle_dl/notifications/telegram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/moodle_dl/notifications/telegram/telegram_formater.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/moodle_dl/notifications/telegram/telegram_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/moodle_dl/notifications/telegram/telegram_shooter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 16:46:16.935193 moodle-dl-2.3.1.7/moodle_dl/notifications/xmpp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/moodle_dl/notifications/xmpp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/moodle_dl/notifications/xmpp/xmpp_formater.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/moodle_dl/notifications/xmpp/xmpp_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/moodle_dl/notifications/xmpp/xmpp_shooter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11626 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/moodle_dl/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    54167 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/moodle_dl/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/moodle_dl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 16:46:16.931193 moodle-dl-2.3.1.7/moodle_dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9972 2023-03-29 16:46:16.000000 moodle-dl-2.3.1.7/moodle_dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-03-29 16:46:16.000000 moodle-dl-2.3.1.7/moodle_dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 16:46:16.000000 moodle-dl-2.3.1.7/moodle_dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-29 16:46:16.000000 moodle-dl-2.3.1.7/moodle_dl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 16:46:16.000000 moodle-dl-2.3.1.7/moodle_dl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-03-29 16:46:16.000000 moodle-dl-2.3.1.7/moodle_dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-29 16:46:16.000000 moodle-dl-2.3.1.7/moodle_dl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 16:46:16.935193 moodle-dl-2.3.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-03-29 16:46:02.000000 moodle-dl-2.3.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:10:32.473604 moodle-dl-2.3.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10080 2023-04-21 09:10:32.473604 moodle-dl-2.3.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:10:32.465604 moodle-dl-2.3.1.8/moodle_dl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/moodle_dl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:10:32.469604 moodle-dl-2.3.1.8/moodle_dl/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/moodle_dl/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25830 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/moodle_dl/cli/config_wizard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8153 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/moodle_dl/cli/database_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/moodle_dl/cli/moodle_wizard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7747 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/moodle_dl/cli/notifications_wizard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11176 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/moodle_dl/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27295 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/moodle_dl/database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:10:32.469604 moodle-dl-2.3.1.8/moodle_dl/downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/moodle_dl/downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/moodle_dl/downloader/download_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:10:32.469604 moodle-dl-2.3.1.8/moodle_dl/downloader/extractors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/moodle_dl/downloader/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/moodle_dl/downloader/extractors/echo360.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12660 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/moodle_dl/downloader/extractors/googledrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/moodle_dl/downloader/extractors/helixmedia_lti.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/moodle_dl/downloader/extractors/kalvidres_lti.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/moodle_dl/downloader/extractors/opencast_lti.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/moodle_dl/downloader/extractors/owncloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/moodle_dl/downloader/extractors/sharepoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/moodle_dl/downloader/extractors/sharepointfiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/moodle_dl/downloader/fake_download_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41144 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/moodle_dl/downloader/task.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17435 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/moodle_dl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:10:32.469604 moodle-dl-2.3.1.8/moodle_dl/moodle/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/moodle_dl/moodle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/moodle_dl/moodle/cookie_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/moodle_dl/moodle/core_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:10:32.469604 moodle-dl-2.3.1.8/moodle_dl/moodle/mods/
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/moodle_dl/moodle/mods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10225 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/moodle_dl/moodle/mods/assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/moodle_dl/moodle/mods/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/moodle_dl/moodle/mods/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/moodle_dl/moodle/mods/folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/moodle_dl/moodle/mods/forum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/moodle_dl/moodle/mods/lesson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/moodle_dl/moodle/mods/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/moodle_dl/moodle/mods/quiz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/moodle_dl/moodle/mods/workshop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29312 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/moodle_dl/moodle/moodle_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12184 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/moodle_dl/moodle/moodle_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15717 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/moodle_dl/moodle/request_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18485 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/moodle_dl/moodle/result_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:10:32.469604 moodle-dl-2.3.1.8/moodle_dl/notifications/
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/moodle_dl/notifications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:10:32.469604 moodle-dl-2.3.1.8/moodle_dl/notifications/console/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/moodle_dl/notifications/console/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/moodle_dl/notifications/console/console_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:10:32.473604 moodle-dl-2.3.1.8/moodle_dl/notifications/mail/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/moodle_dl/notifications/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36960 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/moodle_dl/notifications/mail/header.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/moodle_dl/notifications/mail/header_extender.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10237 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/moodle_dl/notifications/mail/mail_formater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/moodle_dl/notifications/mail/mail_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/moodle_dl/notifications/mail/mail_shooter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/moodle_dl/notifications/notification_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:10:32.473604 moodle-dl-2.3.1.8/moodle_dl/notifications/telegram/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/moodle_dl/notifications/telegram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/moodle_dl/notifications/telegram/telegram_formater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/moodle_dl/notifications/telegram/telegram_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/moodle_dl/notifications/telegram/telegram_shooter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:10:32.473604 moodle-dl-2.3.1.8/moodle_dl/notifications/xmpp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/moodle_dl/notifications/xmpp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/moodle_dl/notifications/xmpp/xmpp_formater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/moodle_dl/notifications/xmpp/xmpp_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/moodle_dl/notifications/xmpp/xmpp_shooter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11626 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/moodle_dl/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54167 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/moodle_dl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/moodle_dl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:10:32.469604 moodle-dl-2.3.1.8/moodle_dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10080 2023-04-21 09:10:32.000000 moodle-dl-2.3.1.8/moodle_dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-04-21 09:10:32.000000 moodle-dl-2.3.1.8/moodle_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 09:10:32.000000 moodle-dl-2.3.1.8/moodle_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-21 09:10:32.000000 moodle-dl-2.3.1.8/moodle_dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 09:10:32.000000 moodle-dl-2.3.1.8/moodle_dl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-21 09:10:32.000000 moodle-dl-2.3.1.8/moodle_dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-21 09:10:32.000000 moodle-dl-2.3.1.8/moodle_dl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 09:10:32.473604 moodle-dl-2.3.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-21 09:10:17.000000 moodle-dl-2.3.1.8/setup.py
```

### Comparing `moodle-dl-2.3.1.7/LICENSE` & `moodle-dl-2.3.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.7/PKG-INFO` & `moodle-dl-2.3.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moodle-dl
-Version: 2.3.1.7
+Version: 2.3.1.8
 Summary: Moodle-DL downloads course content fast from Moodle (eg. lecture pdfs)
 Home-page: https://github.com/C0D3D3V/Moodle-DL
 Author: C0D3D3V
 Author-email: moodle-dl@ist-ein-knaller.de
 License: GPL-3.0
 Project-URL: Documentation, https://github.com/C0D3D3V/Moodle-DL#readme
 Project-URL: Wiki, https://github.com/C0D3D3V/Moodle-DL/wiki
@@ -137,14 +137,17 @@
 [moodle-buddy](https://github.com/marcelreppi/moodle-buddy)
 - Plugin for Firefox and Chrome
 - Mass file download and notification functionality for the Moodle
 
 [moodle-downloader](https://github.com/harsilspatel/moodle-downloader)
 - A chrome extension for batch downloading Moodle resources
 
+[Orga Bot](https://github.com/YoshiiPlayzz/orga_bot)
+- Utilizes moodle-dl to send moodle files via Discord
+
 [discord-moodle-bot](https://github.com/tjarbo/discord-moodle-bot)
 - Discord Notification Service for your moodle courses
 
 If someone wants to link another downloader here, which offers e.g. functions that moodle-dl does not offer, feel free to open an issue. 
 
 
 ---
```

### Comparing `moodle-dl-2.3.1.7/README.md` & `moodle-dl-2.3.1.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -110,14 +110,17 @@
 [moodle-buddy](https://github.com/marcelreppi/moodle-buddy)
 - Plugin for Firefox and Chrome
 - Mass file download and notification functionality for the Moodle
 
 [moodle-downloader](https://github.com/harsilspatel/moodle-downloader)
 - A chrome extension for batch downloading Moodle resources
 
+[Orga Bot](https://github.com/YoshiiPlayzz/orga_bot)
+- Utilizes moodle-dl to send moodle files via Discord
+
 [discord-moodle-bot](https://github.com/tjarbo/discord-moodle-bot)
 - Discord Notification Service for your moodle courses
 
 If someone wants to link another downloader here, which offers e.g. functions that moodle-dl does not offer, feel free to open an issue. 
 
 
 ---
```

### Comparing `moodle-dl-2.3.1.7/moodle_dl/cli/__init__.py` & `moodle-dl-2.3.1.8/moodle_dl/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.7/moodle_dl/cli/config_wizard.py` & `moodle-dl-2.3.1.8/moodle_dl/cli/config_wizard.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.7/moodle_dl/cli/database_manager.py` & `moodle-dl-2.3.1.8/moodle_dl/cli/database_manager.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.7/moodle_dl/cli/moodle_wizard.py` & `moodle-dl-2.3.1.8/moodle_dl/cli/moodle_wizard.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.7/moodle_dl/cli/notifications_wizard.py` & `moodle-dl-2.3.1.8/moodle_dl/cli/notifications_wizard.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.7/moodle_dl/config.py` & `moodle-dl-2.3.1.8/moodle_dl/config.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.7/moodle_dl/database.py` & `moodle-dl-2.3.1.8/moodle_dl/database.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.7/moodle_dl/downloader/download_service.py` & `moodle-dl-2.3.1.8/moodle_dl/downloader/download_service.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.7/moodle_dl/downloader/extractors/__init__.py` & `moodle-dl-2.3.1.8/moodle_dl/downloader/extractors/__init__.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.7/moodle_dl/downloader/extractors/echo360.py` & `moodle-dl-2.3.1.8/moodle_dl/downloader/extractors/echo360.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.7/moodle_dl/downloader/extractors/googledrive.py` & `moodle-dl-2.3.1.8/moodle_dl/downloader/extractors/googledrive.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.7/moodle_dl/downloader/extractors/helixmedia_lti.py` & `moodle-dl-2.3.1.8/moodle_dl/downloader/extractors/helixmedia_lti.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.7/moodle_dl/downloader/extractors/kalvidres_lti.py` & `moodle-dl-2.3.1.8/moodle_dl/downloader/extractors/kalvidres_lti.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.7/moodle_dl/downloader/extractors/opencast_lti.py` & `moodle-dl-2.3.1.8/moodle_dl/downloader/extractors/opencast_lti.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.7/moodle_dl/downloader/extractors/owncloud.py` & `moodle-dl-2.3.1.8/moodle_dl/downloader/extractors/owncloud.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.7/moodle_dl/downloader/extractors/sharepoint.py` & `moodle-dl-2.3.1.8/moodle_dl/downloader/extractors/sharepoint.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.7/moodle_dl/downloader/extractors/sharepointfiles.py` & `moodle-dl-2.3.1.8/moodle_dl/downloader/extractors/sharepointfiles.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.7/moodle_dl/downloader/fake_download_service.py` & `moodle-dl-2.3.1.8/moodle_dl/downloader/fake_download_service.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.7/moodle_dl/downloader/task.py` & `moodle-dl-2.3.1.8/moodle_dl/downloader/task.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.7/moodle_dl/main.py` & `moodle-dl-2.3.1.8/moodle_dl/main.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.7/moodle_dl/moodle/cookie_handler.py` & `moodle-dl-2.3.1.8/moodle_dl/moodle/cookie_handler.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.7/moodle_dl/moodle/core_handler.py` & `moodle-dl-2.3.1.8/moodle_dl/moodle/core_handler.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.7/moodle_dl/moodle/mods/__init__.py` & `moodle-dl-2.3.1.8/moodle_dl/moodle/mods/__init__.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.7/moodle_dl/moodle/mods/assign.py` & `moodle-dl-2.3.1.8/moodle_dl/moodle/mods/assign.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,22 +81,22 @@
             return
 
         if self.version < 2013051400:  # 2.5
             return
 
         # get submissions of all students for all assignments (only teachers can see that)
         indexed_assignment_ids = self.get_indexed_ids_of_mod_instances(assignments)
-        if len(indexed_assignment_ids) == 0:
+        if len(indexed_assignment_ids) <= 0:
             return
 
         assignments_with_all_submissions = (
             await self.client.async_post('mod_assign_get_submissions', {'assignmentids': indexed_assignment_ids})
         ).get('assignments', [])
 
-        if len(assignments_with_all_submissions) == 0:
+        if len(assignments_with_all_submissions) <= 0:
             return
 
         for course_id, modules in assignments.items():
             found_assignment_in_course = False
             for assignment in assignments_with_all_submissions:
                 for _module_id, module in modules.items():
                     if assignment['assignmentid'] == module['id']:
```

### Comparing `moodle-dl-2.3.1.7/moodle_dl/moodle/mods/common.py` & `moodle-dl-2.3.1.8/moodle_dl/moodle/mods/common.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.7/moodle_dl/moodle/mods/data.py` & `moodle-dl-2.3.1.8/moodle_dl/moodle/mods/data.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.7/moodle_dl/moodle/mods/folder.py` & `moodle-dl-2.3.1.8/moodle_dl/moodle/mods/folder.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.7/moodle_dl/moodle/mods/forum.py` & `moodle-dl-2.3.1.8/moodle_dl/moodle/mods/forum.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.7/moodle_dl/moodle/mods/lesson.py` & `moodle-dl-2.3.1.8/moodle_dl/moodle/mods/lesson.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.7/moodle_dl/moodle/mods/page.py` & `moodle-dl-2.3.1.8/moodle_dl/moodle/mods/page.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.7/moodle_dl/moodle/mods/quiz.py` & `moodle-dl-2.3.1.8/moodle_dl/moodle/mods/quiz.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.7/moodle_dl/moodle/mods/workshop.py` & `moodle-dl-2.3.1.8/moodle_dl/moodle/mods/workshop.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.7/moodle_dl/moodle/moodle_constants.py` & `moodle-dl-2.3.1.8/moodle_dl/moodle/moodle_constants.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.7/moodle_dl/moodle/moodle_service.py` & `moodle-dl-2.3.1.8/moodle_dl/moodle/moodle_service.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.7/moodle_dl/moodle/request_helper.py` & `moodle-dl-2.3.1.8/moodle_dl/moodle/request_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -303,32 +303,32 @@
 
     def check_json_for_moodle_error(self, resp_json: Dict, url: str, data: Dict):
         # Check for known errors
         if 'error' in resp_json:
             self.log_failed_request(url, data)
             raise RequestRejectedError(
                 'The Moodle System rejected the Request.'
-                + f" Details: {resp_json.get('error', '')} (Errorcode: {resp_json.get('errorcode', '')},"
-                + f" Stacktrace: {resp_json.get('stacktrace', '')}, Debuginfo: {resp_json.get('debuginfo', '')},"
-                + f" Reproductionlink: {resp_json.get('reproductionlink', '')})"
+                + f" Details: {resp_json.get('error', '')} (Error code: {resp_json.get('errorcode', '')},"
+                + f" Stacktrace: {resp_json.get('stacktrace', '')}, Debug info: {resp_json.get('debuginfo', '')},"
+                + f" Reproduction link: {resp_json.get('reproductionlink', '')})"
             )
 
         if 'exception' in resp_json:
             self.log_failed_request(url, data)
-            errorcode = resp_json.get('errorcode', '')
+            error_code = resp_json.get('errorcode', '')
 
-            if errorcode == 'invalidtoken':
+            if error_code == 'invalidtoken':
                 raise RequestRejectedError(
                     'Your Moodle token has expired.'
                     + ' To create a new one run "moodle-dl -nt -u USERNAME -pw PASSWORD" or "moodle-dl -nt -sso"'
                 )
 
             raise RequestRejectedError(
                 'The Moodle System rejected the Request.'
-                + f" Details: {resp_json.get('exception', '')} (Errorcode: {errorcode},"
+                + f" Details: {resp_json.get('exception', '')} (Error code: {error_code},"
                 + f" Message: {resp_json.get('message', '')})"
             )
 
     @staticmethod
     def recursive_urlencode(data):
         """URL-encode a multidimensional dictionary.
         @param data: the data to be encoded
```

### Comparing `moodle-dl-2.3.1.7/moodle_dl/moodle/result_builder.py` & `moodle-dl-2.3.1.8/moodle_dl/moodle/result_builder.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.7/moodle_dl/notifications/__init__.py` & `moodle-dl-2.3.1.8/moodle_dl/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.7/moodle_dl/notifications/console/console_service.py` & `moodle-dl-2.3.1.8/moodle_dl/notifications/console/console_service.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.7/moodle_dl/notifications/mail/header.png` & `moodle-dl-2.3.1.8/moodle_dl/notifications/mail/header.png`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.7/moodle_dl/notifications/mail/header_extender.png` & `moodle-dl-2.3.1.8/moodle_dl/notifications/mail/header_extender.png`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.7/moodle_dl/notifications/mail/mail_formater.py` & `moodle-dl-2.3.1.8/moodle_dl/notifications/mail/mail_formater.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.7/moodle_dl/notifications/mail/mail_service.py` & `moodle-dl-2.3.1.8/moodle_dl/notifications/mail/mail_service.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.7/moodle_dl/notifications/mail/mail_shooter.py` & `moodle-dl-2.3.1.8/moodle_dl/notifications/mail/mail_shooter.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.7/moodle_dl/notifications/notification_service.py` & `moodle-dl-2.3.1.8/moodle_dl/notifications/notification_service.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.7/moodle_dl/notifications/telegram/telegram_formater.py` & `moodle-dl-2.3.1.8/moodle_dl/notifications/telegram/telegram_formater.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.7/moodle_dl/notifications/telegram/telegram_service.py` & `moodle-dl-2.3.1.8/moodle_dl/notifications/telegram/telegram_service.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.7/moodle_dl/notifications/telegram/telegram_shooter.py` & `moodle-dl-2.3.1.8/moodle_dl/notifications/telegram/telegram_shooter.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.7/moodle_dl/notifications/xmpp/xmpp_formater.py` & `moodle-dl-2.3.1.8/moodle_dl/notifications/xmpp/xmpp_formater.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.7/moodle_dl/notifications/xmpp/xmpp_service.py` & `moodle-dl-2.3.1.8/moodle_dl/notifications/xmpp/xmpp_service.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.7/moodle_dl/notifications/xmpp/xmpp_shooter.py` & `moodle-dl-2.3.1.8/moodle_dl/notifications/xmpp/xmpp_shooter.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.7/moodle_dl/types.py` & `moodle-dl-2.3.1.8/moodle_dl/types.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.7/moodle_dl/utils.py` & `moodle-dl-2.3.1.8/moodle_dl/utils.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.7/moodle_dl.egg-info/PKG-INFO` & `moodle-dl-2.3.1.8/moodle_dl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moodle-dl
-Version: 2.3.1.7
+Version: 2.3.1.8
 Summary: Moodle-DL downloads course content fast from Moodle (eg. lecture pdfs)
 Home-page: https://github.com/C0D3D3V/Moodle-DL
 Author: C0D3D3V
 Author-email: moodle-dl@ist-ein-knaller.de
 License: GPL-3.0
 Project-URL: Documentation, https://github.com/C0D3D3V/Moodle-DL#readme
 Project-URL: Wiki, https://github.com/C0D3D3V/Moodle-DL/wiki
@@ -137,14 +137,17 @@
 [moodle-buddy](https://github.com/marcelreppi/moodle-buddy)
 - Plugin for Firefox and Chrome
 - Mass file download and notification functionality for the Moodle
 
 [moodle-downloader](https://github.com/harsilspatel/moodle-downloader)
 - A chrome extension for batch downloading Moodle resources
 
+[Orga Bot](https://github.com/YoshiiPlayzz/orga_bot)
+- Utilizes moodle-dl to send moodle files via Discord
+
 [discord-moodle-bot](https://github.com/tjarbo/discord-moodle-bot)
 - Discord Notification Service for your moodle courses
 
 If someone wants to link another downloader here, which offers e.g. functions that moodle-dl does not offer, feel free to open an issue. 
 
 
 ---
```

### Comparing `moodle-dl-2.3.1.7/moodle_dl.egg-info/SOURCES.txt` & `moodle-dl-2.3.1.8/moodle_dl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.7/setup.py` & `moodle-dl-2.3.1.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,14 +45,15 @@
         'colorama>=0.4.6',
         'colorlog>=6.7.0',
         'html2text>=2020.1.16',
         'readchar>=4.0.3',
         'requests>=2.24.0',
         'sentry_sdk>=0.13.5',
         'yt_dlp>=2021.10.22',
+        'pytz>=2023.3',
     ],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Console',
         'Intended Audience :: End Users/Desktop',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Programming Language :: Python :: 3 :: Only',
```

