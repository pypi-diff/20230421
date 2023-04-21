# Comparing `tmp/incydr-1.0.0.tar.gz` & `tmp/incydr-1.0.1.tar.gz`

## Comparing `incydr-1.0.0.tar` & `incydr-1.0.1.tar`

### file list

```diff
@@ -1,102 +1,102 @@
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_cli/__init__.py
--rw-r--r--   0        0        0     5146 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_cli/core.py
--rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_cli/cursor.py
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_cli/exceptions.py
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_cli/file_readers.py
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_cli/main.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_cli/render.py
--rw-r--r--   0        0        0    22896 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_cli/rich_utils.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_cli/utils.py
--rw-r--r--   0        0        0     6793 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_cli/cmds/alert_rules.py
--rw-r--r--   0        0        0    12979 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_cli/cmds/alerts.py
--rw-r--r--   0        0        0    10318 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_cli/cmds/audit_log.py
--rw-r--r--   0        0        0    17742 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_cli/cmds/cases.py
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_cli/cmds/departments.py
--rw-r--r--   0        0        0     2755 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_cli/cmds/devices.py
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_cli/cmds/directory_groups.py
--rw-r--r--   0        0        0    10015 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_cli/cmds/file_events.py
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_cli/cmds/models.py
--rw-r--r--   0        0        0    12079 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_cli/cmds/trusted_activities.py
--rw-r--r--   0        0        0    10965 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_cli/cmds/user_risk_profiles.py
--rw-r--r--   0        0        0    15938 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_cli/cmds/users.py
--rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_cli/cmds/utils.py
--rw-r--r--   0        0        0    18682 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_cli/cmds/watchlists.py
--rw-r--r--   0        0        0     3661 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_cli/cmds/options/alert_filter_options.py
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_cli/cmds/options/audit_log_filter_options.py
--rw-r--r--   0        0        0     5243 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_cli/cmds/options/event_filter_options.py
--rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_cli/cmds/options/output_options.py
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_cli/cmds/options/profile_filter_options.py
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_cli/cmds/options/utils.py
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_cli/logger/__init__.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_cli/logger/enums.py
--rw-r--r--   0        0        0     5016 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_cli/logger/handlers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_sdk/__init__.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_sdk/__version__.py
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_sdk/exceptions.py
--rw-r--r--   0        0        0     8171 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_sdk/utils.py
--rw-r--r--   0        0        0     5971 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_sdk/alert_rules/client.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_sdk/alert_rules/models/request.py
--rw-r--r--   0        0        0    16555 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_sdk/alert_rules/models/response.py
--rw-r--r--   0        0        0     5351 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_sdk/alerts/client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_sdk/alerts/models/__init__.py
--rw-r--r--   0        0        0     9912 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_sdk/alerts/models/alert.py
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_sdk/alerts/models/enums.py
--rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_sdk/alerts/models/request.py
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_sdk/alerts/models/response.py
--rw-r--r--   0        0        0    11953 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_sdk/audit_log/client.py
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_sdk/audit_log/models.py
--rw-r--r--   0        0        0    15787 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_sdk/cases/client.py
--rw-r--r--   0        0        0     8301 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_sdk/cases/models.py
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_sdk/core/auth.py
--rw-r--r--   0        0        0    11420 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_sdk/core/client.py
--rw-r--r--   0        0        0     6477 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_sdk/core/models.py
--rw-r--r--   0        0        0     8001 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_sdk/core/settings.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_sdk/core/utils.py
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_sdk/customer/client.py
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_sdk/customer/models.py
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_sdk/departments/client.py
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_sdk/departments/models.py
--rw-r--r--   0        0        0     3720 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_sdk/devices/client.py
--rw-r--r--   0        0        0     7898 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_sdk/devices/models.py
--rw-r--r--   0        0        0     2326 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_sdk/directory_groups/client.py
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_sdk/directory_groups/models.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_sdk/enums/__init__.py
--rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_sdk/enums/alerts.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_sdk/enums/cases.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_sdk/enums/devices.py
--rw-r--r--   0        0        0    17648 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_sdk/enums/file_events.py
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_sdk/enums/trusted_activities.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_sdk/enums/watchlists.py
--rw-r--r--   0        0        0     5093 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_sdk/file_events/client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_sdk/file_events/models/__init__.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_sdk/file_events/models/enums.py
--rw-r--r--   0        0        0    27719 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_sdk/file_events/models/event.py
--rw-r--r--   0        0        0     7447 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_sdk/file_events/models/response.py
--rw-r--r--   0        0        0     9950 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_sdk/queries/alerts.py
--rw-r--r--   0        0        0    12185 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_sdk/queries/file_events.py
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_sdk/queries/utils.py
--rw-r--r--   0        0        0    15252 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_sdk/trusted_activities/client.py
--rw-r--r--   0        0        0     7109 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_sdk/trusted_activities/models.py
--rw-r--r--   0        0        0     9303 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_sdk/user_risk_profiles/client.py
--rw-r--r--   0        0        0     6260 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_sdk/user_risk_profiles/models.py
--rw-r--r--   0        0        0    14022 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_sdk/users/client.py
--rw-r--r--   0        0        0     8679 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_sdk/users/models.py
--rw-r--r--   0        0        0    19130 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_sdk/watchlists/client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_sdk/watchlists/models/__init__.py
--rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_sdk/watchlists/models/requests.py
--rw-r--r--   0        0        0     9515 2020-02-02 00:00:00.000000 incydr-1.0.0/_incydr_sdk/watchlists/models/responses.py
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 incydr-1.0.0/incydr/__init__.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 incydr-1.0.0/incydr/__main__.py
--rw-r--r--   0        0        0     3313 2020-02-02 00:00:00.000000 incydr-1.0.0/incydr/models.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 incydr-1.0.0/incydr/enums/__init__.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 incydr-1.0.0/incydr/enums/alerts.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 incydr-1.0.0/incydr/enums/cases.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 incydr-1.0.0/incydr/enums/devices.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 incydr-1.0.0/incydr/enums/file_events.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 incydr-1.0.0/incydr/enums/trusted_activities.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 incydr-1.0.0/incydr/enums/watchlists.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 incydr-1.0.0/.gitignore
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 incydr-1.0.0/LICENSE.txt
--rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 incydr-1.0.0/README.md
--rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 incydr-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 incydr-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/__init__.py
+-rw-r--r--   0        0        0     5146 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/core.py
+-rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/cursor.py
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/exceptions.py
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/file_readers.py
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/main.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/render.py
+-rw-r--r--   0        0        0    22896 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/rich_utils.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/utils.py
+-rw-r--r--   0        0        0     6793 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/cmds/alert_rules.py
+-rw-r--r--   0        0        0    12979 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/cmds/alerts.py
+-rw-r--r--   0        0        0    10318 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/cmds/audit_log.py
+-rw-r--r--   0        0        0    17742 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/cmds/cases.py
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/cmds/departments.py
+-rw-r--r--   0        0        0     2755 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/cmds/devices.py
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/cmds/directory_groups.py
+-rw-r--r--   0        0        0    10015 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/cmds/file_events.py
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/cmds/models.py
+-rw-r--r--   0        0        0    12079 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/cmds/trusted_activities.py
+-rw-r--r--   0        0        0    10965 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/cmds/user_risk_profiles.py
+-rw-r--r--   0        0        0    15938 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/cmds/users.py
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/cmds/utils.py
+-rw-r--r--   0        0        0    18682 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/cmds/watchlists.py
+-rw-r--r--   0        0        0     3661 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/cmds/options/alert_filter_options.py
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/cmds/options/audit_log_filter_options.py
+-rw-r--r--   0        0        0     5243 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/cmds/options/event_filter_options.py
+-rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/cmds/options/output_options.py
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/cmds/options/profile_filter_options.py
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/cmds/options/utils.py
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/logger/__init__.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/logger/enums.py
+-rw-r--r--   0        0        0     5016 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/logger/handlers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/__init__.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/__version__.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/exceptions.py
+-rw-r--r--   0        0        0     8171 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/utils.py
+-rw-r--r--   0        0        0     5971 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/alert_rules/client.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/alert_rules/models/request.py
+-rw-r--r--   0        0        0    16555 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/alert_rules/models/response.py
+-rw-r--r--   0        0        0     5351 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/alerts/client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/alerts/models/__init__.py
+-rw-r--r--   0        0        0     9912 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/alerts/models/alert.py
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/alerts/models/enums.py
+-rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/alerts/models/request.py
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/alerts/models/response.py
+-rw-r--r--   0        0        0    11953 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/audit_log/client.py
+-rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/audit_log/models.py
+-rw-r--r--   0        0        0    15787 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/cases/client.py
+-rw-r--r--   0        0        0     8301 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/cases/models.py
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/core/auth.py
+-rw-r--r--   0        0        0    11420 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/core/client.py
+-rw-r--r--   0        0        0     6477 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/core/models.py
+-rw-r--r--   0        0        0     8032 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/core/settings.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/core/utils.py
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/customer/client.py
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/customer/models.py
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/departments/client.py
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/departments/models.py
+-rw-r--r--   0        0        0     3720 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/devices/client.py
+-rw-r--r--   0        0        0     7898 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/devices/models.py
+-rw-r--r--   0        0        0     2326 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/directory_groups/client.py
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/directory_groups/models.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/enums/__init__.py
+-rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/enums/alerts.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/enums/cases.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/enums/devices.py
+-rw-r--r--   0        0        0    17648 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/enums/file_events.py
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/enums/trusted_activities.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/enums/watchlists.py
+-rw-r--r--   0        0        0     5093 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/file_events/client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/file_events/models/__init__.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/file_events/models/enums.py
+-rw-r--r--   0        0        0    27719 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/file_events/models/event.py
+-rw-r--r--   0        0        0     7447 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/file_events/models/response.py
+-rw-r--r--   0        0        0     9950 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/queries/alerts.py
+-rw-r--r--   0        0        0    12185 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/queries/file_events.py
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/queries/utils.py
+-rw-r--r--   0        0        0    15252 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/trusted_activities/client.py
+-rw-r--r--   0        0        0     7109 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/trusted_activities/models.py
+-rw-r--r--   0        0        0     9299 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/user_risk_profiles/client.py
+-rw-r--r--   0        0        0     6251 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/user_risk_profiles/models.py
+-rw-r--r--   0        0        0    14022 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/users/client.py
+-rw-r--r--   0        0        0     8679 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/users/models.py
+-rw-r--r--   0        0        0    19130 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/watchlists/client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/watchlists/models/__init__.py
+-rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/watchlists/models/requests.py
+-rw-r--r--   0        0        0     9515 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/watchlists/models/responses.py
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 incydr-1.0.1/incydr/__init__.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 incydr-1.0.1/incydr/__main__.py
+-rw-r--r--   0        0        0     3313 2020-02-02 00:00:00.000000 incydr-1.0.1/incydr/models.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 incydr-1.0.1/incydr/enums/__init__.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 incydr-1.0.1/incydr/enums/alerts.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 incydr-1.0.1/incydr/enums/cases.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 incydr-1.0.1/incydr/enums/devices.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 incydr-1.0.1/incydr/enums/file_events.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 incydr-1.0.1/incydr/enums/trusted_activities.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 incydr-1.0.1/incydr/enums/watchlists.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 incydr-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 incydr-1.0.1/LICENSE.txt
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 incydr-1.0.1/README.md
+-rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 incydr-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 incydr-1.0.1/PKG-INFO
```

### Comparing `incydr-1.0.0/_incydr_cli/__init__.py` & `incydr-1.0.1/_incydr_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_cli/core.py` & `incydr-1.0.1/_incydr_cli/core.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_cli/cursor.py` & `incydr-1.0.1/_incydr_cli/cursor.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_cli/exceptions.py` & `incydr-1.0.1/_incydr_cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_cli/file_readers.py` & `incydr-1.0.1/_incydr_cli/file_readers.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_cli/main.py` & `incydr-1.0.1/_incydr_cli/main.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_cli/render.py` & `incydr-1.0.1/_incydr_cli/render.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_cli/rich_utils.py` & `incydr-1.0.1/_incydr_cli/rich_utils.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_cli/utils.py` & `incydr-1.0.1/_incydr_cli/utils.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_cli/cmds/alert_rules.py` & `incydr-1.0.1/_incydr_cli/cmds/alert_rules.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_cli/cmds/alerts.py` & `incydr-1.0.1/_incydr_cli/cmds/alerts.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_cli/cmds/audit_log.py` & `incydr-1.0.1/_incydr_cli/cmds/audit_log.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_cli/cmds/cases.py` & `incydr-1.0.1/_incydr_cli/cmds/cases.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_cli/cmds/departments.py` & `incydr-1.0.1/_incydr_cli/cmds/departments.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_cli/cmds/devices.py` & `incydr-1.0.1/_incydr_cli/cmds/devices.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_cli/cmds/directory_groups.py` & `incydr-1.0.1/_incydr_cli/cmds/directory_groups.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_cli/cmds/file_events.py` & `incydr-1.0.1/_incydr_cli/cmds/file_events.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_cli/cmds/models.py` & `incydr-1.0.1/_incydr_cli/cmds/models.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_cli/cmds/trusted_activities.py` & `incydr-1.0.1/_incydr_cli/cmds/trusted_activities.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_cli/cmds/user_risk_profiles.py` & `incydr-1.0.1/_incydr_cli/cmds/user_risk_profiles.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_cli/cmds/users.py` & `incydr-1.0.1/_incydr_cli/cmds/users.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_cli/cmds/utils.py` & `incydr-1.0.1/_incydr_cli/cmds/utils.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_cli/cmds/watchlists.py` & `incydr-1.0.1/_incydr_cli/cmds/watchlists.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_cli/cmds/options/alert_filter_options.py` & `incydr-1.0.1/_incydr_cli/cmds/options/alert_filter_options.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_cli/cmds/options/audit_log_filter_options.py` & `incydr-1.0.1/_incydr_cli/cmds/options/audit_log_filter_options.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_cli/cmds/options/event_filter_options.py` & `incydr-1.0.1/_incydr_cli/cmds/options/event_filter_options.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_cli/cmds/options/output_options.py` & `incydr-1.0.1/_incydr_cli/cmds/options/output_options.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_cli/cmds/options/profile_filter_options.py` & `incydr-1.0.1/_incydr_cli/cmds/options/profile_filter_options.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_cli/cmds/options/utils.py` & `incydr-1.0.1/_incydr_cli/cmds/options/utils.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_cli/logger/__init__.py` & `incydr-1.0.1/_incydr_cli/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_cli/logger/handlers.py` & `incydr-1.0.1/_incydr_cli/logger/handlers.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_sdk/exceptions.py` & `incydr-1.0.1/_incydr_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_sdk/utils.py` & `incydr-1.0.1/_incydr_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_sdk/alert_rules/client.py` & `incydr-1.0.1/_incydr_sdk/alert_rules/client.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_sdk/alert_rules/models/response.py` & `incydr-1.0.1/_incydr_sdk/alert_rules/models/response.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_sdk/alerts/client.py` & `incydr-1.0.1/_incydr_sdk/alerts/client.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_sdk/alerts/models/alert.py` & `incydr-1.0.1/_incydr_sdk/alerts/models/alert.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_sdk/alerts/models/enums.py` & `incydr-1.0.1/_incydr_sdk/alerts/models/enums.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_sdk/alerts/models/request.py` & `incydr-1.0.1/_incydr_sdk/alerts/models/request.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_sdk/alerts/models/response.py` & `incydr-1.0.1/_incydr_sdk/alerts/models/response.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_sdk/audit_log/client.py` & `incydr-1.0.1/_incydr_sdk/audit_log/client.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_sdk/audit_log/models.py` & `incydr-1.0.1/_incydr_sdk/audit_log/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 from enum import Enum
+from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
 
 from pydantic import BaseModel
 from pydantic import Field
 
@@ -27,22 +28,22 @@
 
 class AuditEventsPage(ResponseModel):
     """
     A model representing a page of audit events.
 
     **Fields**:
 
-    * **events**: `List[Dict[Optional[str], Optional[str]]]` A list of zero or more events matching the given criteria.
+    * **events**: `List[Dict[Optional[str], Any]]` A list of zero or more events matching the given criteria.
         Each event is represented as a dictionary of property names associated with that event.  These fields may differ
         from event to event.
     * **pagination_range_end_index**: `int` The index of the last result returned, in relation to total results found.
     * **pagination_range_start_index**: `int` The index of the first result returned, in relation to total results found.
     """
 
-    events: List[Dict[Optional[str], Optional[str]]] = Field(
+    events: List[Dict[Optional[str], Any]] = Field(
         None, description="A list of zero or more events matching the given criteria."
     )
     pagination_range_end_index: int = Field(
         None,
         description="The index of the last result returned, in relation to total results found",
         example=62,
         alias="paginationRangeEndIndex",
```

### Comparing `incydr-1.0.0/_incydr_sdk/cases/client.py` & `incydr-1.0.1/_incydr_sdk/cases/client.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_sdk/cases/models.py` & `incydr-1.0.1/_incydr_sdk/cases/models.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_sdk/core/auth.py` & `incydr-1.0.1/_incydr_sdk/core/auth.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_sdk/core/client.py` & `incydr-1.0.1/_incydr_sdk/core/client.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_sdk/core/models.py` & `incydr-1.0.1/_incydr_sdk/core/models.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_sdk/core/settings.py` & `incydr-1.0.1/_incydr_sdk/core/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,15 +158,16 @@
         log_file = values["log_file"]
         log_stderr = values["log_stderr"]
         log_level = values["log_level"]
         logger = values["logger"]
 
         if not hasattr(logger, "_incydr"):
             warnings.warn(
-                "A custom logger has been set, all other log-related settings on the `incydr.Client` are ignored for custom loggers."
+                "A custom logger has been set, all other log-related settings on the `incydr.Client` are ignored for custom loggers.",
+                stacklevel=2,
             )
             return values
 
         logger.handlers.clear()
 
         if log_stderr and use_rich:
             rich_handler = RichHandler(console=_incydr_console, rich_tracebacks=True)
```

### Comparing `incydr-1.0.0/_incydr_sdk/customer/client.py` & `incydr-1.0.1/_incydr_sdk/customer/client.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_sdk/customer/models.py` & `incydr-1.0.1/_incydr_sdk/customer/models.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_sdk/departments/client.py` & `incydr-1.0.1/_incydr_sdk/departments/client.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_sdk/departments/models.py` & `incydr-1.0.1/_incydr_sdk/departments/models.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_sdk/devices/client.py` & `incydr-1.0.1/_incydr_sdk/devices/client.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_sdk/devices/models.py` & `incydr-1.0.1/_incydr_sdk/devices/models.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_sdk/directory_groups/client.py` & `incydr-1.0.1/_incydr_sdk/directory_groups/client.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_sdk/directory_groups/models.py` & `incydr-1.0.1/_incydr_sdk/directory_groups/models.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_sdk/enums/__init__.py` & `incydr-1.0.1/_incydr_sdk/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_sdk/enums/alerts.py` & `incydr-1.0.1/_incydr_sdk/enums/alerts.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_sdk/enums/cases.py` & `incydr-1.0.1/_incydr_sdk/enums/cases.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_sdk/enums/file_events.py` & `incydr-1.0.1/_incydr_sdk/enums/file_events.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_sdk/enums/trusted_activities.py` & `incydr-1.0.1/_incydr_sdk/enums/trusted_activities.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_sdk/enums/watchlists.py` & `incydr-1.0.1/_incydr_sdk/enums/watchlists.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_sdk/file_events/client.py` & `incydr-1.0.1/_incydr_sdk/file_events/client.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_sdk/file_events/models/event.py` & `incydr-1.0.1/_incydr_sdk/file_events/models/event.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_sdk/file_events/models/response.py` & `incydr-1.0.1/_incydr_sdk/file_events/models/response.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_sdk/queries/alerts.py` & `incydr-1.0.1/_incydr_sdk/queries/alerts.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_sdk/queries/file_events.py` & `incydr-1.0.1/_incydr_sdk/queries/file_events.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_sdk/queries/utils.py` & `incydr-1.0.1/_incydr_sdk/queries/utils.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_sdk/trusted_activities/client.py` & `incydr-1.0.1/_incydr_sdk/trusted_activities/client.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_sdk/trusted_activities/models.py` & `incydr-1.0.1/_incydr_sdk/trusted_activities/models.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_sdk/user_risk_profiles/client.py` & `incydr-1.0.1/_incydr_sdk/user_risk_profiles/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         * **support_user**: `bool | None` - When true, return only support users. When false, return only non-support users.
                                             Defaults to returning both
 
         **Returns**: A ['UserRiskProfilesPage'][userriskprofilespage-model] object.
         """
         page_size = page_size or self._parent.settings.page_size
         data = QueryUserRiskProfilesRequest(
-            page_num=page_num,
+            page=page_num,
             page_size=page_size,
             manager_id=manager_id,
             title=title,
             division=division,
             department=department,
             employment_type=employment_type,
             country=country,
```

### Comparing `incydr-1.0.0/_incydr_sdk/user_risk_profiles/models.py` & `incydr-1.0.1/_incydr_sdk/user_risk_profiles/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 from typing import List
 from typing import Optional
 
-from pydantic import BaseModel
 from pydantic import Field
 from rich.markdown import Markdown
 
+from _incydr_sdk.core.models import Model
 from _incydr_sdk.core.models import ResponseModel
 
 
 class Date(ResponseModel):
     year: Optional[int] = Field(
         None,
         description="Year of date. Must be from 1 to 9999, or 0 if specifying a date without\n a year.",
@@ -121,16 +121,16 @@
         alias="totalCount",
     )
     user_risk_profiles: Optional[List[UserRiskProfile]] = Field(
         None, alias="userRiskProfiles"
     )
 
 
-class QueryUserRiskProfilesRequest(BaseModel):
-    page_num: Optional[int]
+class QueryUserRiskProfilesRequest(Model):
+    page: Optional[int]
     page_size: Optional[int]
     manager_id: Optional[str]
     title: Optional[str]
     division: Optional[str]
     department: Optional[str]
     employment_type: Optional[str]
     country: Optional[str]
@@ -140,29 +140,29 @@
     deleted: Optional[bool]
     support_user: Optional[bool]
 
     class Config:
         use_enum_values = True
 
 
-class UpdateUserRiskProfileRequest(BaseModel):
+class UpdateUserRiskProfileRequest(Model):
     endDate: Optional[Date] = None
     notes: Optional[str] = Field(
         None,
         description="Notes to add to the user risk profile.",
         example="These are my notes",
     )
     startDate: Optional[Date] = None
 
 
-class AddCloudAliasesRequest(BaseModel):
+class AddCloudAliasesRequest(Model):
     cloudAliases: Optional[List[str]] = None
     userId: Optional[str] = Field(
         None, description="The ID of the user to add cloud aliases.", example="123"
     )
 
 
-class DeleteCloudAliasesRequest(BaseModel):
+class DeleteCloudAliasesRequest(Model):
     cloudAliases: Optional[List[str]] = None
     userId: Optional[str] = Field(
         None, description="The ID of the user to delete cloud aliases.", example="123"
     )
```

### Comparing `incydr-1.0.0/_incydr_sdk/users/client.py` & `incydr-1.0.1/_incydr_sdk/users/client.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_sdk/users/models.py` & `incydr-1.0.1/_incydr_sdk/users/models.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_sdk/watchlists/client.py` & `incydr-1.0.1/_incydr_sdk/watchlists/client.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_sdk/watchlists/models/requests.py` & `incydr-1.0.1/_incydr_sdk/watchlists/models/requests.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/_incydr_sdk/watchlists/models/responses.py` & `incydr-1.0.1/_incydr_sdk/watchlists/models/responses.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/incydr/__init__.py` & `incydr-1.0.1/incydr/__init__.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/incydr/models.py` & `incydr-1.0.1/incydr/models.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/incydr/enums/file_events.py` & `incydr-1.0.1/incydr/enums/file_events.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/LICENSE.txt` & `incydr-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `incydr-1.0.0/README.md` & `incydr-1.0.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,51 @@
+Metadata-Version: 2.1
+Name: incydr
+Version: 1.0.1
+Summary: Code42's Incydr Python SDK
+Project-URL: Documentation, https://github.com/code42/incydr_python#readme
+Project-URL: Issues, https://github.com/code42/incydr_python/issues
+Project-URL: Source, https://github.com/code42/incydr_python/incydr
+Author-email: Code42 <integrations@code42.com>
+License-Expression: MIT
+License-File: LICENSE.txt
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Python: >=3.7
+Requires-Dist: boltons
+Requires-Dist: isodate
+Requires-Dist: pydantic[dotenv]
+Requires-Dist: python-dateutil
+Requires-Dist: requests
+Requires-Dist: requests-toolbelt
+Requires-Dist: rich
+Provides-Extra: cli
+Requires-Dist: chardet; extra == 'cli'
+Requires-Dist: click; extra == 'cli'
+Description-Content-Type: text/markdown
+
 # Incydr
 
 [![PyPI - Version](https://img.shields.io/pypi/v/incydr.svg)](https://pypi.org/project/incydr)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/incydr.svg)](https://pypi.org/project/incydr)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 -----
 
 The Incydr SDK is a Python client for interacting with the [Code42 Incydr API](https://developer.code42.com/api).
 
 It provides a thin wrapper around the [Requests](https://requests.readthedocs.io/en/latest/) HTTP library with
 helper clients that model Code42 data and validate requests with the help of [Pydantic](https://pydantic-docs.helpmanual.io).
 
-**This project is currently in BETA and subject to breaking changes prior to the 1.0 release.**
-
-Documentation during the beta can be found at https://code42.github.io/incydr_python
+Documentation can be found at https://developer.code42.com.
 
 **Table of Contents**
 
 - [Installation](#installation)
 - [License](#license)
 
 ## Installation
@@ -33,12 +62,12 @@
 $ pip install 'incydr[cli]'
 ```
 
 ```bash
 $ pip install 'incydr[all]'.
 ```
 
-For more details see the [SDK Documentation](docs/sdk/index.md) and the [CLI Documentation](docs/cli/getting_started.md).
+For more details see the [SDK Documentation](https://developer.code42.com/sdk/) and the [CLI Documentation](https://developer.code42.com/cli/).
 
 ## License
 
 `incydr` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

### Comparing `incydr-1.0.0/pyproject.toml` & `incydr-1.0.1/pyproject.toml`

 * *Files identical despite different names*

