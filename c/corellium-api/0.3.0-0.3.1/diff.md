# Comparing `tmp/corellium-api-0.3.0.tar.gz` & `tmp/corellium-api-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corellium-api-0.3.0.tar", last modified: Wed Apr 19 23:37:42 2023, max compression
+gzip compressed data, was "corellium-api-0.3.1.tar", last modified: Fri Apr 21 19:24:27 2023, max compression
```

## Comparing `corellium-api-0.3.0.tar` & `corellium-api-0.3.1.tar`

### file list

```diff
@@ -1,228 +1,232 @@
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-04-19 23:37:42.987334 corellium-api-0.3.0/
--rw-r--r--   0 sam       (1000) sam       (1000)      319 2023-04-19 23:37:42.987334 corellium-api-0.3.0/PKG-INFO
--rw-r--r--   0 sam       (1000) sam       (1000)    28293 2023-04-19 23:26:46.000000 corellium-api-0.3.0/README.md
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-04-19 23:37:42.891338 corellium-api-0.3.0/corellium_api/
--rw-r--r--   0 sam       (1000) sam       (1000)     7298 2023-04-19 23:26:46.000000 corellium-api-0.3.0/corellium_api/__init__.py
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-04-19 23:37:42.891338 corellium-api-0.3.0/corellium_api/api/
--rw-r--r--   0 sam       (1000) sam       (1000)      144 2023-04-19 23:26:46.000000 corellium-api-0.3.0/corellium_api/api/__init__.py
--rw-r--r--   0 sam       (1000) sam       (1000)   856205 2023-04-19 23:26:46.000000 corellium-api-0.3.0/corellium_api/api/corellium_api.py
--rw-r--r--   0 sam       (1000) sam       (1000)    27761 2023-04-19 23:26:46.000000 corellium-api-0.3.0/corellium_api/api_client.py
--rw-r--r--   0 sam       (1000) sam       (1000)    16369 2023-04-19 23:26:46.000000 corellium-api-0.3.0/corellium_api/configuration.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5077 2023-04-19 23:26:46.000000 corellium-api-0.3.0/corellium_api/exceptions.py
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-04-19 23:37:42.951335 corellium-api-0.3.0/corellium_api/models/
--rw-r--r--   0 sam       (1000) sam       (1000)     6757 2023-04-19 23:26:46.000000 corellium-api-0.3.0/corellium_api/models/__init__.py
--rw-r--r--   0 sam       (1000) sam       (1000)     7295 2023-04-19 23:26:43.000000 corellium-api-0.3.0/corellium_api/models/address.py
--rw-r--r--   0 sam       (1000) sam       (1000)     7552 2023-04-19 23:26:43.000000 corellium-api-0.3.0/corellium_api/models/agent_app.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3856 2023-04-19 23:26:43.000000 corellium-api-0.3.0/corellium_api/models/agent_app_ready_response.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4353 2023-04-19 23:26:43.000000 corellium-api-0.3.0/corellium_api/models/agent_app_status.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4438 2023-04-19 23:26:43.000000 corellium-api-0.3.0/corellium_api/models/agent_apps_list.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4528 2023-04-19 23:26:43.000000 corellium-api-0.3.0/corellium_api/models/agent_apps_status_list.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5936 2023-04-19 23:26:43.000000 corellium-api-0.3.0/corellium_api/models/agent_error.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3596 2023-04-19 23:26:43.000000 corellium-api-0.3.0/corellium_api/models/agent_icons.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3648 2023-04-19 23:26:43.000000 corellium-api-0.3.0/corellium_api/models/agent_install_body.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3921 2023-04-19 23:26:43.000000 corellium-api-0.3.0/corellium_api/models/agent_profiles_return.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3683 2023-04-19 23:26:43.000000 corellium-api-0.3.0/corellium_api/models/agent_system_adb_auth.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3948 2023-04-19 23:26:43.000000 corellium-api-0.3.0/corellium_api/models/agent_system_get_prop_body.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3662 2023-04-19 23:26:43.000000 corellium-api-0.3.0/corellium_api/models/agent_value_return.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3803 2023-04-19 23:26:43.000000 corellium-api-0.3.0/corellium_api/models/agreed_ack.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5801 2023-04-19 23:26:43.000000 corellium-api-0.3.0/corellium_api/models/api_conflict_error.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5468 2023-04-19 23:26:43.000000 corellium-api-0.3.0/corellium_api/models/api_error.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5772 2023-04-19 23:26:43.000000 corellium-api-0.3.0/corellium_api/models/api_internal_consistency_error.py
--rw-r--r--   0 sam       (1000) sam       (1000)     6107 2023-04-19 23:26:43.000000 corellium-api-0.3.0/corellium_api/models/api_not_found_error.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3836 2023-04-19 23:26:43.000000 corellium-api-0.3.0/corellium_api/models/api_token.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3055 2023-04-19 23:26:43.000000 corellium-api-0.3.0/corellium_api/models/bit.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3704 2023-04-19 23:26:43.000000 corellium-api-0.3.0/corellium_api/models/btrace_enable_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3369 2023-04-19 23:26:43.000000 corellium-api-0.3.0/corellium_api/models/button.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5898 2023-04-19 23:26:43.000000 corellium-api-0.3.0/corellium_api/models/coupon_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3761 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/create_team.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5544 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/created_by.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4797 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/credentials.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4661 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/domain_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     8135 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/extension.py
--rw-r--r--   0 sam       (1000) sam       (1000)    16317 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/features.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5471 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/file_changes.py
--rw-r--r--   0 sam       (1000) sam       (1000)    13228 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/firmware.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4978 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/gpio_state_definition.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4898 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/gpios_state.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3712 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/grant_trial_request_response.py
--rw-r--r--   0 sam       (1000) sam       (1000)     9581 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/hook.py
--rw-r--r--   0 sam       (1000) sam       (1000)     9950 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/image.py
--rw-r--r--   0 sam       (1000) sam       (1000)    22906 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/instance.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4239 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/instance_agent_state.py
--rw-r--r--   0 sam       (1000) sam       (1000)     8955 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/instance_boot_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3479 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/instance_boot_options_additional_tag.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3682 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/instance_console_endpoint.py
--rw-r--r--   0 sam       (1000) sam       (1000)    14845 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/instance_create_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5707 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/instance_input.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5049 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/instance_netmon_proc_map_state.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4937 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/instance_netmon_state.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4549 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/instance_return.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3600 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/instance_services.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4511 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/instance_start_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3340 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/instance_state.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3679 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/instance_stop_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4522 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/instance_upgrade_body.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5003 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/invitation.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3608 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/invite_revoke_params.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3013 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/invite_revoke_params_ids.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4187 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/kcrange.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5587 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/kernel_task.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4973 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/kernel_thread.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4292 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/media_play_body.py
--rw-r--r--   0 sam       (1000) sam       (1000)     9967 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/model.py
--rw-r--r--   0 sam       (1000) sam       (1000)     6959 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/model_software.py
--rw-r--r--   0 sam       (1000) sam       (1000)     7408 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/net_mon_proc_map_filter.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5831 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/password_change_body.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5844 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/password_reset_body.py
--rw-r--r--   0 sam       (1000) sam       (1000)     6273 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/patch_instance_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     9478 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/peripherals_data.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4162 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/plan.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5173 2023-02-24 02:21:07.000000 corellium-api-0.3.0/corellium_api/models/plan_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     6358 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/project.py
--rw-r--r--   0 sam       (1000) sam       (1000)     8533 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/project_key.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4880 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/project_quota.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5102 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/project_settings.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5461 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/project_usage.py
--rw-r--r--   0 sam       (1000) sam       (1000)     6326 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/proxy_config.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5033 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/rate_info.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3885 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/reset_link_body.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5639 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/role.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4297 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/rotate_body.py
--rw-r--r--   0 sam       (1000) sam       (1000)     8024 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/snapshot.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3873 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/snapshot_creation_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4254 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/snapshot_status.py
--rw-r--r--   0 sam       (1000) sam       (1000)    13441 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/subscriber_invite.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5071 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/team.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3564 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/team_create.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3572 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/text_input.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4459 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/token.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4351 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/touch_curve_input.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3714 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/touch_input.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3829 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/trial.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5945 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/trial_extension.py
--rw-r--r--   0 sam       (1000) sam       (1000)     7578 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/trial_request_metadata.py
--rw-r--r--   0 sam       (1000) sam       (1000)     7298 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/trial_request_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3797 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/update_extension.py
--rw-r--r--   0 sam       (1000) sam       (1000)     6883 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/user.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5655 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/user_error.py
--rw-r--r--   0 sam       (1000) sam       (1000)     6961 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/v1_create_hook_parameters.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4008 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/v1_load_extension_parameters.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3781 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/v1_set_state_body.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5757 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/validation_error.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5174 2023-04-19 23:26:45.000000 corellium-api-0.3.0/corellium_api/models/volume_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4353 2023-04-19 23:26:45.000000 corellium-api-0.3.0/corellium_api/models/vpn_definition.py
--rw-r--r--   0 sam       (1000) sam       (1000)     7963 2023-04-19 23:26:45.000000 corellium-api-0.3.0/corellium_api/models/web_player_create_session_request.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5867 2023-04-19 23:26:45.000000 corellium-api-0.3.0/corellium_api/models/web_player_session.py
--rw-r--r--   0 sam       (1000) sam       (1000)     9860 2023-04-19 23:26:46.000000 corellium-api-0.3.0/corellium_api/rest.py
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-04-19 23:37:42.891338 corellium-api-0.3.0/corellium_api.egg-info/
--rw-r--r--   0 sam       (1000) sam       (1000)      319 2023-04-19 23:37:42.000000 corellium-api-0.3.0/corellium_api.egg-info/PKG-INFO
--rw-r--r--   0 sam       (1000) sam       (1000)     7540 2023-04-19 23:37:42.000000 corellium-api-0.3.0/corellium_api.egg-info/SOURCES.txt
--rw-r--r--   0 sam       (1000) sam       (1000)        1 2023-04-19 23:37:42.000000 corellium-api-0.3.0/corellium_api.egg-info/dependency_links.txt
--rw-r--r--   0 sam       (1000) sam       (1000)       57 2023-04-19 23:37:42.000000 corellium-api-0.3.0/corellium_api.egg-info/requires.txt
--rw-r--r--   0 sam       (1000) sam       (1000)       14 2023-04-19 23:37:42.000000 corellium-api-0.3.0/corellium_api.egg-info/top_level.txt
--rw-r--r--   0 sam       (1000) sam       (1000)       69 2023-04-19 23:37:42.987334 corellium-api-0.3.0/setup.cfg
--rw-r--r--   0 sam       (1000) sam       (1000)     1054 2023-04-19 23:26:46.000000 corellium-api-0.3.0/setup.py
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-04-19 23:37:42.987334 corellium-api-0.3.0/test/
--rw-r--r--   0 sam       (1000) sam       (1000)     1424 2023-04-19 23:26:43.000000 corellium-api-0.3.0/test/test_address.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1518 2023-04-19 23:26:43.000000 corellium-api-0.3.0/test/test_agent_app.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1458 2023-04-19 23:26:43.000000 corellium-api-0.3.0/test/test_agent_app_ready_response.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1384 2023-04-19 23:26:43.000000 corellium-api-0.3.0/test/test_agent_app_status.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1791 2023-04-19 23:26:43.000000 corellium-api-0.3.0/test/test_agent_apps_list.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1614 2023-04-19 23:26:43.000000 corellium-api-0.3.0/test/test_agent_apps_status_list.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1452 2023-04-19 23:26:43.000000 corellium-api-0.3.0/test/test_agent_error.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1304 2023-04-19 23:26:43.000000 corellium-api-0.3.0/test/test_agent_icons.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1368 2023-04-19 23:26:43.000000 corellium-api-0.3.0/test/test_agent_install_body.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1524 2023-04-19 23:26:43.000000 corellium-api-0.3.0/test/test_agent_profiles_return.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1397 2023-04-19 23:26:43.000000 corellium-api-0.3.0/test/test_agent_system_adb_auth.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1475 2023-04-19 23:26:43.000000 corellium-api-0.3.0/test/test_agent_system_get_prop_body.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1369 2023-04-19 23:26:43.000000 corellium-api-0.3.0/test/test_agent_value_return.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1374 2023-04-19 23:26:43.000000 corellium-api-0.3.0/test/test_agreed_ack.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1508 2023-04-19 23:26:43.000000 corellium-api-0.3.0/test/test_api_conflict_error.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1408 2023-04-19 23:26:43.000000 corellium-api-0.3.0/test/test_api_error.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1621 2023-04-19 23:26:43.000000 corellium-api-0.3.0/test/test_api_internal_consistency_error.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1522 2023-04-19 23:26:43.000000 corellium-api-0.3.0/test/test_api_not_found_error.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1315 2023-04-19 23:26:43.000000 corellium-api-0.3.0/test/test_api_token.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1195 2023-04-19 23:26:43.000000 corellium-api-0.3.0/test/test_bit.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1499 2023-04-19 23:26:43.000000 corellium-api-0.3.0/test/test_btrace_enable_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1228 2023-04-19 23:26:43.000000 corellium-api-0.3.0/test/test_button.py
--rw-r--r--   0 sam       (1000) sam       (1000)    21773 2023-04-19 23:26:46.000000 corellium-api-0.3.0/test/test_corellium_api.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1498 2023-04-19 23:26:43.000000 corellium-api-0.3.0/test/test_coupon_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1327 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_create_team.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1381 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_created_by.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1407 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_credentials.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1584 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_domain_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1532 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_extension.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1934 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_features.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1402 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_file_changes.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1880 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_firmware.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1691 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_gpio_state_definition.py
--rw-r--r--   0 sam       (1000) sam       (1000)     2097 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_gpios_state.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1469 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_grant_trial_request_response.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1503 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_hook.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1706 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_image.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3752 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_instance.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1418 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_instance_agent_state.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1686 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_instance_boot_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1522 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_instance_boot_options_additional_tag.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1444 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_instance_console_endpoint.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3029 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_instance_create_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)      840 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_instance_input.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1543 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_instance_netmon_proc_map_state.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1462 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_instance_netmon_state.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1428 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_instance_return.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1592 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_instance_services.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1449 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_instance_start_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1307 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_instance_state.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1403 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_instance_stop_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1455 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_instance_upgrade_body.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1367 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_invitation.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1391 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_invite_revoke_params.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1399 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_invite_revoke_params_ids.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1338 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_kcrange.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1655 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_kernel_task.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1427 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_kernel_thread.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1366 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_media_play_body.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1643 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_model.py
--rw-r--r--   0 sam       (1000) sam       (1000)     2366 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_model_software.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1837 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_net_mon_proc_map_filter.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1559 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_password_change_body.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1546 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_password_reset_body.py
--rw-r--r--   0 sam       (1000) sam       (1000)     2193 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_patch_instance_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1827 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_peripherals_data.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1263 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_plan.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1426 2023-02-24 02:21:07.000000 corellium-api-0.3.0/test/test_plan_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1931 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_project.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1702 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_project_key.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1392 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_project_quota.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1432 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_project_settings.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1422 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_project_usage.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1432 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_proxy_config.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1335 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_rate_info.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1364 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_reset_link_body.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1385 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_role.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1339 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_rotate_body.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1607 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_snapshot.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1472 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_snapshot_creation_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1377 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_snapshot_status.py
--rw-r--r--   0 sam       (1000) sam       (1000)     2289 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_subscriber_invite.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1606 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_team.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1298 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_team_create.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1289 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_text_input.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1380 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_token.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1389 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_touch_curve_input.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1306 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_touch_input.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1284 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_trial.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1450 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_trial_extension.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1572 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_trial_request_metadata.py
--rw-r--r--   0 sam       (1000) sam       (1000)     2081 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_trial_request_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1360 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_update_extension.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1463 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_user.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1428 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_user_error.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1662 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_v1_create_hook_parameters.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1504 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_v1_load_extension_parameters.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1381 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_v1_set_state_body.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1506 2023-04-19 23:26:45.000000 corellium-api-0.3.0/test/test_validation_error.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1456 2023-04-19 23:26:45.000000 corellium-api-0.3.0/test/test_volume_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1459 2023-04-19 23:26:45.000000 corellium-api-0.3.0/test/test_vpn_definition.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3400 2023-04-19 23:26:45.000000 corellium-api-0.3.0/test/test_web_player_create_session_request.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1537 2023-04-19 23:26:45.000000 corellium-api-0.3.0/test/test_web_player_session.py
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-04-21 19:24:27.562211 corellium-api-0.3.1/
+-rw-r--r--   0 sam       (1000) sam       (1000)      319 2023-04-21 19:24:27.562211 corellium-api-0.3.1/PKG-INFO
+-rw-r--r--   0 sam       (1000) sam       (1000)    27335 2023-04-21 19:24:00.000000 corellium-api-0.3.1/README.md
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-04-21 19:24:27.502213 corellium-api-0.3.1/corellium_api/
+-rw-r--r--   0 sam       (1000) sam       (1000)     7269 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/__init__.py
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-04-21 19:24:27.502213 corellium-api-0.3.1/corellium_api/api/
+-rw-r--r--   0 sam       (1000) sam       (1000)      144 2023-04-21 18:54:11.000000 corellium-api-0.3.1/corellium_api/api/__init__.py
+-rw-r--r--   0 sam       (1000) sam       (1000)   817635 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/api/corellium_api.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    27761 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/api_client.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    16369 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/configuration.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5077 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/exceptions.py
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-04-21 19:24:27.534211 corellium-api-0.3.1/corellium_api/models/
+-rw-r--r--   0 sam       (1000) sam       (1000)     6728 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/__init__.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     7295 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/address.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     7552 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/agent_app.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3856 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/agent_app_ready_response.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4353 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/agent_app_status.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4438 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/agent_apps_list.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4528 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/agent_apps_status_list.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5936 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/agent_error.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3596 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/agent_icons.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3648 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/agent_install_body.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3921 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/agent_profiles_return.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3683 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/agent_system_adb_auth.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3948 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/agent_system_get_prop_body.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3662 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/agent_value_return.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3803 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/agreed_ack.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5801 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/api_conflict_error.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5468 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/api_error.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5772 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/api_internal_consistency_error.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     6107 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/api_not_found_error.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3836 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/api_token.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3055 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/bit.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3704 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/btrace_enable_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3369 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/button.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5898 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/coupon_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3761 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/create_team.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5544 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/created_by.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4797 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/credentials.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4661 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/domain_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     8135 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/extension.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    16317 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/features.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5471 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/file_changes.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    13228 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/firmware.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4978 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/gpio_state_definition.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4898 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/gpios_state.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3712 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/grant_trial_request_response.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     9581 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/hook.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     9950 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/image.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    22839 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/instance.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4239 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/instance_agent_state.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     8955 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/instance_boot_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3479 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/instance_boot_options_additional_tag.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3682 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/instance_console_endpoint.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    14845 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/instance_create_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5707 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/instance_input.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4953 2023-04-21 18:54:09.000000 corellium-api-0.3.1/corellium_api/models/instance_netdump_state.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5049 2023-04-21 19:23:53.000000 corellium-api-0.3.1/corellium_api/models/instance_netmon_proc_map_state.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4937 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/instance_netmon_state.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4549 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/instance_return.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3600 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/instance_services.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4511 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/instance_start_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3340 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/instance_state.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3679 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/instance_stop_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4522 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/instance_upgrade_body.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5003 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/invitation.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3608 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/invite_revoke_params.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3013 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/invite_revoke_params_ids.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4187 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/kcrange.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5587 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/kernel_task.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4973 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/kernel_thread.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4292 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/media_play_body.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     9967 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/model.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     6959 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/model_software.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     7408 2023-04-21 19:23:53.000000 corellium-api-0.3.1/corellium_api/models/net_mon_proc_map_filter.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     7240 2023-04-21 18:54:09.000000 corellium-api-0.3.1/corellium_api/models/netdump_filter.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5831 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/password_change_body.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5844 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/password_reset_body.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     6273 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/patch_instance_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     9478 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/peripherals_data.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4162 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/plan.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5173 2023-04-21 19:23:53.000000 corellium-api-0.3.1/corellium_api/models/plan_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     6358 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/project.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     8533 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/project_key.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4880 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/project_quota.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5102 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/project_settings.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5461 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/project_usage.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     6326 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/proxy_config.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5033 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/rate_info.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3885 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/reset_link_body.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5639 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/role.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4297 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/rotate_body.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     8024 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/snapshot.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3873 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/snapshot_creation_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4254 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/snapshot_status.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    13441 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/subscriber_invite.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5071 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/team.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3564 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/team_create.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3572 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/text_input.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4459 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/token.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4351 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/touch_curve_input.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3714 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/touch_input.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3829 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/trial.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5945 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/trial_extension.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     7578 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/trial_request_metadata.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     7298 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/trial_request_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3797 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/update_extension.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     6883 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/user.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5655 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/user_error.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     6961 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/v1_create_hook_parameters.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4008 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/v1_load_extension_parameters.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3781 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/v1_set_state_body.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5757 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/validation_error.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5174 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/volume_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4353 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/vpn_definition.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     7963 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/web_player_create_session_request.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5867 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/web_player_session.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     9860 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/rest.py
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-04-21 19:24:27.502213 corellium-api-0.3.1/corellium_api.egg-info/
+-rw-r--r--   0 sam       (1000) sam       (1000)      319 2023-04-21 19:24:27.000000 corellium-api-0.3.1/corellium_api.egg-info/PKG-INFO
+-rw-r--r--   0 sam       (1000) sam       (1000)     7690 2023-04-21 19:24:27.000000 corellium-api-0.3.1/corellium_api.egg-info/SOURCES.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)        1 2023-04-21 19:24:27.000000 corellium-api-0.3.1/corellium_api.egg-info/dependency_links.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)       57 2023-04-21 19:24:27.000000 corellium-api-0.3.1/corellium_api.egg-info/requires.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)       14 2023-04-21 19:24:27.000000 corellium-api-0.3.1/corellium_api.egg-info/top_level.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)       69 2023-04-21 19:24:27.562211 corellium-api-0.3.1/setup.cfg
+-rw-r--r--   0 sam       (1000) sam       (1000)     1054 2023-04-21 19:24:00.000000 corellium-api-0.3.1/setup.py
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-04-21 19:24:27.558211 corellium-api-0.3.1/test/
+-rw-r--r--   0 sam       (1000) sam       (1000)     1424 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_address.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1518 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_agent_app.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1458 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_agent_app_ready_response.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1384 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_agent_app_status.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1791 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_agent_apps_list.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1614 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_agent_apps_status_list.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1452 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_agent_error.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1304 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_agent_icons.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1368 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_agent_install_body.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1524 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_agent_profiles_return.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1397 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_agent_system_adb_auth.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1475 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_agent_system_get_prop_body.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1369 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_agent_value_return.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1374 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_agreed_ack.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1508 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_api_conflict_error.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1408 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_api_error.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1621 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_api_internal_consistency_error.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1522 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_api_not_found_error.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1315 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_api_token.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1195 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_bit.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1499 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_btrace_enable_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1228 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_button.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    20787 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_corellium_api.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1498 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_coupon_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1327 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_create_team.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1381 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_created_by.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1407 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_credentials.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1584 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_domain_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1532 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_extension.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1934 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_features.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1402 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_file_changes.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1880 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_firmware.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1691 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_gpio_state_definition.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     2097 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_gpios_state.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1469 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_grant_trial_request_response.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1503 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_hook.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1706 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_image.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3732 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_instance.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1418 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_instance_agent_state.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1686 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_instance_boot_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1522 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_instance_boot_options_additional_tag.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1444 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_instance_console_endpoint.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3029 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_instance_create_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)      840 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_instance_input.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1473 2023-04-21 18:54:09.000000 corellium-api-0.3.1/test/test_instance_netdump_state.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1543 2023-04-21 19:23:53.000000 corellium-api-0.3.1/test/test_instance_netmon_proc_map_state.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1462 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_instance_netmon_state.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1428 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_instance_return.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1592 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_instance_services.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1449 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_instance_start_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1307 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_instance_state.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1403 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_instance_stop_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1455 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_instance_upgrade_body.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1367 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_invitation.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1391 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_invite_revoke_params.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1399 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_invite_revoke_params_ids.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1338 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_kcrange.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1655 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_kernel_task.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1427 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_kernel_thread.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1366 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_media_play_body.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1643 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_model.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     2366 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_model_software.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1837 2023-04-21 19:23:53.000000 corellium-api-0.3.1/test/test_net_mon_proc_map_filter.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1765 2023-04-21 18:54:09.000000 corellium-api-0.3.1/test/test_netdump_filter.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1559 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_password_change_body.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1546 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_password_reset_body.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     2193 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_patch_instance_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1827 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_peripherals_data.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1263 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_plan.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1426 2023-04-21 19:23:53.000000 corellium-api-0.3.1/test/test_plan_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1931 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_project.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1702 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_project_key.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1392 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_project_quota.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1432 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_project_settings.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1422 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_project_usage.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1432 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_proxy_config.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1335 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_rate_info.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1364 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_reset_link_body.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1385 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_role.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1339 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_rotate_body.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1607 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_snapshot.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1472 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_snapshot_creation_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1377 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_snapshot_status.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     2289 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_subscriber_invite.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1606 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_team.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1298 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_team_create.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1289 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_text_input.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1380 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_token.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1389 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_touch_curve_input.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1306 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_touch_input.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1284 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_trial.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1450 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_trial_extension.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1572 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_trial_request_metadata.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     2081 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_trial_request_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1360 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_update_extension.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1463 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_user.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1428 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_user_error.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1662 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_v1_create_hook_parameters.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1504 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_v1_load_extension_parameters.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1381 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_v1_set_state_body.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1506 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_validation_error.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1456 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_volume_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1459 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_vpn_definition.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3400 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_web_player_create_session_request.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1537 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_web_player_session.py
```

### Comparing `corellium-api-0.3.0/README.md` & `corellium-api-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # corellium-api
 REST API to manage your virtual devices.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 4.5.0-16740
-- Package version: 0.3.0
+- API version: 4.5.0-16757
+- Package version: 0.3.1
 - Build package: org.openapitools.codegen.languages.PythonLegacyClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation & Usage
@@ -132,27 +132,24 @@
 *CorelliumApi* | [**v1_create_hook**](docs/CorelliumApi.md#v1_create_hook) | **POST** /v1/instances/{instanceId}/hooks | Create hypervisor hook for Instance
 *CorelliumApi* | [**v1_create_image**](docs/CorelliumApi.md#v1_create_image) | **POST** /v1/images | Create a new Image
 *CorelliumApi* | [**v1_create_instance**](docs/CorelliumApi.md#v1_create_instance) | **POST** /v1/instances | Create Instance
 *CorelliumApi* | [**v1_create_project**](docs/CorelliumApi.md#v1_create_project) | **POST** /v1/projects | Create a Project
 *CorelliumApi* | [**v1_create_snapshot**](docs/CorelliumApi.md#v1_create_snapshot) | **POST** /v1/instances/{instanceId}/snapshots | Create Instance Snapshot
 *CorelliumApi* | [**v1_create_subscriber_invite**](docs/CorelliumApi.md#v1_create_subscriber_invite) | **POST** /v1/billing/invites | Create Subscriber Invite
 *CorelliumApi* | [**v1_create_user**](docs/CorelliumApi.md#v1_create_user) | **POST** /v1/users | Create User
-*CorelliumApi* | [**v1_delete_extension**](docs/CorelliumApi.md#v1_delete_extension) | **DELETE** /v1/extensions/{extensionId} | Delete an existing extension
 *CorelliumApi* | [**v1_delete_hook**](docs/CorelliumApi.md#v1_delete_hook) | **DELETE** /v1/hooks/{hookId} | Delete an existing hypervisor hook
 *CorelliumApi* | [**v1_delete_image**](docs/CorelliumApi.md#v1_delete_image) | **DELETE** /v2/images/{imageId} | Delete Image
 *CorelliumApi* | [**v1_delete_instance**](docs/CorelliumApi.md#v1_delete_instance) | **DELETE** /v1/instances/{instanceId} | Remove Instance
 *CorelliumApi* | [**v1_delete_instance_snapshot**](docs/CorelliumApi.md#v1_delete_instance_snapshot) | **DELETE** /v1/instances/{instanceId}/snapshots/{snapshotId} | Delete a Snapshot
 *CorelliumApi* | [**v1_delete_project**](docs/CorelliumApi.md#v1_delete_project) | **DELETE** /v1/projects/{projectId} | Delete a Project
 *CorelliumApi* | [**v1_delete_snapshot**](docs/CorelliumApi.md#v1_delete_snapshot) | **DELETE** /v1/snapshots/{snapshotId} | Delete a Snapshot
 *CorelliumApi* | [**v1_delete_user**](docs/CorelliumApi.md#v1_delete_user) | **DELETE** /v1/users/{userId} | Delete User
 *CorelliumApi* | [**v1_disable_expose_port**](docs/CorelliumApi.md#v1_disable_expose_port) | **POST** /v1/instances/{instanceId}/exposeport/disable | Disable an exposed port on an instance for device access.
 *CorelliumApi* | [**v1_enable_expose_port**](docs/CorelliumApi.md#v1_enable_expose_port) | **POST** /v1/instances/{instanceId}/exposeport/enable | Enable an exposed port on an instance for device access.
 *CorelliumApi* | [**v1_execute_hyper_trace_hooks**](docs/CorelliumApi.md#v1_execute_hyper_trace_hooks) | **POST** /v1/instances/{instanceId}/hooks/execute | Execute Hooks on an instance
-*CorelliumApi* | [**v1_get_extension_by_id**](docs/CorelliumApi.md#v1_get_extension_by_id) | **GET** /v1/extensions/{extensionId} | Get extension by id
-*CorelliumApi* | [**v1_get_extensions**](docs/CorelliumApi.md#v1_get_extensions) | **GET** /v1/extensions | Get all extensions
 *CorelliumApi* | [**v1_get_hook_by_id**](docs/CorelliumApi.md#v1_get_hook_by_id) | **GET** /v1/hooks/{hookId} | Get hypervisor hook by id
 *CorelliumApi* | [**v1_get_hooks**](docs/CorelliumApi.md#v1_get_hooks) | **GET** /v1/instances/{instanceId}/hooks | Get all hypervisor hooks for Instance
 *CorelliumApi* | [**v1_get_image**](docs/CorelliumApi.md#v1_get_image) | **GET** /v1/images/{imageId} | Get Image Metadata
 *CorelliumApi* | [**v1_get_images**](docs/CorelliumApi.md#v1_get_images) | **GET** /v1/images | Get all Images Metadata
 *CorelliumApi* | [**v1_get_instance**](docs/CorelliumApi.md#v1_get_instance) | **GET** /v1/instances/{instanceId} | Get Instance
 *CorelliumApi* | [**v1_get_instance_console**](docs/CorelliumApi.md#v1_get_instance_console) | **GET** /v1/instances/{instanceId}/console | Get console websocket URL
 *CorelliumApi* | [**v1_get_instance_console_log**](docs/CorelliumApi.md#v1_get_instance_console_log) | **GET** /v1/instances/{instanceId}/consoleLog | Get Console Log
@@ -172,18 +169,16 @@
 *CorelliumApi* | [**v1_get_project_vpn_config**](docs/CorelliumApi.md#v1_get_project_vpn_config) | **GET** /v1/projects/{projectId}/vpnconfig/{format} | Get Project VPN Configuration
 *CorelliumApi* | [**v1_get_projects**](docs/CorelliumApi.md#v1_get_projects) | **GET** /v1/projects | Get Projects
 *CorelliumApi* | [**v1_get_reset_link_info**](docs/CorelliumApi.md#v1_get_reset_link_info) | **GET** /v1/users/reset-link-info | Send Password Reset Link Info
 *CorelliumApi* | [**v1_get_snapshot**](docs/CorelliumApi.md#v1_get_snapshot) | **GET** /v1/snapshots/{snapshotId} | Get Snapshot
 *CorelliumApi* | [**v1_instances_instance_id_message_post**](docs/CorelliumApi.md#v1_instances_instance_id_message_post) | **POST** /v1/instances/{instanceId}/message | Receive a message on an iOS vm
 *CorelliumApi* | [**v1_kcrange**](docs/CorelliumApi.md#v1_kcrange) | **GET** /v1/instances/{instanceId}/btrace-kcrange | Get Kernel extension ranges
 *CorelliumApi* | [**v1_list_threads**](docs/CorelliumApi.md#v1_list_threads) | **GET** /v1/instances/{instanceId}/strace/thread-list | Get Running Threads (CoreTrace)
-*CorelliumApi* | [**v1_load_extension**](docs/CorelliumApi.md#v1_load_extension) | **POST** /v1/extensions | Load an extension
 *CorelliumApi* | [**v1_media_play**](docs/CorelliumApi.md#v1_media_play) | **POST** /v1/instances/{instanceId}/media/play | Start playing media
 *CorelliumApi* | [**v1_media_stop**](docs/CorelliumApi.md#v1_media_stop) | **POST** /v1/instances/{instanceId}/media/stop | Stop playing media
-*CorelliumApi* | [**v1_parse_extension_json**](docs/CorelliumApi.md#v1_parse_extension_json) | **POST** /v1/extensions/parse/extension.json | Validates extension.json
 *CorelliumApi* | [**v1_patch_instance**](docs/CorelliumApi.md#v1_patch_instance) | **PATCH** /v1/instances/{instanceId} | Update Instance
 *CorelliumApi* | [**v1_pause_instance**](docs/CorelliumApi.md#v1_pause_instance) | **POST** /v1/instances/{instanceId}/pause | Pause an Instance
 *CorelliumApi* | [**v1_post_instance_input**](docs/CorelliumApi.md#v1_post_instance_input) | **POST** /v1/instances/{instanceId}/input | Provide Instance Input
 *CorelliumApi* | [**v1_ready**](docs/CorelliumApi.md#v1_ready) | **GET** /v1/ready | API Status
 *CorelliumApi* | [**v1_reboot_instance**](docs/CorelliumApi.md#v1_reboot_instance) | **POST** /v1/instances/{instanceId}/reboot | Reboot an Instance
 *CorelliumApi* | [**v1_remove_project_key**](docs/CorelliumApi.md#v1_remove_project_key) | **DELETE** /v1/projects/{projectId}/keys/{keyId} | Delete Project Authorized Key
 *CorelliumApi* | [**v1_remove_team_role_from_project**](docs/CorelliumApi.md#v1_remove_team_role_from_project) | **DELETE** /v1/roles/projects/{projectId}/teams/{teamId}/roles/{roleId} | Remove team role from project
@@ -199,27 +194,26 @@
 *CorelliumApi* | [**v1_set_instance_gpios**](docs/CorelliumApi.md#v1_set_instance_gpios) | **PUT** /v1/instances/{instanceId}/gpios | Set Instance GPIOs
 *CorelliumApi* | [**v1_set_instance_peripherals**](docs/CorelliumApi.md#v1_set_instance_peripherals) | **PUT** /v1/instances/{instanceId}/peripherals | Set Instance Peripherals
 *CorelliumApi* | [**v1_set_instance_state**](docs/CorelliumApi.md#v1_set_instance_state) | **PUT** /v1/instances/{instanceId}/state | Set state of Instance
 *CorelliumApi* | [**v1_snapshot_rename**](docs/CorelliumApi.md#v1_snapshot_rename) | **PATCH** /v1/snapshots/{snapshotId} | Rename a Snapshot
 *CorelliumApi* | [**v1_start_core_trace**](docs/CorelliumApi.md#v1_start_core_trace) | **POST** /v1/instances/{instanceId}/strace/enable | Start CoreTrace on an instance
 *CorelliumApi* | [**v1_start_hyper_trace**](docs/CorelliumApi.md#v1_start_hyper_trace) | **POST** /v1/instances/{instanceId}/btrace/enable | Start HyperTrace on an instance
 *CorelliumApi* | [**v1_start_instance**](docs/CorelliumApi.md#v1_start_instance) | **POST** /v1/instances/{instanceId}/start | Start an Instance
-*CorelliumApi* | [**v1_start_net_mon_proc_map**](docs/CorelliumApi.md#v1_start_net_mon_proc_map) | **POST** /v1/instances/{instanceId}/netmonprocmap/enable | Start Enhanced Network Monitor on an instance.
+*CorelliumApi* | [**v1_start_netdump**](docs/CorelliumApi.md#v1_start_netdump) | **POST** /v1/instances/{instanceId}/netdump/enable | Start Enhanced Network Monitor on an instance.
 *CorelliumApi* | [**v1_start_network_monitor**](docs/CorelliumApi.md#v1_start_network_monitor) | **POST** /v1/instances/{instanceId}/sslsplit/enable | Start Network Monitor on an instance.
 *CorelliumApi* | [**v1_stop_core_trace**](docs/CorelliumApi.md#v1_stop_core_trace) | **POST** /v1/instances/{instanceId}/strace/disable | Stop CoreTrace on an instance.
 *CorelliumApi* | [**v1_stop_hyper_trace**](docs/CorelliumApi.md#v1_stop_hyper_trace) | **POST** /v1/instances/{instanceId}/btrace/disable | Stop HyperTrace on an instance.
 *CorelliumApi* | [**v1_stop_instance**](docs/CorelliumApi.md#v1_stop_instance) | **POST** /v1/instances/{instanceId}/stop | Stop an Instance
-*CorelliumApi* | [**v1_stop_net_mon_proc_map**](docs/CorelliumApi.md#v1_stop_net_mon_proc_map) | **POST** /v1/instances/{instanceId}/netmonprocmap/disable | Stop Enhanced Network Monitor on an instance.
+*CorelliumApi* | [**v1_stop_netdump**](docs/CorelliumApi.md#v1_stop_netdump) | **POST** /v1/instances/{instanceId}/netdump/disable | Stop Enhanced Network Monitor on an instance.
 *CorelliumApi* | [**v1_stop_network_monitor**](docs/CorelliumApi.md#v1_stop_network_monitor) | **POST** /v1/instances/{instanceId}/sslsplit/disable | Stop Network Monitor on an instance.
 *CorelliumApi* | [**v1_team_change**](docs/CorelliumApi.md#v1_team_change) | **PATCH** /v1/teams/{teamId} | Update team
 *CorelliumApi* | [**v1_team_create**](docs/CorelliumApi.md#v1_team_create) | **POST** /v1/teams | Create team
 *CorelliumApi* | [**v1_team_delete**](docs/CorelliumApi.md#v1_team_delete) | **DELETE** /v1/teams/{teamId} | Delete team
 *CorelliumApi* | [**v1_teams**](docs/CorelliumApi.md#v1_teams) | **GET** /v1/teams | Get teams
 *CorelliumApi* | [**v1_unpause_instance**](docs/CorelliumApi.md#v1_unpause_instance) | **POST** /v1/instances/{instanceId}/unpause | Unpause an Instance
-*CorelliumApi* | [**v1_update_extension**](docs/CorelliumApi.md#v1_update_extension) | **PUT** /v1/extensions/{extensionId} | Update an existing extension
 *CorelliumApi* | [**v1_update_hook**](docs/CorelliumApi.md#v1_update_hook) | **PUT** /v1/hooks/{hookId} | Update an existing hypervisor hook
 *CorelliumApi* | [**v1_update_project**](docs/CorelliumApi.md#v1_update_project) | **PATCH** /v1/projects/{projectId} | Update a Project
 *CorelliumApi* | [**v1_update_project_settings**](docs/CorelliumApi.md#v1_update_project_settings) | **PATCH** /v1/projects/{projectId}/settings | Change Project Settings
 *CorelliumApi* | [**v1_update_user**](docs/CorelliumApi.md#v1_update_user) | **PATCH** /v1/users/{userId} | Update User
 *CorelliumApi* | [**v1_upgrade_instance**](docs/CorelliumApi.md#v1_upgrade_instance) | **POST** /v1/instances/{instanceId}/upgrade | Upgrade iOS version
 *CorelliumApi* | [**v1_upload_image_data**](docs/CorelliumApi.md#v1_upload_image_data) | **POST** /v1/images/{imageId} | Upload Image Data
 *CorelliumApi* | [**v1_user_agree_terms**](docs/CorelliumApi.md#v1_user_agree_terms) | **POST** /v1/users/agree | Consent to the current terms and conditions
@@ -270,15 +264,15 @@
  - [Instance](docs/Instance.md)
  - [InstanceAgentState](docs/InstanceAgentState.md)
  - [InstanceBootOptions](docs/InstanceBootOptions.md)
  - [InstanceBootOptionsAdditionalTag](docs/InstanceBootOptionsAdditionalTag.md)
  - [InstanceConsoleEndpoint](docs/InstanceConsoleEndpoint.md)
  - [InstanceCreateOptions](docs/InstanceCreateOptions.md)
  - [InstanceInput](docs/InstanceInput.md)
- - [InstanceNetmonProcMapState](docs/InstanceNetmonProcMapState.md)
+ - [InstanceNetdumpState](docs/InstanceNetdumpState.md)
  - [InstanceNetmonState](docs/InstanceNetmonState.md)
  - [InstanceReturn](docs/InstanceReturn.md)
  - [InstanceServices](docs/InstanceServices.md)
  - [InstanceStartOptions](docs/InstanceStartOptions.md)
  - [InstanceState](docs/InstanceState.md)
  - [InstanceStopOptions](docs/InstanceStopOptions.md)
  - [InstanceUpgradeBody](docs/InstanceUpgradeBody.md)
@@ -287,15 +281,15 @@
  - [InviteRevokeParamsIds](docs/InviteRevokeParamsIds.md)
  - [Kcrange](docs/Kcrange.md)
  - [KernelTask](docs/KernelTask.md)
  - [KernelThread](docs/KernelThread.md)
  - [MediaPlayBody](docs/MediaPlayBody.md)
  - [Model](docs/Model.md)
  - [ModelSoftware](docs/ModelSoftware.md)
- - [NetMonProcMapFilter](docs/NetMonProcMapFilter.md)
+ - [NetdumpFilter](docs/NetdumpFilter.md)
  - [PasswordChangeBody](docs/PasswordChangeBody.md)
  - [PasswordResetBody](docs/PasswordResetBody.md)
  - [PatchInstanceOptions](docs/PatchInstanceOptions.md)
  - [PeripheralsData](docs/PeripheralsData.md)
  - [Plan](docs/Plan.md)
  - [Project](docs/Project.md)
  - [ProjectKey](docs/ProjectKey.md)
```

### Comparing `corellium-api-0.3.0/corellium_api/__init__.py` & `corellium-api-0.3.1/corellium_api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 # flake8: noqa
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "0.3.0"
+__version__ = "0.3.1"
 
 # import apis into sdk package
 from corellium_api.api.corellium_api import CorelliumApi
 
 # import ApiClient
 from corellium_api.api_client import ApiClient
 from corellium_api.configuration import Configuration
@@ -68,15 +68,15 @@
 from corellium_api.models.instance import Instance
 from corellium_api.models.instance_agent_state import InstanceAgentState
 from corellium_api.models.instance_boot_options import InstanceBootOptions
 from corellium_api.models.instance_boot_options_additional_tag import InstanceBootOptionsAdditionalTag
 from corellium_api.models.instance_console_endpoint import InstanceConsoleEndpoint
 from corellium_api.models.instance_create_options import InstanceCreateOptions
 from corellium_api.models.instance_input import InstanceInput
-from corellium_api.models.instance_netmon_proc_map_state import InstanceNetmonProcMapState
+from corellium_api.models.instance_netdump_state import InstanceNetdumpState
 from corellium_api.models.instance_netmon_state import InstanceNetmonState
 from corellium_api.models.instance_return import InstanceReturn
 from corellium_api.models.instance_services import InstanceServices
 from corellium_api.models.instance_start_options import InstanceStartOptions
 from corellium_api.models.instance_state import InstanceState
 from corellium_api.models.instance_stop_options import InstanceStopOptions
 from corellium_api.models.instance_upgrade_body import InstanceUpgradeBody
@@ -85,15 +85,15 @@
 from corellium_api.models.invite_revoke_params_ids import InviteRevokeParamsIds
 from corellium_api.models.kcrange import Kcrange
 from corellium_api.models.kernel_task import KernelTask
 from corellium_api.models.kernel_thread import KernelThread
 from corellium_api.models.media_play_body import MediaPlayBody
 from corellium_api.models.model import Model
 from corellium_api.models.model_software import ModelSoftware
-from corellium_api.models.net_mon_proc_map_filter import NetMonProcMapFilter
+from corellium_api.models.netdump_filter import NetdumpFilter
 from corellium_api.models.password_change_body import PasswordChangeBody
 from corellium_api.models.password_reset_body import PasswordResetBody
 from corellium_api.models.patch_instance_options import PatchInstanceOptions
 from corellium_api.models.peripherals_data import PeripheralsData
 from corellium_api.models.plan import Plan
 from corellium_api.models.project import Project
 from corellium_api.models.project_key import ProjectKey
```

### Comparing `corellium-api-0.3.0/corellium_api/api/corellium_api.py` & `corellium-api-0.3.1/corellium_api/api/corellium_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -6013,148 +6013,14 @@
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
-    def v1_delete_extension(self, extension_id, **kwargs):  # noqa: E501
-        """Delete an existing extension  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.v1_delete_extension(extension_id, async_req=True)
-        >>> result = thread.get()
-
-        :param extension_id: Extension ID (required)
-        :type extension_id: str
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: None
-        """
-        kwargs['_return_http_data_only'] = True
-        return self.v1_delete_extension_with_http_info(extension_id, **kwargs)  # noqa: E501
-
-    def v1_delete_extension_with_http_info(self, extension_id, **kwargs):  # noqa: E501
-        """Delete an existing extension  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.v1_delete_extension_with_http_info(extension_id, async_req=True)
-        >>> result = thread.get()
-
-        :param extension_id: Extension ID (required)
-        :type extension_id: str
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the authentication
-                              in the spec for a single request.
-        :type _request_auth: dict, optional
-        :type _content_type: string, optional: force content-type for the request
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: None
-        """
-
-        local_var_params = locals()
-
-        all_params = [
-            'extension_id'
-        ]
-        all_params.extend(
-            [
-                'async_req',
-                '_return_http_data_only',
-                '_preload_content',
-                '_request_timeout',
-                '_request_auth',
-                '_content_type',
-                '_headers'
-            ]
-        )
-
-        for key, val in six.iteritems(local_var_params['kwargs']):
-            if key not in all_params:
-                raise ApiTypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method v1_delete_extension" % key
-                )
-            local_var_params[key] = val
-        del local_var_params['kwargs']
-        # verify the required parameter 'extension_id' is set
-        if self.api_client.client_side_validation and ('extension_id' not in local_var_params or  # noqa: E501
-                                                        local_var_params['extension_id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `extension_id` when calling `v1_delete_extension`")  # noqa: E501
-
-        collection_formats = {}
-
-        path_params = {}
-        if 'extension_id' in local_var_params:
-            path_params['extensionId'] = local_var_params['extension_id']  # noqa: E501
-
-        query_params = []
-
-        header_params = dict(local_var_params.get('_headers', {}))
-
-        form_params = []
-        local_var_files = {}
-
-        body_params = None
-        # HTTP header `Accept`
-        header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
-
-        # Authentication setting
-        auth_settings = ['BearerAuth']  # noqa: E501
-
-        response_types_map = {}
-
-        return self.api_client.call_api(
-            '/v1/extensions/{extensionId}', 'DELETE',
-            path_params,
-            query_params,
-            header_params,
-            body=body_params,
-            post_params=form_params,
-            files=local_var_files,
-            response_types_map=response_types_map,
-            auth_settings=auth_settings,
-            async_req=local_var_params.get('async_req'),
-            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
-            _preload_content=local_var_params.get('_preload_content', True),
-            _request_timeout=local_var_params.get('_request_timeout'),
-            collection_formats=collection_formats,
-            _request_auth=local_var_params.get('_request_auth'))
-
     def v1_delete_hook(self, hook_id, **kwargs):  # noqa: E501
         """Delete an existing hypervisor hook  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.v1_delete_hook(hook_id, async_req=True)
@@ -7501,301 +7367,14 @@
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
-    def v1_get_extension_by_id(self, extension_id, **kwargs):  # noqa: E501
-        """Get extension by id  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.v1_get_extension_by_id(extension_id, async_req=True)
-        >>> result = thread.get()
-
-        :param extension_id: Extension Id (required)
-        :type extension_id: str
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: Extension
-        """
-        kwargs['_return_http_data_only'] = True
-        return self.v1_get_extension_by_id_with_http_info(extension_id, **kwargs)  # noqa: E501
-
-    def v1_get_extension_by_id_with_http_info(self, extension_id, **kwargs):  # noqa: E501
-        """Get extension by id  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.v1_get_extension_by_id_with_http_info(extension_id, async_req=True)
-        >>> result = thread.get()
-
-        :param extension_id: Extension Id (required)
-        :type extension_id: str
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the authentication
-                              in the spec for a single request.
-        :type _request_auth: dict, optional
-        :type _content_type: string, optional: force content-type for the request
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: tuple(Extension, status_code(int), headers(HTTPHeaderDict))
-        """
-
-        local_var_params = locals()
-
-        all_params = [
-            'extension_id'
-        ]
-        all_params.extend(
-            [
-                'async_req',
-                '_return_http_data_only',
-                '_preload_content',
-                '_request_timeout',
-                '_request_auth',
-                '_content_type',
-                '_headers'
-            ]
-        )
-
-        for key, val in six.iteritems(local_var_params['kwargs']):
-            if key not in all_params:
-                raise ApiTypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method v1_get_extension_by_id" % key
-                )
-            local_var_params[key] = val
-        del local_var_params['kwargs']
-        # verify the required parameter 'extension_id' is set
-        if self.api_client.client_side_validation and ('extension_id' not in local_var_params or  # noqa: E501
-                                                        local_var_params['extension_id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `extension_id` when calling `v1_get_extension_by_id`")  # noqa: E501
-
-        collection_formats = {}
-
-        path_params = {}
-        if 'extension_id' in local_var_params:
-            path_params['extensionId'] = local_var_params['extension_id']  # noqa: E501
-
-        query_params = []
-
-        header_params = dict(local_var_params.get('_headers', {}))
-
-        form_params = []
-        local_var_files = {}
-
-        body_params = None
-        # HTTP header `Accept`
-        header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
-
-        # Authentication setting
-        auth_settings = ['BearerAuth']  # noqa: E501
-
-        response_types_map = {
-            200: "Extension",
-            400: "UserError",
-            403: "ApiError",
-        }
-
-        return self.api_client.call_api(
-            '/v1/extensions/{extensionId}', 'GET',
-            path_params,
-            query_params,
-            header_params,
-            body=body_params,
-            post_params=form_params,
-            files=local_var_files,
-            response_types_map=response_types_map,
-            auth_settings=auth_settings,
-            async_req=local_var_params.get('async_req'),
-            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
-            _preload_content=local_var_params.get('_preload_content', True),
-            _request_timeout=local_var_params.get('_request_timeout'),
-            collection_formats=collection_formats,
-            _request_auth=local_var_params.get('_request_auth'))
-
-    def v1_get_extensions(self, **kwargs):  # noqa: E501
-        """Get all extensions  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.v1_get_extensions(async_req=True)
-        >>> result = thread.get()
-
-        :param limit: limit for pagination results, defaults to 20
-        :type limit: float
-        :param offset: offset for pagination results, defaults to 0
-        :type offset: float
-        :param if_none_match: sha256sum of the last response with the same parameters (optional)
-        :type if_none_match: str
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: list[Extension]
-        """
-        kwargs['_return_http_data_only'] = True
-        return self.v1_get_extensions_with_http_info(**kwargs)  # noqa: E501
-
-    def v1_get_extensions_with_http_info(self, **kwargs):  # noqa: E501
-        """Get all extensions  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.v1_get_extensions_with_http_info(async_req=True)
-        >>> result = thread.get()
-
-        :param limit: limit for pagination results, defaults to 20
-        :type limit: float
-        :param offset: offset for pagination results, defaults to 0
-        :type offset: float
-        :param if_none_match: sha256sum of the last response with the same parameters (optional)
-        :type if_none_match: str
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the authentication
-                              in the spec for a single request.
-        :type _request_auth: dict, optional
-        :type _content_type: string, optional: force content-type for the request
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: tuple(list[Extension], status_code(int), headers(HTTPHeaderDict))
-        """
-
-        local_var_params = locals()
-
-        all_params = [
-            'limit',
-            'offset',
-            'if_none_match'
-        ]
-        all_params.extend(
-            [
-                'async_req',
-                '_return_http_data_only',
-                '_preload_content',
-                '_request_timeout',
-                '_request_auth',
-                '_content_type',
-                '_headers'
-            ]
-        )
-
-        for key, val in six.iteritems(local_var_params['kwargs']):
-            if key not in all_params:
-                raise ApiTypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method v1_get_extensions" % key
-                )
-            local_var_params[key] = val
-        del local_var_params['kwargs']
-
-        collection_formats = {}
-
-        path_params = {}
-
-        query_params = []
-        if 'limit' in local_var_params and local_var_params['limit'] is not None:  # noqa: E501
-            query_params.append(('limit', local_var_params['limit']))  # noqa: E501
-        if 'offset' in local_var_params and local_var_params['offset'] is not None:  # noqa: E501
-            query_params.append(('offset', local_var_params['offset']))  # noqa: E501
-
-        header_params = dict(local_var_params.get('_headers', {}))
-        if 'if_none_match' in local_var_params:
-            header_params['if-none-match'] = local_var_params['if_none_match']  # noqa: E501
-
-        form_params = []
-        local_var_files = {}
-
-        body_params = None
-        # HTTP header `Accept`
-        header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
-
-        # Authentication setting
-        auth_settings = ['BearerAuth']  # noqa: E501
-
-        response_types_map = {
-            200: "list[Extension]",
-            304: None,
-            400: "UserError",
-            403: "ApiError",
-        }
-
-        return self.api_client.call_api(
-            '/v1/extensions', 'GET',
-            path_params,
-            query_params,
-            header_params,
-            body=body_params,
-            post_params=form_params,
-            files=local_var_files,
-            response_types_map=response_types_map,
-            auth_settings=auth_settings,
-            async_req=local_var_params.get('async_req'),
-            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
-            _preload_content=local_var_params.get('_preload_content', True),
-            _request_timeout=local_var_params.get('_request_timeout'),
-            collection_formats=collection_formats,
-            _request_auth=local_var_params.get('_request_auth'))
-
     def v1_get_hook_by_id(self, hook_id, **kwargs):  # noqa: E501
         """Get hypervisor hook by id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.v1_get_hook_by_id(hook_id, async_req=True)
@@ -11572,158 +11151,14 @@
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
-    def v1_load_extension(self, v1_load_extension_parameters, **kwargs):  # noqa: E501
-        """Load an extension  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.v1_load_extension(v1_load_extension_parameters, async_req=True)
-        >>> result = thread.get()
-
-        :param v1_load_extension_parameters: application/json (required)
-        :type v1_load_extension_parameters: V1LoadExtensionParameters
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: Extension
-        """
-        kwargs['_return_http_data_only'] = True
-        return self.v1_load_extension_with_http_info(v1_load_extension_parameters, **kwargs)  # noqa: E501
-
-    def v1_load_extension_with_http_info(self, v1_load_extension_parameters, **kwargs):  # noqa: E501
-        """Load an extension  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.v1_load_extension_with_http_info(v1_load_extension_parameters, async_req=True)
-        >>> result = thread.get()
-
-        :param v1_load_extension_parameters: application/json (required)
-        :type v1_load_extension_parameters: V1LoadExtensionParameters
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the authentication
-                              in the spec for a single request.
-        :type _request_auth: dict, optional
-        :type _content_type: string, optional: force content-type for the request
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: tuple(Extension, status_code(int), headers(HTTPHeaderDict))
-        """
-
-        local_var_params = locals()
-
-        all_params = [
-            'v1_load_extension_parameters'
-        ]
-        all_params.extend(
-            [
-                'async_req',
-                '_return_http_data_only',
-                '_preload_content',
-                '_request_timeout',
-                '_request_auth',
-                '_content_type',
-                '_headers'
-            ]
-        )
-
-        for key, val in six.iteritems(local_var_params['kwargs']):
-            if key not in all_params:
-                raise ApiTypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method v1_load_extension" % key
-                )
-            local_var_params[key] = val
-        del local_var_params['kwargs']
-        # verify the required parameter 'v1_load_extension_parameters' is set
-        if self.api_client.client_side_validation and ('v1_load_extension_parameters' not in local_var_params or  # noqa: E501
-                                                        local_var_params['v1_load_extension_parameters'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `v1_load_extension_parameters` when calling `v1_load_extension`")  # noqa: E501
-
-        collection_formats = {}
-
-        path_params = {}
-
-        query_params = []
-
-        header_params = dict(local_var_params.get('_headers', {}))
-
-        form_params = []
-        local_var_files = {}
-
-        body_params = None
-        if 'v1_load_extension_parameters' in local_var_params:
-            body_params = local_var_params['v1_load_extension_parameters']
-        # HTTP header `Accept`
-        header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
-
-        # HTTP header `Content-Type`
-        header_params['Content-Type'] = local_var_params.get('_content_type',
-            self.api_client.select_header_content_type(
-                ['application/json'],
-                'POST', body_params))  # noqa: E501
-
-        # Authentication setting
-        auth_settings = ['BearerAuth']  # noqa: E501
-
-        response_types_map = {
-            200: "Extension",
-            400: "UserError",
-            403: "ApiError",
-        }
-
-        return self.api_client.call_api(
-            '/v1/extensions', 'POST',
-            path_params,
-            query_params,
-            header_params,
-            body=body_params,
-            post_params=form_params,
-            files=local_var_files,
-            response_types_map=response_types_map,
-            auth_settings=auth_settings,
-            async_req=local_var_params.get('async_req'),
-            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
-            _preload_content=local_var_params.get('_preload_content', True),
-            _request_timeout=local_var_params.get('_request_timeout'),
-            collection_formats=collection_formats,
-            _request_auth=local_var_params.get('_request_auth'))
-
     def v1_media_play(self, instance_id, media_play_body, **kwargs):  # noqa: E501
         """Start playing media  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.v1_media_play(instance_id, media_play_body, async_req=True)
@@ -12001,157 +11436,14 @@
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
-    def v1_parse_extension_json(self, extension, **kwargs):  # noqa: E501
-        """Validates extension.json  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.v1_parse_extension_json(extension, async_req=True)
-        >>> result = thread.get()
-
-        :param extension: extension.json contents (required)
-        :type extension: Extension
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: object
-        """
-        kwargs['_return_http_data_only'] = True
-        return self.v1_parse_extension_json_with_http_info(extension, **kwargs)  # noqa: E501
-
-    def v1_parse_extension_json_with_http_info(self, extension, **kwargs):  # noqa: E501
-        """Validates extension.json  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.v1_parse_extension_json_with_http_info(extension, async_req=True)
-        >>> result = thread.get()
-
-        :param extension: extension.json contents (required)
-        :type extension: Extension
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the authentication
-                              in the spec for a single request.
-        :type _request_auth: dict, optional
-        :type _content_type: string, optional: force content-type for the request
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: tuple(object, status_code(int), headers(HTTPHeaderDict))
-        """
-
-        local_var_params = locals()
-
-        all_params = [
-            'extension'
-        ]
-        all_params.extend(
-            [
-                'async_req',
-                '_return_http_data_only',
-                '_preload_content',
-                '_request_timeout',
-                '_request_auth',
-                '_content_type',
-                '_headers'
-            ]
-        )
-
-        for key, val in six.iteritems(local_var_params['kwargs']):
-            if key not in all_params:
-                raise ApiTypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method v1_parse_extension_json" % key
-                )
-            local_var_params[key] = val
-        del local_var_params['kwargs']
-        # verify the required parameter 'extension' is set
-        if self.api_client.client_side_validation and ('extension' not in local_var_params or  # noqa: E501
-                                                        local_var_params['extension'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `extension` when calling `v1_parse_extension_json`")  # noqa: E501
-
-        collection_formats = {}
-
-        path_params = {}
-
-        query_params = []
-
-        header_params = dict(local_var_params.get('_headers', {}))
-
-        form_params = []
-        local_var_files = {}
-
-        body_params = None
-        if 'extension' in local_var_params:
-            body_params = local_var_params['extension']
-        # HTTP header `Accept`
-        header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
-
-        # HTTP header `Content-Type`
-        header_params['Content-Type'] = local_var_params.get('_content_type',
-            self.api_client.select_header_content_type(
-                ['application/json'],
-                'POST', body_params))  # noqa: E501
-
-        # Authentication setting
-        auth_settings = ['BearerAuth']  # noqa: E501
-
-        response_types_map = {
-            200: "object",
-            400: "UserError",
-        }
-
-        return self.api_client.call_api(
-            '/v1/extensions/parse/extension.json', 'POST',
-            path_params,
-            query_params,
-            header_params,
-            body=body_params,
-            post_params=form_params,
-            files=local_var_files,
-            response_types_map=response_types_map,
-            auth_settings=auth_settings,
-            async_req=local_var_params.get('async_req'),
-            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
-            _preload_content=local_var_params.get('_preload_content', True),
-            _request_timeout=local_var_params.get('_request_timeout'),
-            collection_formats=collection_formats,
-            _request_auth=local_var_params.get('_request_auth'))
-
     def v1_patch_instance(self, instance_id, patch_instance_options, **kwargs):  # noqa: E501
         """Update Instance  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.v1_patch_instance(instance_id, patch_instance_options, async_req=True)
@@ -15512,27 +14804,27 @@
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
-    def v1_start_net_mon_proc_map(self, instance_id, **kwargs):  # noqa: E501
+    def v1_start_netdump(self, instance_id, **kwargs):  # noqa: E501
         """Start Enhanced Network Monitor on an instance.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.v1_start_net_mon_proc_map(instance_id, async_req=True)
+        >>> thread = api.v1_start_netdump(instance_id, async_req=True)
         >>> result = thread.get()
 
         :param instance_id: Instance ID - uuid (required)
         :type instance_id: str
-        :param net_mon_proc_map_filter: 
-        :type net_mon_proc_map_filter: NetMonProcMapFilter
+        :param netdump_filter: 
+        :type netdump_filter: NetdumpFilter
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -15541,29 +14833,29 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.v1_start_net_mon_proc_map_with_http_info(instance_id, **kwargs)  # noqa: E501
+        return self.v1_start_netdump_with_http_info(instance_id, **kwargs)  # noqa: E501
 
-    def v1_start_net_mon_proc_map_with_http_info(self, instance_id, **kwargs):  # noqa: E501
+    def v1_start_netdump_with_http_info(self, instance_id, **kwargs):  # noqa: E501
         """Start Enhanced Network Monitor on an instance.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.v1_start_net_mon_proc_map_with_http_info(instance_id, async_req=True)
+        >>> thread = api.v1_start_netdump_with_http_info(instance_id, async_req=True)
         >>> result = thread.get()
 
         :param instance_id: Instance ID - uuid (required)
         :type instance_id: str
-        :param net_mon_proc_map_filter: 
-        :type net_mon_proc_map_filter: NetMonProcMapFilter
+        :param netdump_filter: 
+        :type netdump_filter: NetdumpFilter
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -15584,15 +14876,15 @@
         :rtype: None
         """
 
         local_var_params = locals()
 
         all_params = [
             'instance_id',
-            'net_mon_proc_map_filter'
+            'netdump_filter'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -15602,22 +14894,22 @@
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method v1_start_net_mon_proc_map" % key
+                    " to method v1_start_netdump" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
         # verify the required parameter 'instance_id' is set
         if self.api_client.client_side_validation and ('instance_id' not in local_var_params or  # noqa: E501
                                                         local_var_params['instance_id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `instance_id` when calling `v1_start_net_mon_proc_map`")  # noqa: E501
+            raise ApiValueError("Missing the required parameter `instance_id` when calling `v1_start_netdump`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'instance_id' in local_var_params:
             path_params['instanceId'] = local_var_params['instance_id']  # noqa: E501
 
@@ -15625,16 +14917,16 @@
 
         header_params = dict(local_var_params.get('_headers', {}))
 
         form_params = []
         local_var_files = {}
 
         body_params = None
-        if 'net_mon_proc_map_filter' in local_var_params:
-            body_params = local_var_params['net_mon_proc_map_filter']
+        if 'netdump_filter' in local_var_params:
+            body_params = local_var_params['netdump_filter']
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = local_var_params.get('_content_type',
             self.api_client.select_header_content_type(
@@ -15643,15 +14935,15 @@
 
         # Authentication setting
         auth_settings = ['BearerAuth']  # noqa: E501
 
         response_types_map = {}
 
         return self.api_client.call_api(
-            '/v1/instances/{instanceId}/netmonprocmap/enable', 'POST',
+            '/v1/instances/{instanceId}/netdump/enable', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_types_map=response_types_map,
@@ -16208,21 +15500,21 @@
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
-    def v1_stop_net_mon_proc_map(self, instance_id, **kwargs):  # noqa: E501
+    def v1_stop_netdump(self, instance_id, **kwargs):  # noqa: E501
         """Stop Enhanced Network Monitor on an instance.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.v1_stop_net_mon_proc_map(instance_id, async_req=True)
+        >>> thread = api.v1_stop_netdump(instance_id, async_req=True)
         >>> result = thread.get()
 
         :param instance_id: Instance ID - uuid (required)
         :type instance_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -16235,23 +15527,23 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.v1_stop_net_mon_proc_map_with_http_info(instance_id, **kwargs)  # noqa: E501
+        return self.v1_stop_netdump_with_http_info(instance_id, **kwargs)  # noqa: E501
 
-    def v1_stop_net_mon_proc_map_with_http_info(self, instance_id, **kwargs):  # noqa: E501
+    def v1_stop_netdump_with_http_info(self, instance_id, **kwargs):  # noqa: E501
         """Stop Enhanced Network Monitor on an instance.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.v1_stop_net_mon_proc_map_with_http_info(instance_id, async_req=True)
+        >>> thread = api.v1_stop_netdump_with_http_info(instance_id, async_req=True)
         >>> result = thread.get()
 
         :param instance_id: Instance ID - uuid (required)
         :type instance_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
@@ -16293,22 +15585,22 @@
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method v1_stop_net_mon_proc_map" % key
+                    " to method v1_stop_netdump" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
         # verify the required parameter 'instance_id' is set
         if self.api_client.client_side_validation and ('instance_id' not in local_var_params or  # noqa: E501
                                                         local_var_params['instance_id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `instance_id` when calling `v1_stop_net_mon_proc_map`")  # noqa: E501
+            raise ApiValueError("Missing the required parameter `instance_id` when calling `v1_stop_netdump`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'instance_id' in local_var_params:
             path_params['instanceId'] = local_var_params['instance_id']  # noqa: E501
 
@@ -16326,15 +15618,15 @@
 
         # Authentication setting
         auth_settings = ['BearerAuth']  # noqa: E501
 
         response_types_map = {}
 
         return self.api_client.call_api(
-            '/v1/instances/{instanceId}/netmonprocmap/disable', 'POST',
+            '/v1/instances/{instanceId}/netdump/disable', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_types_map=response_types_map,
@@ -17165,165 +16457,14 @@
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_types_map=response_types_map,
-            auth_settings=auth_settings,
-            async_req=local_var_params.get('async_req'),
-            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
-            _preload_content=local_var_params.get('_preload_content', True),
-            _request_timeout=local_var_params.get('_request_timeout'),
-            collection_formats=collection_formats,
-            _request_auth=local_var_params.get('_request_auth'))
-
-    def v1_update_extension(self, extension_id, update_extension, **kwargs):  # noqa: E501
-        """Update an existing extension  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.v1_update_extension(extension_id, update_extension, async_req=True)
-        >>> result = thread.get()
-
-        :param extension_id: Extension ID (required)
-        :type extension_id: str
-        :param update_extension: application/json (required)
-        :type update_extension: UpdateExtension
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: None
-        """
-        kwargs['_return_http_data_only'] = True
-        return self.v1_update_extension_with_http_info(extension_id, update_extension, **kwargs)  # noqa: E501
-
-    def v1_update_extension_with_http_info(self, extension_id, update_extension, **kwargs):  # noqa: E501
-        """Update an existing extension  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.v1_update_extension_with_http_info(extension_id, update_extension, async_req=True)
-        >>> result = thread.get()
-
-        :param extension_id: Extension ID (required)
-        :type extension_id: str
-        :param update_extension: application/json (required)
-        :type update_extension: UpdateExtension
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the authentication
-                              in the spec for a single request.
-        :type _request_auth: dict, optional
-        :type _content_type: string, optional: force content-type for the request
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: None
-        """
-
-        local_var_params = locals()
-
-        all_params = [
-            'extension_id',
-            'update_extension'
-        ]
-        all_params.extend(
-            [
-                'async_req',
-                '_return_http_data_only',
-                '_preload_content',
-                '_request_timeout',
-                '_request_auth',
-                '_content_type',
-                '_headers'
-            ]
-        )
-
-        for key, val in six.iteritems(local_var_params['kwargs']):
-            if key not in all_params:
-                raise ApiTypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method v1_update_extension" % key
-                )
-            local_var_params[key] = val
-        del local_var_params['kwargs']
-        # verify the required parameter 'extension_id' is set
-        if self.api_client.client_side_validation and ('extension_id' not in local_var_params or  # noqa: E501
-                                                        local_var_params['extension_id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `extension_id` when calling `v1_update_extension`")  # noqa: E501
-        # verify the required parameter 'update_extension' is set
-        if self.api_client.client_side_validation and ('update_extension' not in local_var_params or  # noqa: E501
-                                                        local_var_params['update_extension'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `update_extension` when calling `v1_update_extension`")  # noqa: E501
-
-        collection_formats = {}
-
-        path_params = {}
-        if 'extension_id' in local_var_params:
-            path_params['extensionId'] = local_var_params['extension_id']  # noqa: E501
-
-        query_params = []
-
-        header_params = dict(local_var_params.get('_headers', {}))
-
-        form_params = []
-        local_var_files = {}
-
-        body_params = None
-        if 'update_extension' in local_var_params:
-            body_params = local_var_params['update_extension']
-        # HTTP header `Accept`
-        header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
-
-        # HTTP header `Content-Type`
-        header_params['Content-Type'] = local_var_params.get('_content_type',
-            self.api_client.select_header_content_type(
-                ['application/json'],
-                'PUT', body_params))  # noqa: E501
-
-        # Authentication setting
-        auth_settings = ['BearerAuth']  # noqa: E501
-
-        response_types_map = {}
-
-        return self.api_client.call_api(
-            '/v1/extensions/{extensionId}', 'PUT',
-            path_params,
-            query_params,
-            header_params,
-            body=body_params,
-            post_params=form_params,
-            files=local_var_files,
-            response_types_map=response_types_map,
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
```

### Comparing `corellium-api-0.3.0/corellium_api/api_client.py` & `corellium-api-0.3.1/corellium_api/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
 import atexit
 import datetime
@@ -74,15 +74,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.3.0/python'
+        self.user_agent = 'OpenAPI-Generator/0.3.1/python'
         self.client_side_validation = configuration.client_side_validation
 
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc_value, traceback):
         await self.close()
```

### Comparing `corellium-api-0.3.0/corellium_api/configuration.py` & `corellium-api-0.3.1/corellium_api/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import copy
@@ -381,16 +381,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 4.5.0-16740\n"\
-               "SDK Package Version: 0.3.0".\
+               "Version of the API: 4.5.0-16757\n"\
+               "SDK Package Version: 0.3.1".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `corellium-api-0.3.0/corellium_api/exceptions.py` & `corellium-api-0.3.1/corellium_api/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 import six
```

### Comparing `corellium-api-0.3.0/corellium_api/models/__init__.py` & `corellium-api-0.3.1/corellium_api/models/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 # import models into model package
@@ -53,15 +53,15 @@
 from corellium_api.models.instance import Instance
 from corellium_api.models.instance_agent_state import InstanceAgentState
 from corellium_api.models.instance_boot_options import InstanceBootOptions
 from corellium_api.models.instance_boot_options_additional_tag import InstanceBootOptionsAdditionalTag
 from corellium_api.models.instance_console_endpoint import InstanceConsoleEndpoint
 from corellium_api.models.instance_create_options import InstanceCreateOptions
 from corellium_api.models.instance_input import InstanceInput
-from corellium_api.models.instance_netmon_proc_map_state import InstanceNetmonProcMapState
+from corellium_api.models.instance_netdump_state import InstanceNetdumpState
 from corellium_api.models.instance_netmon_state import InstanceNetmonState
 from corellium_api.models.instance_return import InstanceReturn
 from corellium_api.models.instance_services import InstanceServices
 from corellium_api.models.instance_start_options import InstanceStartOptions
 from corellium_api.models.instance_state import InstanceState
 from corellium_api.models.instance_stop_options import InstanceStopOptions
 from corellium_api.models.instance_upgrade_body import InstanceUpgradeBody
@@ -70,15 +70,15 @@
 from corellium_api.models.invite_revoke_params_ids import InviteRevokeParamsIds
 from corellium_api.models.kcrange import Kcrange
 from corellium_api.models.kernel_task import KernelTask
 from corellium_api.models.kernel_thread import KernelThread
 from corellium_api.models.media_play_body import MediaPlayBody
 from corellium_api.models.model import Model
 from corellium_api.models.model_software import ModelSoftware
-from corellium_api.models.net_mon_proc_map_filter import NetMonProcMapFilter
+from corellium_api.models.netdump_filter import NetdumpFilter
 from corellium_api.models.password_change_body import PasswordChangeBody
 from corellium_api.models.password_reset_body import PasswordResetBody
 from corellium_api.models.patch_instance_options import PatchInstanceOptions
 from corellium_api.models.peripherals_data import PeripheralsData
 from corellium_api.models.plan import Plan
 from corellium_api.models.project import Project
 from corellium_api.models.project_key import ProjectKey
```

### Comparing `corellium-api-0.3.0/corellium_api/models/address.py` & `corellium-api-0.3.1/corellium_api/models/address.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/agent_app.py` & `corellium-api-0.3.1/corellium_api/models/agent_app.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/agent_app_ready_response.py` & `corellium-api-0.3.1/corellium_api/models/agent_app_ready_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/agent_app_status.py` & `corellium-api-0.3.1/corellium_api/models/agent_app_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/agent_apps_list.py` & `corellium-api-0.3.1/corellium_api/models/agent_apps_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/agent_apps_status_list.py` & `corellium-api-0.3.1/corellium_api/models/agent_apps_status_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/agent_error.py` & `corellium-api-0.3.1/corellium_api/models/agent_error.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/agent_icons.py` & `corellium-api-0.3.1/corellium_api/models/agent_icons.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/agent_install_body.py` & `corellium-api-0.3.1/corellium_api/models/agent_install_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/agent_profiles_return.py` & `corellium-api-0.3.1/corellium_api/models/agent_profiles_return.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/agent_system_adb_auth.py` & `corellium-api-0.3.1/corellium_api/models/agent_system_adb_auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/agent_system_get_prop_body.py` & `corellium-api-0.3.1/corellium_api/models/agent_system_get_prop_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/agent_value_return.py` & `corellium-api-0.3.1/corellium_api/models/agent_value_return.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/agreed_ack.py` & `corellium-api-0.3.1/corellium_api/models/agreed_ack.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/api_conflict_error.py` & `corellium-api-0.3.1/corellium_api/models/api_conflict_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/api_error.py` & `corellium-api-0.3.1/corellium_api/models/api_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/api_internal_consistency_error.py` & `corellium-api-0.3.1/corellium_api/models/api_internal_consistency_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/api_not_found_error.py` & `corellium-api-0.3.1/corellium_api/models/api_not_found_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/api_token.py` & `corellium-api-0.3.1/corellium_api/models/api_token.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/bit.py` & `corellium-api-0.3.1/corellium_api/models/bit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/btrace_enable_options.py` & `corellium-api-0.3.1/corellium_api/models/btrace_enable_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/button.py` & `corellium-api-0.3.1/corellium_api/models/button.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/coupon_options.py` & `corellium-api-0.3.1/corellium_api/models/coupon_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/create_team.py` & `corellium-api-0.3.1/corellium_api/models/create_team.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/created_by.py` & `corellium-api-0.3.1/corellium_api/models/created_by.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/credentials.py` & `corellium-api-0.3.1/corellium_api/models/credentials.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/domain_options.py` & `corellium-api-0.3.1/corellium_api/models/domain_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/extension.py` & `corellium-api-0.3.1/corellium_api/models/extension.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/features.py` & `corellium-api-0.3.1/corellium_api/models/features.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/file_changes.py` & `corellium-api-0.3.1/corellium_api/models/file_changes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/firmware.py` & `corellium-api-0.3.1/corellium_api/models/firmware.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/gpio_state_definition.py` & `corellium-api-0.3.1/corellium_api/models/gpio_state_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/gpios_state.py` & `corellium-api-0.3.1/corellium_api/models/gpios_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/grant_trial_request_response.py` & `corellium-api-0.3.1/corellium_api/models/grant_trial_request_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/hook.py` & `corellium-api-0.3.1/corellium_api/models/hook.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/image.py` & `corellium-api-0.3.1/corellium_api/models/image.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/instance.py` & `corellium-api-0.3.1/corellium_api/models/instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
@@ -56,15 +56,15 @@
         'panicked': 'bool',
         'created': 'datetime',
         'model': 'str',
         'fwpackage': 'str',
         'os': 'str',
         'agent': 'InstanceAgentState',
         'netmon': 'InstanceNetmonState',
-        'netmonprocmap': 'InstanceNetmonProcMapState',
+        'netdump': 'InstanceNetdumpState',
         'expose_port': 'str',
         'fault': 'bool',
         'patches': 'list[str]',
         'created_by': 'CreatedBy'
     }
 
     attribute_map = {
@@ -88,22 +88,22 @@
         'panicked': 'panicked',
         'created': 'created',
         'model': 'model',
         'fwpackage': 'fwpackage',
         'os': 'os',
         'agent': 'agent',
         'netmon': 'netmon',
-        'netmonprocmap': 'netmonprocmap',
+        'netdump': 'netdump',
         'expose_port': 'exposePort',
         'fault': 'fault',
         'patches': 'patches',
         'created_by': 'createdBy'
     }
 
-    def __init__(self, id=None, name=None, key=None, flavor=None, type=None, project=None, state=None, state_changed=None, started_at=None, user_task=None, task_state=None, error=None, boot_options=None, service_ip=None, wifi_ip=None, secondary_ip=None, services=None, panicked=None, created=None, model=None, fwpackage=None, os=None, agent=None, netmon=None, netmonprocmap=None, expose_port=None, fault=None, patches=None, created_by=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, name=None, key=None, flavor=None, type=None, project=None, state=None, state_changed=None, started_at=None, user_task=None, task_state=None, error=None, boot_options=None, service_ip=None, wifi_ip=None, secondary_ip=None, services=None, panicked=None, created=None, model=None, fwpackage=None, os=None, agent=None, netmon=None, netdump=None, expose_port=None, fault=None, patches=None, created_by=None, local_vars_configuration=None):  # noqa: E501
         """Instance - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._name = None
@@ -125,15 +125,15 @@
         self._panicked = None
         self._created = None
         self._model = None
         self._fwpackage = None
         self._os = None
         self._agent = None
         self._netmon = None
-        self._netmonprocmap = None
+        self._netdump = None
         self._expose_port = None
         self._fault = None
         self._patches = None
         self._created_by = None
         self.discriminator = None
 
         self.id = id
@@ -158,16 +158,18 @@
             self.services = services
         self.panicked = panicked
         self.created = created
         self.model = model
         self.fwpackage = fwpackage
         self.os = os
         self.agent = agent
-        self.netmon = netmon
-        self.netmonprocmap = netmonprocmap
+        if netmon is not None:
+            self.netmon = netmon
+        if netdump is not None:
+            self.netdump = netdump
         self.expose_port = expose_port
         self.fault = fault
         self.patches = patches
         if created_by is not None:
             self.created_by = created_by
 
     @property
@@ -709,33 +711,33 @@
         :param netmon: The netmon of this Instance.  # noqa: E501
         :type netmon: InstanceNetmonState
         """
 
         self._netmon = netmon
 
     @property
-    def netmonprocmap(self):
-        """Gets the netmonprocmap of this Instance.  # noqa: E501
+    def netdump(self):
+        """Gets the netdump of this Instance.  # noqa: E501
 
 
-        :return: The netmonprocmap of this Instance.  # noqa: E501
-        :rtype: InstanceNetmonProcMapState
+        :return: The netdump of this Instance.  # noqa: E501
+        :rtype: InstanceNetdumpState
         """
-        return self._netmonprocmap
+        return self._netdump
 
-    @netmonprocmap.setter
-    def netmonprocmap(self, netmonprocmap):
-        """Sets the netmonprocmap of this Instance.
+    @netdump.setter
+    def netdump(self, netdump):
+        """Sets the netdump of this Instance.
 
 
-        :param netmonprocmap: The netmonprocmap of this Instance.  # noqa: E501
-        :type netmonprocmap: InstanceNetmonProcMapState
+        :param netdump: The netdump of this Instance.  # noqa: E501
+        :type netdump: InstanceNetdumpState
         """
 
-        self._netmonprocmap = netmonprocmap
+        self._netdump = netdump
 
     @property
     def expose_port(self):
         """Gets the expose_port of this Instance.  # noqa: E501
 
           # noqa: E501
```

### Comparing `corellium-api-0.3.0/corellium_api/models/instance_agent_state.py` & `corellium-api-0.3.1/corellium_api/models/instance_agent_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/instance_boot_options.py` & `corellium-api-0.3.1/corellium_api/models/instance_boot_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/instance_boot_options_additional_tag.py` & `corellium-api-0.3.1/corellium_api/models/instance_boot_options_additional_tag.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/instance_console_endpoint.py` & `corellium-api-0.3.1/corellium_api/models/instance_console_endpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/instance_create_options.py` & `corellium-api-0.3.1/corellium_api/models/instance_create_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/instance_input.py` & `corellium-api-0.3.1/corellium_api/models/instance_input.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/instance_netmon_proc_map_state.py` & `corellium-api-0.3.1/corellium_api/models/instance_netmon_proc_map_state.py`

 * *Files identical despite different names*

### Comparing `corellium-api-0.3.0/corellium_api/models/instance_netmon_state.py` & `corellium-api-0.3.1/corellium_api/models/instance_netmon_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/instance_return.py` & `corellium-api-0.3.1/corellium_api/models/instance_return.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/instance_services.py` & `corellium-api-0.3.1/corellium_api/models/instance_services.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/instance_start_options.py` & `corellium-api-0.3.1/corellium_api/models/instance_start_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/instance_state.py` & `corellium-api-0.3.1/corellium_api/models/instance_state.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/instance_stop_options.py` & `corellium-api-0.3.1/corellium_api/models/instance_stop_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/instance_upgrade_body.py` & `corellium-api-0.3.1/corellium_api/models/instance_upgrade_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/invitation.py` & `corellium-api-0.3.1/corellium_api/models/invitation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/invite_revoke_params.py` & `corellium-api-0.3.1/corellium_api/models/invite_revoke_params.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/invite_revoke_params_ids.py` & `corellium-api-0.3.1/corellium_api/models/invite_revoke_params_ids.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/kcrange.py` & `corellium-api-0.3.1/corellium_api/models/kcrange.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/kernel_task.py` & `corellium-api-0.3.1/corellium_api/models/kernel_task.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/kernel_thread.py` & `corellium-api-0.3.1/corellium_api/models/kernel_thread.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/media_play_body.py` & `corellium-api-0.3.1/corellium_api/models/media_play_body.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/model.py` & `corellium-api-0.3.1/corellium_api/models/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/model_software.py` & `corellium-api-0.3.1/corellium_api/models/model_software.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/net_mon_proc_map_filter.py` & `corellium-api-0.3.1/corellium_api/models/net_mon_proc_map_filter.py`

 * *Files identical despite different names*

### Comparing `corellium-api-0.3.0/corellium_api/models/password_change_body.py` & `corellium-api-0.3.1/corellium_api/models/password_change_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/password_reset_body.py` & `corellium-api-0.3.1/corellium_api/models/password_reset_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/patch_instance_options.py` & `corellium-api-0.3.1/corellium_api/models/patch_instance_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/peripherals_data.py` & `corellium-api-0.3.1/corellium_api/models/peripherals_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/plan.py` & `corellium-api-0.3.1/corellium_api/models/plan.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/plan_options.py` & `corellium-api-0.3.1/corellium_api/models/plan_options.py`

 * *Files identical despite different names*

### Comparing `corellium-api-0.3.0/corellium_api/models/project.py` & `corellium-api-0.3.1/corellium_api/models/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/project_key.py` & `corellium-api-0.3.1/corellium_api/models/project_key.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/project_quota.py` & `corellium-api-0.3.1/corellium_api/models/project_quota.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/project_settings.py` & `corellium-api-0.3.1/corellium_api/models/project_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/project_usage.py` & `corellium-api-0.3.1/corellium_api/models/project_usage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/proxy_config.py` & `corellium-api-0.3.1/corellium_api/models/proxy_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/rate_info.py` & `corellium-api-0.3.1/corellium_api/models/rate_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/reset_link_body.py` & `corellium-api-0.3.1/corellium_api/models/reset_link_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/role.py` & `corellium-api-0.3.1/corellium_api/models/role.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/rotate_body.py` & `corellium-api-0.3.1/corellium_api/models/rotate_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/snapshot.py` & `corellium-api-0.3.1/corellium_api/models/snapshot.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/snapshot_creation_options.py` & `corellium-api-0.3.1/corellium_api/models/snapshot_creation_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/snapshot_status.py` & `corellium-api-0.3.1/corellium_api/models/snapshot_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/subscriber_invite.py` & `corellium-api-0.3.1/corellium_api/models/subscriber_invite.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/team.py` & `corellium-api-0.3.1/corellium_api/models/team.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/team_create.py` & `corellium-api-0.3.1/corellium_api/models/team_create.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/text_input.py` & `corellium-api-0.3.1/corellium_api/models/text_input.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/token.py` & `corellium-api-0.3.1/corellium_api/models/token.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/touch_curve_input.py` & `corellium-api-0.3.1/corellium_api/models/touch_curve_input.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/touch_input.py` & `corellium-api-0.3.1/corellium_api/models/touch_input.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/trial.py` & `corellium-api-0.3.1/corellium_api/models/trial.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/trial_extension.py` & `corellium-api-0.3.1/corellium_api/models/trial_extension.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/trial_request_metadata.py` & `corellium-api-0.3.1/corellium_api/models/trial_request_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/trial_request_options.py` & `corellium-api-0.3.1/corellium_api/models/trial_request_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/update_extension.py` & `corellium-api-0.3.1/corellium_api/models/update_extension.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/user.py` & `corellium-api-0.3.1/corellium_api/models/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/user_error.py` & `corellium-api-0.3.1/corellium_api/models/user_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/v1_create_hook_parameters.py` & `corellium-api-0.3.1/corellium_api/models/v1_create_hook_parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/v1_load_extension_parameters.py` & `corellium-api-0.3.1/corellium_api/models/v1_load_extension_parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/v1_set_state_body.py` & `corellium-api-0.3.1/corellium_api/models/v1_set_state_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/validation_error.py` & `corellium-api-0.3.1/corellium_api/models/validation_error.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/volume_options.py` & `corellium-api-0.3.1/corellium_api/models/volume_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/vpn_definition.py` & `corellium-api-0.3.1/corellium_api/models/vpn_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/web_player_create_session_request.py` & `corellium-api-0.3.1/corellium_api/models/web_player_create_session_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/models/web_player_session.py` & `corellium-api-0.3.1/corellium_api/models/web_player_session.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.0/corellium_api/rest.py` & `corellium-api-0.3.1/corellium_api/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 import io
 import json
 import logging
```

### Comparing `corellium-api-0.3.0/corellium_api.egg-info/SOURCES.txt` & `corellium-api-0.3.1/corellium_api.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 corellium_api/models/instance.py
 corellium_api/models/instance_agent_state.py
 corellium_api/models/instance_boot_options.py
 corellium_api/models/instance_boot_options_additional_tag.py
 corellium_api/models/instance_console_endpoint.py
 corellium_api/models/instance_create_options.py
 corellium_api/models/instance_input.py
+corellium_api/models/instance_netdump_state.py
 corellium_api/models/instance_netmon_proc_map_state.py
 corellium_api/models/instance_netmon_state.py
 corellium_api/models/instance_return.py
 corellium_api/models/instance_services.py
 corellium_api/models/instance_start_options.py
 corellium_api/models/instance_state.py
 corellium_api/models/instance_stop_options.py
@@ -71,14 +72,15 @@
 corellium_api/models/kcrange.py
 corellium_api/models/kernel_task.py
 corellium_api/models/kernel_thread.py
 corellium_api/models/media_play_body.py
 corellium_api/models/model.py
 corellium_api/models/model_software.py
 corellium_api/models/net_mon_proc_map_filter.py
+corellium_api/models/netdump_filter.py
 corellium_api/models/password_change_body.py
 corellium_api/models/password_reset_body.py
 corellium_api/models/patch_instance_options.py
 corellium_api/models/peripherals_data.py
 corellium_api/models/plan.py
 corellium_api/models/plan_options.py
 corellium_api/models/project.py
@@ -156,14 +158,15 @@
 test/test_instance.py
 test/test_instance_agent_state.py
 test/test_instance_boot_options.py
 test/test_instance_boot_options_additional_tag.py
 test/test_instance_console_endpoint.py
 test/test_instance_create_options.py
 test/test_instance_input.py
+test/test_instance_netdump_state.py
 test/test_instance_netmon_proc_map_state.py
 test/test_instance_netmon_state.py
 test/test_instance_return.py
 test/test_instance_services.py
 test/test_instance_start_options.py
 test/test_instance_state.py
 test/test_instance_stop_options.py
@@ -174,14 +177,15 @@
 test/test_kcrange.py
 test/test_kernel_task.py
 test/test_kernel_thread.py
 test/test_media_play_body.py
 test/test_model.py
 test/test_model_software.py
 test/test_net_mon_proc_map_filter.py
+test/test_netdump_filter.py
 test/test_password_change_body.py
 test/test_password_reset_body.py
 test/test_patch_instance_options.py
 test/test_peripherals_data.py
 test/test_plan.py
 test/test_plan_options.py
 test/test_project.py
```

### Comparing `corellium-api-0.3.0/setup.py` & `corellium-api-0.3.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "corellium-api"
-VERSION = "0.3.0"
+VERSION = "0.3.1"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `corellium-api-0.3.0/test/test_address.py` & `corellium-api-0.3.1/test/test_address.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_agent_app.py` & `corellium-api-0.3.1/test/test_agent_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_agent_app_ready_response.py` & `corellium-api-0.3.1/test/test_agent_app_ready_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_agent_app_status.py` & `corellium-api-0.3.1/test/test_agent_app_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_agent_apps_list.py` & `corellium-api-0.3.1/test/test_agent_apps_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_agent_apps_status_list.py` & `corellium-api-0.3.1/test/test_agent_apps_status_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_agent_error.py` & `corellium-api-0.3.1/test/test_agent_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_agent_icons.py` & `corellium-api-0.3.1/test/test_agent_icons.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_agent_install_body.py` & `corellium-api-0.3.1/test/test_agent_install_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_agent_profiles_return.py` & `corellium-api-0.3.1/test/test_agent_profiles_return.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_agent_system_adb_auth.py` & `corellium-api-0.3.1/test/test_agent_system_adb_auth.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_agent_system_get_prop_body.py` & `corellium-api-0.3.1/test/test_agent_system_get_prop_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_agent_value_return.py` & `corellium-api-0.3.1/test/test_agent_value_return.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_agreed_ack.py` & `corellium-api-0.3.1/test/test_agreed_ack.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_api_conflict_error.py` & `corellium-api-0.3.1/test/test_api_conflict_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_api_error.py` & `corellium-api-0.3.1/test/test_api_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_api_internal_consistency_error.py` & `corellium-api-0.3.1/test/test_api_internal_consistency_error.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_api_not_found_error.py` & `corellium-api-0.3.1/test/test_api_not_found_error.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_api_token.py` & `corellium-api-0.3.1/test/test_api_token.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_bit.py` & `corellium-api-0.3.1/test/test_bit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_btrace_enable_options.py` & `corellium-api-0.3.1/test/test_btrace_enable_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_button.py` & `corellium-api-0.3.1/test/test_button.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_corellium_api.py` & `corellium-api-0.3.1/test/test_corellium_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
@@ -311,21 +311,14 @@
     def test_v1_create_user(self):
         """Test case for v1_create_user
 
         Create User  # noqa: E501
         """
         pass
 
-    def test_v1_delete_extension(self):
-        """Test case for v1_delete_extension
-
-        Delete an existing extension  # noqa: E501
-        """
-        pass
-
     def test_v1_delete_hook(self):
         """Test case for v1_delete_hook
 
         Delete an existing hypervisor hook  # noqa: E501
         """
         pass
 
@@ -388,28 +381,14 @@
     def test_v1_execute_hyper_trace_hooks(self):
         """Test case for v1_execute_hyper_trace_hooks
 
         Execute Hooks on an instance  # noqa: E501
         """
         pass
 
-    def test_v1_get_extension_by_id(self):
-        """Test case for v1_get_extension_by_id
-
-        Get extension by id  # noqa: E501
-        """
-        pass
-
-    def test_v1_get_extensions(self):
-        """Test case for v1_get_extensions
-
-        Get all extensions  # noqa: E501
-        """
-        pass
-
     def test_v1_get_hook_by_id(self):
         """Test case for v1_get_hook_by_id
 
         Get hypervisor hook by id  # noqa: E501
         """
         pass
 
@@ -591,42 +570,28 @@
     def test_v1_list_threads(self):
         """Test case for v1_list_threads
 
         Get Running Threads (CoreTrace)  # noqa: E501
         """
         pass
 
-    def test_v1_load_extension(self):
-        """Test case for v1_load_extension
-
-        Load an extension  # noqa: E501
-        """
-        pass
-
     def test_v1_media_play(self):
         """Test case for v1_media_play
 
         Start playing media  # noqa: E501
         """
         pass
 
     def test_v1_media_stop(self):
         """Test case for v1_media_stop
 
         Stop playing media  # noqa: E501
         """
         pass
 
-    def test_v1_parse_extension_json(self):
-        """Test case for v1_parse_extension_json
-
-        Validates extension.json  # noqa: E501
-        """
-        pass
-
     def test_v1_patch_instance(self):
         """Test case for v1_patch_instance
 
         Update Instance  # noqa: E501
         """
         pass
 
@@ -780,16 +745,16 @@
     def test_v1_start_instance(self):
         """Test case for v1_start_instance
 
         Start an Instance  # noqa: E501
         """
         pass
 
-    def test_v1_start_net_mon_proc_map(self):
-        """Test case for v1_start_net_mon_proc_map
+    def test_v1_start_netdump(self):
+        """Test case for v1_start_netdump
 
         Start Enhanced Network Monitor on an instance.  # noqa: E501
         """
         pass
 
     def test_v1_start_network_monitor(self):
         """Test case for v1_start_network_monitor
@@ -815,16 +780,16 @@
     def test_v1_stop_instance(self):
         """Test case for v1_stop_instance
 
         Stop an Instance  # noqa: E501
         """
         pass
 
-    def test_v1_stop_net_mon_proc_map(self):
-        """Test case for v1_stop_net_mon_proc_map
+    def test_v1_stop_netdump(self):
+        """Test case for v1_stop_netdump
 
         Stop Enhanced Network Monitor on an instance.  # noqa: E501
         """
         pass
 
     def test_v1_stop_network_monitor(self):
         """Test case for v1_stop_network_monitor
@@ -864,21 +829,14 @@
     def test_v1_unpause_instance(self):
         """Test case for v1_unpause_instance
 
         Unpause an Instance  # noqa: E501
         """
         pass
 
-    def test_v1_update_extension(self):
-        """Test case for v1_update_extension
-
-        Update an existing extension  # noqa: E501
-        """
-        pass
-
     def test_v1_update_hook(self):
         """Test case for v1_update_hook
 
         Update an existing hypervisor hook  # noqa: E501
         """
         pass
```

### Comparing `corellium-api-0.3.0/test/test_coupon_options.py` & `corellium-api-0.3.1/test/test_coupon_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_create_team.py` & `corellium-api-0.3.1/test/test_create_team.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_created_by.py` & `corellium-api-0.3.1/test/test_created_by.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_credentials.py` & `corellium-api-0.3.1/test/test_credentials.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_domain_options.py` & `corellium-api-0.3.1/test/test_domain_options.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_extension.py` & `corellium-api-0.3.1/test/test_extension.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_features.py` & `corellium-api-0.3.1/test/test_features.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_file_changes.py` & `corellium-api-0.3.1/test/test_file_changes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_firmware.py` & `corellium-api-0.3.1/test/test_firmware.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_gpio_state_definition.py` & `corellium-api-0.3.1/test/test_gpio_state_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_gpios_state.py` & `corellium-api-0.3.1/test/test_gpios_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_grant_trial_request_response.py` & `corellium-api-0.3.1/test/test_grant_trial_request_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_hook.py` & `corellium-api-0.3.1/test/test_hook.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_image.py` & `corellium-api-0.3.1/test/test_image.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_instance.py` & `corellium-api-0.3.1/test/test_instance.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
@@ -78,15 +78,15 @@
                 agent = corellium_api.models.instance_agent_state.InstanceAgentState(
                     hash = '', 
                     info = '', ), 
                 netmon = corellium_api.models.instance_netmon_state.InstanceNetmonState(
                     hash = '', 
                     info = '', 
                     enabled = True, ), 
-                netmonprocmap = corellium_api.models.instance_netmon_proc_map_state.InstanceNetmonProcMapState(
+                netdump = corellium_api.models.instance_netdump_state.InstanceNetdumpState(
                     hash = '', 
                     info = '', 
                     enabled = True, ), 
                 expose_port = '', 
                 fault = True, 
                 patches = [
                     ''
```

### Comparing `corellium-api-0.3.0/test/test_instance_agent_state.py` & `corellium-api-0.3.1/test/test_instance_agent_state.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_instance_boot_options.py` & `corellium-api-0.3.1/test/test_instance_boot_options.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_instance_boot_options_additional_tag.py` & `corellium-api-0.3.1/test/test_instance_boot_options_additional_tag.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_instance_console_endpoint.py` & `corellium-api-0.3.1/test/test_instance_console_endpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_instance_create_options.py` & `corellium-api-0.3.1/test/test_instance_create_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_instance_input.py` & `corellium-api-0.3.1/test/test_instance_input.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_instance_netmon_proc_map_state.py` & `corellium-api-0.3.1/test/test_instance_netmon_proc_map_state.py`

 * *Files identical despite different names*

### Comparing `corellium-api-0.3.0/test/test_instance_netmon_state.py` & `corellium-api-0.3.1/test/test_instance_netmon_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_instance_return.py` & `corellium-api-0.3.1/test/test_instance_return.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_instance_services.py` & `corellium-api-0.3.1/test/test_instance_services.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_instance_start_options.py` & `corellium-api-0.3.1/test/test_instance_start_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_instance_state.py` & `corellium-api-0.3.1/test/test_instance_state.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_instance_stop_options.py` & `corellium-api-0.3.1/test/test_instance_stop_options.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_instance_upgrade_body.py` & `corellium-api-0.3.1/test/test_instance_upgrade_body.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_invitation.py` & `corellium-api-0.3.1/test/test_invitation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_invite_revoke_params.py` & `corellium-api-0.3.1/test/test_invite_revoke_params.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_invite_revoke_params_ids.py` & `corellium-api-0.3.1/test/test_invite_revoke_params_ids.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_kcrange.py` & `corellium-api-0.3.1/test/test_kcrange.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_kernel_task.py` & `corellium-api-0.3.1/test/test_kernel_task.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_kernel_thread.py` & `corellium-api-0.3.1/test/test_kernel_thread.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_media_play_body.py` & `corellium-api-0.3.1/test/test_media_play_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_model.py` & `corellium-api-0.3.1/test/test_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_model_software.py` & `corellium-api-0.3.1/test/test_model_software.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_net_mon_proc_map_filter.py` & `corellium-api-0.3.1/test/test_net_mon_proc_map_filter.py`

 * *Files identical despite different names*

### Comparing `corellium-api-0.3.0/test/test_password_change_body.py` & `corellium-api-0.3.1/test/test_password_change_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_password_reset_body.py` & `corellium-api-0.3.1/test/test_password_reset_body.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_patch_instance_options.py` & `corellium-api-0.3.1/test/test_patch_instance_options.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_peripherals_data.py` & `corellium-api-0.3.1/test/test_peripherals_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_plan.py` & `corellium-api-0.3.1/test/test_plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_plan_options.py` & `corellium-api-0.3.1/test/test_plan_options.py`

 * *Files identical despite different names*

### Comparing `corellium-api-0.3.0/test/test_project.py` & `corellium-api-0.3.1/test/test_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_project_key.py` & `corellium-api-0.3.1/test/test_project_key.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_project_quota.py` & `corellium-api-0.3.1/test/test_project_quota.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_project_settings.py` & `corellium-api-0.3.1/test/test_project_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_project_usage.py` & `corellium-api-0.3.1/test/test_project_usage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_proxy_config.py` & `corellium-api-0.3.1/test/test_proxy_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_rate_info.py` & `corellium-api-0.3.1/test/test_rate_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_reset_link_body.py` & `corellium-api-0.3.1/test/test_reset_link_body.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_role.py` & `corellium-api-0.3.1/test/test_role.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_rotate_body.py` & `corellium-api-0.3.1/test/test_rotate_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_snapshot.py` & `corellium-api-0.3.1/test/test_snapshot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_snapshot_creation_options.py` & `corellium-api-0.3.1/test/test_snapshot_creation_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_snapshot_status.py` & `corellium-api-0.3.1/test/test_snapshot_status.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_subscriber_invite.py` & `corellium-api-0.3.1/test/test_subscriber_invite.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_team.py` & `corellium-api-0.3.1/test/test_team.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_team_create.py` & `corellium-api-0.3.1/test/test_team_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_text_input.py` & `corellium-api-0.3.1/test/test_text_input.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_token.py` & `corellium-api-0.3.1/test/test_token.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_touch_curve_input.py` & `corellium-api-0.3.1/test/test_touch_curve_input.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_touch_input.py` & `corellium-api-0.3.1/test/test_touch_input.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_trial.py` & `corellium-api-0.3.1/test/test_trial.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_trial_extension.py` & `corellium-api-0.3.1/test/test_trial_extension.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_trial_request_metadata.py` & `corellium-api-0.3.1/test/test_trial_request_metadata.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_trial_request_options.py` & `corellium-api-0.3.1/test/test_trial_request_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_update_extension.py` & `corellium-api-0.3.1/test/test_update_extension.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_user.py` & `corellium-api-0.3.1/test/test_user.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_user_error.py` & `corellium-api-0.3.1/test/test_user_error.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_v1_create_hook_parameters.py` & `corellium-api-0.3.1/test/test_v1_create_hook_parameters.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_v1_load_extension_parameters.py` & `corellium-api-0.3.1/test/test_v1_load_extension_parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_v1_set_state_body.py` & `corellium-api-0.3.1/test/test_v1_set_state_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_validation_error.py` & `corellium-api-0.3.1/test/test_validation_error.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_volume_options.py` & `corellium-api-0.3.1/test/test_volume_options.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_vpn_definition.py` & `corellium-api-0.3.1/test/test_vpn_definition.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_web_player_create_session_request.py` & `corellium-api-0.3.1/test/test_web_player_create_session_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.0/test/test_web_player_session.py` & `corellium-api-0.3.1/test/test_web_player_session.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16740
+    The version of the OpenAPI document: 4.5.0-16757
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

