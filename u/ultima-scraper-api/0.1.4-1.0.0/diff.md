# Comparing `tmp/ultima_scraper_api-0.1.4.tar.gz` & `tmp/ultima_scraper_api-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultima_scraper_api-0.1.4.tar", max compression
+gzip compressed data, was "ultima_scraper_api-1.0.0.tar", max compression
```

## Comparing `ultima_scraper_api-0.1.4.tar` & `ultima_scraper_api-1.0.0.tar`

### file list

```diff
@@ -1,64 +1,55 @@
--rw-r--r--   0        0        0     1030 2023-03-14 12:25:54.105413 ultima_scraper_api-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      175 2022-12-03 17:24:36.799421 ultima_scraper_api-0.1.4/ultima_scraper_api/.readthedocs.yaml
--rw-r--r--   0        0        0     1981 2023-03-10 12:01:29.654229 ultima_scraper_api-0.1.4/ultima_scraper_api/__init__.py
--rw-r--r--   0        0        0        0 2022-12-04 09:00:20.736402 ultima_scraper_api-0.1.4/ultima_scraper_api/__main__.py
--rw-r--r--   0        0        0        0 2022-12-04 15:38:35.491230 ultima_scraper_api-0.1.4/ultima_scraper_api/apis/__init__.py
--rw-r--r--   0        0        0     6789 2023-03-13 07:39:47.981078 ultima_scraper_api-0.1.4/ultima_scraper_api/apis/api_helper.py
--rw-r--r--   0        0        0     1694 2023-03-13 07:53:19.528681 ultima_scraper_api-0.1.4/ultima_scraper_api/apis/api_streamliner.py
--rw-r--r--   0        0        0      696 2022-12-02 16:36:46.812390 ultima_scraper_api-0.1.4/ultima_scraper_api/apis/background_tasks.py
--rw-r--r--   0        0        0    18402 2023-03-12 09:05:18.843851 ultima_scraper_api-0.1.4/ultima_scraper_api/apis/fanhouse/classes/auth_model.py
--rw-r--r--   0        0        0    10314 2022-12-04 18:01:35.271396 ultima_scraper_api-0.1.4/ultima_scraper_api/apis/fanhouse/classes/extras.py
--rw-r--r--   0        0        0      472 2022-08-15 05:41:16.889383 ultima_scraper_api-0.1.4/ultima_scraper_api/apis/fanhouse/classes/hightlight_model.py
--rw-r--r--   0        0        0     3756 2022-12-04 18:01:35.261397 ultima_scraper_api-0.1.4/ultima_scraper_api/apis/fanhouse/classes/message_model.py
--rw-r--r--   0        0        0     4407 2022-12-06 16:33:23.199394 ultima_scraper_api-0.1.4/ultima_scraper_api/apis/fanhouse/classes/post_model.py
--rw-r--r--   0        0        0     2000 2022-08-15 05:41:16.889383 ultima_scraper_api-0.1.4/ultima_scraper_api/apis/fanhouse/classes/story_model.py
--rw-r--r--   0        0        0    27051 2023-03-11 10:29:34.019199 ultima_scraper_api-0.1.4/ultima_scraper_api/apis/fanhouse/classes/user_model.py
--rw-r--r--   0        0        0        0 2022-08-15 05:41:16.892717 ultima_scraper_api-0.1.4/ultima_scraper_api/apis/fanhouse/decorators/decorators.py
--rw-r--r--   0        0        0     3375 2023-03-12 12:51:16.382547 ultima_scraper_api-0.1.4/ultima_scraper_api/apis/fanhouse/onlyfans.py
--rw-r--r--   0        0        0        0 2022-12-04 18:40:55.302026 ultima_scraper_api-0.1.4/ultima_scraper_api/apis/fansly/__init__.py
--rw-r--r--   0        0        0      148 2023-01-27 07:49:17.645344 ultima_scraper_api-0.1.4/ultima_scraper_api/apis/fansly/classes/__init__.py
--rw-r--r--   0        0        0    19294 2023-03-13 06:32:09.390704 ultima_scraper_api-0.1.4/ultima_scraper_api/apis/fansly/classes/auth_model.py
--rw-r--r--   0        0        0     6399 2022-12-06 16:33:24.989436 ultima_scraper_api-0.1.4/ultima_scraper_api/apis/fansly/classes/collection_model.py
--rw-r--r--   0        0        0     3005 2022-01-17 19:20:07.000000 ultima_scraper_api-0.1.4/ultima_scraper_api/apis/fansly/classes/create_story.py
--rw-r--r--   0        0        0    11477 2023-03-11 13:05:32.998139 ultima_scraper_api-0.1.4/ultima_scraper_api/apis/fansly/classes/extras.py
--rw-r--r--   0        0        0      472 2022-01-17 19:20:07.000000 ultima_scraper_api-0.1.4/ultima_scraper_api/apis/fansly/classes/hightlight_model.py
--rw-r--r--   0        0        0     6181 2023-03-11 14:03:57.634915 ultima_scraper_api-0.1.4/ultima_scraper_api/apis/fansly/classes/message_model.py
--rw-r--r--   0        0        0     6760 2023-03-14 07:15:05.559037 ultima_scraper_api-0.1.4/ultima_scraper_api/apis/fansly/classes/post_model.py
--rw-r--r--   0        0        0    28527 2023-03-13 23:55:28.909339 ultima_scraper_api-0.1.4/ultima_scraper_api/apis/fansly/classes/user_model.py
--rw-r--r--   0        0        0        0 2022-01-17 19:20:07.000000 ultima_scraper_api-0.1.4/ultima_scraper_api/apis/fansly/decorators/decorators.py
--rw-r--r--   0        0        0     3394 2023-03-11 11:44:48.226325 ultima_scraper_api-0.1.4/ultima_scraper_api/apis/fansly/fansly.py
--rw-r--r--   0        0        0        0 2022-12-04 09:13:12.413462 ultima_scraper_api-0.1.4/ultima_scraper_api/apis/onlyfans/__init__.py
--rw-r--r--   0        0        0      136 2023-03-12 08:50:34.483731 ultima_scraper_api-0.1.4/ultima_scraper_api/apis/onlyfans/classes/__init__.py
--rw-r--r--   0        0        0    19862 2023-03-14 11:52:46.209968 ultima_scraper_api-0.1.4/ultima_scraper_api/apis/onlyfans/classes/auth_model.py
--rw-r--r--   0        0        0    10617 2023-03-14 05:46:23.534240 ultima_scraper_api-0.1.4/ultima_scraper_api/apis/onlyfans/classes/extras.py
--rw-r--r--   0        0        0      431 2023-03-14 11:16:11.218569 ultima_scraper_api-0.1.4/ultima_scraper_api/apis/onlyfans/classes/hightlight_model.py
--rw-r--r--   0        0        0     3610 2023-03-12 09:22:31.246292 ultima_scraper_api-0.1.4/ultima_scraper_api/apis/onlyfans/classes/message_model.py
--rw-r--r--   0        0        0     4352 2023-03-14 07:13:56.926251 ultima_scraper_api-0.1.4/ultima_scraper_api/apis/onlyfans/classes/post_model.py
--rw-r--r--   0        0        0     1969 2022-10-13 17:05:42.790902 ultima_scraper_api-0.1.4/ultima_scraper_api/apis/onlyfans/classes/story_model.py
--rw-r--r--   0        0        0    27516 2023-03-14 11:18:00.987884 ultima_scraper_api-0.1.4/ultima_scraper_api/apis/onlyfans/classes/user_model.py
--rw-r--r--   0        0        0        0 2022-01-17 19:20:07.000000 ultima_scraper_api-0.1.4/ultima_scraper_api/apis/onlyfans/decorators/decorators.py
--rw-r--r--   0        0        0     3591 2023-03-11 09:21:55.860416 ultima_scraper_api-0.1.4/ultima_scraper_api/apis/onlyfans/onlyfans.py
--rw-r--r--   0        0        0     2678 2023-03-12 07:58:39.963131 ultima_scraper_api-0.1.4/ultima_scraper_api/apis/user_streamliner.py
--rw-r--r--   0        0        0        0 2022-12-04 09:59:08.749358 ultima_scraper_api-0.1.4/ultima_scraper_api/classes/__init__.py
--rw-r--r--   0        0        0    12983 2023-01-30 14:15:08.499950 ultima_scraper_api-0.1.4/ultima_scraper_api/classes/make_settings.py
--rw-r--r--   0        0        0     3977 2023-03-12 11:46:35.721289 ultima_scraper_api-0.1.4/ultima_scraper_api/classes/prepare_directories.py
--rw-r--r--   0        0        0      340 2022-01-17 19:20:07.000000 ultima_scraper_api-0.1.4/ultima_scraper_api/classes/prepare_download.py
--rw-r--r--   0        0        0    13641 2023-03-05 22:04:19.935624 ultima_scraper_api-0.1.4/ultima_scraper_api/classes/prepare_metadata.py
--rw-r--r--   0        0        0      630 2022-01-17 19:20:07.000000 ultima_scraper_api-0.1.4/ultima_scraper_api/classes/prepare_webhooks.py
--rw-r--r--   0        0        0      638 2022-12-03 12:11:12.443198 ultima_scraper_api-0.1.4/ultima_scraper_api/docs/Makefile
--rw-r--r--   0        0        0      804 2022-12-03 12:11:12.443198 ultima_scraper_api-0.1.4/ultima_scraper_api/docs/make.bat
--rw-r--r--   0        0        0       21 2022-12-03 17:06:06.309429 ultima_scraper_api-0.1.4/ultima_scraper_api/docs/requirements.txt
--rw-r--r--   0        0        0     1318 2022-12-03 18:16:52.399681 ultima_scraper_api-0.1.4/ultima_scraper_api/docs/source/conf.py
--rw-r--r--   0        0        0      464 2022-12-03 17:00:27.610084 ultima_scraper_api-0.1.4/ultima_scraper_api/docs/source/index.rst
--rw-r--r--   0        0        0        0 2022-12-04 09:51:18.483387 ultima_scraper_api-0.1.4/ultima_scraper_api/helpers/__init__.py
--rw-r--r--   0        0        0    11470 2023-03-12 12:49:04.742083 ultima_scraper_api-0.1.4/ultima_scraper_api/helpers/main_helper.py
--rw-r--r--   0        0        0        0 2023-01-26 05:39:16.747803 ultima_scraper_api-0.1.4/ultima_scraper_api/managers/__init__.py
--rw-r--r--   0        0        0        0 2023-01-22 17:41:52.794214 ultima_scraper_api-0.1.4/ultima_scraper_api/managers/job_manager/__init__.py
--rw-r--r--   0        0        0     1791 2023-03-04 03:36:24.985587 ultima_scraper_api-0.1.4/ultima_scraper_api/managers/job_manager/job_manager.py
--rw-r--r--   0        0        0        0 2023-01-22 17:42:18.641239 ultima_scraper_api-0.1.4/ultima_scraper_api/managers/job_manager/jobs/__init__.py
--rw-r--r--   0        0        0      666 2023-03-10 12:01:40.541149 ultima_scraper_api-0.1.4/ultima_scraper_api/managers/job_manager/jobs/custom_job.py
--rw-r--r--   0        0        0     1871 2023-03-13 10:56:06.754299 ultima_scraper_api-0.1.4/ultima_scraper_api/managers/scrape_manager.py
--rw-r--r--   0        0        0    10699 2023-03-14 03:20:57.916720 ultima_scraper_api-0.1.4/ultima_scraper_api/managers/session_manager.py
--rw-r--r--   0        0        0        0 2022-12-04 16:42:28.821209 ultima_scraper_api-0.1.4/ultima_scraper_api/py.typed
--rw-r--r--   0        0        0     1753 1970-01-01 00:00:00.000000 ultima_scraper_api-0.1.4/setup.py
--rw-r--r--   0        0        0     1026 1970-01-01 00:00:00.000000 ultima_scraper_api-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1030 2023-04-11 15:16:22.758788 ultima_scraper_api-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      175 2022-12-03 17:24:36.799421 ultima_scraper_api-1.0.0/ultima_scraper_api/.readthedocs.yaml
+-rw-r--r--   0        0        0     2140 2023-03-26 20:22:06.588147 ultima_scraper_api-1.0.0/ultima_scraper_api/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-04 09:00:20.736402 ultima_scraper_api-1.0.0/ultima_scraper_api/__main__.py
+-rw-r--r--   0        0        0        0 2022-12-04 15:38:35.491230 ultima_scraper_api-1.0.0/ultima_scraper_api/apis/__init__.py
+-rw-r--r--   0        0        0     6799 2023-03-25 23:19:49.924231 ultima_scraper_api-1.0.0/ultima_scraper_api/apis/api_helper.py
+-rw-r--r--   0        0        0     1694 2023-03-13 07:53:19.528681 ultima_scraper_api-1.0.0/ultima_scraper_api/apis/api_streamliner.py
+-rw-r--r--   0        0        0      696 2022-12-02 16:36:46.812390 ultima_scraper_api-1.0.0/ultima_scraper_api/apis/background_tasks.py
+-rw-r--r--   0        0        0     2842 2023-04-09 16:10:08.954446 ultima_scraper_api-1.0.0/ultima_scraper_api/apis/fansly/__init__.py
+-rw-r--r--   0        0        0      164 2023-03-26 17:40:00.484637 ultima_scraper_api-1.0.0/ultima_scraper_api/apis/fansly/classes/__init__.py
+-rw-r--r--   0        0        0    19219 2023-04-10 14:08:37.807384 ultima_scraper_api-1.0.0/ultima_scraper_api/apis/fansly/classes/auth_model.py
+-rw-r--r--   0        0        0     6511 2023-04-10 15:12:02.910813 ultima_scraper_api-1.0.0/ultima_scraper_api/apis/fansly/classes/collection_model.py
+-rw-r--r--   0        0        0    11370 2023-04-11 14:57:48.165435 ultima_scraper_api-1.0.0/ultima_scraper_api/apis/fansly/classes/extras.py
+-rw-r--r--   0        0        0      472 2022-01-17 19:20:07.000000 ultima_scraper_api-1.0.0/ultima_scraper_api/apis/fansly/classes/hightlight_model.py
+-rw-r--r--   0        0        0     6216 2023-04-11 15:11:13.965757 ultima_scraper_api-1.0.0/ultima_scraper_api/apis/fansly/classes/message_model.py
+-rw-r--r--   0        0        0     6918 2023-04-09 17:42:13.567826 ultima_scraper_api-1.0.0/ultima_scraper_api/apis/fansly/classes/post_model.py
+-rw-r--r--   0        0        0     3212 2023-03-26 19:02:31.325107 ultima_scraper_api-1.0.0/ultima_scraper_api/apis/fansly/classes/story_model.py
+-rw-r--r--   0        0        0    28526 2023-03-26 18:21:56.425911 ultima_scraper_api-1.0.0/ultima_scraper_api/apis/fansly/classes/user_model.py
+-rw-r--r--   0        0        0        0 2022-01-17 19:20:07.000000 ultima_scraper_api-1.0.0/ultima_scraper_api/apis/fansly/decorators/decorators.py
+-rw-r--r--   0        0        0     3783 2023-04-11 14:58:58.366956 ultima_scraper_api-1.0.0/ultima_scraper_api/apis/fansly/fansly.py
+-rw-r--r--   0        0        0     2505 2023-04-09 16:10:03.007639 ultima_scraper_api-1.0.0/ultima_scraper_api/apis/onlyfans/__init__.py
+-rw-r--r--   0        0        0      153 2023-03-26 20:30:17.157147 ultima_scraper_api-1.0.0/ultima_scraper_api/apis/onlyfans/classes/__init__.py
+-rw-r--r--   0        0        0    19775 2023-04-10 14:11:12.738977 ultima_scraper_api-1.0.0/ultima_scraper_api/apis/onlyfans/classes/auth_model.py
+-rw-r--r--   0        0        0    10554 2023-03-21 11:26:19.768761 ultima_scraper_api-1.0.0/ultima_scraper_api/apis/onlyfans/classes/extras.py
+-rw-r--r--   0        0        0      686 2023-03-25 19:37:35.462288 ultima_scraper_api-1.0.0/ultima_scraper_api/apis/onlyfans/classes/hightlight_model.py
+-rw-r--r--   0        0        0     2748 2023-03-27 06:43:37.105523 ultima_scraper_api-1.0.0/ultima_scraper_api/apis/onlyfans/classes/message_model.py
+-rw-r--r--   0        0        0     3375 2023-03-27 00:23:55.042753 ultima_scraper_api-1.0.0/ultima_scraper_api/apis/onlyfans/classes/post_model.py
+-rw-r--r--   0        0        0     1318 2023-04-09 10:09:44.773447 ultima_scraper_api-1.0.0/ultima_scraper_api/apis/onlyfans/classes/story_model.py
+-rw-r--r--   0        0        0    27336 2023-04-20 16:58:56.954100 ultima_scraper_api-1.0.0/ultima_scraper_api/apis/onlyfans/classes/user_model.py
+-rw-r--r--   0        0        0        0 2022-01-17 19:20:07.000000 ultima_scraper_api-1.0.0/ultima_scraper_api/apis/onlyfans/decorators/decorators.py
+-rw-r--r--   0        0        0     3980 2023-03-28 02:35:06.221154 ultima_scraper_api-1.0.0/ultima_scraper_api/apis/onlyfans/onlyfans.py
+-rw-r--r--   0        0        0     2678 2023-03-12 07:58:39.963131 ultima_scraper_api-1.0.0/ultima_scraper_api/apis/user_streamliner.py
+-rw-r--r--   0        0        0        0 2022-12-04 09:59:08.749358 ultima_scraper_api-1.0.0/ultima_scraper_api/classes/__init__.py
+-rw-r--r--   0        0        0    13187 2023-03-24 22:26:49.870986 ultima_scraper_api-1.0.0/ultima_scraper_api/classes/make_settings.py
+-rw-r--r--   0        0        0     3977 2023-03-12 11:46:35.721289 ultima_scraper_api-1.0.0/ultima_scraper_api/classes/prepare_directories.py
+-rw-r--r--   0        0        0      340 2022-01-17 19:20:07.000000 ultima_scraper_api-1.0.0/ultima_scraper_api/classes/prepare_download.py
+-rw-r--r--   0        0        0    13595 2023-04-11 15:12:54.204494 ultima_scraper_api-1.0.0/ultima_scraper_api/classes/prepare_metadata.py
+-rw-r--r--   0        0        0      630 2022-01-17 19:20:07.000000 ultima_scraper_api-1.0.0/ultima_scraper_api/classes/prepare_webhooks.py
+-rw-r--r--   0        0        0      638 2022-12-03 12:11:12.443198 ultima_scraper_api-1.0.0/ultima_scraper_api/docs/Makefile
+-rw-r--r--   0        0        0      804 2022-12-03 12:11:12.443198 ultima_scraper_api-1.0.0/ultima_scraper_api/docs/make.bat
+-rw-r--r--   0        0        0       21 2022-12-03 17:06:06.309429 ultima_scraper_api-1.0.0/ultima_scraper_api/docs/requirements.txt
+-rw-r--r--   0        0        0     1318 2022-12-03 18:16:52.399681 ultima_scraper_api-1.0.0/ultima_scraper_api/docs/source/conf.py
+-rw-r--r--   0        0        0      464 2022-12-03 17:00:27.610084 ultima_scraper_api-1.0.0/ultima_scraper_api/docs/source/index.rst
+-rw-r--r--   0        0        0        0 2022-12-04 09:51:18.483387 ultima_scraper_api-1.0.0/ultima_scraper_api/helpers/__init__.py
+-rw-r--r--   0        0        0    11469 2023-04-09 08:48:21.278550 ultima_scraper_api-1.0.0/ultima_scraper_api/helpers/main_helper.py
+-rw-r--r--   0        0        0        0 2023-01-26 05:39:16.747803 ultima_scraper_api-1.0.0/ultima_scraper_api/managers/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-22 17:41:52.794214 ultima_scraper_api-1.0.0/ultima_scraper_api/managers/job_manager/__init__.py
+-rw-r--r--   0        0        0     1791 2023-03-04 03:36:24.985587 ultima_scraper_api-1.0.0/ultima_scraper_api/managers/job_manager/job_manager.py
+-rw-r--r--   0        0        0        0 2023-01-22 17:42:18.641239 ultima_scraper_api-1.0.0/ultima_scraper_api/managers/job_manager/jobs/__init__.py
+-rw-r--r--   0        0        0      704 2023-03-24 22:51:29.186132 ultima_scraper_api-1.0.0/ultima_scraper_api/managers/job_manager/jobs/custom_job.py
+-rw-r--r--   0        0        0     2181 2023-03-27 18:00:12.375116 ultima_scraper_api-1.0.0/ultima_scraper_api/managers/scrape_manager.py
+-rw-r--r--   0        0        0    15089 2023-04-11 15:11:25.469328 ultima_scraper_api-1.0.0/ultima_scraper_api/managers/session_manager.py
+-rw-r--r--   0        0        0        0 2022-12-04 16:42:28.821209 ultima_scraper_api-1.0.0/ultima_scraper_api/py.typed
+-rw-r--r--   0        0        0     1623 1970-01-01 00:00:00.000000 ultima_scraper_api-1.0.0/setup.py
+-rw-r--r--   0        0        0     1026 1970-01-01 00:00:00.000000 ultima_scraper_api-1.0.0/PKG-INFO
```

### Comparing `ultima_scraper_api-0.1.4/pyproject.toml` & `ultima_scraper_api-1.0.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ultima-scraper-api"
-version = "0.1.4"
+version = "1.0.0"
 description = ""
 authors = [
     "DIGITALCRIMINALS <89371864+digitalcriminals@users.noreply.github.com>",
 ]
 packages = [{include = "ultima_scraper_api"}]
 include = ["ultima_scraper_api/py.typed"]
```

### Comparing `ultima_scraper_api-0.1.4/ultima_scraper_api/__init__.py` & `ultima_scraper_api-1.0.0/ultima_scraper_api/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,21 +10,25 @@
 
 auth_types = (
     onlyfans_classes.auth_model.create_auth | fansly_classes.auth_model.create_auth
 )
 user_types = (
     onlyfans_classes.user_model.create_user | fansly_classes.user_model.create_user
 )
+story_types = (
+    onlyfans_classes.story_model.create_story | fansly_classes.story_model.create_story
+)
 post_types = (
     onlyfans_classes.post_model.create_post | fansly_classes.post_model.create_post
 )
 message_types = (
     onlyfans_classes.message_model.create_message
     | fansly_classes.message_model.create_message
 )
+content_types = story_types|post_types|message_types
 error_types = onlyfans_classes.extras.ErrorDetails | fansly_classes.extras.ErrorDetails
 
 
 def select_api(option: str, config: Config = Config()):
     """Allows you to select an API
 
     Args:
```

### Comparing `ultima_scraper_api-0.1.4/ultima_scraper_api/apis/api_helper.py` & `ultima_scraper_api-1.0.0/ultima_scraper_api/apis/api_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         api_type = (
             await get_function_name(function_that_called, True)
             if not api_type
             else api_type
         )
         try:
             # We assume the class type is create_user
-            result = getattr(api.temp_scraped, api_type)
+            result = getattr(api.scrape_manager.scraped, api_type)
         except AttributeError:
             # we assume the class type is create_auth
             api_type = api_type.lower()
             result = getattr(api, api_type)
 
     return result
```

### Comparing `ultima_scraper_api-0.1.4/ultima_scraper_api/apis/api_streamliner.py` & `ultima_scraper_api-1.0.0/ultima_scraper_api/apis/api_streamliner.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-0.1.4/ultima_scraper_api/apis/background_tasks.py` & `ultima_scraper_api-1.0.0/ultima_scraper_api/apis/background_tasks.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-0.1.4/ultima_scraper_api/apis/fanhouse/classes/auth_model.py` & `ultima_scraper_api-1.0.0/ultima_scraper_api/apis/onlyfans/classes/auth_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,75 +1,82 @@
 from __future__ import annotations
 
 import asyncio
 import math
 from asyncio.tasks import Task
 from datetime import datetime
 from itertools import chain, product
-from multiprocessing.pool import Pool
 from typing import TYPE_CHECKING, Any, Dict, Optional, Union
 
 from dateutil.relativedelta import relativedelta
-from user_agent import generate_user_agent
-
 from ultima_scraper_api.apis import api_helper
 from ultima_scraper_api.apis.onlyfans.classes.extras import (
+    AuthDetails,
     ErrorDetails,
-    auth_details,
     create_headers,
     endpoint_links,
 )
 from ultima_scraper_api.apis.onlyfans.classes.message_model import create_message
 from ultima_scraper_api.apis.onlyfans.classes.post_model import create_post
 from ultima_scraper_api.apis.onlyfans.classes.user_model import create_user
 from ultima_scraper_api.managers.session_manager import SessionManager
+from user_agent import generate_user_agent
 
 if TYPE_CHECKING:
     from ultima_scraper_api.apis.onlyfans.onlyfans import OnlyFansAPI
 
+# auth_model.py handles functions that only relate to the authenticated user
+# We can create a auth_streamliner that has a parent class of create_user instead
+
 
 class create_auth(create_user):
     def __init__(
         self,
         api: OnlyFansAPI,
         option: dict[str, Any] = {},
         max_threads: int = -1,
+        auth_details: AuthDetails = AuthDetails(),
     ) -> None:
         self.api = api
+        self.users: set[create_user] = set()
+        self.auth_details = auth_details
+        self.session_manager = self._SessionManager(self, max_threads=max_threads)
         create_user.__init__(self, option, self)
         if not self.username:
             self.username = f"u{self.id}"
         self.lists = []
         self.links = api.ContentTypes()
         self.subscriptions: list[create_user] = []
         self.chats = None
         self.archived_stories = {}
         self.mass_messages = []
         self.paid_content: list[create_message | create_post] = []
-        temp_pool = pool if pool else api_helper.multiprocessing()
-        self.session_manager = self._SessionManager(self, max_threads=max_threads)
-        self.auth_details = auth_details()
+        self.auth_attempt = 0
         self.guest = False
         self.active: bool = False
         self.errors: list[ErrorDetails] = []
         self.extras: dict[str, Any] = {}
+        self.blacklist: list[str] = []
 
     class _SessionManager(SessionManager):
         def __init__(
             self,
             auth: create_auth,
             headers: dict[str, Any] = {},
             proxies: list[str] = [],
             max_threads: int = -1,
             use_cookies: bool = True,
         ) -> None:
             SessionManager.__init__(
                 self, auth, headers, proxies, max_threads, use_cookies
             )
 
+    def get_pool(self):
+        return self.api.pool
+
     async def convert_to_user(self):
         user = await self.get_user(self.username)
         for k, _v in user.__dict__.items():
             setattr(user, k, getattr(self, k))
         return user
 
     def update(self, data: Dict[str, Any]):
@@ -77,38 +84,34 @@
             data["username"] = f"u{data['id']}"
         for key, value in data.items():
             found_attr = hasattr(self, key)
             if found_attr:
                 setattr(self, key, value)
 
     async def login(self, max_attempts: int = 10, guest: bool = False):
-        auth_version = "(V1)"
         auth_items = self.auth_details
         if not auth_items:
             return self
         if guest and auth_items:
             auth_items.cookie.auth_id = "0"
-            auth_items.user_agent = str(generate_user_agent())
+            auth_items.user_agent = generate_user_agent()
         link = endpoint_links().customer
         user_agent = auth_items.user_agent
         auth_id = str(auth_items.cookie.auth_id)
         # expected string error is fixed by auth_id
         dynamic_rules = self.session_manager.dynamic_rules
         a: list[Any] = [dynamic_rules, auth_id, auth_items.x_bc, user_agent, link]
         self.session_manager.headers = create_headers(*a)
         if guest:
             self.guest = True
             return self
 
-        count = 1
-        while count < max_attempts + 1:
-            string = f"Auth {auth_version} Attempt {count}/{max_attempts}"
-            print(string)
+        while self.auth_attempt < max_attempts + 1:
             await self.process_auth()
-            count += 1
+            self.auth_attempt += 1
 
             async def resolve_auth(auth: create_auth):
                 if self.errors:
                     error = self.errors[-1]
                     print(error.message)
                     if error.code == 101:
                         if auth_items.support_2fa:
@@ -155,20 +158,20 @@
             if isinstance(user, create_user):
                 self.update(user.__dict__)
         return self
 
     async def process_auth(self):
         if not self.active:
             link = endpoint_links().customer
-            response = await self.session_manager.json_request(link)
-            if response:
-                await self.resolve_auth_errors(response)
+            json_resp = await self.session_manager.json_request(link)
+            if json_resp:
+                await self.resolve_auth_errors(json_resp)
                 if not self.errors:
                     self.active = True
-                    self.update(response)
+                    self.update(json_resp)
             else:
                 # 404'ed
                 self.active = False
         return self
 
     async def resolve_auth_errors(self, response: ErrorDetails | dict[str, Any]):
         # Adds an error object to self.auth.errors
@@ -199,29 +202,55 @@
         self.errors.append(error)
 
     async def get_lists(self, refresh: bool = True, limit: int = 100, offset: int = 0):
         result, status = await api_helper.default_data(self, refresh)
         if status:
             return result
         link = endpoint_links(global_limit=limit, global_offset=offset).lists
-        results = await self.session_manager.json_request(link)
-        self.lists = results
-        return results
+        json_resp = await self.session_manager.json_request(link)
+        self.lists = json_resp
+        return json_resp
+
+    async def get_blacklist(self, local_blacklists: list[str]):
+        bl_ids: list[str] = []
+        remote_blacklists = await self.get_lists()
+        if remote_blacklists:
+            for remote_blacklist in remote_blacklists:
+                for local_blacklist in local_blacklists:
+                    if remote_blacklist["name"] == local_blacklist:
+                        list_users = remote_blacklist["users"]
+                        if remote_blacklist["usersCount"] > 2:
+                            list_id = remote_blacklist["id"]
+                            list_users = await self.get_lists_users(list_id)
+                        if list_users:
+                            users = list_users
+                            bl_ids = [x["username"] for x in users]
+        return bl_ids
+
+    async def match_identifiers(self, identifiers: list[int | str]):
+        if self.id in identifiers or self.username in identifiers:
+            return True
+        else:
+            return False
 
-    async def get_user(
-        self, identifier: Union[str, int]
-    ) -> Union[create_user, ErrorDetails]:
-        link = endpoint_links(identifier).users
-        response = await self.session_manager.json_request(link)
-        if not isinstance(response, ErrorDetails):
-            if not response:
-                print
-            response["session_manager"] = self.session_manager
-            response = create_user(response, self)
-        return response
+    def find_user_by_identifier(self, identifier: int | str):
+        user = [x for x in self.users if x.id == identifier or x.username == identifier]
+        return user
+
+    async def get_user(self, identifier: int | str) -> Union[create_user, ErrorDetails]:
+        valid_user = self.find_user_by_identifier(identifier)
+        if valid_user:
+            return valid_user[0]
+        else:
+            link = endpoint_links(identifier).users
+            response = await self.session_manager.json_request(link)
+            if not isinstance(response, ErrorDetails):
+                response["session_manager"] = self.session_manager
+                response = create_user(response, self)
+            return response
 
     async def get_lists_users(
         self,
         identifier: int | str,
         check: bool = False,
         limit: int = 100,
         offset: int = 0,
@@ -237,18 +266,21 @@
             results2 = await self.get_lists_users(
                 identifier, limit=limit, offset=limit + offset
             )
             results.extend(results2)
         return results
 
     async def get_subscription(
-        self,
-        identifier: int | str = "",
+        self, identifier: int | str = "", custom_list: list[create_user] = []
     ) -> create_user | None:
-        subscriptions = await self.get_subscriptions(refresh=False)
+        subscriptions = (
+            await self.get_subscriptions(refresh=False)
+            if not custom_list
+            else custom_list
+        )
         valid = None
         for subscription in subscriptions:
             if identifier == subscription.username or identifier == subscription.id:
                 valid = subscription
                 break
         return valid
 
@@ -297,15 +329,15 @@
                         )
                         tasks.append(task)
                 results2 = await asyncio.gather(*tasks)
                 for result in results2:
                     if isinstance(result, ErrorDetails):
                         continue
                     if not result:
-                        print
+                        pass
                     subscription2: create_user = result
                     for subscription in subscriptions:
                         if subscription["id"] != subscription2.id:
                             continue
                         subscription = subscription | subscription2.__dict__
                         subscription = create_user(subscription, self)
                         if subscription.isBlocked:
@@ -319,88 +351,80 @@
                 if isinstance(subscription, ErrorDetails):
                     return result
                 subscription.subscribedByData = {}
                 new_date = datetime.now() + relativedelta(years=1)
                 subscription.subscribedByData["expiredAt"] = new_date.isoformat()
                 subscriptions = [subscription]
                 results.append(subscriptions)
-            pool = self.pool
-            tasks = pool.starmap(multi, product(offset_array))
-            results2 = await asyncio.gather(*tasks)
-            results2 = list(filter(None, results2))
-            results.extend(results2)
+            with self.get_pool() as pool:
+                tasks = pool.starmap(multi, product(offset_array))
+                results2 = await asyncio.gather(*tasks)
+                results2 = list(filter(None, results2))
+                results.extend(results2)
         else:
             for identifier in identifiers:
                 if self.id == identifier or self.username == identifier:
                     continue
                 link = endpoint_links(identifier=identifier).users
                 result = await self.session_manager.json_request(link)
                 if isinstance(result, ErrorDetails) or not result["subscribedBy"]:
                     continue
                 subscription = create_user(result, self)
                 if subscription.isBlocked:
                     continue
                 results.append([subscription])
-                print
-            print
         final_results = [x for x in results if x is not None]
         final_results = list(chain(*final_results))
         self.subscriptions = final_results
         return final_results
 
     async def get_chats(
         self,
-        links: Optional[list[str]] = None,
+        links: list[str] = [],
         limit: int = 100,
         offset: int = 0,
+        depth: int = 1,
         refresh: bool = True,
-        inside_loop: bool = False,
     ) -> list[dict[str, Any]]:
         result, status = await api_helper.default_data(self, refresh)
         if status:
             return result
-        if links is None:
-            links = []
-        api_count = self.chatMessagesCount
-        if api_count and not links:
-            link = endpoint_links(
-                identifier=self.id, global_limit=limit, global_offset=offset
-            ).list_chats
-            ceil = math.ceil(api_count / limit)
-            numbers = list(range(ceil))
-            for num in numbers:
-                num = num * limit
-                link = link.replace(f"limit={limit}", f"limit={limit}")
-                new_link = link.replace("offset=0", f"offset={num}")
-                links.append(new_link)
+
         multiplier = self.session_manager.max_threads
-        if links:
-            link = links[-1]
-        else:
-            link = endpoint_links(
-                identifier=self.id, global_limit=limit, global_offset=offset
-            ).list_chats
-        links2 = api_helper.calculate_the_unpredictable(link, limit, multiplier)
-        if not inside_loop:
-            links += links2
-        else:
-            links = links2
-        results = await self.session_manager.bulk_requests(links)
-        results = [await x.json() for x in results if x]
+        temp_limit = limit
+        temp_offset = offset
+        link = endpoint_links(
+            identifier=self.id, global_limit=temp_limit, global_offset=temp_offset
+        ).list_chats
+        unpredictable_links, new_offset = api_helper.calculate_the_unpredictable(
+            link, offset, limit, multiplier, depth
+        )
+        links = unpredictable_links if depth != 1 else links + unpredictable_links
+        results = await self.session_manager.bulk_json_requests(links)
         has_more = results[-1]["hasMore"]
         final_results = [x["list"] for x in results]
         final_results = list(chain.from_iterable(final_results))
+        for result in final_results:
+            result["withUser"] = create_user(result["withUser"], self)
+            result["lastMessage"] = create_message(
+                result["lastMessage"], result["withUser"]
+            )
 
         if has_more:
             results2 = await self.get_chats(
-                links=[links[-1]], limit=limit, offset=limit + offset, inside_loop=True
+                limit=limit,
+                offset=new_offset,
+                depth=depth + 1,
             )
             final_results.extend(results2)
 
-        final_results.sort(key=lambda x: x["withUser"]["id"], reverse=True)
+        if depth == 1:
+            pass
+
+        final_results.sort(key=lambda x: x["withUser"].id, reverse=True)
         self.chats = final_results
         return final_results
 
     async def get_mass_messages(
         self,
         resume: Optional[list[dict[str, Any]]] = None,
         refresh: bool = True,
@@ -448,28 +472,35 @@
     ) -> list[create_message | create_post] | ErrorDetails:
         result, status = await api_helper.default_data(self, refresh)
         if status:
             return result
         link = endpoint_links(global_limit=limit, global_offset=offset).paid_api
         final_results = await self.session_manager.json_request(link)
         if not isinstance(final_results, ErrorDetails):
-            if len(final_results) >= limit and not check:
+            if len(final_results) > 0 and not check:
                 results2 = await self.get_paid_content(
                     limit=limit, offset=limit + offset, inside_loop=True
                 )
                 final_results.extend(results2)
             if not inside_loop:
                 temp: list[create_message | create_post] = []
                 for final_result in final_results:
                     content = None
                     if final_result["responseType"] == "message":
                         user = create_user(final_result["fromUser"], self)
                         content = create_message(final_result, user)
-                        print
                     elif final_result["responseType"] == "post":
                         user = create_user(final_result["author"], self)
                         content = create_post(final_result, user)
                     if content:
                         temp.append(content)
                 final_results = temp
             self.paid_content = final_results
         return final_results
+
+    async def resolve_user(self, post_id: int | None = None):
+        user = None
+        if post_id:
+            post = await self.get_post(post_id)
+            if not isinstance(post, ErrorDetails):
+                user = post.author
+        return user
```

### Comparing `ultima_scraper_api-0.1.4/ultima_scraper_api/apis/fanhouse/classes/extras.py` & `ultima_scraper_api-1.0.0/ultima_scraper_api/apis/onlyfans/classes/extras.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,38 @@
-from __future__ import annotations
-
 import copy
 import math
 from itertools import chain
 from pathlib import Path
-from typing import TYPE_CHECKING, Any, Literal, Optional, Union
-
-if TYPE_CHECKING:
-    from ultima_scraper_api.apis.onlyfans.classes.auth_model import create_auth
+from typing import Any, Literal, Optional, Union
 
 
-class auth_details:
-    def __init__(self, options: dict[str, Any] = {}) -> None:
-        self.username = options.get("username", "")
-        self.cookie = cookie_parser(options.get("cookie", ""))
-        self.x_bc = options.get("x_bc", "")
-        self.user_agent: str = options.get("user_agent", "")
-        self.email = options.get("email", "")
-        self.password = options.get("password", "")
-        self.hashed = options.get("hashed", False)
-        self.support_2fa = options.get("support_2fa", True)
-        self.active = options.get("active", True)
+class AuthDetails:
+    def __init__(self, username:str="", cookie:str="", x_bc:str="",user_agent:str="",email:str="", password:str="", hashed:bool=False,support_2fa:bool=True, active:bool=True) -> None:
+        self.username = username
+        self.cookie = cookie_parser(cookie)
+        self.x_bc = x_bc
+        self.user_agent = user_agent
+        self.email = email
+        self.password = password
+        self.hashed = hashed
+        self.support_2fa = support_2fa
+        self.active = active
 
     def upgrade_legacy(self, options: dict[str, Any]):
         if "cookie" not in options:
             self = legacy_auth_details(options).upgrade(self)
         return self
 
     def export(self):
         new_dict = copy.copy(self.__dict__)
         cookie = self.cookie.convert()
-        new_dict["cookie"] = cookie
+        results = [
+            x for x in cookie.replace(" ", "").split(";") if x and x.split("=")[1]
+        ]
+        new_dict["cookie"] = cookie if results else ""
         return new_dict
 
 
 class legacy_auth_details:
     def __init__(self, option: dict[str, Any] = {}):
         self.username = option.get("username", "")
         self.auth_id = option.get("auth_id", "")
@@ -45,15 +43,15 @@
         self.x_bc = option.get("x_bc", "")
         self.email = option.get("email", "")
         self.password = option.get("password", "")
         self.hashed = option.get("hashed", False)
         self.support_2fa = option.get("support_2fa", True)
         self.active = option.get("active", True)
 
-    def upgrade(self, new_auth_details: auth_details):
+    def upgrade(self, new_auth_details: AuthDetails):
         new_dict = ""
         for key, value in self.__dict__.items():
             value = value if value != None else ""
             skippable = ["username", "user_agent"]
             if key not in skippable:
                 new_dict += f"{key}={value}; "
         new_dict = new_dict.strip()
@@ -62,33 +60,40 @@
 
 
 class cookie_parser:
     def __init__(self, options: str) -> None:
         new_dict: dict[str, Any] = {}
         for crumble in options.strip().split(";"):
             if crumble:
-                key, value = crumble.strip().split("=", 1)
-                new_dict[key] = value
+                split_value = crumble.strip().split("=", 1)
+                if len(split_value) >= 2:
+                    key, value = split_value
+                    new_dict[key] = value
         self.auth_id = new_dict.get("auth_id", "")
         self.sess = new_dict.get("sess", "")
         self.auth_hash = new_dict.get("auth_hash", "")
         self.auth_uniq_ = new_dict.get("auth_uniq_", "")
         self.auth_uid_ = new_dict.get("auth_uid_", "")
+        self.aws_waf_token = new_dict.get("aws-waf-token", "")
 
     def format(self):
         """
         Typically used for adding cookies to requests
         """
-        return self.__dict__
+        final_dict = self.__dict__.copy()
+        final_dict["aws-waf-token"] = final_dict["aws_waf_token"]
+        final_dict.pop("aws_waf_token")
+        return final_dict
 
     def convert(self):
         new_dict = ""
         for key, value in self.__dict__.items():
             key = key.replace("auth_uniq_", f"auth_uniq_{self.auth_id}")
             key = key.replace("auth_uid_", f"auth_uid_{self.auth_id}")
+            key = key.replace("aws_waf_token", f"aws-waf-token")
             new_dict += f"{key}={value}; "
         new_dict = new_dict.strip()
         return new_dict
 
 
 class endpoint_links(object):
     def __init__(
@@ -97,22 +102,20 @@
         identifier2: Optional[int | str] = None,
         identifier3: Optional[int | str] = None,
         text: str = "",
         global_limit: int = 10,
         global_offset: int = 0,
         sort_order: Literal["asc", "desc"] = "desc",
     ):
-        domain = "https://fanhouse.app"
-        api = "/api"
+        domain = "https://onlyfans.com"
+        api = "/api2/v2"
         full_url_path = f"{domain}{api}"
         self.full_url_path = full_url_path
         self.customer = f"https://onlyfans.com/api2/v2/users/me"
-        self.users = (
-            f"https://api.fanhouse.app/api/get-target-user/{identifier}/{identifier2}"
-        )
+        self.users = f"https://onlyfans.com/api2/v2/users/{identifier}"
         self.subscriptions = f"https://onlyfans.com/api2/v2/subscriptions/subscribes?limit={global_limit}&offset={global_offset}&type=active"
         self.lists = f"https://onlyfans.com/api2/v2/lists?limit=100&offset=0"
         self.lists_users = f"https://onlyfans.com/api2/v2/lists/{identifier}/users?limit={global_limit}&offset={global_offset}&query="
         self.list_chats = f"https://onlyfans.com/api2/v2/chats?limit={global_limit}&offset={global_offset}&order=desc"
         self.post_by_id = f"https://onlyfans.com/api2/v2/posts/{identifier}"
         self.message_by_id = f"https://onlyfans.com/api2/v2/chats/{identifier}/messages?limit=10&offset=0&firstId={identifier2}&order=desc&skip_users=all&skip_users_dups=1"
         self.search_chat = f"https://onlyfans.com/api2/v2/chats/{identifier}/messages/search?query={text}"
```

### Comparing `ultima_scraper_api-0.1.4/ultima_scraper_api/apis/fanhouse/classes/message_model.py` & `ultima_scraper_api-1.0.0/ultima_scraper_api/apis/onlyfans/classes/message_model.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,85 +1,61 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, Optional
 
-from ultima_scraper_api.apis.onlyfans.classes import user_model
+from ultima_scraper_api.apis.onlyfans import SiteContent
 from ultima_scraper_api.apis.onlyfans.classes.extras import endpoint_links
 
 if TYPE_CHECKING:
     from ultima_scraper_api.apis.onlyfans.classes.user_model import create_user
 
 
-class create_message:
+class create_message(SiteContent):
     def __init__(self, option: dict[str, Any], user: create_user) -> None:
+
+        author = user.get_authed().find_user_by_identifier(option["fromUser"]["id"])[0]
+        SiteContent.__init__(self, option, author)
         self.responseType: Optional[str] = option.get("responseType")
-        self.text: Optional[str] = option.get("text")
+        self.text: str = option.get("text","")
         self.lockedText: Optional[bool] = option.get("lockedText")
         self.isFree: Optional[bool] = option.get("isFree")
         self.price: Optional[float] = option.get("price")
         self.isMediaReady: Optional[bool] = option.get("isMediaReady")
         self.mediaCount: Optional[int] = option.get("mediaCount")
         self.media: list[dict[str, Any]] = option.get("media", [])
         self.previews: list[dict[str, Any]] = option.get("previews", [])
         self.isTip: Optional[bool] = option.get("isTip")
         self.isReportedByMe: Optional[bool] = option.get("isReportedByMe")
-        self.fromUser = (
-            user
-            if user.id == option["fromUser"]["id"]
-            else user_model.create_user(option["fromUser"], user.get_authed())
-        )
         self.isFromQueue: Optional[bool] = option.get("isFromQueue")
         self.queueId: Optional[int] = option.get("queueId")
         self.canUnsendQueue: Optional[bool] = option.get("canUnsendQueue")
         self.unsendSecondsQueue: Optional[int] = option.get("unsendSecondsQueue")
-        self.id: Optional[int] = option.get("id")
         self.isOpened: Optional[bool] = option.get("isOpened")
         self.isNew: Optional[bool] = option.get("isNew")
         self.createdAt: Optional[str] = option.get("createdAt")
         self.changedAt: Optional[str] = option.get("changedAt")
         self.cancelSeconds: Optional[int] = option.get("cancelSeconds")
         self.isLiked: Optional[bool] = option.get("isLiked")
         self.canPurchase: Optional[bool] = option.get("canPurchase")
         self.canPurchaseReason: Optional[str] = option.get("canPurchaseReason")
         self.canReport: Optional[bool] = option.get("canReport")
 
-    async def get_author(self):
-        return self.fromUser
+    def get_author(self):
+        return self.author
 
     async def buy_message(self):
         """
         This function will buy a ppv message from a model.
         """
         message_price = self.price
         x = {
             "amount": message_price,
             "messageId": self.id,
             "paymentType": "message",
             "token": "",
             "unavailablePaymentGates": [],
         }
         link = endpoint_links().pay
-        result = await self.fromUser.session_manager.json_request(
+        result = await self.author.get_session_manager().json_request(
             link, method="POST", payload=x
         )
         return result
-
-    async def link_picker(self, media: dict[str, Any], video_quality: str):
-        link = ""
-        if "source" in media:
-            quality_key = "source"
-            source = media[quality_key]
-            link = source[quality_key]
-            if link:
-                if media["type"] == "video":
-                    qualities = media["videoSources"]
-                    qualities = dict(sorted(qualities.items(), reverse=False))
-                    qualities[quality_key] = source[quality_key]
-                    for quality, quality_link in qualities.items():
-                        video_quality = video_quality.removesuffix("p")
-                        if quality == video_quality:
-                            if quality_link:
-                                link = quality_link
-                                break
-        if "src" in media:
-            link = media["src"]
-        return link
```

### Comparing `ultima_scraper_api-0.1.4/ultima_scraper_api/apis/fanhouse/classes/user_model.py` & `ultima_scraper_api-1.0.0/ultima_scraper_api/apis/fansly/classes/user_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 from __future__ import annotations
 
 import math
-from itertools import chain
-from pathlib import Path
 from typing import TYPE_CHECKING, Any, Optional, Union
 from urllib import parse
 
-import ultima_scraper_api.apis.onlyfans.classes.message_model as message_model
+import ultima_scraper_api.apis.fansly.classes.message_model as message_model
 from ultima_scraper_api.apis import api_helper
-from ultima_scraper_api.apis.onlyfans.classes import post_model
-from ultima_scraper_api.apis.onlyfans.classes.extras import ErrorDetails, endpoint_links
-from ultima_scraper_api.apis.onlyfans.classes.hightlight_model import create_highlight
-from ultima_scraper_api.apis.onlyfans.classes.story_model import create_story
+from ultima_scraper_api.apis.fansly.classes import collection_model, post_model
+from ultima_scraper_api.apis.fansly.classes.extras import (
+    ErrorDetails,
+    endpoint_links,
+    handle_refresh,
+)
+from ultima_scraper_api.apis.fansly.classes.hightlight_model import create_highlight
+from ultima_scraper_api.apis.fansly.classes.story_model import create_story
+from ultima_scraper_api.apis.user_streamliner import StreamlinedUser
+from ultima_scraper_api.managers.scrape_manager import ScrapeManager
 
 if TYPE_CHECKING:
-    from ultima_scraper_api.apis.onlyfans.classes.auth_model import create_auth
-    from ultima_scraper_api.apis.onlyfans.classes.post_model import create_post
-    from ultima_scraper_api.classes.prepare_directories import (
-        DirectoryManager,
-        FileManager,
-    )
+    from ultima_scraper_api.apis.fansly.classes.auth_model import create_auth
+    from ultima_scraper_api.apis.fansly.classes.post_model import create_post
 
 
-class create_user:
-    def __init__(self, option: dict[str, Any], authed: create_auth) -> None:
-        from ultima_scraper_api.classes.prepare_directories import (
-            DirectoryManager,
-            FileManager,
-        )
-
-        self.avatar: Optional[str] = option.get("avatar")
-        self.avatarThumbs: Optional[list[str]] = option.get("avatarThumbs")
-        self.header: Optional[str] = option.get("header")
-        self.headerSize: Optional[dict[str, int]] = option.get("headerSize")
-        self.headerThumbs: Optional[list[str]] = option.get("headerThumbs")
+class create_user(StreamlinedUser):
+    def __init__(
+        self,
+        option: dict[str, Any],
+        authed: create_auth,
+    ) -> None:
+
+        self.avatar: Any = option.get("avatar")
+        self.avatarThumbs: Any = option.get("avatarThumbs")
+        self.header: Any = option.get("banner")
+        self.headerSize: Any = option.get("headerSize")
+        self.headerThumbs: Any = option.get("headerThumbs")
         self.id: int = option.get("id")
         self.name: str = option.get("name")
         self.username: str = option.get("username")
         self.canLookStory: bool = option.get("canLookStory")
         self.canCommentStory: bool = option.get("canCommentStory")
         self.hasNotViewedStory: bool = option.get("hasNotViewedStory")
         self.isVerified: bool = option.get("isVerified")
@@ -50,15 +50,17 @@
         self.tipsMin: int = option.get("tipsMin")
         self.tipsMax: int = option.get("tipsMax")
         self.canEarn: bool = option.get("canEarn")
         self.canAddSubscriber: bool = option.get("canAddSubscriber")
         self.subscribePrice: int = option.get("subscribePrice")
         self.hasStripe: bool = option.get("hasStripe")
         self.isStripeExist: bool = option.get("isStripeExist")
-        self.subscriptionBundles: list = option.get("subscriptionBundles")
+        self.subscriptionBundles: list[dict[Any, Any]] = option.get(
+            "subscriptionTiers", []
+        )
         self.canSendChatToAll: bool = option.get("canSendChatToAll")
         self.creditsMin: int = option.get("creditsMin")
         self.creditsMax: int = option.get("creditsMax")
         self.isPaywallRestriction: bool = option.get("isPaywallRestriction")
         self.unprofitable: bool = option.get("unprofitable")
         self.listsSort: str = option.get("listsSort")
         self.listsSortOrder: str = option.get("listsSortOrder")
@@ -66,37 +68,40 @@
         self.joinDate: str = option.get("joinDate")
         self.isReferrerAllowed: bool = option.get("isReferrerAllowed")
         self.about: str = option.get("about")
         self.rawAbout: str = option.get("rawAbout")
         self.website: str = option.get("website")
         self.wishlist: str = option.get("wishlist")
         self.location: str = option.get("location")
+        timeline_status = option.get("timelineStats", {})
         self.postsCount: int = option.get("postsCount")
         self.archivedPostsCount: int = option.get("archivedPostsCount")
-        self.photosCount: int = option.get("photosCount")
-        self.videosCount: int = option.get("videosCount")
+        self.photosCount: int = timeline_status.get("imageCount")
+        self.videosCount: int = timeline_status.get("videoCount")
         self.audiosCount: int = option.get("audiosCount")
         self.mediasCount: int = option.get("mediasCount")
-        self.promotions: list[dict[str, Any]] = option.get("promotions", {})
+        self.promotions: list = option.get("promotions")
         self.lastSeen: Any = option.get("lastSeen")
         self.favoritesCount: int = option.get("favoritesCount")
         self.favoritedCount: int = option.get("favoritedCount")
         self.showPostsInFeed: bool = option.get("showPostsInFeed")
         self.canReceiveChatMessage: bool = option.get("canReceiveChatMessage")
         self.isPerformer: bool = option.get("isPerformer")
         self.isRealPerformer: bool = option.get("isRealPerformer")
         self.isSpotifyConnected: bool = option.get("isSpotifyConnected")
         self.subscribersCount: int = option.get("subscribersCount")
         self.hasPinnedPosts: bool = option.get("hasPinnedPosts")
         self.canChat: bool = option.get("canChat")
         self.callPrice: int = option.get("callPrice")
         self.isPrivateRestriction: bool = option.get("isPrivateRestriction")
+        self.following: bool = option.get("following")
         self.showSubscribersCount: bool = option.get("showSubscribersCount")
         self.showMediaCount: bool = option.get("showMediaCount")
-        self.subscribedByData: Any = option.get("subscribedByData")
+        self.subscribed: bool = option.get("subscribed", False)
+        self.subscribedByData: Any = option.get("subscription")
         self.subscribedOnData: Any = option.get("subscribedOnData")
         self.canPromotion: bool = option.get("canPromotion")
         self.canCreatePromotion: bool = option.get("canCreatePromotion")
         self.canCreateTrial: bool = option.get("canCreateTrial")
         self.isAdultContent: bool = option.get("isAdultContent")
         self.isBlocked: bool = option.get("isBlocked")
         self.canTrialSend: bool = option.get("canTrialSend")
@@ -114,15 +119,15 @@
         self.isLegalApprovedAllowed: bool = option.get("isLegalApprovedAllowed")
         self.isTwitterConnected: bool = option.get("isTwitterConnected")
         self.twitterUsername: Any = option.get("twitterUsername")
         self.isAllowTweets: bool = option.get("isAllowTweets")
         self.isPaymentCardConnected: bool = option.get("isPaymentCardConnected")
         self.referalUrl: str = option.get("referalUrl")
         self.isVisibleOnline: bool = option.get("isVisibleOnline")
-        self.subscribesCount: int = option.get("subscribesCount", 0)
+        self.subscribesCount: int = option.get("subscribesCount")
         self.canPinPost: bool = option.get("canPinPost")
         self.hasNewAlerts: bool = option.get("hasNewAlerts")
         self.hasNewHints: bool = option.get("hasNewHints")
         self.hasNewChangedPriceSubscriptions: bool = option.get(
             "hasNewChangedPriceSubscriptions"
         )
         self.notificationsCount: int = option.get("notificationsCount")
@@ -214,202 +219,213 @@
         self.isCountryWithVat: bool = option.get("isCountryWithVat")
         self.connectedOfAccounts: list = option.get("connectedOfAccounts")
         self.hasPassword: bool = option.get("hasPassword")
         self.canConnectOfAccount: bool = option.get("canConnectOfAccount")
         self.pinnedPostsCount: int = option.get("pinnedPostsCount")
         self.maxPinnedPostsCount: int = option.get("maxPinnedPostsCount")
         # Custom
-        self.__authed = authed
-        self.directory_manager: DirectoryManager = DirectoryManager(
-            authed.api.get_site_settings()
-        )
-        self.file_manager: FileManager = FileManager(self.directory_manager)
+        authed.users.add(self)
         self.scraped = authed.api.ContentTypes()
         self.temp_scraped = authed.api.ContentTypes()
         self.download_info: dict[str, Any] = {}
+        self.duplicate_media = []
+        self.scrape_manager = ScrapeManager(authed.session_manager)
         self.__raw__ = option
+        StreamlinedUser.__init__(self, authed)
+
+    def __eq__(self, other: Any):
+        if isinstance(self, create_user):
+            if self.id == other.id:
+                return True
+        return False
+
+    def __hash__(self) -> int:
+        return hash((self.id))
 
     def get_link(self):
-        link = f"https://onlyfans.com/{self.username}"
+        link = f"https://fansly.com/{self.username}"
         return link
 
     def is_me(self) -> bool:
         status = False
         if self.email:
             status = True
         return status
 
-    def get_authed(self):
-        return self.__authed
-
-    def get_session_manager(self):
-        return self.__authed.session_manager
-
     async def get_stories(
         self, refresh: bool = True, limit: int = 100, offset: int = 0
     ) -> list[create_story]:
         result, status = await api_helper.default_data(self, refresh)
         if status:
             return result
         link = [
             endpoint_links(
                 identifier=self.id, global_limit=limit, global_offset=offset
             ).stories_api
         ]
+        return []
         results = await api_helper.scrape_endpoint_links(
             link, self.get_session_manager()
         )
         results = [create_story(x) for x in results]
         self.temp_scraped.Stories = results
         return results
 
     async def get_highlights(
-        self,
-        identifier: int | str = "",
-        refresh: bool = True,
-        limit: int = 100,
-        offset: int = 0,
-        hightlight_id: int | str = "",
-    ) -> Union[list[create_highlight], list[create_story]]:
-        result, status = await api_helper.default_data(self, refresh)
-        if status:
-            return result
+        self, identifier="", refresh=True, limit=100, offset=0, hightlight_id=""
+    ) -> list:
+        api_type = "highlights"
+        if not refresh:
+            result = handle_refresh(self, api_type)
+            if result:
+                return result
         if not identifier:
             identifier = self.id
         if not hightlight_id:
             link = endpoint_links(
                 identifier=identifier, global_limit=limit, global_offset=offset
             ).list_highlights
-            results = await self.get_session_manager().json_request(link)
-            results = await api_helper.remove_errors(results)
-            if results:
-                pass
+            results = await self.session_manager.json_request(link)
+            results = await remove_errors(results)
             results = [create_highlight(x) for x in results]
         else:
             link = endpoint_links(
                 identifier=hightlight_id, global_limit=limit, global_offset=offset
             ).highlight
-            results = await self.get_session_manager().json_request(link)
+            results = await self.session_manager.json_request(link)
             results = [create_story(x) for x in results["stories"]]
         return results
 
     async def get_posts(
         self,
         links: Optional[list[str]] = None,
         limit: int = 10,
         offset: int = 0,
         refresh: bool = True,
     ) -> list[create_post]:
         result, status = await api_helper.default_data(self, refresh)
         if status:
             return result
-        if links is None:
-            links = []
-        if not links:
-            epl = endpoint_links()
-            link = epl.list_posts(self.id)
-            links = epl.create_links(link, self.postsCount)
-        results = await api_helper.scrape_endpoint_links(
-            links, self.get_session_manager()
-        )
-        final_results = self.finalize_content_set(results)
-        self.temp_scraped.Posts = final_results
+        temp_results: list[Any] = []
+        while True:
+            link = endpoint_links(identifier=self.id, global_offset=offset).post_api
+            response = await self.get_session_manager().json_request(link)
+            data = response["response"]
+            temp_posts = data.get("posts")
+            if not temp_posts:
+                break
+            offset = temp_posts[-1]["id"]
+            temp_results.append(data)
+        results = api_helper.merge_dictionaries(temp_results)
+        final_results = []
+        if results:
+            final_results = [
+                post_model.create_post(x, self, results) for x in results["posts"]
+            ]
+            self.temp_scraped.Posts = final_results
         return final_results
 
     async def get_post(
         self, identifier: Optional[int | str] = None, limit: int = 10, offset: int = 0
     ) -> Union[create_post, ErrorDetails]:
         if not identifier:
             identifier = self.id
         link = endpoint_links(
             identifier=identifier, global_limit=limit, global_offset=offset
         ).post_by_id
         result = await self.get_session_manager().json_request(link)
         if isinstance(result, dict):
             temp_result: dict[str, Any] = result
-            final_result = post_model.create_post(temp_result, self)
+            final_result = post_model.create_post(temp_result, self, temp_result)
             return final_result
         return result
 
+    async def get_groups(self) -> ErrorDetails | dict[str, Any]:
+        link = endpoint_links().groups_api
+        response: ErrorDetails | dict[
+            str, Any
+        ] = await self.get_session_manager().json_request(link)
+        if isinstance(response, dict):
+            final_response: dict[str, Any] = response["response"]
+            return final_response
+        return response
+
     async def get_messages(
         self,
         links: Optional[list[str]] = None,
-        limit: int = 10,
-        offset: int = 0,
+        limit: int = 100000,
+        before: str = "",
         refresh: bool = True,
         inside_loop: bool = False,
-    ):
+    ) -> list[Any]:
         result, status = await api_helper.default_data(self, refresh)
         if status:
             return result
-        if links is None:
-            links = []
-        multiplier = self.get_session_manager().max_threads
-        if links:
-            link = links[-1]
-        else:
+        groups = await self.get_groups()
+        if isinstance(groups, ErrorDetails):
+            return []
+        found_id: Optional[int] = None
+        for group in groups["groups"]:
+            for user in group["users"]:
+                if self.id == user["userId"]:
+                    found_id = user["groupId"]
+                    break
+                print
+            print
+        final_results: list[message_model.create_message] = []
+        if found_id:
+            if links is None:
+                links = []
+
             link = endpoint_links(
-                identifier=self.id, global_limit=limit, global_offset=offset
+                identifier=found_id, global_limit=limit, before_id=before
             ).message_api
             links.append(link)
-        links2 = api_helper.calculate_the_unpredictable(link, limit, multiplier)
-        if not inside_loop:
-            links += links2
-        else:
-            links = links2
-        results = await self.session_manager.bulk_requests(links)
-        results = [await x.json() for x in results if x]
-        results = await api_helper.remove_errors(results)
-        final_results = []
-        if isinstance(results, list):
-            results = [x for x in results if x]
-            has_more = results[-1]["hasMore"] if results else False
-            final_results = [x["list"] for x in results if "list" in x]
-            final_results = list(chain.from_iterable(final_results))
 
-            if has_more:
+            results = await self.get_session_manager().bulk_requests(links)
+            results = [await x.json() for x in results if x]
+            results = await api_helper.remove_errors(results)
+            results = api_helper.merge_dictionaries(results)
+            if not results:
+                return []
+            extras = results["response"]
+            final_results = extras["messages"]
+
+            if final_results:
+                lastId = final_results[-1]["id"]
                 results2 = await self.get_messages(
                     links=[links[-1]],
                     limit=limit,
-                    offset=limit + offset,
+                    before=lastId,
                     inside_loop=True,
                 )
                 final_results.extend(results2)
-            print
             if not inside_loop:
                 final_results = [
-                    message_model.create_message(x, self) for x in final_results if x
+                    message_model.create_message(x, self, extras)
+                    for x in final_results
+                    if x
                 ]
-            else:
-                final_results.sort(key=lambda x: x["fromUser"]["id"], reverse=True)
             self.temp_scraped.Messages = final_results
         return final_results
 
     async def get_message_by_id(
-        self,
-        user_id: Optional[int] = None,
-        message_id: Optional[int] = None,
-        refresh: bool = True,
-        limit: int = 10,
-        offset: int = 0,
+        self, user_id=None, message_id=None, refresh=True, limit=10, offset=0
     ):
         if not user_id:
             user_id = self.id
         link = endpoint_links(
             identifier=user_id,
             identifier2=message_id,
             global_limit=limit,
             global_offset=offset,
         ).message_by_id
-        response = await self.get_session_manager().json_request(link)
+        response = await self.session_manager.json_request(link)
         if isinstance(response, dict):
-            temp_response: dict[str, Any] = response
-            results: list[dict[str, Any]] = [
-                x for x in temp_response["list"] if x["id"] == message_id
-            ]
+            results = [x for x in response["list"] if x["id"] == message_id]
             result = results[0] if results else {}
             final_result = message_model.create_message(result, self)
             return final_result
         return response
 
     async def get_archived_stories(
         self, refresh: bool = True, limit: int = 100, offset: int = 0
@@ -443,97 +459,95 @@
             ceil = math.ceil(api_count / limit)
             numbers = list(range(ceil))
             for num in numbers:
                 num = num * limit
                 link = link.replace(f"limit={limit}", f"limit={limit}")
                 new_link = link.replace("offset=0", f"offset={num}")
                 links.append(new_link)
-        results = await api_helper.scrape_endpoint_links(
-            links, self.get_session_manager()
-        )
+        results = await self.scrape_manager.bulk_scrape(links)
         final_results = self.finalize_content_set(results)
 
         self.temp_scraped.Archived.Posts = final_results
         return final_results
 
+    async def get_archived(self, api):
+        items = []
+        if self.is_me():
+            item = {}
+            item["type"] = "Stories"
+            item["results"] = [await self.get_archived_stories()]
+            items.append(item)
+        item = {}
+        item["type"] = "Posts"
+        # item["results"] = test
+        item["results"] = await self.get_archived_posts()
+        items.append(item)
+        return items
+
     async def search_chat(
-        self,
-        identifier: int | str = "",
-        text: str = "",
-        refresh: bool = True,
-        limit: int = 10,
-        offset: int = 0,
+        self, identifier="", text="", refresh=True, limit=10, offset=0
     ):
-        # Onlyfans can't do a simple search, so this is broken. If you want it to "work", don't use commas, or basically any mysql injection characters (lol)
         if identifier:
-            identifier = parse.urljoin(str(identifier), "messages")
-        else:
-            identifier = self.id
+            identifier = parse.urljoin(identifier, "messages")
         link = endpoint_links(
             identifier=identifier, text=text, global_limit=limit, global_offset=offset
         ).search_chat
-        results = await self.get_session_manager().json_request(link)
+        results = await self.session_manager.json_request(link)
         return results
 
     async def search_messages(
-        self,
-        identifier: int | str = "",
-        text: str = "",
-        refresh: bool = True,
-        limit: int = 10,
-        offset: int = 0,
+        self, identifier="", text="", refresh=True, limit=10, offset=0
     ):
-        # Onlyfans can't do a simple search, so this is broken. If you want it to "work", don't use commas, or basically any mysql injection characters (lol)
         if identifier:
-            identifier = parse.urljoin(str(identifier), "messages")
+            identifier = parse.urljoin(identifier, "messages")
         text = parse.quote_plus(text)
         link = endpoint_links(
             identifier=identifier, text=text, global_limit=limit, global_offset=offset
         ).search_messages
-        results = await self.get_session_manager().json_request(link)
+        results = await self.session_manager.json_request(link)
         return results
 
     async def like(self, category: str, identifier: int):
         link = endpoint_links(identifier=category, identifier2=identifier).like
-        results = await self.get_session_manager().json_request(link, method="POST")
+        results = await self.session_manager.json_request(link, method="POST")
         return results
 
     async def unlike(self, category: str, identifier: int):
         link = endpoint_links(identifier=category, identifier2=identifier).like
-        results = await self.get_session_manager().json_request(link, method="DELETE")
+        results = await self.session_manager.json_request(link, method="DELETE")
         return results
 
     async def subscription_price(self):
         """
         Returns subscription price. This includes the promotional price.
         """
         subscription_price = self.subscribePrice
         if self.promotions:
             for promotion in self.promotions:
-                promotion_price: int = promotion["price"]
+                promotion_price = promotion["price"]
                 if promotion_price < subscription_price:
                     subscription_price = promotion_price
         return subscription_price
 
     async def buy_subscription(self):
         """
         This function will subscribe to a model. If the model has a promotion available, it will use it.
         """
         subscription_price = await self.subscription_price()
-        x: dict[str, Any] = {
+        x = {
             "paymentType": "subscribe",
             "userId": self.id,
             "subscribeSource": "profile",
             "amount": subscription_price,
             "token": "",
             "unavailablePaymentGates": [],
         }
-        if self.__authed.creditBalance >= subscription_price:
+        if self.subscriber.creditBalance >= subscription_price:
             link = endpoint_links().pay
-            result = await self.get_session_manager().json_request(
+            result = await self.session_manager.json_request(
                 link, method="POST", payload=x
             )
         else:
             result = ErrorDetails(
                 {"code": 2011, "message": "Insufficient Credit Balance"}
             )
         return result
@@ -551,42 +565,70 @@
                 case "post":
                     created = post_model.create_post(result, self)
                     final_results.append(created)
                 case _:
                     print
         return final_results
 
-    def create_directory_manager(self):
-        from ultima_scraper_api.classes.prepare_directories import DirectoryManager
-
-        api = self.get_api()
-        base_directory_manager = api.base_directory_manager
-        profile_directory = base_directory_manager.profile.root_directory.joinpath(
-            self.username
-        )
-
-        metadata_directory = base_directory_manager.root_metadata_directory
-        download_directory = base_directory_manager.root_download_directory
-        self.directory_manager = DirectoryManager(
-            api.get_site_settings(),
-            profile_directory,
-            metadata_directory,
-            download_directory,
-        )
-        self.file_manager.directory_manager = self.directory_manager
-        return self.directory_manager
-
-    def get_api(self):
-        return self.__authed.api
-
     async def if_scraped(self):
         status = False
         for key, value in self.scraped.__dict__.items():
             if key == "Archived":
                 for _key_2, value in value.__dict__.items():
                     if value:
                         status = True
                         return status
             if value:
                 status = True
                 break
         return status
+
+    async def match_identifiers(self, identifiers: list[int | str]):
+        if self.id in identifiers or self.username in identifiers:
+            return True
+        else:
+            return False
+
+    async def find_duplicate_media(self):
+        for post in self.scraped.Posts:
+            for media in post["medias"]:
+                a = [
+                    media_2
+                    for post_2 in self.scraped.Posts
+                    for media_2 in post_2["medias"]
+                    if media["media_id"] != media_2["media_id"]
+                    and media["filename"] == media_2["filename"]
+                ]
+                if a:
+                    self.duplicate_media.extend(a)
+        return self.duplicate_media
+
+    async def get_collections(self):
+        link = endpoint_links(identifier=self.id).collections_api
+        results = await self.get_session_manager().json_request(link)
+        return results["response"]
+
+    async def get_collection_content(self, collection: dict[str, Any], offset: int = 0):
+        temp_responses: list[dict[str, Any]] = []
+        while True:
+            link = endpoint_links(
+                identifier=collection["id"], global_limit=25, global_offset=offset
+            ).collection_api
+            results = await self.get_session_manager().json_request(link)
+            response = results["response"]
+            album_content = response["albumContent"]
+            if not album_content:
+                break
+            offset = int(album_content[-1]["id"])
+            temp_responses.append(response)
+        responses = api_helper.merge_dictionaries(temp_responses)
+        final_result = collection_model.create_collection(collection, self, responses)
+        return final_result
+
+    async def get_avatar(self):
+        return self.avatar["locations"][0]["location"] if self.header else None
+
+    async def get_header(self):
+        return self.header["locations"][0]["location"] if self.header else None
+
+    async def is_subscribed(self):
+        pass
```

### Comparing `ultima_scraper_api-0.1.4/ultima_scraper_api/apis/fanhouse/onlyfans.py` & `ultima_scraper_api-1.0.0/ultima_scraper_api/apis/fansly/fansly.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from typing import Any, Literal, Optional, Union
 
 from ultima_scraper_api.apis.api_streamliner import StreamlinedAPI
-from ultima_scraper_api.apis.onlyfans.classes.auth_model import create_auth
-from ultima_scraper_api.apis.onlyfans.classes.extras import auth_details, endpoint_links
-from ultima_scraper_api.apis.onlyfans.classes.user_model import create_user
+from ultima_scraper_api.apis.fansly.classes.auth_model import create_auth
+from ultima_scraper_api.apis.fansly.classes.extras import AuthDetails, endpoint_links
+from ultima_scraper_api.apis.fansly.classes.user_model import create_user
 from ultima_scraper_api.classes.make_settings import Config
 
 
-class start(StreamlinedAPI):
+class FanslyAPI(StreamlinedAPI):
     def __init__(self, config: Config) -> None:
-        self.site_name: Literal["OnlyFans"] = "OnlyFans"
+        self.site_name: Literal["Fansly"] = "Fansly"
         StreamlinedAPI.__init__(self, self, config)
         self.auths: list[create_auth] = []
         self.subscriptions: list[create_user] = []
         self.endpoint_links = endpoint_links
 
     def add_auth(
         self, auth_json: dict[str, Any] = {}, only_active: bool = False
@@ -23,18 +23,20 @@
         Args:
             auth_json (dict[str, str], optional): []. Defaults to {}.
             only_active (bool, optional): [description]. Defaults to False.
 
         Returns:
             create_auth: [Auth object]
         """
-        auth = create_auth(self, pool=self.pool, max_threads=self.max_threads)
-        if only_active and not auth_json.get("active"):
+        temp_auth_details = AuthDetails(**auth_json).upgrade_legacy(auth_json)
+        auth = create_auth(
+            self, max_threads=self.max_threads, auth_details=temp_auth_details
+        )
+        if only_active and not auth.auth_details.active:
             return auth
-        temp_auth_details = auth_details(auth_json).upgrade_legacy(auth_json)
         auth.auth_details = temp_auth_details
         auth.extras["settings"] = self.config
         self.auths.append(auth)
         return auth
 
     def get_auth(self, identifier: Union[str, int]) -> Optional[create_auth]:
         final_auth = None
@@ -43,52 +45,61 @@
                 final_auth = auth
             elif auth.username == identifier:
                 final_auth = auth
             if final_auth:
                 break
         return final_auth
 
-    def create_auth_details(self, auth_json: dict[str, Any] = {}) -> auth_details:
+    def create_auth_details(self, auth_json: dict[str, Any] = {}) -> AuthDetails:
         """If you've got a auth.json file, you can load it into python and pass it through here.
 
         Args:
             auth_json (dict[str, Any], optional): [description]. Defaults to {}.
 
         Returns:
             auth_details: [auth_details object]
         """
-        return auth_details(auth_json).upgrade_legacy(auth_json)
+        return AuthDetails(**auth_json).upgrade_legacy(auth_json)
 
     class ContentTypes:
         def __init__(self) -> None:
             class ArchivedTypes:
                 def __init__(self) -> None:
                     self.Posts = []
 
                 def __iter__(self):
                     for attr, value in self.__dict__.items():
                         yield attr, value
 
             self.Stories = []
             self.Posts = []
-            self.Archived = ArchivedTypes()
+            # self.Archived = ArchivedTypes()
             self.Chats = []
             self.Messages = []
             self.Highlights = []
             self.MassMessages = []
 
         def __iter__(self):
             for attr, value in self.__dict__.items():
                 yield attr, value
 
-        async def get_keys(self):
+        def get_keys(self):
             return [item[0] for item in self]
 
-    class Locations:
+    class MediaTypes:
         def __init__(self) -> None:
-            self.Images = ["photo"]
+            self.Images = ["photo", "image"]
             self.Videos = ["video", "stream", "gif"]
             self.Audios = ["audio"]
             self.Texts = ["text"]
 
-        async def get_keys(self):
+        def get_keys(self):
             return [item[0] for item in self.__dict__.items()]
+
+        def find_by_value(self, value: str):
+            final_media_type = None
+            for media_type, alt_media_types in self.__dict__.items():
+                if value in alt_media_types:
+                    final_media_type = media_type
+            if not final_media_type:
+                raise Exception("No media type found")
+            return final_media_type
```

### Comparing `ultima_scraper_api-0.1.4/ultima_scraper_api/apis/fansly/classes/auth_model.py` & `ultima_scraper_api-1.0.0/ultima_scraper_api/apis/fansly/classes/auth_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,40 +2,38 @@
 
 import asyncio
 from datetime import datetime
 from itertools import chain, product
 from typing import TYPE_CHECKING, Any, Dict, Optional, Union
 
 from dateutil.relativedelta import relativedelta
-from user_agent import generate_user_agent
-
 from ultima_scraper_api.apis import api_helper
 from ultima_scraper_api.apis.fansly.classes.extras import (
+    AuthDetails,
     ErrorDetails,
-    auth_details,
-    content_types,
     create_headers,
     endpoint_links,
 )
 from ultima_scraper_api.apis.fansly.classes.message_model import create_message
 from ultima_scraper_api.apis.fansly.classes.post_model import create_post
 from ultima_scraper_api.apis.fansly.classes.user_model import create_user
 from ultima_scraper_api.managers.session_manager import SessionManager
+from user_agent import generate_user_agent
 
 if TYPE_CHECKING:
     from ultima_scraper_api.apis.fansly.fansly import FanslyAPI
 
 
 class create_auth(create_user):
     def __init__(
         self,
         api: FanslyAPI,
         option: dict[str, Any] = {},
         max_threads: int = -1,
-        auth_details: auth_details = auth_details(),
+        auth_details: AuthDetails = AuthDetails(),
     ) -> None:
         self.api = api
         self.users: set[create_user] = set()
         self.auth_details = auth_details
         self.session_manager = self._SessionManager(self, max_threads=max_threads)
         create_user.__init__(self, option, self)
         if not self.username:
@@ -391,16 +389,15 @@
             identifier=self.id, global_limit=temp_limit, global_offset=temp_offset
         ).list_chats
         unpredictable_links, new_offset = api_helper.calculate_the_unpredictable(
             link, offset, limit, multiplier, depth
         )
         links = unpredictable_links if depth != 1 else links + unpredictable_links
 
-        results = await self.session_manager.bulk_requests(links)
-        results = [await x.json() for x in results if x]
+        results = await self.session_manager.bulk_json_requests(links)
         has_more = results[-1]["response"]["data"]
         final_results = api_helper.merge_dictionaries(results)["response"]
 
         if has_more:
             results2 = await self.get_chats(
                 limit=temp_limit,
                 offset=new_offset,
```

### Comparing `ultima_scraper_api-0.1.4/ultima_scraper_api/apis/fansly/classes/collection_model.py` & `ultima_scraper_api-1.0.0/ultima_scraper_api/apis/fansly/classes/collection_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any
 
+from ultima_scraper_api.apis.fansly import SiteContent
 from ultima_scraper_api.apis.fansly.classes.extras import endpoint_links
 
 if TYPE_CHECKING:
     from ultima_scraper_api.apis.fansly.classes.user_model import create_user
 
 
-class create_collection:
+class create_collection(SiteContent):
     def __init__(
         self, option: dict[str, Any], user: create_user, extra: dict[str, Any]
     ) -> None:
+        SiteContent.__init__(self, option, user)
         self.responseType: str = option.get("responseType")
         self.id: int = int(option["id"])
-        self.postedAt: str = int(option.get("createdAt",0)/1000)
+        self.createdAt: str = int(option.get("createdAt",0)/1000)
         self.postedAtPrecise: str = option.get("postedAtPrecise")
         self.expiredAt: Any = option.get("expiredAt")
         self.author = user
         text: str = option.get("text", "")
         self.text = str(text or "")
         raw_text: str = option.get("rawText", "")
         self.rawText = str(raw_text or "")
@@ -81,15 +83,15 @@
                         if temp_media:
                             final_media.append(temp_media)
         self.media: list[Any] = final_media
         self.canViewMedia: bool = option.get("canViewMedia")
         self.preview: list[int] = option.get("preview", [])
         self.canPurchase: bool = option.get("canPurchase")
 
-    async def get_author(self):
+    def get_author(self):
         return self.author
 
     async def favorite(self):
         link = endpoint_links(
             identifier=f"{self.responseType}s",
             identifier2=self.id,
             identifier3=self.author.id,
```

### Comparing `ultima_scraper_api-0.1.4/ultima_scraper_api/apis/fansly/classes/create_story.py` & `ultima_scraper_api-1.0.0/ultima_scraper_api/apis/fansly/classes/story_model.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,17 @@
-from typing import Any
+from typing import TYPE_CHECKING, Any
 
+from ultima_scraper_api.apis.fansly import SiteContent
 
-class create_story:
-    def __init__(self, option: dict[str, Any] = {}) -> None:
-        self.id: int = option.get("id")
+if TYPE_CHECKING:
+    from ultima_scraper_api.apis.onlyfans.classes.user_model import create_user
+
+class create_story(SiteContent):
+    def __init__(self, option: dict[str, Any], user: "create_user") -> None:
+        SiteContent.__init__(self, option, user)
         self.userId: int = option.get("userId")
         self.createdAt: str = option.get("createdAt")
         self.expiredAt: str = option.get("expiredAt")
         self.isReady: bool = option.get("isReady")
         self.viewersCount: int = option.get("viewersCount")
         self.viewers: list = option.get("viewers")
         self.canLike: bool = option.get("canLike")
```

### Comparing `ultima_scraper_api-0.1.4/ultima_scraper_api/apis/fansly/classes/extras.py` & `ultima_scraper_api-1.0.0/ultima_scraper_api/apis/fansly/classes/extras.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import copy
 import math
 from itertools import chain
 from pathlib import Path
 from typing import Any, Literal, Optional, Union
 
 
-class auth_details:
-    def __init__(self, options: dict[str, Any] = {}) -> None:
-        self.username = options.get("username", "")
-        self.authorization = options.get("authorization", "")
-        self.user_agent: str = options.get("user_agent", "")
-        self.email = options.get("email", "")
-        self.password = options.get("password", "")
-        self.hashed = options.get("hashed", False)
-        self.support_2fa = options.get("support_2fa", True)
-        self.active = options.get("active", True)
+class AuthDetails:
+    def __init__(self, username:str="", authorization:str="", user_agent:str="",email:str="", password:str="", hashed:bool=False,support_2fa:bool=True, active:bool=True) -> None:
+        self.username = username
+        self.authorization = authorization
+        self.user_agent = user_agent
+        self.email = email
+        self.password = password
+        self.hashed = hashed
+        self.support_2fa = support_2fa
+        self.active = active
 
     def upgrade_legacy(self, options: dict[str, Any]):
         return self
 
     def export(self):
         new_dict = copy.copy(self.__dict__)
         return new_dict
@@ -35,23 +35,22 @@
         self.x_bc = option.get("x_bc", "")
         self.email = option.get("email", "")
         self.password = option.get("password", "")
         self.hashed = option.get("hashed", False)
         self.support_2fa = option.get("support_2fa", True)
         self.active = option.get("active", True)
 
-    def upgrade(self, new_auth_details: auth_details):
+    def upgrade(self, new_auth_details: AuthDetails):
         new_dict = ""
         for key, value in self.__dict__.items():
             value = value if value != None else ""
             skippable = ["username", "user_agent"]
             if key not in skippable:
                 new_dict += f"{key}={value}; "
         new_dict = new_dict.strip()
-        new_auth_details.cookie = cookie_parser(new_dict)
         return new_auth_details
 
 
 class cookie_parser:
     def __init__(self, options: str) -> None:
         new_dict = {}
         for crumble in options.strip().split(";"):
```

### Comparing `ultima_scraper_api-0.1.4/ultima_scraper_api/apis/fansly/classes/message_model.py` & `ultima_scraper_api-1.0.0/ultima_scraper_api/apis/fansly/classes/message_model.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, Optional
 
+from ultima_scraper_api.apis.fansly import SiteContent
 from ultima_scraper_api.apis.fansly.classes.extras import endpoint_links
 
 if TYPE_CHECKING:
     from ultima_scraper_api.apis.fansly.classes.user_model import create_user
 
 
-class create_message:
+class create_message(SiteContent):
     def __init__(
         self, option: dict[str, Any], user: create_user, extra: dict[Any, Any] = {}
     ) -> None:
+        author = user
+        SiteContent.__init__(self, option, author)
         self.responseType: Optional[str] = option.get("responseType")
-        self.text: Optional[str] = option["content"]
+        self.text: str = option["content"]
         self.lockedText: Optional[bool] = option.get("lockedText")
         self.isFree: Optional[bool] = option.get("isFree")
         self.price: Optional[float] = option.get("price")
         self.isMediaReady: Optional[bool] = option.get("isMediaReady")
         self.mediaCount: Optional[int] = option.get("mediaCount")
         self.media: list[Any] = option.get("attachments", [])
         self.previews: list[dict[str, Any]] = option.get("previews", [])
         self.isTip: Optional[bool] = option.get("isTip")
         self.isReportedByMe: Optional[bool] = option.get("isReportedByMe")
         self.fromUser = user.get_authed().find_user_by_identifier(option["senderId"])[0]
         self.isFromQueue: Optional[bool] = option.get("isFromQueue")
         self.queueId: Optional[int] = option.get("queueId")
         self.canUnsendQueue: Optional[bool] = option.get("canUnsendQueue")
         self.unsendSecondsQueue: Optional[int] = option.get("unsendSecondsQueue")
-        self.id: Optional[int] = option.get("id")
         self.isOpened: Optional[bool] = option.get("isOpened")
         self.isNew: Optional[bool] = option.get("isNew")
         self.createdAt: Optional[str] = option.get("createdAt")
         self.changedAt: Optional[str] = option.get("changedAt")
         self.cancelSeconds: Optional[int] = option.get("cancelSeconds")
         self.isLiked: Optional[bool] = option.get("isLiked")
         self.canPurchase: Optional[bool] = option.get("canPurchase")
@@ -44,25 +46,25 @@
         final_media_ids: list[Any] = []
         for attachment in self.attachments:
             attachment_content_id = attachment["contentId"]
             match attachment["contentType"]:
                 case 1:
                     final_media_ids.append(attachment_content_id)
                 case 2:
-                    for bundle in extra.get("accountMediaBundles",[]):
+                    for bundle in extra.get("accountMediaBundles", []):
                         if bundle["id"] == attachment_content_id:
                             final_media_ids.extend(bundle["accountMediaIds"])
                 case 32001:
                     pass
                 case _:
                     pass
         final_media: list[Any] = []
         if final_media_ids and extra:
             for final_media_id in final_media_ids:
-                for account_media in extra.get("accountMedia",[]):
+                for account_media in extra.get("accountMedia", []):
                     if account_media["id"] == final_media_id:
                         temp_media = None
                         if "preview" in account_media:
                             temp_media = account_media["preview"]
                             self.previews.append(temp_media)
                         if (
                             account_media["media"]["locations"]
@@ -70,15 +72,15 @@
                         ):
                             temp_media = account_media["media"]
                         if temp_media:
                             final_media.append(temp_media)
         self.media = final_media
         self.user = user
 
-    async def get_author(self):
+    def get_author(self):
         return self.fromUser
 
     async def buy_message(self):
         """
         This function will buy a ppv message from a model.
         """
         message_price = self.price
@@ -86,17 +88,15 @@
             "amount": message_price,
             "messageId": self.id,
             "paymentType": "message",
             "token": "",
             "unavailablePaymentGates": [],
         }
         link = endpoint_links().pay
-        result = await self.user.session_manager.json_request(
-            link, method="POST", payload=x
-        )
+        result = await self.user.get_session_manager().json_request(link)
         return result
 
     async def link_picker(self, media: dict[Any, Any], target_quality: str):
         # There are two media results at play here.
         # The top-level `media` element itself represents the original source quality.
         # It may also contain a `variants` list entry with alternate encoding qualities.
         # Each variant has a similar structure to the main media element.
```

### Comparing `ultima_scraper_api-0.1.4/ultima_scraper_api/apis/fansly/classes/post_model.py` & `ultima_scraper_api-1.0.0/ultima_scraper_api/apis/fansly/classes/post_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any
 
+from ultima_scraper_api.apis.fansly import SiteContent
 from ultima_scraper_api.apis.fansly.classes.extras import endpoint_links
 
 if TYPE_CHECKING:
     from ultima_scraper_api.apis.fansly.classes.user_model import (
         create_auth,
         create_user,
     )
 
 
-class create_post:
+class create_post(SiteContent):
     def __init__(
         self,
         option: dict[str, Any],
         user: create_auth | create_user,
         extra: dict[str, Any],
     ) -> None:
+        SiteContent.__init__(self, option, user)
         self.responseType: str = option.get("responseType")
-        self.id: int = int(option["id"])
-        self.postedAt: str = option.get("createdAt")
+        self.createdAt: str = option.get("createdAt")
         self.postedAtPrecise: str = option.get("postedAtPrecise")
         self.expiredAt: Any = option.get("expiredAt")
         self.author = user
         text: str = option.get("content", "")
         self.text = str(text or "")
         raw_text: str = option.get("rawText", "")
         self.rawText = str(raw_text or "")
@@ -74,28 +75,29 @@
         if final_media_ids:
             for final_media_id in final_media_ids:
                 for account_media in extra["accountMedia"]:
                     if account_media["id"] == final_media_id:
                         temp_media = None
                         if "preview" in account_media:
                             temp_media = account_media["preview"]
-                            self.previews.append(temp_media)
+                            if not account_media["access"]:
+                                self.preview_ids.append(int(account_media["previewId"]))
+                                self.previews.append(temp_media)
                         if (
                             account_media["media"]["locations"]
-                            or account_media["media"]["variants"]
                         ):
                             temp_media = account_media["media"]
                         if temp_media:
                             final_media.append(temp_media)
         self.media: list[Any] = final_media
         self.canViewMedia: bool = option.get("canViewMedia")
         self.preview: list[int] = option.get("preview", [])
         self.canPurchase: bool = option.get("canPurchase")
 
-    async def get_author(self):
+    def get_author(self):
         return self.author
 
     async def get_comments(self):
         epl = endpoint_links()
         link = epl.list_comments(self.responseType, self.id)
         links = epl.create_links(link, self.commentsCount)
         if links:
```

### Comparing `ultima_scraper_api-0.1.4/ultima_scraper_api/apis/fansly/classes/user_model.py` & `ultima_scraper_api-1.0.0/ultima_scraper_api/apis/onlyfans/classes/user_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,36 @@
 from __future__ import annotations
 
 import math
+from itertools import chain
 from typing import TYPE_CHECKING, Any, Optional, Union
 from urllib import parse
 
-import ultima_scraper_api.apis.fansly.classes.message_model as message_model
+import ultima_scraper_api.apis.onlyfans.classes.message_model as message_model
 from ultima_scraper_api.apis import api_helper
-from ultima_scraper_api.apis.fansly.classes import collection_model, post_model
-from ultima_scraper_api.apis.fansly.classes.create_story import create_story
-from ultima_scraper_api.apis.fansly.classes.extras import (
-    ErrorDetails,
-    endpoint_links,
-    handle_refresh,
-)
-from ultima_scraper_api.apis.fansly.classes.hightlight_model import create_highlight
+from ultima_scraper_api.apis.onlyfans.classes import post_model
+from ultima_scraper_api.apis.onlyfans.classes.extras import ErrorDetails, endpoint_links
+from ultima_scraper_api.apis.onlyfans.classes.hightlight_model import create_highlight
+from ultima_scraper_api.apis.onlyfans.classes.story_model import create_story
 from ultima_scraper_api.apis.user_streamliner import StreamlinedUser
 from ultima_scraper_api.managers.scrape_manager import ScrapeManager
 
 if TYPE_CHECKING:
-    from ultima_scraper_api.apis.fansly.classes.auth_model import create_auth
-    from ultima_scraper_api.apis.fansly.classes.post_model import create_post
+    from ultima_scraper_api.apis.onlyfans.classes.auth_model import create_auth
+    from ultima_scraper_api.apis.onlyfans.classes.post_model import create_post
 
 
 class create_user(StreamlinedUser):
-    def __init__(
-        self,
-        option: dict[str, Any],
-        authed: create_auth,
-    ) -> None:
-
-        self.avatar: Any = option.get("avatar")
-        self.avatarThumbs: Any = option.get("avatarThumbs")
-        self.header: Any = option.get("banner")
-        self.headerSize: Any = option.get("headerSize")
-        self.headerThumbs: Any = option.get("headerThumbs")
+    def __init__(self, option: dict[str, Any], authed: create_auth) -> None:
+
+        self.avatar: Optional[str] = option.get("avatar")
+        self.avatarThumbs: Optional[list[str]] = option.get("avatarThumbs")
+        self.header: Optional[str] = option.get("header")
+        self.headerSize: Optional[dict[str, int]] = option.get("headerSize")
+        self.headerThumbs: Optional[list[str]] = option.get("headerThumbs")
         self.id: int = option.get("id")
         self.name: str = option.get("name")
         self.username: str = option.get("username")
         self.canLookStory: bool = option.get("canLookStory")
         self.canCommentStory: bool = option.get("canCommentStory")
         self.hasNotViewedStory: bool = option.get("hasNotViewedStory")
         self.isVerified: bool = option.get("isVerified")
@@ -50,17 +43,15 @@
         self.tipsMin: int = option.get("tipsMin")
         self.tipsMax: int = option.get("tipsMax")
         self.canEarn: bool = option.get("canEarn")
         self.canAddSubscriber: bool = option.get("canAddSubscriber")
         self.subscribePrice: int = option.get("subscribePrice")
         self.hasStripe: bool = option.get("hasStripe")
         self.isStripeExist: bool = option.get("isStripeExist")
-        self.subscriptionBundles: list[dict[Any, Any]] = option.get(
-            "subscriptionTiers", []
-        )
+        self.subscriptionBundles: list = option.get("subscriptionBundles")
         self.canSendChatToAll: bool = option.get("canSendChatToAll")
         self.creditsMin: int = option.get("creditsMin")
         self.creditsMax: int = option.get("creditsMax")
         self.isPaywallRestriction: bool = option.get("isPaywallRestriction")
         self.unprofitable: bool = option.get("unprofitable")
         self.listsSort: str = option.get("listsSort")
         self.listsSortOrder: str = option.get("listsSortOrder")
@@ -68,41 +59,39 @@
         self.joinDate: str = option.get("joinDate")
         self.isReferrerAllowed: bool = option.get("isReferrerAllowed")
         self.about: str = option.get("about")
         self.rawAbout: str = option.get("rawAbout")
         self.website: str = option.get("website")
         self.wishlist: str = option.get("wishlist")
         self.location: str = option.get("location")
-        timeline_status = option.get("timelineStats", {})
         self.postsCount: int = option.get("postsCount")
         self.archivedPostsCount: int = option.get("archivedPostsCount")
-        self.photosCount: int = timeline_status.get("imageCount")
-        self.videosCount: int = timeline_status.get("videoCount")
+        self.photosCount: int = option.get("photosCount")
+        self.videosCount: int = option.get("videosCount")
         self.audiosCount: int = option.get("audiosCount")
         self.mediasCount: int = option.get("mediasCount")
-        self.promotions: list = option.get("promotions")
+        self.promotions: list[dict[str, Any]] = option.get("promotions", {})
         self.lastSeen: Any = option.get("lastSeen")
         self.favoritesCount: int = option.get("favoritesCount")
         self.favoritedCount: int = option.get("favoritedCount")
         self.showPostsInFeed: bool = option.get("showPostsInFeed")
         self.canReceiveChatMessage: bool = option.get("canReceiveChatMessage")
         self.isPerformer: bool = option.get("isPerformer")
         self.isRealPerformer: bool = option.get("isRealPerformer")
         self.isSpotifyConnected: bool = option.get("isSpotifyConnected")
         self.subscribersCount: int = option.get("subscribersCount")
         self.hasPinnedPosts: bool = option.get("hasPinnedPosts")
         self.canChat: bool = option.get("canChat")
         self.callPrice: int = option.get("callPrice")
         self.isPrivateRestriction: bool = option.get("isPrivateRestriction")
-        self.following: bool = option.get("following")
         self.showSubscribersCount: bool = option.get("showSubscribersCount")
         self.showMediaCount: bool = option.get("showMediaCount")
-        self.subscribed: bool = option.get("subscribed", False)
-        self.subscribedByData: Any = option.get("subscription")
+        self.subscribedByData: Any = option.get("subscribedByData")
         self.subscribedOnData: Any = option.get("subscribedOnData")
+        self.subscribedIsExpiredNow: bool = option.get("subscribedIsExpiredNow")
         self.canPromotion: bool = option.get("canPromotion")
         self.canCreatePromotion: bool = option.get("canCreatePromotion")
         self.canCreateTrial: bool = option.get("canCreateTrial")
         self.isAdultContent: bool = option.get("isAdultContent")
         self.isBlocked: bool = option.get("isBlocked")
         self.canTrialSend: bool = option.get("canTrialSend")
         self.canAddPhone: bool = option.get("canAddPhone")
@@ -119,15 +108,15 @@
         self.isLegalApprovedAllowed: bool = option.get("isLegalApprovedAllowed")
         self.isTwitterConnected: bool = option.get("isTwitterConnected")
         self.twitterUsername: Any = option.get("twitterUsername")
         self.isAllowTweets: bool = option.get("isAllowTweets")
         self.isPaymentCardConnected: bool = option.get("isPaymentCardConnected")
         self.referalUrl: str = option.get("referalUrl")
         self.isVisibleOnline: bool = option.get("isVisibleOnline")
-        self.subscribesCount: int = option.get("subscribesCount")
+        self.subscribesCount: int = option.get("subscribesCount", 0)
         self.canPinPost: bool = option.get("canPinPost")
         self.hasNewAlerts: bool = option.get("hasNewAlerts")
         self.hasNewHints: bool = option.get("hasNewHints")
         self.hasNewChangedPriceSubscriptions: bool = option.get(
             "hasNewChangedPriceSubscriptions"
         )
         self.notificationsCount: int = option.get("notificationsCount")
@@ -220,16 +209,14 @@
         self.connectedOfAccounts: list = option.get("connectedOfAccounts")
         self.hasPassword: bool = option.get("hasPassword")
         self.canConnectOfAccount: bool = option.get("canConnectOfAccount")
         self.pinnedPostsCount: int = option.get("pinnedPostsCount")
         self.maxPinnedPostsCount: int = option.get("maxPinnedPostsCount")
         # Custom
         authed.users.add(self)
-        self.scraped = authed.api.ContentTypes()
-        self.temp_scraped = authed.api.ContentTypes()
         self.download_info: dict[str, Any] = {}
         self.duplicate_media = []
         self.scrape_manager = ScrapeManager(authed.session_manager)
         self.__raw__ = option
         StreamlinedUser.__init__(self, authed)
 
     def __eq__(self, other: Any):
@@ -238,209 +225,194 @@
                 return True
         return False
 
     def __hash__(self) -> int:
         return hash((self.id))
 
     def get_link(self):
-        link = f"https://fansly.com/{self.username}"
+        link = f"https://onlyfans.com/{self.username}"
         return link
 
     def is_me(self) -> bool:
         status = False
         if self.email:
             status = True
         return status
 
     async def get_stories(
         self, refresh: bool = True, limit: int = 100, offset: int = 0
     ) -> list[create_story]:
         result, status = await api_helper.default_data(self, refresh)
         if status:
             return result
-        link = [
+        links = [
             endpoint_links(
                 identifier=self.id, global_limit=limit, global_offset=offset
             ).stories_api
         ]
-        return []
-        results = await api_helper.scrape_endpoint_links(
-            link, self.get_session_manager()
-        )
-        results = [create_story(x) for x in results]
-        self.temp_scraped.Stories = results
-        return results
+
+        results = await self.scrape_manager.bulk_scrape(links)
+        final_results = [create_story(x, self) for x in results]
+        self.scrape_manager.scraped.Stories = final_results
+        return final_results
 
     async def get_highlights(
-        self, identifier="", refresh=True, limit=100, offset=0, hightlight_id=""
-    ) -> list:
-        api_type = "highlights"
-        if not refresh:
-            result = handle_refresh(self, api_type)
-            if result:
-                return result
+        self,
+        identifier: int | str = "",
+        refresh: bool = True,
+        limit: int = 100,
+        offset: int = 0,
+        hightlight_id: int | str = "",
+    ) -> list[create_highlight] | list[create_story]:
+        from ultima_scraper_api import error_types
+
+        default_result, status = await api_helper.default_data(self, refresh)
+        if status:
+            return default_result
+        final_results = []
         if not identifier:
             identifier = self.id
         if not hightlight_id:
             link = endpoint_links(
                 identifier=identifier, global_limit=limit, global_offset=offset
             ).list_highlights
-            results = await self.session_manager.json_request(link)
-            results = await remove_errors(results)
-            results = [create_highlight(x) for x in results]
+            result: dict[str, Any] = await self.get_session_manager().json_request(link)
+            final_results = [create_highlight(x, self) for x in result.get("list", [])]
         else:
             link = endpoint_links(
                 identifier=hightlight_id, global_limit=limit, global_offset=offset
             ).highlight
-            results = await self.session_manager.json_request(link)
-            results = [create_story(x) for x in results["stories"]]
-        return results
+            result = await self.get_session_manager().json_request(link)
+            if not isinstance(result, error_types):
+                final_results = [create_story(x, self) for x in result["stories"]]
+        return final_results
 
     async def get_posts(
         self,
         links: Optional[list[str]] = None,
         limit: int = 10,
         offset: int = 0,
         refresh: bool = True,
     ) -> list[create_post]:
         result, status = await api_helper.default_data(self, refresh)
         if status:
             return result
-        temp_results: list[Any] = []
-        while True:
-            link = endpoint_links(identifier=self.id, global_offset=offset).post_api
-            response = await self.get_session_manager().json_request(link)
-            data = response["response"]
-            temp_posts = data.get("posts")
-            if not temp_posts:
-                break
-            offset = temp_posts[-1]["id"]
-            temp_results.append(data)
-        results = api_helper.merge_dictionaries(temp_results)
-        final_results = []
-        if results:
-            final_results = [
-                post_model.create_post(x, self, results) for x in results["posts"]
-            ]
-            self.temp_scraped.Posts = final_results
+        if links is None:
+            links = []
+        if not links:
+            epl = endpoint_links()
+            link = epl.list_posts(self.id)
+            links = epl.create_links(link, self.postsCount)
+        results = await self.scrape_manager.bulk_scrape(links)
+        final_results = self.finalize_content_set(results)
+        self.scrape_manager.scraped.Posts = final_results
         return final_results
 
     async def get_post(
         self, identifier: Optional[int | str] = None, limit: int = 10, offset: int = 0
     ) -> Union[create_post, ErrorDetails]:
         if not identifier:
             identifier = self.id
         link = endpoint_links(
             identifier=identifier, global_limit=limit, global_offset=offset
         ).post_by_id
         result = await self.get_session_manager().json_request(link)
         if isinstance(result, dict):
             temp_result: dict[str, Any] = result
-            final_result = post_model.create_post(temp_result, self, temp_result)
+            final_result = post_model.create_post(temp_result, self)
+            if not final_result.author.id:
+                final_result.author = create_user(final_result.__raw__["author"], self)
+                pass
             return final_result
         return result
 
-    async def get_groups(self) -> ErrorDetails | dict[str, Any]:
-        link = endpoint_links().groups_api
-        response: ErrorDetails | dict[
-            str, Any
-        ] = await self.get_session_manager().json_request(link)
-        if isinstance(response, dict):
-            final_response: dict[str, Any] = response["response"]
-            return final_response
-        return response
-
     async def get_messages(
         self,
-        links: Optional[list[str]] = None,
-        limit: int = 100000,
-        before: str = "",
+        links: list[str] = [],
+        limit: int = 10,
+        offset: int = 0,
+        depth: int = 1,
         refresh: bool = True,
-        inside_loop: bool = False,
-    ) -> list[Any]:
+    ):
         result, status = await api_helper.default_data(self, refresh)
         if status:
             return result
-        groups = await self.get_groups()
-        if isinstance(groups, ErrorDetails):
-            return []
-        found_id: Optional[int] = None
-        for group in groups["groups"]:
-            for user in group["users"]:
-                if self.id == user["userId"]:
-                    found_id = user["groupId"]
-                    break
-                print
-            print
-        final_results: list[message_model.create_message] = []
-        if found_id:
-            if links is None:
-                links = []
-
-            link = endpoint_links(
-                identifier=found_id, global_limit=limit, before_id=before
-            ).message_api
-            links.append(link)
-
-            results = await self.get_session_manager().bulk_requests(links)
-            results = [await x.json() for x in results if x]
-            results = await api_helper.remove_errors(results)
-            results = api_helper.merge_dictionaries(results)
-            if not results:
-                return []
-            extras = results["response"]
-            final_results = extras["messages"]
+        multiplier = self.get_session_manager().max_threads
+        temp_limit = limit
+        temp_offset = offset
+        link = endpoint_links(
+            identifier=self.id, global_limit=temp_limit, global_offset=temp_offset
+        ).message_api
+        unpredictable_links, new_offset = api_helper.calculate_the_unpredictable(
+            link, offset, limit, multiplier, depth
+        )
+        links = unpredictable_links if depth != 1 else links + unpredictable_links
+        results = await self.get_session_manager().bulk_json_requests(links)
+        results = await api_helper.remove_errors(results)
+        final_results = []
+        if isinstance(results, list):
+            results = [x for x in results if x]
+            has_more = results[-1]["hasMore"] if results else False
+            final_results = [x["list"] for x in results if "list" in x]
+            final_results = list(chain.from_iterable(final_results))
 
-            if final_results:
-                lastId = final_results[-1]["id"]
+            if has_more:
                 results2 = await self.get_messages(
-                    links=[links[-1]],
-                    limit=limit,
-                    before=lastId,
-                    inside_loop=True,
+                    limit=temp_limit,
+                    offset=new_offset,
+                    depth=depth + 1,
                 )
                 final_results.extend(results2)
-            if not inside_loop:
+            if depth == 1:
                 final_results = [
-                    message_model.create_message(x, self, extras)
-                    for x in final_results
-                    if x
+                    message_model.create_message(x, self) for x in final_results if x
                 ]
-            self.temp_scraped.Messages = final_results
+                pass
+            else:
+                final_results.sort(key=lambda x: x["fromUser"]["id"], reverse=True)
+            self.scrape_manager.scraped.Messages = final_results
         return final_results
 
     async def get_message_by_id(
-        self, user_id=None, message_id=None, refresh=True, limit=10, offset=0
+        self,
+        user_id: Optional[int] = None,
+        message_id: Optional[int] = None,
+        refresh: bool = True,
+        limit: int = 10,
+        offset: int = 0,
     ):
         if not user_id:
             user_id = self.id
         link = endpoint_links(
             identifier=user_id,
             identifier2=message_id,
             global_limit=limit,
             global_offset=offset,
         ).message_by_id
-        response = await self.session_manager.json_request(link)
+        response = await self.get_session_manager().json_request(link)
         if isinstance(response, dict):
-            results = [x for x in response["list"] if x["id"] == message_id]
+            temp_response: dict[str, Any] = response
+            results: list[dict[str, Any]] = [
+                x for x in temp_response["list"] if x["id"] == message_id
+            ]
             result = results[0] if results else {}
             final_result = message_model.create_message(result, self)
             return final_result
         return response
 
     async def get_archived_stories(
         self, refresh: bool = True, limit: int = 100, offset: int = 0
     ):
         result, status = await api_helper.default_data(self, refresh)
         if status:
             return result
         link = endpoint_links(global_limit=limit, global_offset=offset).archived_stories
         results = await self.get_session_manager().json_request(link)
         results = await api_helper.remove_errors(results)
-        results = [create_story(x) for x in results]
+        results = [create_story(x, self) for x in results]
         return results
 
     async def get_archived_posts(
         self,
         links: Optional[list[str]] = None,
         refresh: bool = True,
         limit: int = 10,
@@ -459,106 +431,104 @@
             ceil = math.ceil(api_count / limit)
             numbers = list(range(ceil))
             for num in numbers:
                 num = num * limit
                 link = link.replace(f"limit={limit}", f"limit={limit}")
                 new_link = link.replace("offset=0", f"offset={num}")
                 links.append(new_link)
+
         results = await self.scrape_manager.bulk_scrape(links)
         final_results = self.finalize_content_set(results)
 
-        self.temp_scraped.Archived.Posts = final_results
+        self.scrape_manager.scraped.Posts.extend(final_results)
         return final_results
 
-    async def get_archived(self, api):
-        items = []
-        if self.is_me():
-            item = {}
-            item["type"] = "Stories"
-            item["results"] = [await self.get_archived_stories()]
-            items.append(item)
-        item = {}
-        item["type"] = "Posts"
-        # item["results"] = test
-        item["results"] = await self.get_archived_posts()
-        items.append(item)
-        return items
-
     async def search_chat(
-        self, identifier="", text="", refresh=True, limit=10, offset=0
+        self,
+        identifier: int | str = "",
+        text: str = "",
+        refresh: bool = True,
+        limit: int = 10,
+        offset: int = 0,
     ):
+        # Onlyfans can't do a simple search, so this is broken. If you want it to "work", don't use commas, or basically any mysql injection characters (lol)
         if identifier:
-            identifier = parse.urljoin(identifier, "messages")
+            identifier = parse.urljoin(str(identifier), "messages")
+        else:
+            identifier = self.id
         link = endpoint_links(
             identifier=identifier, text=text, global_limit=limit, global_offset=offset
         ).search_chat
-        results = await self.session_manager.json_request(link)
+        results = await self.get_session_manager().json_request(link)
         return results
 
     async def search_messages(
-        self, identifier="", text="", refresh=True, limit=10, offset=0
+        self,
+        identifier: int | str = "",
+        text: str = "",
+        refresh: bool = True,
+        limit: int = 10,
+        offset: int = 0,
     ):
+        # Onlyfans can't do a simple search, so this is broken. If you want it to "work", don't use commas, or basically any mysql injection characters (lol)
         if identifier:
-            identifier = parse.urljoin(identifier, "messages")
+            identifier = parse.urljoin(str(identifier), "messages")
         text = parse.quote_plus(text)
         link = endpoint_links(
             identifier=identifier, text=text, global_limit=limit, global_offset=offset
         ).search_messages
-        results = await self.session_manager.json_request(link)
+        results = await self.get_session_manager().json_request(link)
         return results
 
     async def like(self, category: str, identifier: int):
         link = endpoint_links(identifier=category, identifier2=identifier).like
-        results = await self.session_manager.json_request(link, method="POST")
+        results = await self.get_session_manager().json_request(link, method="POST")
         return results
 
     async def unlike(self, category: str, identifier: int):
         link = endpoint_links(identifier=category, identifier2=identifier).like
-        results = await self.session_manager.json_request(link, method="DELETE")
+        results = await self.get_session_manager().json_request(link, method="DELETE")
         return results
 
     async def subscription_price(self):
         """
         Returns subscription price. This includes the promotional price.
         """
         subscription_price = self.subscribePrice
         if self.promotions:
             for promotion in self.promotions:
-                promotion_price = promotion["price"]
+                promotion_price: int = promotion["price"]
                 if promotion_price < subscription_price:
                     subscription_price = promotion_price
         return subscription_price
 
     async def buy_subscription(self):
         """
         This function will subscribe to a model. If the model has a promotion available, it will use it.
         """
         subscription_price = await self.subscription_price()
-        x = {
+        x: dict[str, Any] = {
             "paymentType": "subscribe",
             "userId": self.id,
             "subscribeSource": "profile",
             "amount": subscription_price,
             "token": "",
             "unavailablePaymentGates": [],
         }
-        if self.subscriber.creditBalance >= subscription_price:
+        if self.get_authed().creditBalance >= subscription_price:
             link = endpoint_links().pay
-            result = await self.session_manager.json_request(
+            result = await self.get_session_manager().json_request(
                 link, method="POST", payload=x
             )
         else:
             result = ErrorDetails(
                 {"code": 2011, "message": "Insufficient Credit Balance"}
             )
         return result
 
-    def set_scraped(self, name: str, scraped: list[Any]):
-        setattr(self.scraped, name, scraped)
-
     def finalize_content_set(self, results: list[dict[str, Any]] | list[str]):
         final_results: list[create_post] = []
         for result in results:
             if isinstance(result, str):
                 continue
             content_type = result["responseType"]
             match content_type:
@@ -585,50 +555,31 @@
     async def match_identifiers(self, identifiers: list[int | str]):
         if self.id in identifiers or self.username in identifiers:
             return True
         else:
             return False
 
     async def find_duplicate_media(self):
+        # A user had 10 photos but only 5 were downloaded, this was because some media on OnlyFans have the same filename but an invalid link.
+        # Even if the link returns a 404, OnlyFans still counts it as a valid media when providing model statistics.
+        # I'll have to create a diagnosis function that checks if any media fails to download and return the reason why.
         for post in self.scraped.Posts:
             for media in post["medias"]:
                 a = [
                     media_2
                     for post_2 in self.scraped.Posts
                     for media_2 in post_2["medias"]
                     if media["media_id"] != media_2["media_id"]
                     and media["filename"] == media_2["filename"]
                 ]
                 if a:
                     self.duplicate_media.extend(a)
         return self.duplicate_media
 
-    async def get_collections(self):
-        link = endpoint_links(identifier=self.id).collections_api
-        results = await self.get_session_manager().json_request(link)
-        return results["response"]
-
-    async def get_collection_content(self, collection: dict[str, Any], offset: int = 0):
-        temp_responses: list[dict[str, Any]] = []
-        while True:
-            link = endpoint_links(
-                identifier=collection["id"], global_limit=25, global_offset=offset
-            ).collection_api
-            results = await self.get_session_manager().json_request(link)
-            response = results["response"]
-            album_content = response["albumContent"]
-            if not album_content:
-                break
-            offset = int(album_content[-1]["id"])
-            temp_responses.append(response)
-        responses = api_helper.merge_dictionaries(temp_responses)
-        final_result = collection_model.create_collection(collection, self, responses)
-        return final_result
-
     async def get_avatar(self):
-        return self.avatar["locations"][0]["location"] if self.header else None
+        return self.avatar
 
     async def get_header(self):
-        return self.header["locations"][0]["location"] if self.header else None
+        return self.header
 
     async def is_subscribed(self):
-        pass
+        return not self.subscribedIsExpiredNow
```

### Comparing `ultima_scraper_api-0.1.4/ultima_scraper_api/apis/fansly/fansly.py` & `ultima_scraper_api-1.0.0/ultima_scraper_api/apis/onlyfans/onlyfans.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from typing import Any, Literal, Optional, Union
 
 from ultima_scraper_api.apis.api_streamliner import StreamlinedAPI
-from ultima_scraper_api.apis.fansly.classes.auth_model import create_auth
-from ultima_scraper_api.apis.fansly.classes.extras import auth_details, endpoint_links
-from ultima_scraper_api.apis.fansly.classes.user_model import create_user
+from ultima_scraper_api.apis.onlyfans.classes.auth_model import create_auth
+from ultima_scraper_api.apis.onlyfans.classes.extras import AuthDetails, endpoint_links
+from ultima_scraper_api.apis.onlyfans.classes.user_model import create_user
 from ultima_scraper_api.classes.make_settings import Config
 
 
-class FanslyAPI(StreamlinedAPI):
-    def __init__(self, config: Config) -> None:
-        self.site_name: Literal["Fansly"] = "Fansly"
+class OnlyFansAPI(StreamlinedAPI):
+    def __init__(self, config: Config = Config()) -> None:
+        self.site_name: Literal["OnlyFans"] = "OnlyFans"
         StreamlinedAPI.__init__(self, self, config)
         self.auths: list[create_auth] = []
         self.subscriptions: list[create_user] = []
         self.endpoint_links = endpoint_links
 
     def add_auth(
         self, auth_json: dict[str, Any] = {}, only_active: bool = False
@@ -23,16 +23,18 @@
         Args:
             auth_json (dict[str, str], optional): []. Defaults to {}.
             only_active (bool, optional): [description]. Defaults to False.
 
         Returns:
             create_auth: [Auth object]
         """
-        temp_auth_details = auth_details(auth_json).upgrade_legacy(auth_json)
-        auth = create_auth(self, max_threads=self.max_threads,auth_details=temp_auth_details)
+        temp_auth_details = AuthDetails(**auth_json).upgrade_legacy(auth_json)
+        auth = create_auth(
+            self, max_threads=self.max_threads, auth_details=temp_auth_details
+        )
         if only_active and not auth.auth_details.active:
             return auth
         auth.auth_details = temp_auth_details
         auth.extras["settings"] = self.config
         self.auths.append(auth)
         return auth
 
@@ -43,52 +45,65 @@
                 final_auth = auth
             elif auth.username == identifier:
                 final_auth = auth
             if final_auth:
                 break
         return final_auth
 
-    def create_auth_details(self, auth_json: dict[str, Any] = {}) -> auth_details:
+    def create_auth_details(self, auth_json: dict[str, Any] = {}) -> AuthDetails:
         """If you've got a auth.json file, you can load it into python and pass it through here.
 
         Args:
             auth_json (dict[str, Any], optional): [description]. Defaults to {}.
 
         Returns:
             auth_details: [auth_details object]
         """
-        return auth_details(auth_json).upgrade_legacy(auth_json)
+        return AuthDetails(**auth_json).upgrade_legacy(auth_json)
 
     class ContentTypes:
         def __init__(self) -> None:
             class ArchivedTypes:
                 def __init__(self) -> None:
                     self.Posts = []
 
                 def __iter__(self):
                     for attr, value in self.__dict__.items():
                         yield attr, value
 
             self.Stories = []
             self.Posts = []
-            self.Archived = ArchivedTypes()
+            # self.Archived = ArchivedTypes()
             self.Chats = []
             self.Messages = []
             self.Highlights = []
             self.MassMessages = []
 
         def __iter__(self):
             for attr, value in self.__dict__.items():
                 yield attr, value
 
-        async def get_keys(self):
+        def get_keys(self):
             return [item[0] for item in self]
 
-    class Locations:
+        async def response_type_to_key(self, value:str):
+            result = [x[0] for x in self if x[0].lower() == f"{value}s"]
+            if result:
+                return result[0]
+
+    class MediaTypes:
         def __init__(self) -> None:
-            self.Images = ["photo", "image"]
+            self.Images = ["photo"]
             self.Videos = ["video", "stream", "gif"]
             self.Audios = ["audio"]
             self.Texts = ["text"]
 
-        async def get_keys(self):
+        def get_keys(self):
             return [item[0] for item in self.__dict__.items()]
+        def find_by_value(self,value:str):
+            final_media_type = None
+            for media_type, alt_media_types in self.__dict__.items():
+                if value in alt_media_types:
+                    final_media_type = media_type
+            if not final_media_type:
+                raise Exception("No media type found")
+            return final_media_type
```

### Comparing `ultima_scraper_api-0.1.4/ultima_scraper_api/apis/user_streamliner.py` & `ultima_scraper_api-1.0.0/ultima_scraper_api/apis/user_streamliner.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-0.1.4/ultima_scraper_api/classes/make_settings.py` & `ultima_scraper_api-1.0.0/ultima_scraper_api/classes/make_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import copy
 import uuid as uuid
 from pathlib import Path
 from typing import Any, Literal, Tuple, get_args
 
+import orjson
 from yarl import URL
 
 site_name_literals = Literal["OnlyFans", "Fansly"]
 site_names: Tuple[site_name_literals, ...] = get_args(site_name_literals)
 
 current_version = None
 
@@ -286,14 +287,18 @@
                     return self.onlyfans.settings
                 else:
                     return self.fansly.settings
 
         self.info = Info()
         self.settings = Settings(**settings)
         self.supported = Supported(**supported)
+    def import_json(self, file_path:Path):
+        with file_path.open(encoding="utf-8") as o_file:
+            json_file = orjson.loads(o_file.read())
+            return Config(**json_file)
 
     def export(self) -> Config:
         base = copy.deepcopy(self)
         for name in site_names:
             SS = base.supported.get_settings(site_name=name)
             for key, value in SS.__dict__.items():
                 match key:
@@ -303,8 +308,8 @@
                         SS.__dict__[key] = new_list
                     case "file_directory_format" | "filename_format" | "metadata_directory_format":
                         value_: Path = value
                         final_path = value_.as_posix()
                         SS.__dict__[key] = final_path
                     case _:
                         pass
-        return base
+        return base
```

### Comparing `ultima_scraper_api-0.1.4/ultima_scraper_api/classes/prepare_directories.py` & `ultima_scraper_api-1.0.0/ultima_scraper_api/classes/prepare_directories.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-0.1.4/ultima_scraper_api/classes/prepare_metadata.py` & `ultima_scraper_api-1.0.0/ultima_scraper_api/classes/prepare_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
         api_type: str = "",
     ) -> None:
         self.version = global_version
         fixed_metadata = self.fix_metadata(metadata, standard_format, api_type)
         self.content = format_content(
             fixed_metadata["version"], fixed_metadata["content"]
         ).content
+        pass
 
     def fix_metadata(
         self,
         metadata: dict[str, Any] | list[dict[str, Any]],
         standard_format: bool = False,
         api_type: str = "",
     ):
@@ -115,16 +116,14 @@
                         print
                 setattr(value, key2, old_status)
                 value2 = old_status
                 new_status = new_value2
                 for post in old_status:
                     if key != "Texts":
                         for old_media in post.medias:
-                            # if old_item.post_id == 1646808:
-                            #     l = True
                             new_found = None
                             new_items = [
                                 x for x in new_status if post.post_id == x.post_id
                             ]
                             if new_items:
                                 for new_item in (x for x in new_items if not new_found):
                                     for new_media in (
@@ -259,20 +258,20 @@
                     input("METADATA VERSION: INVALID")
                 setattr(new_item, old_key, new_posts)
         self.content = new_content
 
     class post_item(create_metadata, object):
         def __init__(self, option={}):
             # create_metadata.__init__(self, option)
-            self.post_id = option.get("post_id", None)
-            self.text = option.get("text", "")
-            self.price = option.get("price", 0)
+            self.post_id: int = option.get("post_id", None)
+            self.text: str = option.get("text", "")
+            self.price: float = option.get("price", 0)
             self.paid = option.get("paid", False)
             self.medias = option.get("medias", [])
-            self.postedAt = option.get("postedAt", "")
+            self.createdAt: str = option.get("createdAt", option.get("postedAt", ""))
 
     class media_item(create_metadata):
         def __init__(self, option={}):
             # create_metadata.__init__(self, option)
             self.media_id = option.get("media_id", None)
             link = option.get("link", [])
             if link:
@@ -315,16 +314,14 @@
         return new_wl
 
     def __iter__(self):
         for attr, value in self.__dict__.items():
             yield attr, value
 
 
-
-
 # Legacy .db and .json files
 # We'll just merge things together based on their api_type
 # create_metadata fixes metadata automatically
 async def legacy_metadata_fixer(
     new_metadata_filepath: Path, legacy_metadata_filepaths: list[Path]
 ) -> tuple[create_metadata, list[Path]]:
     delete_legacy_metadatas: list[Path] = []
```

### Comparing `ultima_scraper_api-0.1.4/ultima_scraper_api/classes/prepare_webhooks.py` & `ultima_scraper_api-1.0.0/ultima_scraper_api/classes/prepare_webhooks.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-0.1.4/ultima_scraper_api/docs/Makefile` & `ultima_scraper_api-1.0.0/ultima_scraper_api/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-0.1.4/ultima_scraper_api/docs/make.bat` & `ultima_scraper_api-1.0.0/ultima_scraper_api/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-0.1.4/ultima_scraper_api/docs/source/conf.py` & `ultima_scraper_api-1.0.0/ultima_scraper_api/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-0.1.4/ultima_scraper_api/helpers/main_helper.py` & `ultima_scraper_api-1.0.0/ultima_scraper_api/helpers/main_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,21 +7,20 @@
 import shutil
 import subprocess
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, BinaryIO, Literal
 
 import orjson
 import requests
-from aiofiles import os as async_os
-from bs4 import BeautifulSoup
-from mergedeep import Strategy, merge  # type: ignore
-
 import ultima_scraper_api
 import ultima_scraper_api.classes.make_settings as make_settings
 import ultima_scraper_api.classes.prepare_webhooks as prepare_webhooks
+from aiofiles import os as async_os
+from bs4 import BeautifulSoup
+from mergedeep import Strategy, merge  # type: ignore
 
 if TYPE_CHECKING:
     pass
 
 api_types = ultima_scraper_api.api_types
 auth_types = ultima_scraper_api.auth_types
 user_types = ultima_scraper_api.user_types
```

### Comparing `ultima_scraper_api-0.1.4/ultima_scraper_api/managers/job_manager/job_manager.py` & `ultima_scraper_api-1.0.0/ultima_scraper_api/managers/job_manager/job_manager.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-0.1.4/ultima_scraper_api/managers/job_manager/jobs/custom_job.py` & `ultima_scraper_api-1.0.0/ultima_scraper_api/managers/job_manager/jobs/custom_job.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,14 +10,15 @@
         self.api_type = api_type
         self.media_types: list[str] = []
         self.min = 0
         self.task = None
         self.result = []
         self.done = False
         self.options: list[str] = []
+        self.blacklist:list[str] = []
 
     def add_media_type(self, media_type: str):
         self.media_types.append(media_type)
 
     def convert_to_dill(self):
         old = copy.copy(self)
         delattr(old, "task")
```

### Comparing `ultima_scraper_api-0.1.4/ultima_scraper_api/managers/scrape_manager.py` & `ultima_scraper_api-1.0.0/ultima_scraper_api/managers/scrape_manager.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from ultima_scraper_api.managers.session_manager import SessionManager
 
 
 class ScrapeManager:
     def __init__(self, session_manager: SessionManager) -> None:
         self.session_manager = session_manager
         self.handle_errors = True
+        self.scraped = session_manager.auth.api.ContentTypes()
 
     async def bulk_scrape(self, urls: list[str]):
         result = await asyncio.gather(
             *[self.scrape(x) for x in urls], return_exceptions=True
         )
         final_result = list(chain(*result))
         return final_result
@@ -42,7 +43,14 @@
             else:
                 handle_error_ = fansly_classes.extras.ErrorDetails
 
             result = await handle_error_(json_res).format(extras)
             if self.handle_errors:
                 return await handle_error_details(result)
         return json_res
+
+    async def handle_refresh(self, item: Any):
+        abc = getattr(self.session_manager.auth, f"get_{item.responseType}")
+        return abc
+
+    def set_scraped(self, name: str, scraped: list[Any]):
+        setattr(self.scraped, name, scraped)
```

### Comparing `ultima_scraper_api-0.1.4/setup.py` & `ultima_scraper_api-1.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['ultima_scraper_api',
  'ultima_scraper_api.apis',
- 'ultima_scraper_api.apis.fanhouse',
- 'ultima_scraper_api.apis.fanhouse.classes',
- 'ultima_scraper_api.apis.fanhouse.decorators',
  'ultima_scraper_api.apis.fansly',
  'ultima_scraper_api.apis.fansly.classes',
  'ultima_scraper_api.apis.fansly.decorators',
  'ultima_scraper_api.apis.onlyfans',
  'ultima_scraper_api.apis.onlyfans.classes',
  'ultima_scraper_api.apis.onlyfans.decorators',
  'ultima_scraper_api.classes',
@@ -39,15 +36,15 @@
  'requests[socks]==2.28.2',
  'sphinx-autoapi>=2.0.0,<3.0.0',
  'sphinx-rtd-theme>=1.1.1,<2.0.0',
  'user-agent>=0.1.10,<0.2.0']
 
 setup_kwargs = {
     'name': 'ultima-scraper-api',
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

### Comparing `ultima_scraper_api-0.1.4/PKG-INFO` & `ultima_scraper_api-1.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultima-scraper-api
-Version: 0.1.4
+Version: 1.0.0
 Summary: 
 Author: DIGITALCRIMINALS
 Author-email: 89371864+digitalcriminals@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

