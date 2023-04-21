# Comparing `tmp/swibots-1.1.4.tar.gz` & `tmp/swibots-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swibots-1.1.4.tar", last modified: Mon Mar 20 17:20:10 2023, max compression
+gzip compressed data, was "swibots-1.1.5.tar", last modified: Fri Apr 21 00:44:43 2023, max compression
```

## Comparing `swibots-1.1.4.tar` & `swibots-1.1.5.tar`

### file list

```diff
@@ -1,218 +1,218 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 17:20:10.634280 swibots-1.1.4/
--rw-r--r--   0 root         (0) root         (0)     1817 2023-03-20 17:20:10.632608 swibots-1.1.4/PKG-INFO
--r---w----   0 root         (0) root         (0)     1538 2023-01-19 02:17:00.000000 swibots-1.1.4/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-20 17:20:10.635045 swibots-1.1.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      731 2023-03-20 16:59:00.000000 swibots-1.1.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 17:20:08.088720 swibots-1.1.4/swibots/
--rw-r--r--   0 root         (0) root         (0)      236 2023-01-16 12:19:14.000000 swibots-1.1.4/swibots/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 17:20:08.199994 swibots-1.1.4/swibots/api/
--rw-r--r--   0 root         (0) root         (0)      140 2023-01-16 06:31:11.000000 swibots-1.1.4/swibots/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2236 2023-01-21 06:26:21.000000 swibots-1.1.4/swibots/api/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 17:20:08.233162 swibots-1.1.4/swibots/api/auth/
--rw-r--r--   0 root         (0) root         (0)       85 2023-01-16 07:03:12.000000 swibots-1.1.4/swibots/api/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1220 2023-01-23 17:55:04.000000 swibots-1.1.4/swibots/api/auth/auth_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 17:20:08.256536 swibots-1.1.4/swibots/api/auth/controllers/
--rw-r--r--   0 root         (0) root         (0)       73 2023-01-09 05:33:14.000000 swibots-1.1.4/swibots/api/auth/controllers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1514 2023-02-04 19:02:18.000000 swibots-1.1.4/swibots/api/auth/controllers/user_controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 17:20:08.303174 swibots-1.1.4/swibots/api/auth/methods/
--rwxr-xr-x   0 root         (0) root         (0)       94 2023-02-04 19:02:18.000000 swibots-1.1.4/swibots/api/auth/methods/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      650 2023-02-04 19:02:18.000000 swibots-1.1.4/swibots/api/auth/methods/get_me.py
--rw-r--r--   0 root         (0) root         (0)      837 2023-02-04 19:02:18.000000 swibots-1.1.4/swibots/api/auth/methods/login.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 17:20:08.342275 swibots-1.1.4/swibots/api/auth/models/
--rw-r--r--   0 root         (0) root         (0)       56 2023-01-13 05:35:17.000000 swibots-1.1.4/swibots/api/auth/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4642 2023-01-19 01:21:52.000000 swibots-1.1.4/swibots/api/auth/models/auth_user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 17:20:08.391564 swibots-1.1.4/swibots/api/bot/
--rwxr-xr-x   0 root         (0) root         (0)       83 2023-01-16 06:01:42.000000 swibots-1.1.4/swibots/api/bot/__init__.py
--r---w----   0 root         (0) root         (0)     1141 2023-01-23 17:54:24.000000 swibots-1.1.4/swibots/api/bot/bot_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 17:20:08.424703 swibots-1.1.4/swibots/api/bot/controllers/
--r---w----   0 root         (0) root         (0)       71 2023-01-15 12:54:24.000000 swibots-1.1.4/swibots/api/bot/controllers/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     1790 2023-02-04 19:02:01.000000 swibots-1.1.4/swibots/api/bot/controllers/bot_controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 17:20:08.488588 swibots-1.1.4/swibots/api/bot/methods/
--rwxr-xr-x   0 root         (0) root         (0)      209 2023-02-04 19:02:01.000000 swibots-1.1.4/swibots/api/bot/methods/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      540 2023-02-04 19:02:01.000000 swibots-1.1.4/swibots/api/bot/methods/delete_bot_info.py
--rwxr-xr-x   0 root         (0) root         (0)      582 2023-02-04 19:02:01.000000 swibots-1.1.4/swibots/api/bot/methods/get_bot_info.py
--rwxr-xr-x   0 root         (0) root         (0)      615 2023-02-04 19:02:01.000000 swibots-1.1.4/swibots/api/bot/methods/update_bot_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 17:20:08.537199 swibots-1.1.4/swibots/api/bot/models/
--rwxr-xr-x   0 root         (0) root         (0)      116 2023-01-15 13:00:36.000000 swibots-1.1.4/swibots/api/bot/models/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      955 2023-01-19 01:21:52.000000 swibots-1.1.4/swibots/api/bot/models/bot_command_info.py
--rwxr-xr-x   0 root         (0) root         (0)     1585 2023-01-19 01:21:52.000000 swibots-1.1.4/swibots/api/bot/models/bot_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 17:20:08.577098 swibots-1.1.4/swibots/api/chat/
--rw-r--r--   0 root         (0) root         (0)      107 2023-01-16 06:01:20.000000 swibots-1.1.4/swibots/api/chat/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5372 2023-02-04 19:02:18.000000 swibots-1.1.4/swibots/api/chat/chat_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 17:20:08.596717 swibots-1.1.4/swibots/api/chat/controllers/
--rw-r--r--   0 root         (0) root         (0)       83 2023-01-15 12:53:45.000000 swibots-1.1.4/swibots/api/chat/controllers/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    21518 2023-02-08 08:21:26.000000 swibots-1.1.4/swibots/api/chat/controllers/message_controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 17:20:08.683181 swibots-1.1.4/swibots/api/chat/events/
--rwxr-xr-x   0 root         (0) root         (0)      326 2023-02-04 19:02:18.000000 swibots-1.1.4/swibots/api/chat/events/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     2073 2023-02-06 20:56:35.000000 swibots-1.1.4/swibots/api/chat/events/callback_query_event.py
--rwxr-xr-x   0 root         (0) root         (0)     2731 2023-02-04 19:02:18.000000 swibots-1.1.4/swibots/api/chat/events/chat_event.py
--rwxr-xr-x   0 root         (0) root         (0)     2095 2023-02-04 19:02:18.000000 swibots-1.1.4/swibots/api/chat/events/command_event.py
--rwxr-xr-x   0 root         (0) root         (0)     2103 2023-02-04 19:02:18.000000 swibots-1.1.4/swibots/api/chat/events/inline_query_event.py
--rwxr-xr-x   0 root         (0) root         (0)     2434 2023-02-06 21:23:12.000000 swibots-1.1.4/swibots/api/chat/events/message_event.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 17:20:09.005109 swibots-1.1.4/swibots/api/chat/methods/
--rwxr-xr-x   0 root         (0) root         (0)     1709 2023-02-04 19:02:18.000000 swibots-1.1.4/swibots/api/chat/methods/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      654 2023-02-04 19:02:18.000000 swibots-1.1.4/swibots/api/chat/methods/answer_inline_query.py
--rwxr-xr-x   0 root         (0) root         (0)      693 2023-01-19 01:21:52.000000 swibots-1.1.4/swibots/api/chat/methods/clear_conversation.py
--rwxr-xr-x   0 root         (0) root         (0)      705 2023-02-04 19:02:01.000000 swibots-1.1.4/swibots/api/chat/methods/delete_message.py
--rwxr-xr-x   0 root         (0) root         (0)      707 2023-02-04 19:02:01.000000 swibots-1.1.4/swibots/api/chat/methods/delete_messages_from_user.py
--rwxr-xr-x   0 root         (0) root         (0)     1358 2023-02-04 19:02:18.000000 swibots-1.1.4/swibots/api/chat/methods/download_media.py
--rwxr-xr-x   0 root         (0) root         (0)      750 2023-02-04 19:02:18.000000 swibots-1.1.4/swibots/api/chat/methods/edit_message.py
--rwxr-xr-x   0 root         (0) root         (0)      853 2023-02-04 19:02:18.000000 swibots-1.1.4/swibots/api/chat/methods/edit_message_text.py
--rwxr-xr-x   0 root         (0) root         (0)      693 2023-02-04 19:02:01.000000 swibots-1.1.4/swibots/api/chat/methods/flag_message.py
--rwxr-xr-x   0 root         (0) root         (0)     1192 2023-02-04 19:02:18.000000 swibots-1.1.4/swibots/api/chat/methods/forward_message.py
--rwxr-xr-x   0 root         (0) root         (0)     1139 2023-02-04 19:02:01.000000 swibots-1.1.4/swibots/api/chat/methods/get_channel_chat_history.py
--rwxr-xr-x   0 root         (0) root         (0)      725 2023-01-19 01:21:52.000000 swibots-1.1.4/swibots/api/chat/methods/get_community_media_files.py
--rwxr-xr-x   0 root         (0) root         (0)      883 2023-02-04 19:02:01.000000 swibots-1.1.4/swibots/api/chat/methods/get_community_media_files_by_status.py
--rwxr-xr-x   0 root         (0) root         (0)      636 2023-01-19 01:21:52.000000 swibots-1.1.4/swibots/api/chat/methods/get_flag_messages.py
--rwxr-xr-x   0 root         (0) root         (0)     1090 2023-02-04 19:02:01.000000 swibots-1.1.4/swibots/api/chat/methods/get_group_chat_history.py
--rwxr-xr-x   0 root         (0) root         (0)      649 2023-02-04 19:02:01.000000 swibots-1.1.4/swibots/api/chat/methods/get_message.py
--rwxr-xr-x   0 root         (0) root         (0)      707 2023-02-04 19:02:01.000000 swibots-1.1.4/swibots/api/chat/methods/get_messages.py
--rwxr-xr-x   0 root         (0) root         (0)     1102 2023-02-04 19:02:01.000000 swibots-1.1.4/swibots/api/chat/methods/get_messages_between_users.py
--rwxr-xr-x   0 root         (0) root         (0)      560 2023-02-04 19:02:18.000000 swibots-1.1.4/swibots/api/chat/methods/get_unread_messages_count.py
--rwxr-xr-x   0 root         (0) root         (0)      785 2023-02-04 19:02:01.000000 swibots-1.1.4/swibots/api/chat/methods/get_user_media_files.py
--rwxr-xr-x   0 root         (0) root         (0)      881 2023-02-08 08:22:32.000000 swibots-1.1.4/swibots/api/chat/methods/reply_message.py
--rwxr-xr-x   0 root         (0) root         (0)     1032 2023-02-08 08:20:23.000000 swibots-1.1.4/swibots/api/chat/methods/reply_message_text.py
--rwxr-xr-x   0 root         (0) root         (0)      849 2023-02-08 08:19:39.000000 swibots-1.1.4/swibots/api/chat/methods/send_message.py
--rwxr-xr-x   0 root         (0) root         (0)     1136 2023-02-04 19:02:18.000000 swibots-1.1.4/swibots/api/chat/methods/send_text.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 17:20:09.174193 swibots-1.1.4/swibots/api/chat/models/
--rw-r--r--   0 root         (0) root         (0)      305 2023-02-04 19:02:18.000000 swibots-1.1.4/swibots/api/chat/models/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      920 2023-02-06 20:55:52.000000 swibots-1.1.4/swibots/api/chat/models/group_chat_history.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 17:20:09.314560 swibots-1.1.4/swibots/api/chat/models/inline/
--rwxr-xr-x   0 root         (0) root         (0)      565 2023-02-04 19:02:18.000000 swibots-1.1.4/swibots/api/chat/models/inline/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     1371 2023-02-04 19:02:18.000000 swibots-1.1.4/swibots/api/chat/models/inline/base_typed_inline_query_result.py
--rwxr-xr-x   0 root         (0) root         (0)     2533 2023-02-04 19:02:18.000000 swibots-1.1.4/swibots/api/chat/models/inline/inline_query.py
--rwxr-xr-x   0 root         (0) root         (0)     1871 2023-02-04 19:02:18.000000 swibots-1.1.4/swibots/api/chat/models/inline/inline_query_answer.py
--rwxr-xr-x   0 root         (0) root         (0)      991 2023-02-04 19:02:18.000000 swibots-1.1.4/swibots/api/chat/models/inline/inline_query_result.py
--rwxr-xr-x   0 root         (0) root         (0)     1158 2023-02-04 19:02:18.000000 swibots-1.1.4/swibots/api/chat/models/inline/inline_query_result_article.py
--rw-r--r--   0 root         (0) root         (0)     1273 2023-02-04 19:02:18.000000 swibots-1.1.4/swibots/api/chat/models/inline/inline_query_result_document.py
--rw-r--r--   0 root         (0) root         (0)     1620 2023-02-04 19:02:18.000000 swibots-1.1.4/swibots/api/chat/models/inline/inline_query_result_photo.py
--rw-r--r--   0 root         (0) root         (0)     1760 2023-02-04 19:02:18.000000 swibots-1.1.4/swibots/api/chat/models/inline/inline_query_result_video.py
--rwxr-xr-x   0 root         (0) root         (0)      581 2023-02-04 19:02:18.000000 swibots-1.1.4/swibots/api/chat/models/inline/input_message_content.py
--rwxr-xr-x   0 root         (0) root         (0)      201 2023-02-04 19:02:18.000000 swibots-1.1.4/swibots/api/chat/models/inline/types.py
--rwxr-xr-x   0 root         (0) root         (0)      886 2023-02-08 07:21:24.000000 swibots-1.1.4/swibots/api/chat/models/inline_keyboard_button.py
--rwxr-xr-x   0 root         (0) root         (0)      170 2023-01-18 20:49:52.000000 swibots-1.1.4/swibots/api/chat/models/inline_keyboard_color.py
--rwxr-xr-x   0 root         (0) root         (0)      146 2023-02-04 19:02:01.000000 swibots-1.1.4/swibots/api/chat/models/inline_keyboard_size.py
--rwxr-xr-x   0 root         (0) root         (0)     2065 2023-02-08 07:22:42.000000 swibots-1.1.4/swibots/api/chat/models/inline_markup.py
--rw-r--r--   0 root         (0) root         (0)    10769 2023-02-08 09:10:55.000000 swibots-1.1.4/swibots/api/chat/models/message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 17:20:09.322976 swibots-1.1.4/swibots/api/common/
--rwxr-xr-x   0 root         (0) root         (0)       44 2023-01-16 06:01:00.000000 swibots-1.1.4/swibots/api/common/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 17:20:09.350256 swibots-1.1.4/swibots/api/common/events/
--rwxr-xr-x   0 root         (0) root         (0)       46 2023-01-13 06:20:04.000000 swibots-1.1.4/swibots/api/common/events/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     2789 2023-01-23 19:39:48.000000 swibots-1.1.4/swibots/api/common/events/event.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 17:20:09.397805 swibots-1.1.4/swibots/api/common/models/
--rwxr-xr-x   0 root         (0) root         (0)      101 2023-02-06 20:55:52.000000 swibots-1.1.4/swibots/api/common/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2004 2023-02-07 07:11:30.000000 swibots-1.1.4/swibots/api/common/models/media.py
--rwxr-xr-x   0 root         (0) root         (0)     1565 2023-02-04 19:02:18.000000 swibots-1.1.4/swibots/api/common/models/media_upload_request.py
--rwxr-xr-x   0 root         (0) root         (0)     1706 2023-02-04 19:02:18.000000 swibots-1.1.4/swibots/api/common/models/user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 17:20:09.426152 swibots-1.1.4/swibots/api/community/
--rwxr-xr-x   0 root         (0) root         (0)       90 2023-01-16 06:00:40.000000 swibots-1.1.4/swibots/api/community/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5059 2023-03-20 17:15:06.000000 swibots-1.1.4/swibots/api/community/community_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 17:20:09.469598 swibots-1.1.4/swibots/api/community/controllers/
--rw-r--r--   0 root         (0) root         (0)      102 2023-02-06 20:55:52.000000 swibots-1.1.4/swibots/api/community/controllers/__init__.py
--rw-r--r--   0 root         (0) root         (0)      595 2023-02-06 20:55:52.000000 swibots-1.1.4/swibots/api/community/controllers/channel_controller.py
--rwxr-xr-x   0 root         (0) root         (0)      616 2023-02-06 20:55:52.000000 swibots-1.1.4/swibots/api/community/controllers/community_controller.py
--rw-r--r--   0 root         (0) root         (0)      576 2023-02-06 20:55:52.000000 swibots-1.1.4/swibots/api/community/controllers/group_controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 17:20:09.629922 swibots-1.1.4/swibots/api/community/events/
--rwxr-xr-x   0 root         (0) root         (0)      566 2023-01-16 23:20:36.000000 swibots-1.1.4/swibots/api/community/events/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     1387 2023-03-20 17:12:26.000000 swibots-1.1.4/swibots/api/community/events/channel_created_event.py
--rwxr-xr-x   0 root         (0) root         (0)     1387 2023-03-20 17:12:56.000000 swibots-1.1.4/swibots/api/community/events/channel_deleted_event.py
--rwxr-xr-x   0 root         (0) root         (0)     1387 2023-03-20 17:12:44.000000 swibots-1.1.4/swibots/api/community/events/channel_updated_event.py
--rwxr-xr-x   0 root         (0) root         (0)     2303 2023-01-23 19:25:02.000000 swibots-1.1.4/swibots/api/community/events/community_event.py
--rwxr-xr-x   0 root         (0) root         (0)     1383 2023-02-04 19:02:01.000000 swibots-1.1.4/swibots/api/community/events/community_updated_event.py
--rwxr-xr-x   0 root         (0) root         (0)     1381 2023-03-20 17:13:37.000000 swibots-1.1.4/swibots/api/community/events/group_created_event.py
--rwxr-xr-x   0 root         (0) root         (0)     1381 2023-03-20 17:14:02.000000 swibots-1.1.4/swibots/api/community/events/group_deleted_event.py
--rwxr-xr-x   0 root         (0) root         (0)     1381 2023-03-20 17:13:49.000000 swibots-1.1.4/swibots/api/community/events/group_updated_event.py
--rwxr-xr-x   0 root         (0) root         (0)     1380 2023-03-20 17:14:48.000000 swibots-1.1.4/swibots/api/community/events/member_joined_event.py
--rwxr-xr-x   0 root         (0) root         (0)     1377 2023-03-20 17:15:06.000000 swibots-1.1.4/swibots/api/community/events/member_left_event.py
--rwxr-xr-x   0 root         (0) root         (0)     1373 2023-03-20 17:14:14.000000 swibots-1.1.4/swibots/api/community/events/user_banned_event.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 17:20:09.681973 swibots-1.1.4/swibots/api/community/methods/
--rwxr-xr-x   0 root         (0) root         (0)      194 2023-02-04 19:02:18.000000 swibots-1.1.4/swibots/api/community/methods/__init__.py
--rw-r--r--   0 root         (0) root         (0)      643 2023-02-06 20:55:52.000000 swibots-1.1.4/swibots/api/community/methods/get_channel.py
--rwxr-xr-x   0 root         (0) root         (0)      668 2023-02-04 19:02:18.000000 swibots-1.1.4/swibots/api/community/methods/get_community.py
--rw-r--r--   0 root         (0) root         (0)      619 2023-02-06 20:55:52.000000 swibots-1.1.4/swibots/api/community/methods/get_group.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 17:20:09.733604 swibots-1.1.4/swibots/api/community/models/
--rwxr-xr-x   0 root         (0) root         (0)      132 2023-01-13 05:39:45.000000 swibots-1.1.4/swibots/api/community/models/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     2743 2023-02-04 19:02:01.000000 swibots-1.1.4/swibots/api/community/models/channel.py
--rwxr-xr-x   0 root         (0) root         (0)     2954 2023-01-21 07:06:56.000000 swibots-1.1.4/swibots/api/community/models/community.py
--rwxr-xr-x   0 root         (0) root         (0)     2720 2023-01-21 07:07:04.000000 swibots-1.1.4/swibots/api/community/models/group.py
--rwxr-xr-x   0 root         (0) root         (0)     9347 2023-02-04 19:02:18.000000 swibots-1.1.4/swibots/app.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 17:20:09.834493 swibots-1.1.4/swibots/base/
--rw-r--r--   0 root         (0) root         (0)      262 2023-01-16 05:59:47.000000 swibots-1.1.4/swibots/base/__init__.py
--rw-r--r--   0 root         (0) root         (0)       69 2023-01-09 05:33:14.000000 swibots-1.1.4/swibots/base/rest_controller.py
--rw-r--r--   0 root         (0) root         (0)      370 2023-01-19 01:21:52.000000 swibots-1.1.4/swibots/base/rest_request.py
--rw-r--r--   0 root         (0) root         (0)      644 2023-01-19 01:21:52.000000 swibots-1.1.4/swibots/base/rest_response.py
--rw-r--r--   0 root         (0) root         (0)     4261 2023-02-06 20:55:52.000000 swibots-1.1.4/swibots/base/switch_client.py
--rw-r--r--   0 root         (0) root         (0)     1180 2023-01-21 06:58:45.000000 swibots-1.1.4/swibots/base/switch_object.py
--rwxr-xr-x   0 root         (0) root         (0)      543 2023-01-19 01:21:52.000000 swibots-1.1.4/swibots/base/switch_ws_async_client.py
--rwxr-xr-x   0 root         (0) root         (0)     4329 2023-02-04 19:02:18.000000 swibots-1.1.4/swibots/bot_app.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 17:20:09.901160 swibots-1.1.4/swibots/bots/
--rwxr-xr-x   0 root         (0) root         (0)      201 2023-01-17 03:43:24.000000 swibots-1.1.4/swibots/bots/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     4646 2023-02-06 20:55:52.000000 swibots-1.1.4/swibots/bots/bot.py
--rwxr-xr-x   0 root         (0) root         (0)     1646 2023-01-19 01:21:52.000000 swibots-1.1.4/swibots/bots/bot_context.py
--rwxr-xr-x   0 root         (0) root         (0)      109 2023-01-14 17:55:20.000000 swibots-1.1.4/swibots/bots/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 17:20:10.144074 swibots-1.1.4/swibots/bots/decorators/
--rwxr-xr-x   0 root         (0) root         (0)      999 2023-02-04 19:02:18.000000 swibots-1.1.4/swibots/bots/decorators/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      540 2023-01-19 01:21:52.000000 swibots-1.1.4/swibots/bots/decorators/on_callback_query.py
--rwxr-xr-x   0 root         (0) root         (0)      510 2023-02-04 19:02:01.000000 swibots-1.1.4/swibots/bots/decorators/on_channel_created.py
--rwxr-xr-x   0 root         (0) root         (0)      544 2023-02-04 19:02:01.000000 swibots-1.1.4/swibots/bots/decorators/on_channel_deleted.py
--rwxr-xr-x   0 root         (0) root         (0)      541 2023-02-04 19:02:01.000000 swibots-1.1.4/swibots/bots/decorators/on_channel_updated.py
--rwxr-xr-x   0 root         (0) root         (0)      574 2023-01-19 01:21:52.000000 swibots-1.1.4/swibots/bots/decorators/on_command.py
--rwxr-xr-x   0 root         (0) root         (0)      544 2023-02-04 19:02:01.000000 swibots-1.1.4/swibots/bots/decorators/on_community_updated.py
--rwxr-xr-x   0 root         (0) root         (0)      536 2023-02-04 19:02:01.000000 swibots-1.1.4/swibots/bots/decorators/on_group_created.py
--rwxr-xr-x   0 root         (0) root         (0)      536 2023-02-04 19:02:01.000000 swibots-1.1.4/swibots/bots/decorators/on_group_deleted.py
--rwxr-xr-x   0 root         (0) root         (0)      534 2023-02-04 19:02:01.000000 swibots-1.1.4/swibots/bots/decorators/on_group_updated.py
--rw-r--r--   0 root         (0) root         (0)      537 2023-02-04 19:02:18.000000 swibots-1.1.4/swibots/bots/decorators/on_inline_query.py
--rwxr-xr-x   0 root         (0) root         (0)      534 2023-02-04 19:02:01.000000 swibots-1.1.4/swibots/bots/decorators/on_member_joined.py
--rwxr-xr-x   0 root         (0) root         (0)      529 2023-02-04 19:02:01.000000 swibots-1.1.4/swibots/bots/decorators/on_member_left.py
--rwxr-xr-x   0 root         (0) root         (0)      503 2023-01-19 01:21:52.000000 swibots-1.1.4/swibots/bots/decorators/on_message.py
--rwxr-xr-x   0 root         (0) root         (0)      543 2023-01-19 01:21:52.000000 swibots-1.1.4/swibots/bots/decorators/on_unknown_command.py
--rwxr-xr-x   0 root         (0) root         (0)      509 2023-02-04 19:02:01.000000 swibots-1.1.4/swibots/bots/decorators/on_user_banned.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 17:20:10.178674 swibots-1.1.4/swibots/bots/filters/
--rwxr-xr-x   0 root         (0) root         (0)       22 2023-01-16 03:25:36.000000 swibots-1.1.4/swibots/bots/filters/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     7703 2023-02-10 23:07:32.000000 swibots-1.1.4/swibots/bots/filters/filter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 17:20:10.400801 swibots-1.1.4/swibots/bots/handlers/
--rwxr-xr-x   0 root         (0) root         (0)     1300 2023-02-04 19:02:18.000000 swibots-1.1.4/swibots/bots/handlers/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     1048 2023-01-19 01:21:52.000000 swibots-1.1.4/swibots/bots/handlers/base_handler.py
--rwxr-xr-x   0 root         (0) root         (0)      985 2023-02-04 19:02:01.000000 swibots-1.1.4/swibots/bots/handlers/callback_query_handler.py
--rwxr-xr-x   0 root         (0) root         (0)      681 2023-03-20 17:12:26.000000 swibots-1.1.4/swibots/bots/handlers/channel_created_handler.py
--rwxr-xr-x   0 root         (0) root         (0)      688 2023-03-20 17:12:57.000000 swibots-1.1.4/swibots/bots/handlers/channel_deleted_handler.py
--rwxr-xr-x   0 root         (0) root         (0)      734 2023-03-20 17:12:44.000000 swibots-1.1.4/swibots/bots/handlers/channel_updated_handler.py
--rwxr-xr-x   0 root         (0) root         (0)     1514 2023-01-19 01:21:52.000000 swibots-1.1.4/swibots/bots/handlers/command_handler.py
--rwxr-xr-x   0 root         (0) root         (0)      686 2023-01-19 01:21:52.000000 swibots-1.1.4/swibots/bots/handlers/community_updated_handler.py
--rwxr-xr-x   0 root         (0) root         (0)     1325 2023-02-04 19:02:01.000000 swibots-1.1.4/swibots/bots/handlers/event_handler.py
--rwxr-xr-x   0 root         (0) root         (0)      680 2023-03-20 17:13:37.000000 swibots-1.1.4/swibots/bots/handlers/group_created_handler.py
--rwxr-xr-x   0 root         (0) root         (0)      775 2023-03-20 17:14:02.000000 swibots-1.1.4/swibots/bots/handlers/group_deleted_handler.py
--rwxr-xr-x   0 root         (0) root         (0)      775 2023-03-20 17:13:49.000000 swibots-1.1.4/swibots/bots/handlers/group_updated_handler.py
--rw-r--r--   0 root         (0) root         (0)      867 2023-02-04 19:02:18.000000 swibots-1.1.4/swibots/bots/handlers/inline_query_handler.py
--rwxr-xr-x   0 root         (0) root         (0)      679 2023-03-20 17:14:48.000000 swibots-1.1.4/swibots/bots/handlers/member_joined_handler.py
--rwxr-xr-x   0 root         (0) root         (0)      674 2023-03-20 17:15:07.000000 swibots-1.1.4/swibots/bots/handlers/member_left_handler.py
--rwxr-xr-x   0 root         (0) root         (0)      960 2023-02-04 19:02:01.000000 swibots-1.1.4/swibots/bots/handlers/message_handler.py
--rwxr-xr-x   0 root         (0) root         (0)      885 2023-01-19 01:21:52.000000 swibots-1.1.4/swibots/bots/handlers/unknown_command_handler.py
--rwxr-xr-x   0 root         (0) root         (0)      670 2023-03-20 17:14:14.000000 swibots-1.1.4/swibots/bots/handlers/user_banned_handler.py
--rwxr-xr-x   0 root         (0) root         (0)      285 2023-01-23 21:16:29.000000 swibots-1.1.4/swibots/bots/register_command.py
--rwxr-xr-x   0 root         (0) root         (0)     1589 2023-01-23 17:48:03.000000 swibots-1.1.4/swibots/config.py
--rw-r--r--   0 root         (0) root         (0)     1333 2023-02-04 19:02:18.000000 swibots-1.1.4/swibots/error.py
--rwxr-xr-x   0 root         (0) root         (0)      854 2023-03-20 17:15:29.000000 swibots-1.1.4/swibots/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 17:20:10.449309 swibots-1.1.4/swibots/utils/
--rw-r--r--   0 root         (0) root         (0)       75 2023-01-16 05:53:47.000000 swibots-1.1.4/swibots/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5880 2023-02-04 19:02:18.000000 swibots-1.1.4/swibots/utils/rest_client.py
--rw-r--r--   0 root         (0) root         (0)     2475 2023-02-04 19:02:18.000000 swibots-1.1.4/swibots/utils/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 17:20:10.479736 swibots-1.1.4/swibots/utils/ws/
--rw-r--r--   0 root         (0) root         (0)       48 2023-01-19 05:23:27.000000 swibots-1.1.4/swibots/utils/ws/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 17:20:10.532679 swibots-1.1.4/swibots/utils/ws/asyncstomp/
--rw-r--r--   0 root         (0) root         (0)      150 2023-01-09 05:33:14.000000 swibots-1.1.4/swibots/utils/ws/asyncstomp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9743 2023-01-21 06:34:39.000000 swibots-1.1.4/swibots/utils/ws/asyncstomp/async_ws_client.py
--rw-r--r--   0 root         (0) root         (0)      980 2023-01-19 01:21:52.000000 swibots-1.1.4/swibots/utils/ws/asyncstomp/async_ws_subscription.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 17:20:10.586196 swibots-1.1.4/swibots/utils/ws/common/
--rw-r--r--   0 root         (0) root         (0)      100 2023-01-09 05:33:14.000000 swibots-1.1.4/swibots/utils/ws/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1654 2023-01-09 05:33:14.000000 swibots-1.1.4/swibots/utils/ws/common/ws_frame.py
--rw-r--r--   0 root         (0) root         (0)      430 2023-01-09 05:33:14.000000 swibots-1.1.4/swibots/utils/ws/common/ws_message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 17:20:08.153648 swibots-1.1.4/swibots.egg-info/
--rwxr-xr-x   0 root         (0) root         (0)     1817 2023-03-20 17:20:07.000000 swibots-1.1.4/swibots.egg-info/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)     7316 2023-03-20 17:20:07.000000 swibots-1.1.4/swibots.egg-info/SOURCES.txt
--rwxr-xr-x   0 root         (0) root         (0)        1 2023-03-20 17:20:07.000000 swibots-1.1.4/swibots.egg-info/dependency_links.txt
--rwxr-xr-x   0 root         (0) root         (0)       31 2023-03-20 17:20:07.000000 swibots-1.1.4/swibots.egg-info/requires.txt
--rwxr-xr-x   0 root         (0) root         (0)       14 2023-03-20 17:20:07.000000 swibots-1.1.4/swibots.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 17:20:10.603369 swibots-1.1.4/tests/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 05:56:05.000000 swibots-1.1.4/tests/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      202 2023-01-15 22:26:25.000000 swibots-1.1.4/tests/tests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:44:43.321254 swibots-1.1.5/
+-rw-r--r--   0 root         (0) root         (0)     1817 2023-04-21 00:44:43.317507 swibots-1.1.5/PKG-INFO
+-r---w----   0 root         (0) root         (0)     1538 2023-01-19 02:17:00.000000 swibots-1.1.5/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-21 00:44:43.322785 swibots-1.1.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      731 2023-04-21 00:44:17.000000 swibots-1.1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:44:40.574046 swibots-1.1.5/swibots/
+-rw-r--r--   0 root         (0) root         (0)      236 2023-01-16 12:19:14.000000 swibots-1.1.5/swibots/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:44:40.652274 swibots-1.1.5/swibots/api/
+-rw-r--r--   0 root         (0) root         (0)      140 2023-01-16 06:31:11.000000 swibots-1.1.5/swibots/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2236 2023-01-21 06:26:21.000000 swibots-1.1.5/swibots/api/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:44:40.675828 swibots-1.1.5/swibots/api/auth/
+-rw-r--r--   0 root         (0) root         (0)       85 2023-01-16 07:03:12.000000 swibots-1.1.5/swibots/api/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1220 2023-01-23 17:55:04.000000 swibots-1.1.5/swibots/api/auth/auth_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:44:40.702730 swibots-1.1.5/swibots/api/auth/controllers/
+-rw-r--r--   0 root         (0) root         (0)       73 2023-01-09 05:33:14.000000 swibots-1.1.5/swibots/api/auth/controllers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1514 2023-02-04 19:02:18.000000 swibots-1.1.5/swibots/api/auth/controllers/user_controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:44:40.736364 swibots-1.1.5/swibots/api/auth/methods/
+-rwxr-xr-x   0 root         (0) root         (0)       94 2023-02-04 19:02:18.000000 swibots-1.1.5/swibots/api/auth/methods/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      650 2023-02-04 19:02:18.000000 swibots-1.1.5/swibots/api/auth/methods/get_me.py
+-rw-r--r--   0 root         (0) root         (0)      837 2023-02-04 19:02:18.000000 swibots-1.1.5/swibots/api/auth/methods/login.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:44:40.756860 swibots-1.1.5/swibots/api/auth/models/
+-rw-r--r--   0 root         (0) root         (0)       56 2023-01-13 05:35:17.000000 swibots-1.1.5/swibots/api/auth/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4642 2023-01-19 01:21:52.000000 swibots-1.1.5/swibots/api/auth/models/auth_user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:44:40.778229 swibots-1.1.5/swibots/api/bot/
+-rwxr-xr-x   0 root         (0) root         (0)       83 2023-01-16 06:01:42.000000 swibots-1.1.5/swibots/api/bot/__init__.py
+-r---w----   0 root         (0) root         (0)     1141 2023-01-23 17:54:24.000000 swibots-1.1.5/swibots/api/bot/bot_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:44:40.802151 swibots-1.1.5/swibots/api/bot/controllers/
+-r---w----   0 root         (0) root         (0)       71 2023-01-15 12:54:24.000000 swibots-1.1.5/swibots/api/bot/controllers/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     1790 2023-02-04 19:02:01.000000 swibots-1.1.5/swibots/api/bot/controllers/bot_controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:44:40.911836 swibots-1.1.5/swibots/api/bot/methods/
+-rwxr-xr-x   0 root         (0) root         (0)      209 2023-02-04 19:02:01.000000 swibots-1.1.5/swibots/api/bot/methods/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      540 2023-02-04 19:02:01.000000 swibots-1.1.5/swibots/api/bot/methods/delete_bot_info.py
+-rwxr-xr-x   0 root         (0) root         (0)      582 2023-02-04 19:02:01.000000 swibots-1.1.5/swibots/api/bot/methods/get_bot_info.py
+-rwxr-xr-x   0 root         (0) root         (0)      615 2023-02-04 19:02:01.000000 swibots-1.1.5/swibots/api/bot/methods/update_bot_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:44:40.971965 swibots-1.1.5/swibots/api/bot/models/
+-rwxr-xr-x   0 root         (0) root         (0)      116 2023-01-15 13:00:36.000000 swibots-1.1.5/swibots/api/bot/models/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      955 2023-01-19 01:21:52.000000 swibots-1.1.5/swibots/api/bot/models/bot_command_info.py
+-rwxr-xr-x   0 root         (0) root         (0)     1585 2023-01-19 01:21:52.000000 swibots-1.1.5/swibots/api/bot/models/bot_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:44:41.034271 swibots-1.1.5/swibots/api/chat/
+-rw-r--r--   0 root         (0) root         (0)      107 2023-01-16 06:01:20.000000 swibots-1.1.5/swibots/api/chat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5372 2023-02-04 19:02:18.000000 swibots-1.1.5/swibots/api/chat/chat_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:44:41.090045 swibots-1.1.5/swibots/api/chat/controllers/
+-rw-r--r--   0 root         (0) root         (0)       83 2023-01-15 12:53:45.000000 swibots-1.1.5/swibots/api/chat/controllers/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    21518 2023-02-08 08:21:26.000000 swibots-1.1.5/swibots/api/chat/controllers/message_controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:44:41.173209 swibots-1.1.5/swibots/api/chat/events/
+-rwxr-xr-x   0 root         (0) root         (0)      326 2023-02-04 19:02:18.000000 swibots-1.1.5/swibots/api/chat/events/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     2073 2023-02-06 20:56:35.000000 swibots-1.1.5/swibots/api/chat/events/callback_query_event.py
+-rwxr-xr-x   0 root         (0) root         (0)     2731 2023-02-04 19:02:18.000000 swibots-1.1.5/swibots/api/chat/events/chat_event.py
+-rwxr-xr-x   0 root         (0) root         (0)     2095 2023-02-04 19:02:18.000000 swibots-1.1.5/swibots/api/chat/events/command_event.py
+-rwxr-xr-x   0 root         (0) root         (0)     2103 2023-02-04 19:02:18.000000 swibots-1.1.5/swibots/api/chat/events/inline_query_event.py
+-rwxr-xr-x   0 root         (0) root         (0)     2434 2023-02-06 21:23:12.000000 swibots-1.1.5/swibots/api/chat/events/message_event.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:44:41.577514 swibots-1.1.5/swibots/api/chat/methods/
+-rwxr-xr-x   0 root         (0) root         (0)     1709 2023-02-04 19:02:18.000000 swibots-1.1.5/swibots/api/chat/methods/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      654 2023-02-04 19:02:18.000000 swibots-1.1.5/swibots/api/chat/methods/answer_inline_query.py
+-rwxr-xr-x   0 root         (0) root         (0)      693 2023-01-19 01:21:52.000000 swibots-1.1.5/swibots/api/chat/methods/clear_conversation.py
+-rwxr-xr-x   0 root         (0) root         (0)      705 2023-02-04 19:02:01.000000 swibots-1.1.5/swibots/api/chat/methods/delete_message.py
+-rwxr-xr-x   0 root         (0) root         (0)      707 2023-02-04 19:02:01.000000 swibots-1.1.5/swibots/api/chat/methods/delete_messages_from_user.py
+-rwxr-xr-x   0 root         (0) root         (0)     1358 2023-02-04 19:02:18.000000 swibots-1.1.5/swibots/api/chat/methods/download_media.py
+-rwxr-xr-x   0 root         (0) root         (0)      750 2023-02-04 19:02:18.000000 swibots-1.1.5/swibots/api/chat/methods/edit_message.py
+-rwxr-xr-x   0 root         (0) root         (0)      853 2023-02-04 19:02:18.000000 swibots-1.1.5/swibots/api/chat/methods/edit_message_text.py
+-rwxr-xr-x   0 root         (0) root         (0)      693 2023-02-04 19:02:01.000000 swibots-1.1.5/swibots/api/chat/methods/flag_message.py
+-rwxr-xr-x   0 root         (0) root         (0)     1192 2023-02-04 19:02:18.000000 swibots-1.1.5/swibots/api/chat/methods/forward_message.py
+-rwxr-xr-x   0 root         (0) root         (0)     1139 2023-02-04 19:02:01.000000 swibots-1.1.5/swibots/api/chat/methods/get_channel_chat_history.py
+-rwxr-xr-x   0 root         (0) root         (0)      725 2023-01-19 01:21:52.000000 swibots-1.1.5/swibots/api/chat/methods/get_community_media_files.py
+-rwxr-xr-x   0 root         (0) root         (0)      883 2023-02-04 19:02:01.000000 swibots-1.1.5/swibots/api/chat/methods/get_community_media_files_by_status.py
+-rwxr-xr-x   0 root         (0) root         (0)      636 2023-01-19 01:21:52.000000 swibots-1.1.5/swibots/api/chat/methods/get_flag_messages.py
+-rwxr-xr-x   0 root         (0) root         (0)     1090 2023-02-04 19:02:01.000000 swibots-1.1.5/swibots/api/chat/methods/get_group_chat_history.py
+-rwxr-xr-x   0 root         (0) root         (0)      649 2023-02-04 19:02:01.000000 swibots-1.1.5/swibots/api/chat/methods/get_message.py
+-rwxr-xr-x   0 root         (0) root         (0)      707 2023-02-04 19:02:01.000000 swibots-1.1.5/swibots/api/chat/methods/get_messages.py
+-rwxr-xr-x   0 root         (0) root         (0)     1102 2023-02-04 19:02:01.000000 swibots-1.1.5/swibots/api/chat/methods/get_messages_between_users.py
+-rwxr-xr-x   0 root         (0) root         (0)      560 2023-02-04 19:02:18.000000 swibots-1.1.5/swibots/api/chat/methods/get_unread_messages_count.py
+-rwxr-xr-x   0 root         (0) root         (0)      785 2023-02-04 19:02:01.000000 swibots-1.1.5/swibots/api/chat/methods/get_user_media_files.py
+-rwxr-xr-x   0 root         (0) root         (0)      881 2023-02-08 08:22:32.000000 swibots-1.1.5/swibots/api/chat/methods/reply_message.py
+-rwxr-xr-x   0 root         (0) root         (0)     1032 2023-02-08 08:20:23.000000 swibots-1.1.5/swibots/api/chat/methods/reply_message_text.py
+-rwxr-xr-x   0 root         (0) root         (0)      849 2023-02-08 08:19:39.000000 swibots-1.1.5/swibots/api/chat/methods/send_message.py
+-rwxr-xr-x   0 root         (0) root         (0)     1136 2023-02-04 19:02:18.000000 swibots-1.1.5/swibots/api/chat/methods/send_text.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:44:41.666579 swibots-1.1.5/swibots/api/chat/models/
+-rw-r--r--   0 root         (0) root         (0)      305 2023-02-04 19:02:18.000000 swibots-1.1.5/swibots/api/chat/models/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      920 2023-02-06 20:55:52.000000 swibots-1.1.5/swibots/api/chat/models/group_chat_history.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:44:41.825804 swibots-1.1.5/swibots/api/chat/models/inline/
+-rwxr-xr-x   0 root         (0) root         (0)      565 2023-02-04 19:02:18.000000 swibots-1.1.5/swibots/api/chat/models/inline/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     1371 2023-02-04 19:02:18.000000 swibots-1.1.5/swibots/api/chat/models/inline/base_typed_inline_query_result.py
+-rwxr-xr-x   0 root         (0) root         (0)     2533 2023-02-04 19:02:18.000000 swibots-1.1.5/swibots/api/chat/models/inline/inline_query.py
+-rwxr-xr-x   0 root         (0) root         (0)     1871 2023-02-04 19:02:18.000000 swibots-1.1.5/swibots/api/chat/models/inline/inline_query_answer.py
+-rwxr-xr-x   0 root         (0) root         (0)      991 2023-02-04 19:02:18.000000 swibots-1.1.5/swibots/api/chat/models/inline/inline_query_result.py
+-rwxr-xr-x   0 root         (0) root         (0)     1158 2023-02-04 19:02:18.000000 swibots-1.1.5/swibots/api/chat/models/inline/inline_query_result_article.py
+-rw-r--r--   0 root         (0) root         (0)     1273 2023-02-04 19:02:18.000000 swibots-1.1.5/swibots/api/chat/models/inline/inline_query_result_document.py
+-rw-r--r--   0 root         (0) root         (0)     1620 2023-02-04 19:02:18.000000 swibots-1.1.5/swibots/api/chat/models/inline/inline_query_result_photo.py
+-rw-r--r--   0 root         (0) root         (0)     1760 2023-02-04 19:02:18.000000 swibots-1.1.5/swibots/api/chat/models/inline/inline_query_result_video.py
+-rwxr-xr-x   0 root         (0) root         (0)      581 2023-02-04 19:02:18.000000 swibots-1.1.5/swibots/api/chat/models/inline/input_message_content.py
+-rwxr-xr-x   0 root         (0) root         (0)      201 2023-02-04 19:02:18.000000 swibots-1.1.5/swibots/api/chat/models/inline/types.py
+-rwxr-xr-x   0 root         (0) root         (0)      886 2023-02-08 07:21:24.000000 swibots-1.1.5/swibots/api/chat/models/inline_keyboard_button.py
+-rwxr-xr-x   0 root         (0) root         (0)      170 2023-01-18 20:49:52.000000 swibots-1.1.5/swibots/api/chat/models/inline_keyboard_color.py
+-rwxr-xr-x   0 root         (0) root         (0)      146 2023-02-04 19:02:01.000000 swibots-1.1.5/swibots/api/chat/models/inline_keyboard_size.py
+-rwxr-xr-x   0 root         (0) root         (0)     2065 2023-02-08 07:22:42.000000 swibots-1.1.5/swibots/api/chat/models/inline_markup.py
+-rw-r--r--   0 root         (0) root         (0)    10769 2023-02-08 09:10:55.000000 swibots-1.1.5/swibots/api/chat/models/message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:44:41.842733 swibots-1.1.5/swibots/api/common/
+-rwxr-xr-x   0 root         (0) root         (0)       44 2023-01-16 06:01:00.000000 swibots-1.1.5/swibots/api/common/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:44:41.868199 swibots-1.1.5/swibots/api/common/events/
+-rwxr-xr-x   0 root         (0) root         (0)       46 2023-01-13 06:20:04.000000 swibots-1.1.5/swibots/api/common/events/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     2789 2023-01-23 19:39:48.000000 swibots-1.1.5/swibots/api/common/events/event.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:44:41.925739 swibots-1.1.5/swibots/api/common/models/
+-rwxr-xr-x   0 root         (0) root         (0)      101 2023-02-06 20:55:52.000000 swibots-1.1.5/swibots/api/common/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2004 2023-02-07 07:11:30.000000 swibots-1.1.5/swibots/api/common/models/media.py
+-rwxr-xr-x   0 root         (0) root         (0)     1565 2023-02-04 19:02:18.000000 swibots-1.1.5/swibots/api/common/models/media_upload_request.py
+-rwxr-xr-x   0 root         (0) root         (0)     1706 2023-02-04 19:02:18.000000 swibots-1.1.5/swibots/api/common/models/user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:44:41.952314 swibots-1.1.5/swibots/api/community/
+-rwxr-xr-x   0 root         (0) root         (0)       90 2023-01-16 06:00:40.000000 swibots-1.1.5/swibots/api/community/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5059 2023-03-20 17:15:06.000000 swibots-1.1.5/swibots/api/community/community_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:44:42.011323 swibots-1.1.5/swibots/api/community/controllers/
+-rw-r--r--   0 root         (0) root         (0)      102 2023-02-06 20:55:52.000000 swibots-1.1.5/swibots/api/community/controllers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      595 2023-02-06 20:55:52.000000 swibots-1.1.5/swibots/api/community/controllers/channel_controller.py
+-rwxr-xr-x   0 root         (0) root         (0)      616 2023-02-06 20:55:52.000000 swibots-1.1.5/swibots/api/community/controllers/community_controller.py
+-rw-r--r--   0 root         (0) root         (0)      576 2023-02-06 20:55:52.000000 swibots-1.1.5/swibots/api/community/controllers/group_controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:44:42.152321 swibots-1.1.5/swibots/api/community/events/
+-rwxr-xr-x   0 root         (0) root         (0)      566 2023-01-16 23:20:36.000000 swibots-1.1.5/swibots/api/community/events/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     1387 2023-03-20 17:12:26.000000 swibots-1.1.5/swibots/api/community/events/channel_created_event.py
+-rwxr-xr-x   0 root         (0) root         (0)     1387 2023-03-20 17:12:56.000000 swibots-1.1.5/swibots/api/community/events/channel_deleted_event.py
+-rwxr-xr-x   0 root         (0) root         (0)     1387 2023-03-20 17:12:44.000000 swibots-1.1.5/swibots/api/community/events/channel_updated_event.py
+-rwxr-xr-x   0 root         (0) root         (0)     2303 2023-01-23 19:25:02.000000 swibots-1.1.5/swibots/api/community/events/community_event.py
+-rwxr-xr-x   0 root         (0) root         (0)     1383 2023-02-04 19:02:01.000000 swibots-1.1.5/swibots/api/community/events/community_updated_event.py
+-rwxr-xr-x   0 root         (0) root         (0)     1381 2023-03-20 17:13:37.000000 swibots-1.1.5/swibots/api/community/events/group_created_event.py
+-rwxr-xr-x   0 root         (0) root         (0)     1381 2023-03-20 17:14:02.000000 swibots-1.1.5/swibots/api/community/events/group_deleted_event.py
+-rwxr-xr-x   0 root         (0) root         (0)     1381 2023-03-20 17:13:49.000000 swibots-1.1.5/swibots/api/community/events/group_updated_event.py
+-rwxr-xr-x   0 root         (0) root         (0)     1380 2023-03-20 17:14:48.000000 swibots-1.1.5/swibots/api/community/events/member_joined_event.py
+-rwxr-xr-x   0 root         (0) root         (0)     1377 2023-03-20 17:15:06.000000 swibots-1.1.5/swibots/api/community/events/member_left_event.py
+-rwxr-xr-x   0 root         (0) root         (0)     1373 2023-03-20 17:14:14.000000 swibots-1.1.5/swibots/api/community/events/user_banned_event.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:44:42.202681 swibots-1.1.5/swibots/api/community/methods/
+-rwxr-xr-x   0 root         (0) root         (0)      194 2023-02-04 19:02:18.000000 swibots-1.1.5/swibots/api/community/methods/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      643 2023-02-06 20:55:52.000000 swibots-1.1.5/swibots/api/community/methods/get_channel.py
+-rwxr-xr-x   0 root         (0) root         (0)      668 2023-02-04 19:02:18.000000 swibots-1.1.5/swibots/api/community/methods/get_community.py
+-rw-r--r--   0 root         (0) root         (0)      619 2023-02-06 20:55:52.000000 swibots-1.1.5/swibots/api/community/methods/get_group.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:44:42.251380 swibots-1.1.5/swibots/api/community/models/
+-rwxr-xr-x   0 root         (0) root         (0)      132 2023-01-13 05:39:45.000000 swibots-1.1.5/swibots/api/community/models/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     2743 2023-02-04 19:02:01.000000 swibots-1.1.5/swibots/api/community/models/channel.py
+-rwxr-xr-x   0 root         (0) root         (0)     2954 2023-01-21 07:06:56.000000 swibots-1.1.5/swibots/api/community/models/community.py
+-rwxr-xr-x   0 root         (0) root         (0)     2720 2023-01-21 07:07:04.000000 swibots-1.1.5/swibots/api/community/models/group.py
+-rwxr-xr-x   0 root         (0) root         (0)     9347 2023-04-17 03:16:12.000000 swibots-1.1.5/swibots/app.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:44:42.384398 swibots-1.1.5/swibots/base/
+-rw-r--r--   0 root         (0) root         (0)      262 2023-01-16 05:59:47.000000 swibots-1.1.5/swibots/base/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       69 2023-01-09 05:33:14.000000 swibots-1.1.5/swibots/base/rest_controller.py
+-rw-r--r--   0 root         (0) root         (0)      370 2023-01-19 01:21:52.000000 swibots-1.1.5/swibots/base/rest_request.py
+-rw-r--r--   0 root         (0) root         (0)      644 2023-01-19 01:21:52.000000 swibots-1.1.5/swibots/base/rest_response.py
+-rw-r--r--   0 root         (0) root         (0)     4261 2023-02-06 20:55:52.000000 swibots-1.1.5/swibots/base/switch_client.py
+-rw-r--r--   0 root         (0) root         (0)     1180 2023-01-21 06:58:45.000000 swibots-1.1.5/swibots/base/switch_object.py
+-rwxr-xr-x   0 root         (0) root         (0)      543 2023-01-19 01:21:52.000000 swibots-1.1.5/swibots/base/switch_ws_async_client.py
+-rwxr-xr-x   0 root         (0) root         (0)     4329 2023-02-04 19:02:18.000000 swibots-1.1.5/swibots/bot_app.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:44:42.485667 swibots-1.1.5/swibots/bots/
+-rwxr-xr-x   0 root         (0) root         (0)      201 2023-01-17 03:43:24.000000 swibots-1.1.5/swibots/bots/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     4646 2023-04-20 23:47:00.000000 swibots-1.1.5/swibots/bots/bot.py
+-rwxr-xr-x   0 root         (0) root         (0)     1646 2023-01-19 01:21:52.000000 swibots-1.1.5/swibots/bots/bot_context.py
+-rwxr-xr-x   0 root         (0) root         (0)      109 2023-01-14 17:55:20.000000 swibots-1.1.5/swibots/bots/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:44:42.695019 swibots-1.1.5/swibots/bots/decorators/
+-rwxr-xr-x   0 root         (0) root         (0)      999 2023-02-04 19:02:18.000000 swibots-1.1.5/swibots/bots/decorators/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      540 2023-01-19 01:21:52.000000 swibots-1.1.5/swibots/bots/decorators/on_callback_query.py
+-rwxr-xr-x   0 root         (0) root         (0)      510 2023-02-04 19:02:01.000000 swibots-1.1.5/swibots/bots/decorators/on_channel_created.py
+-rwxr-xr-x   0 root         (0) root         (0)      544 2023-02-04 19:02:01.000000 swibots-1.1.5/swibots/bots/decorators/on_channel_deleted.py
+-rwxr-xr-x   0 root         (0) root         (0)      541 2023-02-04 19:02:01.000000 swibots-1.1.5/swibots/bots/decorators/on_channel_updated.py
+-rwxr-xr-x   0 root         (0) root         (0)      574 2023-01-19 01:21:52.000000 swibots-1.1.5/swibots/bots/decorators/on_command.py
+-rwxr-xr-x   0 root         (0) root         (0)      544 2023-02-04 19:02:01.000000 swibots-1.1.5/swibots/bots/decorators/on_community_updated.py
+-rwxr-xr-x   0 root         (0) root         (0)      536 2023-02-04 19:02:01.000000 swibots-1.1.5/swibots/bots/decorators/on_group_created.py
+-rwxr-xr-x   0 root         (0) root         (0)      536 2023-02-04 19:02:01.000000 swibots-1.1.5/swibots/bots/decorators/on_group_deleted.py
+-rwxr-xr-x   0 root         (0) root         (0)      534 2023-02-04 19:02:01.000000 swibots-1.1.5/swibots/bots/decorators/on_group_updated.py
+-rw-r--r--   0 root         (0) root         (0)      537 2023-02-04 19:02:18.000000 swibots-1.1.5/swibots/bots/decorators/on_inline_query.py
+-rwxr-xr-x   0 root         (0) root         (0)      534 2023-02-04 19:02:01.000000 swibots-1.1.5/swibots/bots/decorators/on_member_joined.py
+-rwxr-xr-x   0 root         (0) root         (0)      529 2023-02-04 19:02:01.000000 swibots-1.1.5/swibots/bots/decorators/on_member_left.py
+-rwxr-xr-x   0 root         (0) root         (0)      503 2023-01-19 01:21:52.000000 swibots-1.1.5/swibots/bots/decorators/on_message.py
+-rwxr-xr-x   0 root         (0) root         (0)      543 2023-01-19 01:21:52.000000 swibots-1.1.5/swibots/bots/decorators/on_unknown_command.py
+-rwxr-xr-x   0 root         (0) root         (0)      509 2023-02-04 19:02:01.000000 swibots-1.1.5/swibots/bots/decorators/on_user_banned.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:44:42.723666 swibots-1.1.5/swibots/bots/filters/
+-rwxr-xr-x   0 root         (0) root         (0)       22 2023-01-16 03:25:36.000000 swibots-1.1.5/swibots/bots/filters/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     7785 2023-04-21 00:39:37.000000 swibots-1.1.5/swibots/bots/filters/filter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:44:43.105462 swibots-1.1.5/swibots/bots/handlers/
+-rwxr-xr-x   0 root         (0) root         (0)     1300 2023-02-04 19:02:18.000000 swibots-1.1.5/swibots/bots/handlers/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     1048 2023-01-19 01:21:52.000000 swibots-1.1.5/swibots/bots/handlers/base_handler.py
+-rwxr-xr-x   0 root         (0) root         (0)      985 2023-02-04 19:02:01.000000 swibots-1.1.5/swibots/bots/handlers/callback_query_handler.py
+-rwxr-xr-x   0 root         (0) root         (0)      681 2023-03-20 17:12:26.000000 swibots-1.1.5/swibots/bots/handlers/channel_created_handler.py
+-rwxr-xr-x   0 root         (0) root         (0)      688 2023-03-20 17:12:57.000000 swibots-1.1.5/swibots/bots/handlers/channel_deleted_handler.py
+-rwxr-xr-x   0 root         (0) root         (0)      734 2023-03-20 17:12:44.000000 swibots-1.1.5/swibots/bots/handlers/channel_updated_handler.py
+-rwxr-xr-x   0 root         (0) root         (0)     1514 2023-01-19 01:21:52.000000 swibots-1.1.5/swibots/bots/handlers/command_handler.py
+-rwxr-xr-x   0 root         (0) root         (0)      686 2023-01-19 01:21:52.000000 swibots-1.1.5/swibots/bots/handlers/community_updated_handler.py
+-rwxr-xr-x   0 root         (0) root         (0)     1325 2023-04-21 00:21:17.000000 swibots-1.1.5/swibots/bots/handlers/event_handler.py
+-rwxr-xr-x   0 root         (0) root         (0)      680 2023-03-20 17:13:37.000000 swibots-1.1.5/swibots/bots/handlers/group_created_handler.py
+-rwxr-xr-x   0 root         (0) root         (0)      775 2023-03-20 17:14:02.000000 swibots-1.1.5/swibots/bots/handlers/group_deleted_handler.py
+-rwxr-xr-x   0 root         (0) root         (0)      775 2023-03-20 17:13:49.000000 swibots-1.1.5/swibots/bots/handlers/group_updated_handler.py
+-rw-r--r--   0 root         (0) root         (0)      867 2023-02-04 19:02:18.000000 swibots-1.1.5/swibots/bots/handlers/inline_query_handler.py
+-rwxr-xr-x   0 root         (0) root         (0)      679 2023-03-20 17:14:48.000000 swibots-1.1.5/swibots/bots/handlers/member_joined_handler.py
+-rwxr-xr-x   0 root         (0) root         (0)      674 2023-03-20 17:15:07.000000 swibots-1.1.5/swibots/bots/handlers/member_left_handler.py
+-rwxr-xr-x   0 root         (0) root         (0)      960 2023-02-04 19:02:01.000000 swibots-1.1.5/swibots/bots/handlers/message_handler.py
+-rwxr-xr-x   0 root         (0) root         (0)      885 2023-01-19 01:21:52.000000 swibots-1.1.5/swibots/bots/handlers/unknown_command_handler.py
+-rwxr-xr-x   0 root         (0) root         (0)      670 2023-03-20 17:14:14.000000 swibots-1.1.5/swibots/bots/handlers/user_banned_handler.py
+-rwxr-xr-x   0 root         (0) root         (0)      285 2023-01-23 21:16:29.000000 swibots-1.1.5/swibots/bots/register_command.py
+-rwxr-xr-x   0 root         (0) root         (0)     1589 2023-01-23 17:48:03.000000 swibots-1.1.5/swibots/config.py
+-rw-r--r--   0 root         (0) root         (0)     1333 2023-02-04 19:02:18.000000 swibots-1.1.5/swibots/error.py
+-rwxr-xr-x   0 root         (0) root         (0)      854 2023-03-20 17:15:29.000000 swibots-1.1.5/swibots/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:44:43.155954 swibots-1.1.5/swibots/utils/
+-rw-r--r--   0 root         (0) root         (0)       75 2023-01-16 05:53:47.000000 swibots-1.1.5/swibots/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5880 2023-04-20 23:47:11.000000 swibots-1.1.5/swibots/utils/rest_client.py
+-rw-r--r--   0 root         (0) root         (0)     2475 2023-02-04 19:02:18.000000 swibots-1.1.5/swibots/utils/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:44:43.168357 swibots-1.1.5/swibots/utils/ws/
+-rw-r--r--   0 root         (0) root         (0)       48 2023-01-19 05:23:27.000000 swibots-1.1.5/swibots/utils/ws/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:44:43.221159 swibots-1.1.5/swibots/utils/ws/asyncstomp/
+-rw-r--r--   0 root         (0) root         (0)      150 2023-01-09 05:33:14.000000 swibots-1.1.5/swibots/utils/ws/asyncstomp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9743 2023-01-21 06:34:39.000000 swibots-1.1.5/swibots/utils/ws/asyncstomp/async_ws_client.py
+-rw-r--r--   0 root         (0) root         (0)      980 2023-01-19 01:21:52.000000 swibots-1.1.5/swibots/utils/ws/asyncstomp/async_ws_subscription.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:44:43.267184 swibots-1.1.5/swibots/utils/ws/common/
+-rw-r--r--   0 root         (0) root         (0)      100 2023-01-09 05:33:14.000000 swibots-1.1.5/swibots/utils/ws/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-01-09 05:33:14.000000 swibots-1.1.5/swibots/utils/ws/common/ws_frame.py
+-rw-r--r--   0 root         (0) root         (0)      430 2023-01-09 05:33:14.000000 swibots-1.1.5/swibots/utils/ws/common/ws_message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:44:40.631728 swibots-1.1.5/swibots.egg-info/
+-rwxr-xr-x   0 root         (0) root         (0)     1817 2023-04-21 00:44:39.000000 swibots-1.1.5/swibots.egg-info/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)     7316 2023-04-21 00:44:40.000000 swibots-1.1.5/swibots.egg-info/SOURCES.txt
+-rwxr-xr-x   0 root         (0) root         (0)        1 2023-04-21 00:44:39.000000 swibots-1.1.5/swibots.egg-info/dependency_links.txt
+-rwxr-xr-x   0 root         (0) root         (0)       31 2023-04-21 00:44:39.000000 swibots-1.1.5/swibots.egg-info/requires.txt
+-rwxr-xr-x   0 root         (0) root         (0)       14 2023-04-21 00:44:39.000000 swibots-1.1.5/swibots.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:44:43.295630 swibots-1.1.5/tests/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 05:56:05.000000 swibots-1.1.5/tests/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      202 2023-01-15 22:26:25.000000 swibots-1.1.5/tests/tests.py
```

### Comparing `swibots-1.1.4/PKG-INFO` & `swibots-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swibots
-Version: 1.1.4
+Version: 1.1.5
 Summary: Switch bot api
 Home-page: https://github.com/switchcollab/Switch-Bots-Python-Library
 Author: switchadmin
 Author-email: support@switch.pe
 License: LGPLv3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `swibots-1.1.4/README.md` & `swibots-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/setup.py` & `swibots-1.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     long_description = pypandoc.convert_file("README.md", "rst")
 except (IOError, ImportError):
     long_description = open("README.md").read()
 
 
 setup(
     name="swibots",
-    version="1.1.4",
+    version="1.1.5",
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/switchcollab/Switch-Bots-Python-Library",
     description="Switch bot api",
     author="switchadmin",
     author_email="support@switch.pe",
```

### Comparing `swibots-1.1.4/swibots/api/api_client.py` & `swibots-1.1.5/swibots/api/api_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/auth/auth_client.py` & `swibots-1.1.5/swibots/api/auth/auth_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/auth/controllers/user_controller.py` & `swibots-1.1.5/swibots/api/auth/controllers/user_controller.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/auth/methods/get_me.py` & `swibots-1.1.5/swibots/api/auth/methods/get_me.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/auth/methods/login.py` & `swibots-1.1.5/swibots/api/auth/methods/login.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/auth/models/auth_user.py` & `swibots-1.1.5/swibots/api/auth/models/auth_user.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/bot/bot_client.py` & `swibots-1.1.5/swibots/api/bot/bot_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/bot/controllers/bot_controller.py` & `swibots-1.1.5/swibots/api/bot/controllers/bot_controller.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/bot/methods/delete_bot_info.py` & `swibots-1.1.5/swibots/api/bot/methods/delete_bot_info.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/bot/methods/get_bot_info.py` & `swibots-1.1.5/swibots/api/bot/methods/get_bot_info.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/bot/methods/update_bot_info.py` & `swibots-1.1.5/swibots/api/bot/methods/update_bot_info.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/bot/models/bot_command_info.py` & `swibots-1.1.5/swibots/api/bot/models/bot_command_info.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/bot/models/bot_info.py` & `swibots-1.1.5/swibots/api/bot/models/bot_info.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/chat/chat_client.py` & `swibots-1.1.5/swibots/api/chat/chat_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/chat/controllers/message_controller.py` & `swibots-1.1.5/swibots/api/chat/controllers/message_controller.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/chat/events/callback_query_event.py` & `swibots-1.1.5/swibots/api/chat/events/callback_query_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/chat/events/chat_event.py` & `swibots-1.1.5/swibots/api/chat/events/chat_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/chat/events/command_event.py` & `swibots-1.1.5/swibots/api/chat/events/command_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/chat/events/inline_query_event.py` & `swibots-1.1.5/swibots/api/chat/events/inline_query_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/chat/events/message_event.py` & `swibots-1.1.5/swibots/api/chat/events/message_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/chat/methods/__init__.py` & `swibots-1.1.5/swibots/api/chat/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/chat/methods/answer_inline_query.py` & `swibots-1.1.5/swibots/api/chat/methods/answer_inline_query.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/chat/methods/clear_conversation.py` & `swibots-1.1.5/swibots/api/chat/methods/clear_conversation.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/chat/methods/delete_message.py` & `swibots-1.1.5/swibots/api/chat/methods/delete_message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/chat/methods/delete_messages_from_user.py` & `swibots-1.1.5/swibots/api/chat/methods/delete_messages_from_user.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/chat/methods/download_media.py` & `swibots-1.1.5/swibots/api/chat/methods/download_media.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/chat/methods/edit_message.py` & `swibots-1.1.5/swibots/api/chat/methods/edit_message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/chat/methods/edit_message_text.py` & `swibots-1.1.5/swibots/api/chat/methods/edit_message_text.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/chat/methods/flag_message.py` & `swibots-1.1.5/swibots/api/chat/methods/flag_message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/chat/methods/forward_message.py` & `swibots-1.1.5/swibots/api/chat/methods/forward_message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/chat/methods/get_channel_chat_history.py` & `swibots-1.1.5/swibots/api/chat/methods/get_channel_chat_history.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/chat/methods/get_community_media_files.py` & `swibots-1.1.5/swibots/api/chat/methods/get_community_media_files.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/chat/methods/get_community_media_files_by_status.py` & `swibots-1.1.5/swibots/api/chat/methods/get_community_media_files_by_status.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/chat/methods/get_flag_messages.py` & `swibots-1.1.5/swibots/api/chat/methods/get_flag_messages.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/chat/methods/get_group_chat_history.py` & `swibots-1.1.5/swibots/api/chat/methods/get_group_chat_history.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/chat/methods/get_message.py` & `swibots-1.1.5/swibots/api/chat/methods/get_message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/chat/methods/get_messages.py` & `swibots-1.1.5/swibots/api/chat/methods/get_messages.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/chat/methods/get_messages_between_users.py` & `swibots-1.1.5/swibots/api/chat/methods/get_messages_between_users.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/chat/methods/get_unread_messages_count.py` & `swibots-1.1.5/swibots/api/chat/methods/get_unread_messages_count.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/chat/methods/get_user_media_files.py` & `swibots-1.1.5/swibots/api/chat/methods/get_user_media_files.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/chat/methods/reply_message.py` & `swibots-1.1.5/swibots/api/chat/methods/reply_message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/chat/methods/reply_message_text.py` & `swibots-1.1.5/swibots/api/chat/methods/reply_message_text.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/chat/methods/send_message.py` & `swibots-1.1.5/swibots/api/chat/methods/send_message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/chat/methods/send_text.py` & `swibots-1.1.5/swibots/api/chat/methods/send_text.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/chat/models/group_chat_history.py` & `swibots-1.1.5/swibots/api/chat/models/group_chat_history.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/chat/models/inline/__init__.py` & `swibots-1.1.5/swibots/api/chat/models/inline/__init__.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/chat/models/inline/base_typed_inline_query_result.py` & `swibots-1.1.5/swibots/api/chat/models/inline/base_typed_inline_query_result.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/chat/models/inline/inline_query.py` & `swibots-1.1.5/swibots/api/chat/models/inline/inline_query.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/chat/models/inline/inline_query_answer.py` & `swibots-1.1.5/swibots/api/chat/models/inline/inline_query_answer.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/chat/models/inline/inline_query_result.py` & `swibots-1.1.5/swibots/api/chat/models/inline/inline_query_result.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/chat/models/inline/inline_query_result_article.py` & `swibots-1.1.5/swibots/api/chat/models/inline/inline_query_result_article.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/chat/models/inline/inline_query_result_document.py` & `swibots-1.1.5/swibots/api/chat/models/inline/inline_query_result_document.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/chat/models/inline/inline_query_result_photo.py` & `swibots-1.1.5/swibots/api/chat/models/inline/inline_query_result_photo.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/chat/models/inline/inline_query_result_video.py` & `swibots-1.1.5/swibots/api/chat/models/inline/inline_query_result_video.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/chat/models/inline/input_message_content.py` & `swibots-1.1.5/swibots/api/chat/models/inline/input_message_content.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/chat/models/inline_keyboard_button.py` & `swibots-1.1.5/swibots/api/chat/models/inline_keyboard_button.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/chat/models/inline_markup.py` & `swibots-1.1.5/swibots/api/chat/models/inline_markup.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/chat/models/message.py` & `swibots-1.1.5/swibots/api/chat/models/message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/common/events/event.py` & `swibots-1.1.5/swibots/api/common/events/event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/common/models/media.py` & `swibots-1.1.5/swibots/api/common/models/media.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/common/models/media_upload_request.py` & `swibots-1.1.5/swibots/api/common/models/media_upload_request.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/common/models/user.py` & `swibots-1.1.5/swibots/api/common/models/user.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/community/community_client.py` & `swibots-1.1.5/swibots/api/community/community_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/community/controllers/channel_controller.py` & `swibots-1.1.5/swibots/api/community/controllers/channel_controller.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/community/controllers/community_controller.py` & `swibots-1.1.5/swibots/api/community/controllers/community_controller.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/community/controllers/group_controller.py` & `swibots-1.1.5/swibots/api/community/controllers/group_controller.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/community/events/__init__.py` & `swibots-1.1.5/swibots/api/community/events/__init__.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/community/events/channel_created_event.py` & `swibots-1.1.5/swibots/api/community/events/channel_created_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/community/events/channel_deleted_event.py` & `swibots-1.1.5/swibots/api/community/events/channel_deleted_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/community/events/channel_updated_event.py` & `swibots-1.1.5/swibots/api/community/events/channel_updated_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/community/events/community_event.py` & `swibots-1.1.5/swibots/api/community/events/community_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/community/events/community_updated_event.py` & `swibots-1.1.5/swibots/api/community/events/community_updated_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/community/events/group_created_event.py` & `swibots-1.1.5/swibots/api/community/events/group_created_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/community/events/group_deleted_event.py` & `swibots-1.1.5/swibots/api/community/events/group_deleted_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/community/events/group_updated_event.py` & `swibots-1.1.5/swibots/api/community/events/group_updated_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/community/events/member_joined_event.py` & `swibots-1.1.5/swibots/api/community/events/member_joined_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/community/events/member_left_event.py` & `swibots-1.1.5/swibots/api/community/events/member_left_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/community/events/user_banned_event.py` & `swibots-1.1.5/swibots/api/community/events/user_banned_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/community/methods/get_channel.py` & `swibots-1.1.5/swibots/api/community/methods/get_channel.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/community/methods/get_community.py` & `swibots-1.1.5/swibots/api/community/methods/get_community.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/community/methods/get_group.py` & `swibots-1.1.5/swibots/api/community/methods/get_group.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/community/models/channel.py` & `swibots-1.1.5/swibots/api/community/models/channel.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/community/models/community.py` & `swibots-1.1.5/swibots/api/community/models/community.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/api/community/models/group.py` & `swibots-1.1.5/swibots/api/community/models/group.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/app.py` & `swibots-1.1.5/swibots/app.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/base/rest_response.py` & `swibots-1.1.5/swibots/base/rest_response.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/base/switch_client.py` & `swibots-1.1.5/swibots/base/switch_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/base/switch_object.py` & `swibots-1.1.5/swibots/base/switch_object.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/base/switch_ws_async_client.py` & `swibots-1.1.5/swibots/base/switch_ws_async_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/bot_app.py` & `swibots-1.1.5/swibots/bot_app.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/bots/bot.py` & `swibots-1.1.5/swibots/bots/bot.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/bots/bot_context.py` & `swibots-1.1.5/swibots/bots/bot_context.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/bots/decorators/__init__.py` & `swibots-1.1.5/swibots/bots/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/bots/decorators/on_callback_query.py` & `swibots-1.1.5/swibots/bots/decorators/on_callback_query.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/bots/decorators/on_channel_deleted.py` & `swibots-1.1.5/swibots/bots/decorators/on_channel_deleted.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/bots/decorators/on_channel_updated.py` & `swibots-1.1.5/swibots/bots/decorators/on_channel_updated.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/bots/decorators/on_command.py` & `swibots-1.1.5/swibots/bots/decorators/on_command.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/bots/decorators/on_community_updated.py` & `swibots-1.1.5/swibots/bots/decorators/on_community_updated.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/bots/decorators/on_group_created.py` & `swibots-1.1.5/swibots/bots/decorators/on_group_created.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/bots/decorators/on_group_deleted.py` & `swibots-1.1.5/swibots/bots/decorators/on_group_deleted.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/bots/decorators/on_group_updated.py` & `swibots-1.1.5/swibots/bots/decorators/on_group_updated.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/bots/decorators/on_inline_query.py` & `swibots-1.1.5/swibots/bots/decorators/on_inline_query.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/bots/decorators/on_member_joined.py` & `swibots-1.1.5/swibots/bots/decorators/on_member_joined.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/bots/decorators/on_member_left.py` & `swibots-1.1.5/swibots/bots/decorators/on_member_left.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/bots/decorators/on_unknown_command.py` & `swibots-1.1.5/swibots/bots/decorators/on_unknown_command.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/bots/filters/filter.py` & `swibots-1.1.5/swibots/bots/filters/filter.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Optional
 from swibots.api.chat.events import MessageEvent
 from swibots.api.chat.events.chat_event import ChatEvent
 from swibots.api.common.events import Event
 from swibots.bots.bot_context import BotContext
 from swibots.utils.types import SCT, FilterCallback
 from swibots.types import EventType
+from typing import Callable, Union, List, Pattern
 
 
 class Filter:
     async def __call__(self, ctx: BotContext) -> bool:
         raise NotImplementedError
 
     def __invert__(self):
@@ -119,66 +120,76 @@
     return not incoming(ctx)
 
 
 outgoing = create(outgoing_filter)
 """Filter outgoing messages. Messages that are sent by the user."""
 
 
-async def community(community_id: Optional[SCT[str]]):
-    """Filter messages coming from a specific community."""
-    async def func(self, ctx: BotContext[Event]):
+class community(Filter, set):
+    """Filter events comming from a specific community or communities"""
+
+    def __init__(self, community_id: Optional[SCT[str]]):
+        community_id = community_id
+
+    async def __call__(self, ctx: BotContext[Event]):
         community_id = self.community_id
         if community_id is None:
             return bool(ctx.event.community_id is not None)
         if isinstance(community_id, str):
             community_id = frozenset({community_id})
         else:
             community_id = frozenset(community_id)
         return bool(ctx.event.community_id in community_id)
-    return create(func, name="CommunityFilter", community_id=community_id)
 
 
-async def channel(channel_id: Optional[SCT[str]]):
-    """Filter messages coming from a specific channel."""
-    async def func(self, ctx: BotContext[Event]):
+class channel(Filter, set):
+    """Filter events comming from a specific channel or channels"""
+
+    def __init__(self, channel_id: Optional[SCT[str]]):
+        channel_id = channel_id
+
+    async def __call__(self, ctx: BotContext[Event]):
         channel_id = self.channel_id
         if channel_id is None:
             return bool(ctx.event.channel_id is not None)
         if isinstance(channel_id, str):
             channel_id = frozenset({channel_id})
         else:
             channel_id = frozenset(channel_id)
         return bool(ctx.event.channel_id in channel_id)
-    return create(func, name="ChannelFilter", channel_id=channel_id)
 
 
-async def group(group_id: Optional[SCT[str]]):
-    async def func(self, ctx: BotContext[Event]):
+class group(Filter, set):
+    def __init__(self, group_id: Optional[SCT[str]]):
+        group_id = group_id
+
+    async def __call__(self, ctx: BotContext[Event]):
         group_id = self.group_id
         if group_id is None:
             return bool(ctx.event.group_id is not None)
         if isinstance(group_id, str):
             group_id = frozenset({group_id})
         else:
             group_id = frozenset(group_id)
         return bool(ctx.event.group_id in group_id)
-    return create(func, name="GroupFilter", group_id=group_id)
 
 
-async def user(user_id: Optional[SCT[str]]):
-    async def func(self, ctx: BotContext[Event]):
+class user(Filter, set):
+    def __init__(self, user_id: Optional[SCT[int]]):
+        user_id = user_id
+
+    async def __call__(self, ctx: BotContext[Event]):
         user_id = self.user_id
         if user_id is None:
             return bool(ctx.event.action_by_id is not None)
-        if isinstance(user_id, str):
+        if isinstance(user_id, int):
             user_id = frozenset({user_id})
         else:
             user_id = frozenset(user_id)
         return bool(ctx.event.action_by_id in user_id)
-    return create(func, name="UserFilter", user_id=user_id)
 
 
 def text(text: Optional[SCT[str]]):
     async def func(self, ctx: BotContext[MessageEvent]):
         text = self.text
         if text is None:
             return bool(ctx.event.message is not None and ctx.event.message.message is not None)
```

### Comparing `swibots-1.1.4/swibots/bots/handlers/__init__.py` & `swibots-1.1.5/swibots/bots/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/bots/handlers/base_handler.py` & `swibots-1.1.5/swibots/bots/handlers/base_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/bots/handlers/callback_query_handler.py` & `swibots-1.1.5/swibots/bots/handlers/callback_query_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/bots/handlers/channel_created_handler.py` & `swibots-1.1.5/swibots/bots/handlers/channel_created_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/bots/handlers/channel_deleted_handler.py` & `swibots-1.1.5/swibots/bots/handlers/channel_deleted_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/bots/handlers/channel_updated_handler.py` & `swibots-1.1.5/swibots/bots/handlers/channel_updated_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/bots/handlers/command_handler.py` & `swibots-1.1.5/swibots/bots/handlers/command_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/bots/handlers/community_updated_handler.py` & `swibots-1.1.5/swibots/bots/handlers/community_updated_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/bots/handlers/event_handler.py` & `swibots-1.1.5/swibots/bots/handlers/event_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/bots/handlers/group_created_handler.py` & `swibots-1.1.5/swibots/bots/handlers/group_created_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/bots/handlers/group_deleted_handler.py` & `swibots-1.1.5/swibots/bots/handlers/group_deleted_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/bots/handlers/group_updated_handler.py` & `swibots-1.1.5/swibots/bots/handlers/group_updated_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/bots/handlers/inline_query_handler.py` & `swibots-1.1.5/swibots/bots/handlers/inline_query_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/bots/handlers/member_joined_handler.py` & `swibots-1.1.5/swibots/bots/handlers/member_joined_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/bots/handlers/member_left_handler.py` & `swibots-1.1.5/swibots/bots/handlers/member_left_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/bots/handlers/message_handler.py` & `swibots-1.1.5/swibots/bots/handlers/message_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/bots/handlers/unknown_command_handler.py` & `swibots-1.1.5/swibots/bots/handlers/unknown_command_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/bots/handlers/user_banned_handler.py` & `swibots-1.1.5/swibots/bots/handlers/user_banned_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/config.py` & `swibots-1.1.5/swibots/config.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/error.py` & `swibots-1.1.5/swibots/error.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/types.py` & `swibots-1.1.5/swibots/types.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/utils/rest_client.py` & `swibots-1.1.5/swibots/utils/rest_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/utils/types.py` & `swibots-1.1.5/swibots/utils/types.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/utils/ws/asyncstomp/async_ws_client.py` & `swibots-1.1.5/swibots/utils/ws/asyncstomp/async_ws_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/utils/ws/asyncstomp/async_ws_subscription.py` & `swibots-1.1.5/swibots/utils/ws/asyncstomp/async_ws_subscription.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots/utils/ws/common/ws_frame.py` & `swibots-1.1.5/swibots/utils/ws/common/ws_frame.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.4/swibots.egg-info/PKG-INFO` & `swibots-1.1.5/swibots.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swibots
-Version: 1.1.4
+Version: 1.1.5
 Summary: Switch bot api
 Home-page: https://github.com/switchcollab/Switch-Bots-Python-Library
 Author: switchadmin
 Author-email: support@switch.pe
 License: LGPLv3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `swibots-1.1.4/swibots.egg-info/SOURCES.txt` & `swibots-1.1.5/swibots.egg-info/SOURCES.txt`

 * *Files identical despite different names*

