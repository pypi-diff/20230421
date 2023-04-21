# Comparing `tmp/sunshine-conversations-client-9.8.0.tar.gz` & `tmp/sunshine-conversations-client-9.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sunshine-conversations-client-9.8.0.tar", last modified: Wed Jun 29 18:40:02 2022, max compression
+gzip compressed data, was "dist/sunshine-conversations-client-9.9.0.tar", last modified: Tue Jul 12 21:40:18 2022, max compression
```

## Comparing `sunshine-conversations-client-9.8.0.tar` & `sunshine-conversations-client-9.9.0.tar`

### file list

```diff
@@ -1,308 +1,308 @@
-drwxr-xr-x   0 runner    (1200) runner    (1200)        0 2022-06-29 18:40:02.000000 sunshine-conversations-client-9.8.0/
-drwxr-xr-x   0 runner    (1200) runner    (1200)        0 2022-06-29 18:40:02.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/
-drwxr-xr-x   0 runner    (1200) runner    (1200)        0 2022-06-29 18:40:02.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/api/
--rw-r--r--   0 runner    (1200) runner    (1200)     1352 2022-06-29 18:39:50.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/api/__init__.py
--rw-r--r--   0 runner    (1200) runner    (1200)     7738 2022-06-29 18:39:50.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/api/activities_api.py
--rw-r--r--   0 runner    (1200) runner    (1200)    23381 2022-06-29 18:39:50.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/api/app_keys_api.py
--rw-r--r--   0 runner    (1200) runner    (1200)    27297 2022-06-29 18:39:50.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/api/apps_api.py
--rw-r--r--   0 runner    (1200) runner    (1200)    28914 2022-06-29 18:39:50.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/api/attachments_api.py
--rw-r--r--   0 runner    (1200) runner    (1200)    21904 2022-06-29 18:39:50.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/api/clients_api.py
--rw-r--r--   0 runner    (1200) runner    (1200)    32745 2022-06-29 18:39:50.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/api/conversations_api.py
--rw-r--r--   0 runner    (1200) runner    (1200)    27534 2022-06-29 18:39:50.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/api/custom_integration_api_keys_api.py
--rw-r--r--   0 runner    (1200) runner    (1200)    32070 2022-06-29 18:39:50.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/api/integrations_api.py
--rw-r--r--   0 runner    (1200) runner    (1200)    27510 2022-06-29 18:39:50.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/api/messages_api.py
--rw-r--r--   0 runner    (1200) runner    (1200)    19060 2022-06-29 18:39:50.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/api/o_auth_endpoints_api.py
--rw-r--r--   0 runner    (1200) runner    (1200)    21789 2022-06-29 18:39:50.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/api/participants_api.py
--rw-r--r--   0 runner    (1200) runner    (1200)    28668 2022-06-29 18:39:50.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/api/switchboard_actions_api.py
--rw-r--r--   0 runner    (1200) runner    (1200)    30749 2022-06-29 18:39:50.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/api/switchboard_integrations_api.py
--rw-r--r--   0 runner    (1200) runner    (1200)    23999 2022-06-29 18:39:50.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/api/switchboards_api.py
--rw-r--r--   0 runner    (1200) runner    (1200)    32741 2022-06-29 18:39:50.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/api/users_api.py
--rw-r--r--   0 runner    (1200) runner    (1200)    34891 2022-06-29 18:39:50.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/api/webhooks_api.py
-drwxr-xr-x   0 runner    (1200) runner    (1200)        0 2022-06-29 18:40:02.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/
--rw-r--r--   0 runner    (1200) runner    (1200)    24228 2022-06-29 18:39:50.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/__init__.py
--rw-r--r--   0 runner    (1200) runner    (1200)     4019 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/accept_control_body.py
--rw-r--r--   0 runner    (1200) runner    (1200)    14389 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/action.py
--rw-r--r--   0 runner    (1200) runner    (1200)    13749 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/action_subset.py
--rw-r--r--   0 runner    (1200) runner    (1200)     5141 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/activity.py
--rw-r--r--   0 runner    (1200) runner    (1200)     4083 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/activity_all_of.py
--rw-r--r--   0 runner    (1200) runner    (1200)     4847 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/activity_post.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3443 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/activity_post_all_of.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3819 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/activity_types.py
--rw-r--r--   0 runner    (1200) runner    (1200)     8640 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/android.py
--rw-r--r--   0 runner    (1200) runner    (1200)     8091 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/android_all_of.py
--rw-r--r--   0 runner    (1200) runner    (1200)     8374 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/android_update.py
--rw-r--r--   0 runner    (1200) runner    (1200)     6699 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/android_update_all_of.py
--rw-r--r--   0 runner    (1200) runner    (1200)     5053 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/api_key.py
--rw-r--r--   0 runner    (1200) runner    (1200)     6021 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/app.py
--rw-r--r--   0 runner    (1200) runner    (1200)     5646 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/app_create_body.py
--rw-r--r--   0 runner    (1200) runner    (1200)     5053 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/app_key.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3701 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/app_key_create_body.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3419 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/app_key_list_response.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3351 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/app_key_response.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3736 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/app_list_filter.py
--rw-r--r--   0 runner    (1200) runner    (1200)     4593 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/app_list_response.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3288 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/app_response.py
--rw-r--r--   0 runner    (1200) runner    (1200)    14777 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/app_settings.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3310 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/app_sub_schema.py
--rw-r--r--   0 runner    (1200) runner    (1200)     5484 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/app_update_body.py
--rw-r--r--   0 runner    (1200) runner    (1200)     7000 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/apple.py
--rw-r--r--   0 runner    (1200) runner    (1200)     6451 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/apple_all_of.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3372 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/apple_update.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3716 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/attachment_delete_body.py
--rw-r--r--   0 runner    (1200) runner    (1200)     4141 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/attachment_media_token_body.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3669 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/attachment_media_token_response.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3569 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/attachment_response.py
--rw-r--r--   0 runner    (1200) runner    (1200)     4307 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/attachment_schema.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3517 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/attachment_upload_body.py
--rw-r--r--   0 runner    (1200) runner    (1200)     7236 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/author.py
--rw-r--r--   0 runner    (1200) runner    (1200)     5555 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/author_webhook.py
--rw-r--r--   0 runner    (1200) runner    (1200)     7220 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/buy.py
--rw-r--r--   0 runner    (1200) runner    (1200)     6313 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/carousel_message.py
--rw-r--r--   0 runner    (1200) runner    (1200)     4477 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/carousel_message_display_settings.py
--rw-r--r--   0 runner    (1200) runner    (1200)    14164 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/client.py
--rw-r--r--   0 runner    (1200) runner    (1200)     6089 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/client_add_event.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3439 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/client_add_event_all_of.py
--rw-r--r--   0 runner    (1200) runner    (1200)     8420 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/client_add_event_all_of_payload.py
--rw-r--r--   0 runner    (1200) runner    (1200)     4133 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/client_association.py
--rw-r--r--   0 runner    (1200) runner    (1200)     5355 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/client_create.py
--rw-r--r--   0 runner    (1200) runner    (1200)     4716 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/client_list_response.py
--rw-r--r--   0 runner    (1200) runner    (1200)     6158 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/client_remove_event.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3472 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/client_remove_event_all_of.py
--rw-r--r--   0 runner    (1200) runner    (1200)     9851 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/client_remove_event_all_of_payload.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3319 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/client_response.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3103 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/client_type.py
--rw-r--r--   0 runner    (1200) runner    (1200)     6158 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/client_update_event.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3472 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/client_update_event_all_of.py
--rw-r--r--   0 runner    (1200) runner    (1200)     6918 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/client_update_event_all_of_payload.py
--rw-r--r--   0 runner    (1200) runner    (1200)     5069 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/confirmation.py
--rw-r--r--   0 runner    (1200) runner    (1200)    16710 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/content.py
--rw-r--r--   0 runner    (1200) runner    (1200)    17039 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation.py
--rw-r--r--   0 runner    (1200) runner    (1200)    10933 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_all_of.py
--rw-r--r--   0 runner    (1200) runner    (1200)    10539 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_create_body.py
--rw-r--r--   0 runner    (1200) runner    (1200)     6296 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_create_event.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3538 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_create_event_all_of.py
--rw-r--r--   0 runner    (1200) runner    (1200)    10044 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_create_event_all_of_payload.py
--rw-r--r--   0 runner    (1200) runner    (1200)     6250 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_join_event.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3516 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_join_event_all_of.py
--rw-r--r--   0 runner    (1200) runner    (1200)     4585 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_join_event_all_of_payload.py
--rw-r--r--   0 runner    (1200) runner    (1200)     6273 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_leave_event.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3527 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_leave_event_all_of.py
--rw-r--r--   0 runner    (1200) runner    (1200)     4597 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_leave_event_all_of_payload.py
--rw-r--r--   0 runner    (1200) runner    (1200)     4676 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_list_filter.py
--rw-r--r--   0 runner    (1200) runner    (1200)     4962 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_list_response.py
--rw-r--r--   0 runner    (1200) runner    (1200)     6613 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_message_delivery_channel_event.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3663 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_message_delivery_channel_event_all_of.py
--rw-r--r--   0 runner    (1200) runner    (1200)     6613 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_message_delivery_failure_event.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3663 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_message_delivery_failure_event_all_of.py
--rw-r--r--   0 runner    (1200) runner    (1200)     9410 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_message_delivery_payload.py
--rw-r--r--   0 runner    (1200) runner    (1200)     5114 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_message_delivery_payload_destination.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3670 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_message_delivery_payload_external_messages.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3580 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_message_delivery_payload_message.py
--rw-r--r--   0 runner    (1200) runner    (1200)     6553 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_message_delivery_user_event.py
--rw-r--r--   0 runner    (1200) runner    (1200)     6319 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_message_event.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3549 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_message_event_all_of.py
--rw-r--r--   0 runner    (1200) runner    (1200)     5889 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_message_event_all_of_payload.py
--rw-r--r--   0 runner    (1200) runner    (1200)     6342 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_postback_event.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3560 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_postback_event_all_of.py
--rw-r--r--   0 runner    (1200) runner    (1200)     6358 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_postback_event_all_of_payload.py
--rw-r--r--   0 runner    (1200) runner    (1200)     6250 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_read_event.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3516 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_read_event_all_of.py
--rw-r--r--   0 runner    (1200) runner    (1200)     4632 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_read_event_all_of_payload.py
--rw-r--r--   0 runner    (1200) runner    (1200)     6296 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_remove_event.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3538 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_remove_event_all_of.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3766 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_remove_event_all_of_payload.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3585 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_response.py
--rw-r--r--   0 runner    (1200) runner    (1200)     9139 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_truncated.py
--rw-r--r--   0 runner    (1200) runner    (1200)     2845 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_type.py
--rw-r--r--   0 runner    (1200) runner    (1200)     6296 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_typing_event.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3538 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_typing_event_all_of.py
--rw-r--r--   0 runner    (1200) runner    (1200)     4658 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_typing_event_all_of_payload.py
--rw-r--r--   0 runner    (1200) runner    (1200)     8263 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_update_body.py
--rw-r--r--   0 runner    (1200) runner    (1200)     5086 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/custom.py
--rw-r--r--   0 runner    (1200) runner    (1200)     4497 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/custom_all_of.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3376 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/custom_update.py
--rw-r--r--   0 runner    (1200) runner    (1200)     5281 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/destination.py
--rw-r--r--   0 runner    (1200) runner    (1200)    12469 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/device.py
--rw-r--r--   0 runner    (1200) runner    (1200)     5375 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/event_sub_schema.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3485 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/extra_channel_options.py
--rw-r--r--   0 runner    (1200) runner    (1200)     5940 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/extra_channel_options_messenger.py
--rw-r--r--   0 runner    (1200) runner    (1200)    14639 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/field.py
--rw-r--r--   0 runner    (1200) runner    (1200)     7961 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/file_message.py
--rw-r--r--   0 runner    (1200) runner    (1200)     5549 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/form_message.py
--rw-r--r--   0 runner    (1200) runner    (1200)     5559 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/form_response_message.py
--rw-r--r--   0 runner    (1200) runner    (1200)     7242 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/image_message.py
--rw-r--r--   0 runner    (1200) runner    (1200)     6531 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/inline_object.py
--rw-r--r--   0 runner    (1200) runner    (1200)    13722 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/instagram.py
--rw-r--r--   0 runner    (1200) runner    (1200)    13293 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/instagram_all_of.py
--rw-r--r--   0 runner    (1200) runner    (1200)     5403 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/instagram_update.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3680 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/instagram_update_all_of.py
--rw-r--r--   0 runner    (1200) runner    (1200)     6898 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/integration.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3709 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/integration_api_key.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3553 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/integration_api_key_list_response.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3347 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/integration_api_key_response.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3899 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/integration_id.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3544 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/integration_list_filter.py
--rw-r--r--   0 runner    (1200) runner    (1200)     4921 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/integration_list_response.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3474 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/integration_response.py
--rw-r--r--   0 runner    (1200) runner    (1200)     4103 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/integration_type.py
--rw-r--r--   0 runner    (1200) runner    (1200)    38651 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/integration_update.py
--rw-r--r--   0 runner    (1200) runner    (1200)     4500 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/integration_update_base.py
--rw-r--r--   0 runner    (1200) runner    (1200)     9864 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/ios.py
--rw-r--r--   0 runner    (1200) runner    (1200)     9355 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/ios_all_of.py
--rw-r--r--   0 runner    (1200) runner    (1200)     9858 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/ios_update.py
--rw-r--r--   0 runner    (1200) runner    (1200)     8239 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/ios_update_all_of.py
--rw-r--r--   0 runner    (1200) runner    (1200)    11468 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/item.py
--rw-r--r--   0 runner    (1200) runner    (1200)    11734 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/line.py
--rw-r--r--   0 runner    (1200) runner    (1200)    11265 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/line_all_of.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3368 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/line_update.py
--rw-r--r--   0 runner    (1200) runner    (1200)     8150 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/link.py
--rw-r--r--   0 runner    (1200) runner    (1200)     4131 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/links.py
--rw-r--r--   0 runner    (1200) runner    (1200)     5525 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/list_message.py
--rw-r--r--   0 runner    (1200) runner    (1200)     6021 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/location_message.py
--rw-r--r--   0 runner    (1200) runner    (1200)     4456 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/location_message_coordinates.py
--rw-r--r--   0 runner    (1200) runner    (1200)     4309 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/location_message_location.py
--rw-r--r--   0 runner    (1200) runner    (1200)     5632 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/location_request.py
--rw-r--r--   0 runner    (1200) runner    (1200)    12139 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/mailgun.py
--rw-r--r--   0 runner    (1200) runner    (1200)    11630 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/mailgun_all_of.py
--rw-r--r--   0 runner    (1200) runner    (1200)     8064 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/mailgun_update.py
--rw-r--r--   0 runner    (1200) runner    (1200)     6369 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/mailgun_update_all_of.py
--rw-r--r--   0 runner    (1200) runner    (1200)     8284 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/match_criteria.py
--rw-r--r--   0 runner    (1200) runner    (1200)     5592 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/match_criteria_base.py
--rw-r--r--   0 runner    (1200) runner    (1200)     7428 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/match_criteria_mailgun.py
--rw-r--r--   0 runner    (1200) runner    (1200)     5266 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/match_criteria_mailgun_all_of.py
--rw-r--r--   0 runner    (1200) runner    (1200)     7153 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/match_criteria_messagebird.py
--rw-r--r--   0 runner    (1200) runner    (1200)     4939 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/match_criteria_messagebird_all_of.py
--rw-r--r--   0 runner    (1200) runner    (1200)     7048 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/match_criteria_twilio.py
--rw-r--r--   0 runner    (1200) runner    (1200)     4874 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/match_criteria_twilio_all_of.py
--rw-r--r--   0 runner    (1200) runner    (1200)     7090 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/match_criteria_whatsapp.py
--rw-r--r--   0 runner    (1200) runner    (1200)     4900 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/match_criteria_whatsapp_all_of.py
--rw-r--r--   0 runner    (1200) runner    (1200)     9293 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/message.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3396 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/message_bird_update.py
--rw-r--r--   0 runner    (1200) runner    (1200)     4757 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/message_list_response.py
--rw-r--r--   0 runner    (1200) runner    (1200)     5473 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/message_override.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3395 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/message_override_apple.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3367 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/message_override_line.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3507 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/message_override_messenger.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3403 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/message_override_payload.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3479 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/message_override_whatsapp.py
--rw-r--r--   0 runner    (1200) runner    (1200)     8556 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/message_post.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3420 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/message_post_response.py
--rw-r--r--   0 runner    (1200) runner    (1200)     9566 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/message_webhook.py
--rw-r--r--   0 runner    (1200) runner    (1200)    10666 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/messagebird.py
--rw-r--r--   0 runner    (1200) runner    (1200)    10137 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/messagebird_all_of.py
--rw-r--r--   0 runner    (1200) runner    (1200)     9613 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/messenger.py
--rw-r--r--   0 runner    (1200) runner    (1200)     9104 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/messenger_all_of.py
--rw-r--r--   0 runner    (1200) runner    (1200)     5403 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/messenger_update.py
--rw-r--r--   0 runner    (1200) runner    (1200)     5564 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/meta.py
--rw-r--r--   0 runner    (1200) runner    (1200)     5738 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/offer_control_body.py
--rw-r--r--   0 runner    (1200) runner    (1200)     6699 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/page.py
--rw-r--r--   0 runner    (1200) runner    (1200)     9222 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/participant.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3399 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/participant_join_body.py
--rw-r--r--   0 runner    (1200) runner    (1200)     5880 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/participant_leave_body.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3913 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/participant_leave_body_participant_id.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3954 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/participant_leave_body_user_external_id.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3695 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/participant_leave_body_user_id.py
--rw-r--r--   0 runner    (1200) runner    (1200)     4815 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/participant_list_response.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3474 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/participant_response.py
--rw-r--r--   0 runner    (1200) runner    (1200)     6806 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/participant_sub_schema.py
--rw-r--r--   0 runner    (1200) runner    (1200)     5840 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/participant_with_user_external_id.py
--rw-r--r--   0 runner    (1200) runner    (1200)     5545 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/participant_with_user_id.py
--rw-r--r--   0 runner    (1200) runner    (1200)     5536 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/pass_control_body.py
--rw-r--r--   0 runner    (1200) runner    (1200)     6421 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/postback.py
--rw-r--r--   0 runner    (1200) runner    (1200)     4748 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/postback_webhook.py
--rw-r--r--   0 runner    (1200) runner    (1200)     6451 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/prechat_capture.py
--rw-r--r--   0 runner    (1200) runner    (1200)     9865 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/profile.py
--rw-r--r--   0 runner    (1200) runner    (1200)     5217 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/quoted_message.py
--rw-r--r--   0 runner    (1200) runner    (1200)     4768 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/quoted_message_external_message_id.py
--rw-r--r--   0 runner    (1200) runner    (1200)     4214 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/quoted_message_message.py
--rw-r--r--   0 runner    (1200) runner    (1200)     4184 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/referral.py
--rw-r--r--   0 runner    (1200) runner    (1200)     5202 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/referral_details.py
--rw-r--r--   0 runner    (1200) runner    (1200)     7615 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/reply.py
--rw-r--r--   0 runner    (1200) runner    (1200)    10269 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/source.py
--rw-r--r--   0 runner    (1200) runner    (1200)     9927 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/source_webhook.py
--rw-r--r--   0 runner    (1200) runner    (1200)     2826 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/status.py
--rw-r--r--   0 runner    (1200) runner    (1200)     6417 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/switchboard.py
--rw-r--r--   0 runner    (1200) runner    (1200)     6319 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/switchboard_accept_control.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3549 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/switchboard_accept_control_all_of.py
--rw-r--r--   0 runner    (1200) runner    (1200)     5408 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/switchboard_accept_control_all_of_payload.py
--rw-r--r--   0 runner    (1200) runner    (1200)     6480 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/switchboard_accept_control_failure.py
--rw-r--r--   0 runner    (1200) runner    (1200)    12395 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/switchboard_integration.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3626 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/switchboard_accept_control_failure_all_of.py
--rw-r--r--   0 runner    (1200) runner    (1200)     6142 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/switchboard_accept_control_failure_all_of_payload.py
--rw-r--r--   0 runner    (1200) runner    (1200)    11171 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/switchboard_integration_create_body.py
--rw-r--r--   0 runner    (1200) runner    (1200)     4034 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/switchboard_integration_list_response.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3936 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/switchboard_integration_response.py
--rw-r--r--   0 runner    (1200) runner    (1200)    11313 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/switchboard_integration_update_body.py
--rw-r--r--   0 runner    (1200) runner    (1200)     7050 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/switchboard_integration_webhook.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3650 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/switchboard_list_response.py
--rw-r--r--   0 runner    (1200) runner    (1200)     6296 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/switchboard_offer_control.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3538 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/switchboard_offer_control_all_of.py
--rw-r--r--   0 runner    (1200) runner    (1200)     5638 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/switchboard_offer_control_all_of_payload.py
--rw-r--r--   0 runner    (1200) runner    (1200)     6460 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/switchboard_offer_control_failure.py
--rw-r--r--   0 runner    (1200) runner    (1200)     6273 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/switchboard_pass_control.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3527 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/switchboard_pass_control_all_of.py
--rw-r--r--   0 runner    (1200) runner    (1200)     5482 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/switchboard_pass_control_all_of_payload.py
--rw-r--r--   0 runner    (1200) runner    (1200)     6440 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/switchboard_pass_control_failure.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3552 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/switchboard_response.py
--rw-r--r--   0 runner    (1200) runner    (1200)     5583 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/switchboard_update_body.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3730 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/target.py
--rw-r--r--   0 runner    (1200) runner    (1200)     6755 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/telegram.py
--rw-r--r--   0 runner    (1200) runner    (1200)     6206 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/telegram_all_of.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3384 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/telegram_update.py
--rw-r--r--   0 runner    (1200) runner    (1200)     4770 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/template_message.py
--rw-r--r--   0 runner    (1200) runner    (1200)     6153 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/text_message.py
--rw-r--r--   0 runner    (1200) runner    (1200)     9174 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/twilio.py
--rw-r--r--   0 runner    (1200) runner    (1200)     8645 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/twilio_all_of.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3376 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/twilio_update.py
--rw-r--r--   0 runner    (1200) runner    (1200)    11816 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/twitter.py
--rw-r--r--   0 runner    (1200) runner    (1200)    11327 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/twitter_all_of.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3380 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/twitter_update.py
--rw-r--r--   0 runner    (1200) runner    (1200)     6273 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/user.py
--rw-r--r--   0 runner    (1200) runner    (1200)     4679 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/user_all_of.py
--rw-r--r--   0 runner    (1200) runner    (1200)     7413 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/user_create_body.py
--rw-r--r--   0 runner    (1200) runner    (1200)     6089 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/user_merge_event.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3439 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/user_merge_event_all_of.py
--rw-r--r--   0 runner    (1200) runner    (1200)     9329 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/user_merge_event_all_of_payload.py
--rw-r--r--   0 runner    (1200) runner    (1200)     4701 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/user_merge_event_all_of_payload_merged_clients.py
--rw-r--r--   0 runner    (1200) runner    (1200)     4909 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/user_merge_event_all_of_payload_merged_conversations.py
--rw-r--r--   0 runner    (1200) runner    (1200)     4647 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/user_merge_event_all_of_payload_merged_users.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3321 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/user_response.py
--rw-r--r--   0 runner    (1200) runner    (1200)     4427 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/user_truncated.py
--rw-r--r--   0 runner    (1200) runner    (1200)     5363 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/user_update_body.py
--rw-r--r--   0 runner    (1200) runner    (1200)     6112 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/user_update_event.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3450 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/user_update_event_all_of.py
--rw-r--r--   0 runner    (1200) runner    (1200)     5887 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/user_update_event_all_of_payload.py
--rw-r--r--   0 runner    (1200) runner    (1200)     6668 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/viber.py
--rw-r--r--   0 runner    (1200) runner    (1200)     6119 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/viber_all_of.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3372 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/viber_update.py
--rw-r--r--   0 runner    (1200) runner    (1200)    22825 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/web.py
--rw-r--r--   0 runner    (1200) runner    (1200)    22536 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/web_all_of.py
--rw-r--r--   0 runner    (1200) runner    (1200)    21957 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/web_update.py
--rw-r--r--   0 runner    (1200) runner    (1200)    20538 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/web_update_all_of.py
--rw-r--r--   0 runner    (1200) runner    (1200)     9194 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/webhook.py
--rw-r--r--   0 runner    (1200) runner    (1200)     6723 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/webhook_body.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3346 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/webhook_create_body.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3564 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/webhook_list_response.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3420 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/webhook_response.py
--rw-r--r--   0 runner    (1200) runner    (1200)     4171 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/webhook_sub_schema.py
--rw-r--r--   0 runner    (1200) runner    (1200)    11482 2022-06-29 18:39:49.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/webview.py
--rw-r--r--   0 runner    (1200) runner    (1200)     9123 2022-06-29 18:39:50.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/whats_app_update.py
--rw-r--r--   0 runner    (1200) runner    (1200)     7444 2022-06-29 18:39:50.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/whats_app_update_all_of.py
--rw-r--r--   0 runner    (1200) runner    (1200)    11585 2022-06-29 18:39:50.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/whatsapp.py
--rw-r--r--   0 runner    (1200) runner    (1200)    11076 2022-06-29 18:39:50.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/whatsapp_all_of.py
--rw-r--r--   0 runner    (1200) runner    (1200)    26033 2022-06-29 18:39:50.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/__init__.py
--rw-r--r--   0 runner    (1200) runner    (1200)    26616 2022-06-29 18:39:50.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/api_client.py
--rw-r--r--   0 runner    (1200) runner    (1200)    13566 2022-06-29 18:39:50.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/configuration.py
--rw-r--r--   0 runner    (1200) runner    (1200)     3677 2022-06-29 18:39:50.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/exceptions.py
--rw-r--r--   0 runner    (1200) runner    (1200)    12224 2022-06-29 18:39:50.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/rest.py
--rw-r--r--   0 runner    (1200) runner    (1200)       24 2022-06-29 18:39:50.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client/undefined.py
-drwxr-xr-x   0 runner    (1200) runner    (1200)        0 2022-06-29 18:40:02.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client.egg-info/
--rw-r--r--   0 runner    (1200) runner    (1200)      660 2022-06-29 18:40:02.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1200) runner    (1200)    17831 2022-06-29 18:40:02.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1200) runner    (1200)        1 2022-06-29 18:40:02.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1200) runner    (1200)       48 2022-06-29 18:40:02.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1200) runner    (1200)       30 2022-06-29 18:40:02.000000 sunshine-conversations-client-9.8.0/sunshine_conversations_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1200) runner    (1200)    27935 2022-06-29 18:39:50.000000 sunshine-conversations-client-9.8.0/README.md
--rw-r--r--   0 runner    (1200) runner    (1200)       69 2022-06-29 18:40:02.000000 sunshine-conversations-client-9.8.0/setup.cfg
--rw-r--r--   0 runner    (1200) runner    (1200)     1231 2022-06-29 18:39:50.000000 sunshine-conversations-client-9.8.0/setup.py
--rw-r--r--   0 runner    (1200) runner    (1200)      660 2022-06-29 18:40:02.000000 sunshine-conversations-client-9.8.0/PKG-INFO
+drwxr-xr-x   0 runner    (1200) runner    (1200)        0 2022-07-12 21:40:18.000000 sunshine-conversations-client-9.9.0/
+drwxr-xr-x   0 runner    (1200) runner    (1200)        0 2022-07-12 21:40:18.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/
+drwxr-xr-x   0 runner    (1200) runner    (1200)        0 2022-07-12 21:40:18.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/api/
+-rw-r--r--   0 runner    (1200) runner    (1200)     1352 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/api/__init__.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     7738 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/api/activities_api.py
+-rw-r--r--   0 runner    (1200) runner    (1200)    23381 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/api/app_keys_api.py
+-rw-r--r--   0 runner    (1200) runner    (1200)    27297 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/api/apps_api.py
+-rw-r--r--   0 runner    (1200) runner    (1200)    28914 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/api/attachments_api.py
+-rw-r--r--   0 runner    (1200) runner    (1200)    21904 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/api/clients_api.py
+-rw-r--r--   0 runner    (1200) runner    (1200)    32745 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/api/conversations_api.py
+-rw-r--r--   0 runner    (1200) runner    (1200)    27534 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/api/custom_integration_api_keys_api.py
+-rw-r--r--   0 runner    (1200) runner    (1200)    32070 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/api/integrations_api.py
+-rw-r--r--   0 runner    (1200) runner    (1200)    27510 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/api/messages_api.py
+-rw-r--r--   0 runner    (1200) runner    (1200)    19060 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/api/o_auth_endpoints_api.py
+-rw-r--r--   0 runner    (1200) runner    (1200)    21789 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/api/participants_api.py
+-rw-r--r--   0 runner    (1200) runner    (1200)    28668 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/api/switchboard_actions_api.py
+-rw-r--r--   0 runner    (1200) runner    (1200)    30749 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/api/switchboard_integrations_api.py
+-rw-r--r--   0 runner    (1200) runner    (1200)    23999 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/api/switchboards_api.py
+-rw-r--r--   0 runner    (1200) runner    (1200)    32741 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/api/users_api.py
+-rw-r--r--   0 runner    (1200) runner    (1200)    34891 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/api/webhooks_api.py
+drwxr-xr-x   0 runner    (1200) runner    (1200)        0 2022-07-12 21:40:18.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/
+-rw-r--r--   0 runner    (1200) runner    (1200)    24228 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/__init__.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     4019 2022-07-12 21:40:05.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/accept_control_body.py
+-rw-r--r--   0 runner    (1200) runner    (1200)    14389 2022-07-12 21:40:05.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/action.py
+-rw-r--r--   0 runner    (1200) runner    (1200)    13749 2022-07-12 21:40:05.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/action_subset.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     5141 2022-07-12 21:40:05.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/activity.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     4083 2022-07-12 21:40:05.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/activity_all_of.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     4847 2022-07-12 21:40:05.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/activity_post.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3443 2022-07-12 21:40:05.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/activity_post_all_of.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3819 2022-07-12 21:40:05.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/activity_types.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     8640 2022-07-12 21:40:05.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/android.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     8091 2022-07-12 21:40:05.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/android_all_of.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     8374 2022-07-12 21:40:05.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/android_update.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     6699 2022-07-12 21:40:05.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/android_update_all_of.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     5053 2022-07-12 21:40:05.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/api_key.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     6021 2022-07-12 21:40:05.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/app.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     5646 2022-07-12 21:40:05.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/app_create_body.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     5053 2022-07-12 21:40:05.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/app_key.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3701 2022-07-12 21:40:05.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/app_key_create_body.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3419 2022-07-12 21:40:05.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/app_key_list_response.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3351 2022-07-12 21:40:05.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/app_key_response.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3736 2022-07-12 21:40:05.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/app_list_filter.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     4593 2022-07-12 21:40:05.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/app_list_response.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3288 2022-07-12 21:40:05.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/app_response.py
+-rw-r--r--   0 runner    (1200) runner    (1200)    16019 2022-07-12 21:40:05.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/app_settings.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3310 2022-07-12 21:40:05.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/app_sub_schema.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     5484 2022-07-12 21:40:05.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/app_update_body.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     7000 2022-07-12 21:40:05.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/apple.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     6451 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/apple_all_of.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3372 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/apple_update.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3716 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/attachment_delete_body.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     4141 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/attachment_media_token_body.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3669 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/attachment_media_token_response.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3569 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/attachment_response.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     4307 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/attachment_schema.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3517 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/attachment_upload_body.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     7236 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/author.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     5555 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/author_webhook.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     7220 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/buy.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     6313 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/carousel_message.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     4477 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/carousel_message_display_settings.py
+-rw-r--r--   0 runner    (1200) runner    (1200)    14164 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/client.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     6089 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/client_add_event.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3439 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/client_add_event_all_of.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     8420 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/client_add_event_all_of_payload.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     4133 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/client_association.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     5355 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/client_create.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     4716 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/client_list_response.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     6158 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/client_remove_event.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3472 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/client_remove_event_all_of.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     9851 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/client_remove_event_all_of_payload.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3319 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/client_response.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3103 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/client_type.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     6158 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/client_update_event.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3472 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/client_update_event_all_of.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     6918 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/client_update_event_all_of_payload.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     5069 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/confirmation.py
+-rw-r--r--   0 runner    (1200) runner    (1200)    16710 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/content.py
+-rw-r--r--   0 runner    (1200) runner    (1200)    17039 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation.py
+-rw-r--r--   0 runner    (1200) runner    (1200)    10933 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_all_of.py
+-rw-r--r--   0 runner    (1200) runner    (1200)    10539 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_create_body.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     6296 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_create_event.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3538 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_create_event_all_of.py
+-rw-r--r--   0 runner    (1200) runner    (1200)    10044 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_create_event_all_of_payload.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     6250 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_join_event.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3516 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_join_event_all_of.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     4585 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_join_event_all_of_payload.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     6273 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_leave_event.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3527 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_leave_event_all_of.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     4597 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_leave_event_all_of_payload.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     4676 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_list_filter.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     4962 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_list_response.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     6613 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_message_delivery_channel_event.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3663 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_message_delivery_channel_event_all_of.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     6613 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_message_delivery_failure_event.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3663 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_message_delivery_failure_event_all_of.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     9410 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_message_delivery_payload.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     5114 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_message_delivery_payload_destination.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3670 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_message_delivery_payload_external_messages.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3580 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_message_delivery_payload_message.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     6553 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_message_delivery_user_event.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     6319 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_message_event.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3549 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_message_event_all_of.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     5889 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_message_event_all_of_payload.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     6342 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_postback_event.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3560 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_postback_event_all_of.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     6358 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_postback_event_all_of_payload.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     6250 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_read_event.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3516 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_read_event_all_of.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     4632 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_read_event_all_of_payload.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     6296 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_remove_event.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3538 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_remove_event_all_of.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3766 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_remove_event_all_of_payload.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3585 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_response.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     9139 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_truncated.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     2845 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_type.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     6296 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_typing_event.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3538 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_typing_event_all_of.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     4658 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_typing_event_all_of_payload.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     8263 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_update_body.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     5086 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/custom.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     4497 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/custom_all_of.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3376 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/custom_update.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     5281 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/destination.py
+-rw-r--r--   0 runner    (1200) runner    (1200)    12469 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/device.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     5375 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/event_sub_schema.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3485 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/extra_channel_options.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     5940 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/extra_channel_options_messenger.py
+-rw-r--r--   0 runner    (1200) runner    (1200)    14639 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/field.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     7961 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/file_message.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     5549 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/form_message.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     5559 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/form_response_message.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     7242 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/image_message.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     6531 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/inline_object.py
+-rw-r--r--   0 runner    (1200) runner    (1200)    13722 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/instagram.py
+-rw-r--r--   0 runner    (1200) runner    (1200)    13293 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/instagram_all_of.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     5403 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/instagram_update.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3680 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/instagram_update_all_of.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     6898 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/integration.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3709 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/integration_api_key.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3553 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/integration_api_key_list_response.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3347 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/integration_api_key_response.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3899 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/integration_id.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3544 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/integration_list_filter.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     4921 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/integration_list_response.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3474 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/integration_response.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     4103 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/integration_type.py
+-rw-r--r--   0 runner    (1200) runner    (1200)    38651 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/integration_update.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     4500 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/integration_update_base.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     9864 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/ios.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     9355 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/ios_all_of.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     9858 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/ios_update.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     8239 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/ios_update_all_of.py
+-rw-r--r--   0 runner    (1200) runner    (1200)    11468 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/item.py
+-rw-r--r--   0 runner    (1200) runner    (1200)    11734 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/line.py
+-rw-r--r--   0 runner    (1200) runner    (1200)    11265 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/line_all_of.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3368 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/line_update.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     8150 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/link.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     4131 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/links.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     5525 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/list_message.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     6021 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/location_message.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     4456 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/location_message_coordinates.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     4309 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/location_message_location.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     5632 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/location_request.py
+-rw-r--r--   0 runner    (1200) runner    (1200)    12139 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/mailgun.py
+-rw-r--r--   0 runner    (1200) runner    (1200)    11630 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/mailgun_all_of.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     8064 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/mailgun_update.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     6369 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/mailgun_update_all_of.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     8284 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/match_criteria.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     5592 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/match_criteria_base.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     7428 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/match_criteria_mailgun.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     5266 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/match_criteria_mailgun_all_of.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     7153 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/match_criteria_messagebird.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     4939 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/match_criteria_messagebird_all_of.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     7048 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/match_criteria_twilio.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     4874 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/match_criteria_twilio_all_of.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     7090 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/match_criteria_whatsapp.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     4900 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/match_criteria_whatsapp_all_of.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     9293 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/message.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3396 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/message_bird_update.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     4757 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/message_list_response.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     5473 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/message_override.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3395 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/message_override_apple.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3367 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/message_override_line.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3507 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/message_override_messenger.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3403 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/message_override_payload.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3479 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/message_override_whatsapp.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     8556 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/message_post.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3420 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/message_post_response.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     9566 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/message_webhook.py
+-rw-r--r--   0 runner    (1200) runner    (1200)    10666 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/messagebird.py
+-rw-r--r--   0 runner    (1200) runner    (1200)    10137 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/messagebird_all_of.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     9613 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/messenger.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     9104 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/messenger_all_of.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     5403 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/messenger_update.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     5564 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/meta.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     5738 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/offer_control_body.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     6699 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/page.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     9222 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/participant.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3399 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/participant_join_body.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     5880 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/participant_leave_body.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3913 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/participant_leave_body_participant_id.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3954 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/participant_leave_body_user_external_id.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3695 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/participant_leave_body_user_id.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     4815 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/participant_list_response.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3474 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/participant_response.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     6806 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/participant_sub_schema.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     5840 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/participant_with_user_external_id.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     5545 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/participant_with_user_id.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     5536 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/pass_control_body.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     6421 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/postback.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     4748 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/postback_webhook.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     6451 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/prechat_capture.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     9865 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/profile.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     5217 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/quoted_message.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     4768 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/quoted_message_external_message_id.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     4214 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/quoted_message_message.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     4184 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/referral.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     5202 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/referral_details.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     7615 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/reply.py
+-rw-r--r--   0 runner    (1200) runner    (1200)    10269 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/source.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     9927 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/source_webhook.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     2826 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/status.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     6417 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/switchboard.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     6319 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/switchboard_accept_control.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3549 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/switchboard_accept_control_all_of.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     5408 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/switchboard_accept_control_all_of_payload.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     6480 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/switchboard_accept_control_failure.py
+-rw-r--r--   0 runner    (1200) runner    (1200)    12395 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/switchboard_integration.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3626 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/switchboard_accept_control_failure_all_of.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     6142 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/switchboard_accept_control_failure_all_of_payload.py
+-rw-r--r--   0 runner    (1200) runner    (1200)    11171 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/switchboard_integration_create_body.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     4034 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/switchboard_integration_list_response.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3936 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/switchboard_integration_response.py
+-rw-r--r--   0 runner    (1200) runner    (1200)    11313 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/switchboard_integration_update_body.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     7050 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/switchboard_integration_webhook.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3650 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/switchboard_list_response.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     6296 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/switchboard_offer_control.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3538 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/switchboard_offer_control_all_of.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     5638 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/switchboard_offer_control_all_of_payload.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     6460 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/switchboard_offer_control_failure.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     6273 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/switchboard_pass_control.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3527 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/switchboard_pass_control_all_of.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     5482 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/switchboard_pass_control_all_of_payload.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     6440 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/switchboard_pass_control_failure.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3552 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/switchboard_response.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     5583 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/switchboard_update_body.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3730 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/target.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     6755 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/telegram.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     6206 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/telegram_all_of.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3384 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/telegram_update.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     4770 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/template_message.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     6153 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/text_message.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     9174 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/twilio.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     8645 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/twilio_all_of.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3376 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/twilio_update.py
+-rw-r--r--   0 runner    (1200) runner    (1200)    11816 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/twitter.py
+-rw-r--r--   0 runner    (1200) runner    (1200)    11327 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/twitter_all_of.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3380 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/twitter_update.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     6273 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/user.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     4679 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/user_all_of.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     7413 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/user_create_body.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     6089 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/user_merge_event.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3439 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/user_merge_event_all_of.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     9329 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/user_merge_event_all_of_payload.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     4701 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/user_merge_event_all_of_payload_merged_clients.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     4909 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/user_merge_event_all_of_payload_merged_conversations.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     4647 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/user_merge_event_all_of_payload_merged_users.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3321 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/user_response.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     4427 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/user_truncated.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     5363 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/user_update_body.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     6112 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/user_update_event.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3450 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/user_update_event_all_of.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     5887 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/user_update_event_all_of_payload.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     6668 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/viber.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     6119 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/viber_all_of.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3372 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/viber_update.py
+-rw-r--r--   0 runner    (1200) runner    (1200)    22825 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/web.py
+-rw-r--r--   0 runner    (1200) runner    (1200)    22536 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/web_all_of.py
+-rw-r--r--   0 runner    (1200) runner    (1200)    21957 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/web_update.py
+-rw-r--r--   0 runner    (1200) runner    (1200)    20538 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/web_update_all_of.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     9194 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/webhook.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     6723 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/webhook_body.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3346 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/webhook_create_body.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3564 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/webhook_list_response.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3420 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/webhook_response.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     4171 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/webhook_sub_schema.py
+-rw-r--r--   0 runner    (1200) runner    (1200)    11482 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/webview.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     9123 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/whats_app_update.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     7444 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/whats_app_update_all_of.py
+-rw-r--r--   0 runner    (1200) runner    (1200)    11585 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/whatsapp.py
+-rw-r--r--   0 runner    (1200) runner    (1200)    11076 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/whatsapp_all_of.py
+-rw-r--r--   0 runner    (1200) runner    (1200)    26033 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/__init__.py
+-rw-r--r--   0 runner    (1200) runner    (1200)    26616 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/api_client.py
+-rw-r--r--   0 runner    (1200) runner    (1200)    13566 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/configuration.py
+-rw-r--r--   0 runner    (1200) runner    (1200)     3677 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/exceptions.py
+-rw-r--r--   0 runner    (1200) runner    (1200)    12224 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/rest.py
+-rw-r--r--   0 runner    (1200) runner    (1200)       24 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client/undefined.py
+drwxr-xr-x   0 runner    (1200) runner    (1200)        0 2022-07-12 21:40:18.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client.egg-info/
+-rw-r--r--   0 runner    (1200) runner    (1200)      660 2022-07-12 21:40:18.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1200) runner    (1200)    17831 2022-07-12 21:40:18.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1200) runner    (1200)        1 2022-07-12 21:40:18.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1200) runner    (1200)       48 2022-07-12 21:40:18.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1200) runner    (1200)       30 2022-07-12 21:40:18.000000 sunshine-conversations-client-9.9.0/sunshine_conversations_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1200) runner    (1200)    27935 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/README.md
+-rw-r--r--   0 runner    (1200) runner    (1200)       69 2022-07-12 21:40:18.000000 sunshine-conversations-client-9.9.0/setup.cfg
+-rw-r--r--   0 runner    (1200) runner    (1200)     1231 2022-07-12 21:40:06.000000 sunshine-conversations-client-9.9.0/setup.py
+-rw-r--r--   0 runner    (1200) runner    (1200)      660 2022-07-12 21:40:18.000000 sunshine-conversations-client-9.9.0/PKG-INFO
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/api/__init__.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/api/activities_api.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/api/activities_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/api/app_keys_api.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/api/app_keys_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/api/apps_api.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/api/apps_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/api/attachments_api.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/api/attachments_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/api/clients_api.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/api/clients_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/api/conversations_api.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/api/conversations_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/api/custom_integration_api_keys_api.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/api/custom_integration_api_keys_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/api/integrations_api.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/api/integrations_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/api/messages_api.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/api/messages_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/api/o_auth_endpoints_api.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/api/o_auth_endpoints_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/api/participants_api.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/api/participants_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/api/switchboard_actions_api.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/api/switchboard_actions_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/api/switchboard_integrations_api.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/api/switchboard_integrations_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/api/switchboards_api.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/api/switchboards_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/api/users_api.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/api/users_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/api/webhooks_api.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/api/webhooks_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/__init__.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 
 # flake8: noqa
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 # import models into model package
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/accept_control_body.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/accept_control_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/action.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/action.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/action_subset.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/action_subset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/activity.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/activity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/activity_all_of.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/activity_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/activity_post.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/activity_post.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/activity_post_all_of.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/activity_post_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/activity_types.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/activity_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/android.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/android.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/android_all_of.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/android_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/android_update.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/android_update.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/android_update_all_of.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/android_update_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/api_key.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/api_key.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/app.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/app_create_body.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/app_create_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/app_key.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/app_key.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/app_key_create_body.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/app_key_create_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/app_key_list_response.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/app_key_list_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/app_key_response.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/app_key_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/app_list_filter.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/app_list_filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/app_list_response.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/app_list_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/app_response.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/app_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/app_settings.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/app_settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -36,45 +36,48 @@
         'conversation_retention_seconds': 'int',
         'mask_credit_card_numbers': 'bool',
         'use_animal_names': 'bool',
         'echo_postback': 'bool',
         'ignore_auto_conversation_start': 'bool',
         'multi_convo_enabled': 'bool',
         'attachments_access': 'str',
-        'attachments_token_expiration_seconds': 'int'
+        'attachments_token_expiration_seconds': 'int',
+        'app_localization_enabled': 'bool'
     }
 
     attribute_map = {
         'conversation_retention_seconds': 'conversationRetentionSeconds',
         'mask_credit_card_numbers': 'maskCreditCardNumbers',
         'use_animal_names': 'useAnimalNames',
         'echo_postback': 'echoPostback',
         'ignore_auto_conversation_start': 'ignoreAutoConversationStart',
         'multi_convo_enabled': 'multiConvoEnabled',
         'attachments_access': 'attachmentsAccess',
-        'attachments_token_expiration_seconds': 'attachmentsTokenExpirationSeconds'
+        'attachments_token_expiration_seconds': 'attachmentsTokenExpirationSeconds',
+        'app_localization_enabled': 'appLocalizationEnabled'
     }
 
     nulls = set()
 
-    def __init__(self, conversation_retention_seconds=None, mask_credit_card_numbers=None, use_animal_names=None, echo_postback=None, ignore_auto_conversation_start=None, multi_convo_enabled=None, attachments_access=None, attachments_token_expiration_seconds=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, conversation_retention_seconds=None, mask_credit_card_numbers=None, use_animal_names=None, echo_postback=None, ignore_auto_conversation_start=None, multi_convo_enabled=None, attachments_access=None, attachments_token_expiration_seconds=None, app_localization_enabled=None, local_vars_configuration=None):  # noqa: E501
         """AppSettings - a model defined in OpenAPI"""  # noqa: E501
         
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._conversation_retention_seconds = None
         self._mask_credit_card_numbers = None
         self._use_animal_names = None
         self._echo_postback = None
         self._ignore_auto_conversation_start = None
         self._multi_convo_enabled = None
         self._attachments_access = None
         self._attachments_token_expiration_seconds = None
+        self._app_localization_enabled = None
         self.discriminator = None
 
         if conversation_retention_seconds is not None:
             self.conversation_retention_seconds = conversation_retention_seconds
         if mask_credit_card_numbers is not None:
             self.mask_credit_card_numbers = mask_credit_card_numbers
         if use_animal_names is not None:
@@ -85,14 +88,16 @@
             self.ignore_auto_conversation_start = ignore_auto_conversation_start
         if multi_convo_enabled is not None:
             self.multi_convo_enabled = multi_convo_enabled
         if attachments_access is not None:
             self.attachments_access = attachments_access
         if attachments_token_expiration_seconds is not None:
             self.attachments_token_expiration_seconds = attachments_token_expiration_seconds
+        if app_localization_enabled is not None:
+            self.app_localization_enabled = app_localization_enabled
 
     @property
     def conversation_retention_seconds(self):
         """Gets the conversation_retention_seconds of this AppSettings.  # noqa: E501
 
         Number of seconds of inactivity before a conversation’s messages  will be automatically deleted. See  [Conversation Retention Seconds](https://docs.smooch.io/guide/creating-and-managing-apps/#conversation-retention-seconds) for more information.   # noqa: E501
 
@@ -273,14 +278,37 @@
 
         :param attachments_token_expiration_seconds: The attachments_token_expiration_seconds of this AppSettings.  # noqa: E501
         :type: int
         """
 
         self._attachments_token_expiration_seconds = attachments_token_expiration_seconds
 
+    @property
+    def app_localization_enabled(self):
+        """Gets the app_localization_enabled of this AppSettings.  # noqa: E501
+
+        A boolean specifying whether the messages authored by the Sunshine Conversations platform should be localized.   # noqa: E501
+
+        :return: The app_localization_enabled of this AppSettings.  # noqa: E501
+        :rtype: bool
+        """
+        return self._app_localization_enabled
+
+    @app_localization_enabled.setter
+    def app_localization_enabled(self, app_localization_enabled):
+        """Sets the app_localization_enabled of this AppSettings.
+
+        A boolean specifying whether the messages authored by the Sunshine Conversations platform should be localized.   # noqa: E501
+
+        :param app_localization_enabled: The app_localization_enabled of this AppSettings.  # noqa: E501
+        :type: bool
+        """
+
+        self._app_localization_enabled = app_localization_enabled
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/app_sub_schema.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/app_sub_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/app_update_body.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/app_update_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/apple.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/apple.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/apple_all_of.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/apple_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/apple_update.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/apple_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/attachment_delete_body.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/attachment_delete_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/attachment_media_token_body.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/attachment_media_token_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/attachment_media_token_response.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/attachment_media_token_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/attachment_response.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/attachment_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/attachment_schema.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/attachment_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/attachment_upload_body.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/attachment_upload_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/author.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/author.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/author_webhook.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/author_webhook.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/buy.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/buy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/carousel_message.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/carousel_message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/carousel_message_display_settings.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/carousel_message_display_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/client.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/client_add_event.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/client_add_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/client_add_event_all_of.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/client_add_event_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/client_add_event_all_of_payload.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/client_add_event_all_of_payload.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/client_association.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/client_association.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/client_create.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/client_create.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/client_list_response.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/client_list_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/client_remove_event.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/client_remove_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/client_remove_event_all_of.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/client_remove_event_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/client_remove_event_all_of_payload.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/client_remove_event_all_of_payload.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/client_response.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/client_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/client_type.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/client_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/client_update_event.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/client_update_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/client_update_event_all_of.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/client_update_event_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/client_update_event_all_of_payload.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/client_update_event_all_of_payload.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/confirmation.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/confirmation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/content.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/content.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_all_of.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_create_body.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_create_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_create_event.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_create_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_create_event_all_of.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_create_event_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_create_event_all_of_payload.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_create_event_all_of_payload.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_join_event.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_join_event.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_join_event_all_of.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_join_event_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_join_event_all_of_payload.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_join_event_all_of_payload.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_leave_event.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_leave_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_leave_event_all_of.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_leave_event_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_leave_event_all_of_payload.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_leave_event_all_of_payload.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_list_filter.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_list_filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_list_response.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_list_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_message_delivery_channel_event.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_message_delivery_channel_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_message_delivery_channel_event_all_of.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_message_delivery_channel_event_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_message_delivery_failure_event.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_message_delivery_failure_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_message_delivery_failure_event_all_of.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_message_delivery_failure_event_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_message_delivery_payload.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_message_delivery_payload.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_message_delivery_payload_destination.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_message_delivery_payload_destination.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_message_delivery_payload_external_messages.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_message_delivery_payload_external_messages.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_message_delivery_payload_message.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_message_delivery_payload_message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_message_delivery_user_event.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_message_delivery_user_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_message_event.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_message_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_message_event_all_of.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_message_event_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_message_event_all_of_payload.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_message_event_all_of_payload.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_postback_event.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_postback_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_postback_event_all_of.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_postback_event_all_of.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_postback_event_all_of_payload.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_postback_event_all_of_payload.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_read_event.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_read_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_read_event_all_of.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_read_event_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_read_event_all_of_payload.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_read_event_all_of_payload.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_remove_event.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_remove_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_remove_event_all_of.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_remove_event_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_remove_event_all_of_payload.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_remove_event_all_of_payload.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_response.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_truncated.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_truncated.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_type.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_typing_event.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_typing_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_typing_event_all_of.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_typing_event_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_typing_event_all_of_payload.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_typing_event_all_of_payload.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/conversation_update_body.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/conversation_update_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/custom.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/custom.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/custom_all_of.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/custom_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/custom_update.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/line_update.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -18,15 +18,15 @@
 from sunshine_conversations_client.undefined import Undefined
 
 try:
     IntegrationUpdateBase = __import__("sunshine_conversations_client.model."+re.sub(r'(?<!^)(?=[A-Z])', '_', "IntegrationUpdateBase").lower(), fromlist=("IntegrationUpdateBase")).IntegrationUpdateBase
 except ImportError:
     pass
 
-class CustomUpdate(IntegrationUpdateBase):
+class LineUpdate(IntegrationUpdateBase):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -41,15 +41,15 @@
 
     attribute_map = {
     }
 
     nulls = set()
 
     def __init__(self, local_vars_configuration=None, **kwargs):  # noqa: E501
-        """CustomUpdate - a model defined in OpenAPI"""  # noqa: E501
+        """LineUpdate - a model defined in OpenAPI"""  # noqa: E501
         super().__init__(**kwargs)
 
         if (super().openapi_types is not None):
             all_types = super().openapi_types.copy()
             all_types.update(self.openapi_types)
             self.openapi_types = all_types
 
@@ -93,18 +93,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, CustomUpdate):
+        if not isinstance(other, LineUpdate):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, CustomUpdate):
+        if not isinstance(other, LineUpdate):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/destination.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/destination.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/device.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/device.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/event_sub_schema.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/event_sub_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/extra_channel_options.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/extra_channel_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/extra_channel_options_messenger.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/extra_channel_options_messenger.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/field.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/field.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/file_message.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/file_message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/form_message.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/form_message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/form_response_message.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/form_response_message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/image_message.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/image_message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/inline_object.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/inline_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/instagram.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/instagram.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/instagram_all_of.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/instagram_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/instagram_update.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/instagram_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/instagram_update_all_of.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/instagram_update_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/integration.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/integration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/integration_api_key.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/integration_api_key.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/integration_api_key_list_response.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/integration_api_key_list_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/integration_api_key_response.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/integration_api_key_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/integration_id.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/integration_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/integration_list_filter.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/integration_list_filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/integration_list_response.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/integration_list_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/integration_response.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/integration_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/integration_type.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/integration_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/integration_update.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/integration_update.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/integration_update_base.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/integration_update_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/ios.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/ios.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/ios_all_of.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/ios_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/ios_update.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/ios_update.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/ios_update_all_of.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/ios_update_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/item.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/item.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/line.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/line.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/line_all_of.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/line_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/line_update.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/viber_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -18,15 +18,15 @@
 from sunshine_conversations_client.undefined import Undefined
 
 try:
     IntegrationUpdateBase = __import__("sunshine_conversations_client.model."+re.sub(r'(?<!^)(?=[A-Z])', '_', "IntegrationUpdateBase").lower(), fromlist=("IntegrationUpdateBase")).IntegrationUpdateBase
 except ImportError:
     pass
 
-class LineUpdate(IntegrationUpdateBase):
+class ViberUpdate(IntegrationUpdateBase):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -41,15 +41,15 @@
 
     attribute_map = {
     }
 
     nulls = set()
 
     def __init__(self, local_vars_configuration=None, **kwargs):  # noqa: E501
-        """LineUpdate - a model defined in OpenAPI"""  # noqa: E501
+        """ViberUpdate - a model defined in OpenAPI"""  # noqa: E501
         super().__init__(**kwargs)
 
         if (super().openapi_types is not None):
             all_types = super().openapi_types.copy()
             all_types.update(self.openapi_types)
             self.openapi_types = all_types
 
@@ -93,18 +93,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, LineUpdate):
+        if not isinstance(other, ViberUpdate):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, LineUpdate):
+        if not isinstance(other, ViberUpdate):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/link.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/link.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/links.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/links.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/list_message.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/list_message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/location_message.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/location_message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/location_message_coordinates.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/location_message_coordinates.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/location_message_location.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/location_message_location.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/location_request.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/location_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/mailgun.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/mailgun.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/mailgun_all_of.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/mailgun_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/mailgun_update.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/mailgun_update.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/mailgun_update_all_of.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/mailgun_update_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/match_criteria.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/match_criteria.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/match_criteria_base.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/match_criteria_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/match_criteria_mailgun.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/match_criteria_mailgun.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/match_criteria_mailgun_all_of.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/match_criteria_mailgun_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/match_criteria_messagebird.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/match_criteria_messagebird.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/match_criteria_messagebird_all_of.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/match_criteria_messagebird_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/match_criteria_twilio.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/match_criteria_twilio.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/match_criteria_twilio_all_of.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/match_criteria_twilio_all_of.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/match_criteria_whatsapp.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/match_criteria_whatsapp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/match_criteria_whatsapp_all_of.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/match_criteria_whatsapp_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/message.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/message_bird_update.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/message_bird_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/message_list_response.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/message_list_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/message_override.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/message_override.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/message_override_apple.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/message_override_apple.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/message_override_line.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/message_override_line.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/message_override_messenger.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/message_override_messenger.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/message_override_payload.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/message_override_payload.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/message_override_whatsapp.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/message_override_whatsapp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/message_post.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/message_post.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/message_post_response.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/message_post_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/message_webhook.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/message_webhook.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/messagebird.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/messagebird.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/messagebird_all_of.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/messagebird_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/messenger.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/messenger.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/messenger_all_of.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/messenger_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/messenger_update.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/messenger_update.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/meta.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/meta.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/offer_control_body.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/offer_control_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/page.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/page.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/participant.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/participant.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/participant_join_body.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/participant_join_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/participant_leave_body.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/participant_leave_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/participant_leave_body_participant_id.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/participant_leave_body_participant_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/participant_leave_body_user_external_id.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/participant_leave_body_user_external_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/participant_leave_body_user_id.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/participant_leave_body_user_id.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/participant_list_response.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/participant_list_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/participant_response.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/participant_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/participant_sub_schema.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/participant_sub_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/participant_with_user_external_id.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/participant_with_user_external_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/participant_with_user_id.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/participant_with_user_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/pass_control_body.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/pass_control_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/postback.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/postback.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/postback_webhook.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/postback_webhook.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/prechat_capture.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/prechat_capture.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/profile.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/quoted_message.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/quoted_message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/quoted_message_external_message_id.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/quoted_message_external_message_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/quoted_message_message.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/quoted_message_message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/referral.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/referral.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/referral_details.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/referral_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/reply.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/reply.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/source.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/source_webhook.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/source_webhook.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/status.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/status.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/switchboard.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/switchboard.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/switchboard_accept_control.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/switchboard_accept_control.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/switchboard_accept_control_all_of.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/switchboard_accept_control_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/switchboard_accept_control_all_of_payload.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/switchboard_accept_control_all_of_payload.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/switchboard_accept_control_failure.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/switchboard_accept_control_failure.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/switchboard_integration.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/switchboard_integration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/switchboard_accept_control_failure_all_of.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/switchboard_accept_control_failure_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/switchboard_accept_control_failure_all_of_payload.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/switchboard_accept_control_failure_all_of_payload.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/switchboard_integration_create_body.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/switchboard_integration_create_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/switchboard_integration_list_response.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/switchboard_integration_list_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/switchboard_integration_response.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/switchboard_integration_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/switchboard_integration_update_body.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/switchboard_integration_update_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/switchboard_integration_webhook.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/switchboard_integration_webhook.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/switchboard_list_response.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/switchboard_list_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/switchboard_offer_control.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/switchboard_offer_control.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/switchboard_offer_control_all_of.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/switchboard_offer_control_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/switchboard_offer_control_all_of_payload.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/switchboard_offer_control_all_of_payload.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/switchboard_offer_control_failure.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/switchboard_offer_control_failure.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/switchboard_pass_control.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/switchboard_pass_control.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/switchboard_pass_control_all_of.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/switchboard_pass_control_all_of.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/switchboard_pass_control_all_of_payload.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/switchboard_pass_control_all_of_payload.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/switchboard_pass_control_failure.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/switchboard_pass_control_failure.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/switchboard_response.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/switchboard_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/switchboard_update_body.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/switchboard_update_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/target.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/target.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/telegram.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/telegram.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/telegram_all_of.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/telegram_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/telegram_update.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/telegram_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/template_message.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/template_message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/text_message.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/text_message.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/twilio.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/twilio.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/twilio_all_of.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/twilio_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/twilio_update.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/twilio_update.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/twitter.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/twitter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/twitter_all_of.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/twitter_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/twitter_update.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/twitter_update.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/user.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/user_all_of.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/user_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/user_create_body.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/user_create_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/user_merge_event.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/user_merge_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/user_merge_event_all_of.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/user_merge_event_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/user_merge_event_all_of_payload.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/user_merge_event_all_of_payload.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/user_merge_event_all_of_payload_merged_clients.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/user_merge_event_all_of_payload_merged_clients.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/user_merge_event_all_of_payload_merged_conversations.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/user_merge_event_all_of_payload_merged_conversations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/user_merge_event_all_of_payload_merged_users.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/user_merge_event_all_of_payload_merged_users.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/user_response.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/user_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/user_truncated.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/user_truncated.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/user_update_body.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/user_update_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/user_update_event.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/user_update_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/user_update_event_all_of.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/user_update_event_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/user_update_event_all_of_payload.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/user_update_event_all_of_payload.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/viber.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/viber.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/viber_all_of.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/viber_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/viber_update.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/custom_update.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -18,15 +18,15 @@
 from sunshine_conversations_client.undefined import Undefined
 
 try:
     IntegrationUpdateBase = __import__("sunshine_conversations_client.model."+re.sub(r'(?<!^)(?=[A-Z])', '_', "IntegrationUpdateBase").lower(), fromlist=("IntegrationUpdateBase")).IntegrationUpdateBase
 except ImportError:
     pass
 
-class ViberUpdate(IntegrationUpdateBase):
+class CustomUpdate(IntegrationUpdateBase):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -41,15 +41,15 @@
 
     attribute_map = {
     }
 
     nulls = set()
 
     def __init__(self, local_vars_configuration=None, **kwargs):  # noqa: E501
-        """ViberUpdate - a model defined in OpenAPI"""  # noqa: E501
+        """CustomUpdate - a model defined in OpenAPI"""  # noqa: E501
         super().__init__(**kwargs)
 
         if (super().openapi_types is not None):
             all_types = super().openapi_types.copy()
             all_types.update(self.openapi_types)
             self.openapi_types = all_types
 
@@ -93,18 +93,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ViberUpdate):
+        if not isinstance(other, CustomUpdate):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, ViberUpdate):
+        if not isinstance(other, CustomUpdate):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/web.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/web.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/web_all_of.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/web_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/web_update.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/web_update.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/web_update_all_of.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/web_update_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/webhook.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/webhook.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/webhook_body.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/webhook_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/webhook_create_body.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/webhook_create_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/webhook_list_response.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/webhook_list_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/webhook_response.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/webhook_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/webhook_sub_schema.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/webhook_sub_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/webview.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/webview.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/whats_app_update.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/whats_app_update.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/whats_app_update_all_of.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/whats_app_update_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/whatsapp.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/whatsapp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/model/whatsapp_all_of.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/model/whatsapp_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/__init__.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # coding: utf-8
 
 # flake8: noqa
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "9.8.0"
+__version__ = "9.9.0"
 
 # import apis into sdk package
 from sunshine_conversations_client.api.activities_api import ActivitiesApi
 from sunshine_conversations_client.api.app_keys_api import AppKeysApi
 from sunshine_conversations_client.api.apps_api import AppsApi
 from sunshine_conversations_client.api.attachments_api import AttachmentsApi
 from sunshine_conversations_client.api.clients_api import ClientsApi
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/api_client.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
 import atexit
 import datetime
@@ -72,15 +72,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/9.8.0/python'
+        self.user_agent = 'OpenAPI-Generator/9.9.0/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/configuration.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import copy
@@ -353,16 +353,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 9.8.0\n"\
-               "SDK Package Version: 9.8.0".\
+               "Version of the API: 9.9.0\n"\
+               "SDK Package Version: 9.9.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/exceptions.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import six
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client/rest.py` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import io
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client.egg-info/PKG-INFO` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sunshine-conversations-client
-Version: 9.8.0
+Version: 9.9.0
 Summary: Sunshine Conversations API
 Home-page: UNKNOWN
 Author: OpenAPI Generator community
 Author-email: team@openapitools.org
 License: UNKNOWN
 Description:         The Python package for the Sunshine Conversations API
```

### Comparing `sunshine-conversations-client-9.8.0/sunshine_conversations_client.egg-info/SOURCES.txt` & `sunshine-conversations-client-9.9.0/sunshine_conversations_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sunshine-conversations-client-9.8.0/README.md` & `sunshine-conversations-client-9.9.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # sunshine-conversations-client
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 9.8.0
-- Package version: 9.8.0
+- API version: 9.9.0
+- Package version: 9.9.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation & Usage
```

### Comparing `sunshine-conversations-client-9.8.0/setup.py` & `sunshine-conversations-client-9.9.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # coding: utf-8
 
 """
     Sunshine Conversations API
 
-    The version of the OpenAPI document: 9.8.0
+    The version of the OpenAPI document: 9.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "sunshine-conversations-client"
-VERSION = "9.8.0"
+VERSION = "9.9.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `sunshine-conversations-client-9.8.0/PKG-INFO` & `sunshine-conversations-client-9.9.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sunshine-conversations-client
-Version: 9.8.0
+Version: 9.9.0
 Summary: Sunshine Conversations API
 Home-page: UNKNOWN
 Author: OpenAPI Generator community
 Author-email: team@openapitools.org
 License: UNKNOWN
 Description:         The Python package for the Sunshine Conversations API
```

