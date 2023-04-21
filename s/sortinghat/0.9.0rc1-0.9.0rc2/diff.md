# Comparing `tmp/sortinghat-0.9.0rc1.tar.gz` & `tmp/sortinghat-0.9.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sortinghat-0.9.0rc1.tar", max compression
+gzip compressed data, was "sortinghat-0.9.0rc2.tar", max compression
```

## Comparing `sortinghat-0.9.0rc1.tar` & `sortinghat-0.9.0rc2.tar`

### file list

```diff
@@ -1,130 +1,130 @@
--rw-r--r--   0        0        0      363 2023-04-20 16:55:14.079059 sortinghat-0.9.0rc1/AUTHORS
--rw-r--r--   0        0        0    35147 2023-04-20 16:55:14.079059 sortinghat-0.9.0rc1/LICENSE
--rw-r--r--   0        0        0    11752 2023-04-20 16:55:14.079059 sortinghat-0.9.0rc1/NEWS
--rw-r--r--   0        0        0     8566 2023-04-20 16:55:14.079059 sortinghat-0.9.0rc1/README.md
--rw-r--r--   0        0        0     2013 2023-04-20 16:55:14.079059 sortinghat-0.9.0rc1/pyproject.toml
--rw-r--r--   0        0        0       91 2023-04-20 16:55:14.079059 sortinghat-0.9.0rc1/sortinghat/_version.py
--rw-r--r--   0        0        0        0 2023-04-20 16:55:14.079059 sortinghat-0.9.0rc1/sortinghat/app/__init__.py
--rw-r--r--   0        0        0     1250 2023-04-20 16:55:14.079059 sortinghat-0.9.0rc1/sortinghat/app/schema.py
--rw-r--r--   0        0        0      518 2023-04-20 16:55:14.079059 sortinghat-0.9.0rc1/sortinghat/app/urls.py
--rw-r--r--   0        0        0      196 2023-04-20 16:55:14.079059 sortinghat-0.9.0rc1/sortinghat/app/wsgi.py
--rw-r--r--   0        0        0        0 2023-04-20 16:55:14.079059 sortinghat-0.9.0rc1/sortinghat/cli/__init__.py
--rw-r--r--   0        0        0      977 2023-04-20 16:55:14.079059 sortinghat-0.9.0rc1/sortinghat/cli/client/__init__.py
--rw-r--r--   0        0        0     5738 2023-04-20 16:55:14.079059 sortinghat-0.9.0rc1/sortinghat/cli/client/client.py
--rw-r--r--   0        0        0    43408 2023-04-20 16:55:14.079059 sortinghat-0.9.0rc1/sortinghat/cli/client/schema.py
--rw-r--r--   0        0        0        0 2023-04-20 16:55:14.079059 sortinghat-0.9.0rc1/sortinghat/cli/cmds/__init__.py
--rw-r--r--   0        0        0     3072 2023-04-20 16:55:14.079059 sortinghat-0.9.0rc1/sortinghat/cli/cmds/add.py
--rw-r--r--   0        0        0     6145 2023-04-20 16:55:14.079059 sortinghat-0.9.0rc1/sortinghat/cli/cmds/config.py
--rw-r--r--   0        0        0     3219 2023-04-20 16:55:14.079059 sortinghat-0.9.0rc1/sortinghat/cli/cmds/countries.py
--rw-r--r--   0        0        0     3462 2023-04-20 16:55:14.079059 sortinghat-0.9.0rc1/sortinghat/cli/cmds/enroll.py
--rw-r--r--   0        0        0     2860 2023-04-20 16:55:14.079059 sortinghat-0.9.0rc1/sortinghat/cli/cmds/lock.py
--rw-r--r--   0        0        0     2342 2023-04-20 16:55:14.079059 sortinghat-0.9.0rc1/sortinghat/cli/cmds/merge.py
--rw-r--r--   0        0        0     2352 2023-04-20 16:55:14.079059 sortinghat-0.9.0rc1/sortinghat/cli/cmds/mv.py
--rw-r--r--   0        0        0     7466 2023-04-20 16:55:14.079059 sortinghat-0.9.0rc1/sortinghat/cli/cmds/orgs.py
--rw-r--r--   0        0        0     2934 2023-04-20 16:55:14.079059 sortinghat-0.9.0rc1/sortinghat/cli/cmds/profile.py
--rw-r--r--   0        0        0     1992 2023-04-20 16:55:14.079059 sortinghat-0.9.0rc1/sortinghat/cli/cmds/rm.py
--rw-r--r--   0        0        0     2909 2023-04-20 16:55:14.079059 sortinghat-0.9.0rc1/sortinghat/cli/cmds/show.py
--rw-r--r--   0        0        0     2365 2023-04-20 16:55:14.079059 sortinghat-0.9.0rc1/sortinghat/cli/cmds/split.py
--rw-r--r--   0        0        0     3364 2023-04-20 16:55:14.079059 sortinghat-0.9.0rc1/sortinghat/cli/cmds/withdraw.py
--rwxr-xr-x   0        0        0     2857 2023-04-20 16:55:14.083059 sortinghat-0.9.0rc1/sortinghat/cli/sortinghat.py
--rw-r--r--   0        0        0       43 2023-04-20 16:55:14.083059 sortinghat-0.9.0rc1/sortinghat/cli/templates/add.tmpl
--rw-r--r--   0        0        0       23 2023-04-20 16:55:14.083059 sortinghat-0.9.0rc1/sortinghat/cli/templates/config.tmpl
--rw-r--r--   0        0        0       83 2023-04-20 16:55:14.083059 sortinghat-0.9.0rc1/sortinghat/cli/templates/countries.tmpl
--rw-r--r--   0        0        0       54 2023-04-20 16:55:14.083059 sortinghat-0.9.0rc1/sortinghat/cli/templates/lock.tmpl
--rw-r--r--   0        0        0      169 2023-04-20 16:55:14.083059 sortinghat-0.9.0rc1/sortinghat/cli/templates/mv.tmpl
--rw-r--r--   0        0        0      208 2023-04-20 16:55:14.083059 sortinghat-0.9.0rc1/sortinghat/cli/templates/organizations.tmpl
--rw-r--r--   0        0        0      375 2023-04-20 16:55:14.083059 sortinghat-0.9.0rc1/sortinghat/cli/templates/profile.tmpl
--rw-r--r--   0        0        0      106 2023-04-20 16:55:14.083059 sortinghat-0.9.0rc1/sortinghat/cli/templates/rm.tmpl
--rw-r--r--   0        0        0     1016 2023-04-20 16:55:14.083059 sortinghat-0.9.0rc1/sortinghat/cli/templates/show.tmpl
--rw-r--r--   0        0        0       69 2023-04-20 16:55:14.083059 sortinghat-0.9.0rc1/sortinghat/cli/templates/split.tmpl
--rw-r--r--   0        0        0     4856 2023-04-20 16:55:14.083059 sortinghat-0.9.0rc1/sortinghat/cli/utils.py
--rw-r--r--   0        0        0        0 2023-04-20 16:55:14.083059 sortinghat-0.9.0rc1/sortinghat/config/__init__.py
--rw-r--r--   0        0        0     9252 2023-04-20 16:55:14.083059 sortinghat-0.9.0rc1/sortinghat/config/settings.py
--rw-r--r--   0        0        0       20 2023-04-20 16:55:14.083059 sortinghat-0.9.0rc1/sortinghat/config/tenants.json
--rw-r--r--   0        0        0     1544 2023-04-20 16:55:14.083059 sortinghat-0.9.0rc1/sortinghat/core/admin.py
--rw-r--r--   0        0        0    50534 2023-04-20 16:55:14.083059 sortinghat-0.9.0rc1/sortinghat/core/api.py
--rw-r--r--   0        0        0      926 2023-04-20 16:55:14.083059 sortinghat-0.9.0rc1/sortinghat/core/apps.py
--rw-r--r--   0        0        0     5169 2023-04-20 16:55:14.083059 sortinghat-0.9.0rc1/sortinghat/core/aux.py
--rw-r--r--   0        0        0      997 2023-04-20 16:55:14.083059 sortinghat-0.9.0rc1/sortinghat/core/context.py
--rw-r--r--   0        0        0    37055 2023-04-20 16:55:14.083059 sortinghat-0.9.0rc1/sortinghat/core/db.py
--rw-r--r--   0        0        0     3019 2023-04-20 16:55:14.083059 sortinghat-0.9.0rc1/sortinghat/core/decorators.py
--rw-r--r--   0        0        0     3875 2023-04-20 16:55:14.083059 sortinghat-0.9.0rc1/sortinghat/core/errors.py
--rw-r--r--   0        0        0    41236 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/core/fixtures/countries.json
--rw-r--r--   0        0        0     7820 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/core/importer/backend.py
--rw-r--r--   0        0        0     7136 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/core/importer/backends/mailmap.py
--rw-r--r--   0        0        0     5817 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/core/importer/base.py
--rw-r--r--   0        0        0     2143 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/core/importer/models.py
--rw-r--r--   0        0        0     2059 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/core/importer/utils.py
--rw-r--r--   0        0        0    25814 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/core/jobs.py
--rw-r--r--   0        0        0     7298 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/core/log.py
--rw-r--r--   0        0        0        0 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/core/management/__init__.py
--rw-r--r--   0        0        0        0 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/core/management/commands/__init__.py
--rw-r--r--   0        0        0     4155 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/core/management/commands/create_groups.py
--rw-r--r--   0        0        0     4354 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/core/middleware.py
--rw-r--r--   0        0        0    14035 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/core/migrations/0001_sortinghat.py
--rw-r--r--   0        0        0     1717 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/core/migrations/0002_importidentitiestask.py
--rw-r--r--   0        0        0     1502 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/core/migrations/0003_multi_tenancy.py
--rw-r--r--   0        0        0        0 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/core/migrations/__init__.py
--rw-r--r--   0        0        0    11931 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/core/models.py
--rw-r--r--   0        0        0      839 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/core/recommendations/__init__.py
--rw-r--r--   0        0        0     4272 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/core/recommendations/affiliation.py
--rw-r--r--   0        0        0     3137 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/core/recommendations/engine.py
--rw-r--r--   0        0        0     5313 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/core/recommendations/exclusion.py
--rw-r--r--   0        0        0     5642 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/core/recommendations/gender.py
--rw-r--r--   0        0        0     9134 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/core/recommendations/matching.py
--rw-r--r--   0        0        0    74254 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/core/schema.py
--rw-r--r--   0        0        0     2394 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/core/tenant.py
--rw-r--r--   0        0        0     2944 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/core/views.py
--rw-r--r--   0        0        0        0 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/server/__init__.py
--rw-r--r--   0        0        0    13705 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/server/sortinghat_admin.py
--rw-r--r--   0        0        0     2884 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/server/sortinghatd.py
--rw-r--r--   0        0        0     2365 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/server/sortinghatw.py
--rwxr-xr-x   0        0        0     9218 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/server/utils/create_sh_0_7_fixture.py
--rw-r--r--   0        0        0     3485 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/utils/__init__.py
--rw-r--r--   0        0        0        0 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/cli/__init__.py
--rw-r--r--   0        0        0       57 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/cli/config_file.cfg
--rw-r--r--   0        0        0     7601 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/cli/test_cmd_add.py
--rw-r--r--   0        0        0    17698 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/cli/test_cmd_config.py
--rw-r--r--   0        0        0    10234 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/cli/test_cmd_countries.py
--rw-r--r--   0        0        0     7597 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/cli/test_cmd_enroll.py
--rw-r--r--   0        0        0     5397 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/cli/test_cmd_lock.py
--rw-r--r--   0        0        0     3851 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/cli/test_cmd_merge.py
--rw-r--r--   0        0        0     5041 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/cli/test_cmd_mv.py
--rw-r--r--   0        0        0    13658 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/cli/test_cmd_orgs.py
--rw-r--r--   0        0        0     9117 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/cli/test_cmd_profile.py
--rw-r--r--   0        0        0     4599 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/cli/test_cmd_rm.py
--rw-r--r--   0        0        0    10993 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/cli/test_cmd_show.py
--rw-r--r--   0        0        0     5280 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/cli/test_cmd_split.py
--rw-r--r--   0        0        0     6294 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/cli/test_cmd_withdraw.py
--rw-r--r--   0        0        0        0 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/importer/__init__.py
--rw-r--r--   0        0        0        0 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/importer/mocked_package/__init__.py
--rw-r--r--   0        0        0     1055 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/importer/mocked_package/backend_a.py
--rw-r--r--   0        0        0        0 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/importer/mocked_package/nested_package/__init__.py
--rw-r--r--   0        0        0      950 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/importer/mocked_package/nested_package/nested_backend_b.py
--rw-r--r--   0        0        0     1050 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/importer/mocked_package/nested_package/nested_backend_c.py
--rw-r--r--   0        0        0      865 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/importer/mocked_package/nested_package/nested_not_backend.py
--rw-r--r--   0        0        0     4797 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/importer/test_backend.py
--rw-r--r--   0        0        0     2416 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/importer/test_utils.py
--rw-r--r--   0        0        0        0 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/rec/__init__.py
--rw-r--r--   0        0        0     7474 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/rec/test_affiliations.py
--rw-r--r--   0        0        0     2922 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/rec/test_engine.py
--rw-r--r--   0        0        0     3937 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/rec/test_exclusion.py
--rw-r--r--   0        0        0     8536 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/rec/test_gender.py
--rw-r--r--   0        0        0    11764 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/rec/test_matches.py
--rw-r--r--   0        0        0      825 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/runners.py
--rw-r--r--   0        0        0        0 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/tenants/__init__.py
--rw-r--r--   0        0        0     3781 2023-04-20 16:55:14.091060 sortinghat-0.9.0rc1/tests/tenants/test_jobs.py
--rw-r--r--   0        0        0     2273 2023-04-20 16:55:14.091060 sortinghat-0.9.0rc1/tests/tenants/test_middleware.py
--rw-r--r--   0        0        0     5872 2023-04-20 16:55:14.091060 sortinghat-0.9.0rc1/tests/tenants/test_schema.py
--rw-r--r--   0        0        0   258794 2023-04-20 16:55:14.091060 sortinghat-0.9.0rc1/tests/test_api.py
--rw-r--r--   0        0        0    18369 2023-04-20 16:55:14.091060 sortinghat-0.9.0rc1/tests/test_aux.py
--rw-r--r--   0        0        0    10449 2023-04-20 16:55:14.091060 sortinghat-0.9.0rc1/tests/test_client.py
--rw-r--r--   0        0        0   125568 2023-04-20 16:55:14.091060 sortinghat-0.9.0rc1/tests/test_db.py
--rw-r--r--   0        0        0     9257 2023-04-20 16:55:14.091060 sortinghat-0.9.0rc1/tests/test_errors.py
--rw-r--r--   0        0        0    54990 2023-04-20 16:55:14.091060 sortinghat-0.9.0rc1/tests/test_jobs.py
--rw-r--r--   0        0        0    14074 2023-04-20 16:55:14.091060 sortinghat-0.9.0rc1/tests/test_log.py
--rw-r--r--   0        0        0    47504 2023-04-20 16:55:14.091060 sortinghat-0.9.0rc1/tests/test_model.py
--rw-r--r--   0        0        0   399040 2023-04-20 16:55:14.091060 sortinghat-0.9.0rc1/tests/test_schema.py
--rw-r--r--   0        0        0     6316 2023-04-20 16:55:14.091060 sortinghat-0.9.0rc1/tests/test_utils.py
--rw-r--r--   0        0        0    10402 1970-01-01 00:00:00.000000 sortinghat-0.9.0rc1/PKG-INFO
+-rw-r--r--   0        0        0      363 2023-04-21 09:49:24.043503 sortinghat-0.9.0rc2/AUTHORS
+-rw-r--r--   0        0        0    35147 2023-04-21 09:49:24.043503 sortinghat-0.9.0rc2/LICENSE
+-rw-r--r--   0        0        0    11752 2023-04-21 09:49:24.043503 sortinghat-0.9.0rc2/NEWS
+-rw-r--r--   0        0        0     8566 2023-04-21 09:49:24.043503 sortinghat-0.9.0rc2/README.md
+-rw-r--r--   0        0        0     2013 2023-04-21 09:49:24.043503 sortinghat-0.9.0rc2/pyproject.toml
+-rw-r--r--   0        0        0       91 2023-04-21 09:49:24.047503 sortinghat-0.9.0rc2/sortinghat/_version.py
+-rw-r--r--   0        0        0        0 2023-04-21 09:49:24.047503 sortinghat-0.9.0rc2/sortinghat/app/__init__.py
+-rw-r--r--   0        0        0     1250 2023-04-21 09:49:24.047503 sortinghat-0.9.0rc2/sortinghat/app/schema.py
+-rw-r--r--   0        0        0      518 2023-04-21 09:49:24.047503 sortinghat-0.9.0rc2/sortinghat/app/urls.py
+-rw-r--r--   0        0        0      196 2023-04-21 09:49:24.047503 sortinghat-0.9.0rc2/sortinghat/app/wsgi.py
+-rw-r--r--   0        0        0        0 2023-04-21 09:49:24.047503 sortinghat-0.9.0rc2/sortinghat/cli/__init__.py
+-rw-r--r--   0        0        0      977 2023-04-21 09:49:24.047503 sortinghat-0.9.0rc2/sortinghat/cli/client/__init__.py
+-rw-r--r--   0        0        0     5738 2023-04-21 09:49:24.047503 sortinghat-0.9.0rc2/sortinghat/cli/client/client.py
+-rw-r--r--   0        0        0    43408 2023-04-21 09:49:24.047503 sortinghat-0.9.0rc2/sortinghat/cli/client/schema.py
+-rw-r--r--   0        0        0        0 2023-04-21 09:49:24.047503 sortinghat-0.9.0rc2/sortinghat/cli/cmds/__init__.py
+-rw-r--r--   0        0        0     3072 2023-04-21 09:49:24.047503 sortinghat-0.9.0rc2/sortinghat/cli/cmds/add.py
+-rw-r--r--   0        0        0     6145 2023-04-21 09:49:24.047503 sortinghat-0.9.0rc2/sortinghat/cli/cmds/config.py
+-rw-r--r--   0        0        0     3219 2023-04-21 09:49:24.047503 sortinghat-0.9.0rc2/sortinghat/cli/cmds/countries.py
+-rw-r--r--   0        0        0     3462 2023-04-21 09:49:24.047503 sortinghat-0.9.0rc2/sortinghat/cli/cmds/enroll.py
+-rw-r--r--   0        0        0     2860 2023-04-21 09:49:24.047503 sortinghat-0.9.0rc2/sortinghat/cli/cmds/lock.py
+-rw-r--r--   0        0        0     2342 2023-04-21 09:49:24.047503 sortinghat-0.9.0rc2/sortinghat/cli/cmds/merge.py
+-rw-r--r--   0        0        0     2352 2023-04-21 09:49:24.047503 sortinghat-0.9.0rc2/sortinghat/cli/cmds/mv.py
+-rw-r--r--   0        0        0     7466 2023-04-21 09:49:24.047503 sortinghat-0.9.0rc2/sortinghat/cli/cmds/orgs.py
+-rw-r--r--   0        0        0     2934 2023-04-21 09:49:24.047503 sortinghat-0.9.0rc2/sortinghat/cli/cmds/profile.py
+-rw-r--r--   0        0        0     1992 2023-04-21 09:49:24.047503 sortinghat-0.9.0rc2/sortinghat/cli/cmds/rm.py
+-rw-r--r--   0        0        0     2909 2023-04-21 09:49:24.047503 sortinghat-0.9.0rc2/sortinghat/cli/cmds/show.py
+-rw-r--r--   0        0        0     2365 2023-04-21 09:49:24.047503 sortinghat-0.9.0rc2/sortinghat/cli/cmds/split.py
+-rw-r--r--   0        0        0     3364 2023-04-21 09:49:24.047503 sortinghat-0.9.0rc2/sortinghat/cli/cmds/withdraw.py
+-rwxr-xr-x   0        0        0     2857 2023-04-21 09:49:24.047503 sortinghat-0.9.0rc2/sortinghat/cli/sortinghat.py
+-rw-r--r--   0        0        0       43 2023-04-21 09:49:24.047503 sortinghat-0.9.0rc2/sortinghat/cli/templates/add.tmpl
+-rw-r--r--   0        0        0       23 2023-04-21 09:49:24.047503 sortinghat-0.9.0rc2/sortinghat/cli/templates/config.tmpl
+-rw-r--r--   0        0        0       83 2023-04-21 09:49:24.047503 sortinghat-0.9.0rc2/sortinghat/cli/templates/countries.tmpl
+-rw-r--r--   0        0        0       54 2023-04-21 09:49:24.047503 sortinghat-0.9.0rc2/sortinghat/cli/templates/lock.tmpl
+-rw-r--r--   0        0        0      169 2023-04-21 09:49:24.047503 sortinghat-0.9.0rc2/sortinghat/cli/templates/mv.tmpl
+-rw-r--r--   0        0        0      208 2023-04-21 09:49:24.047503 sortinghat-0.9.0rc2/sortinghat/cli/templates/organizations.tmpl
+-rw-r--r--   0        0        0      375 2023-04-21 09:49:24.047503 sortinghat-0.9.0rc2/sortinghat/cli/templates/profile.tmpl
+-rw-r--r--   0        0        0      106 2023-04-21 09:49:24.047503 sortinghat-0.9.0rc2/sortinghat/cli/templates/rm.tmpl
+-rw-r--r--   0        0        0     1016 2023-04-21 09:49:24.047503 sortinghat-0.9.0rc2/sortinghat/cli/templates/show.tmpl
+-rw-r--r--   0        0        0       69 2023-04-21 09:49:24.047503 sortinghat-0.9.0rc2/sortinghat/cli/templates/split.tmpl
+-rw-r--r--   0        0        0     4856 2023-04-21 09:49:24.047503 sortinghat-0.9.0rc2/sortinghat/cli/utils.py
+-rw-r--r--   0        0        0        0 2023-04-21 09:49:24.047503 sortinghat-0.9.0rc2/sortinghat/config/__init__.py
+-rw-r--r--   0        0        0     9252 2023-04-21 09:49:24.047503 sortinghat-0.9.0rc2/sortinghat/config/settings.py
+-rw-r--r--   0        0        0       20 2023-04-21 09:49:24.047503 sortinghat-0.9.0rc2/sortinghat/config/tenants.json
+-rw-r--r--   0        0        0     1544 2023-04-21 09:49:24.047503 sortinghat-0.9.0rc2/sortinghat/core/admin.py
+-rw-r--r--   0        0        0    50534 2023-04-21 09:49:24.047503 sortinghat-0.9.0rc2/sortinghat/core/api.py
+-rw-r--r--   0        0        0      926 2023-04-21 09:49:24.047503 sortinghat-0.9.0rc2/sortinghat/core/apps.py
+-rw-r--r--   0        0        0     5169 2023-04-21 09:49:24.047503 sortinghat-0.9.0rc2/sortinghat/core/aux.py
+-rw-r--r--   0        0        0      997 2023-04-21 09:49:24.047503 sortinghat-0.9.0rc2/sortinghat/core/context.py
+-rw-r--r--   0        0        0    37055 2023-04-21 09:49:24.047503 sortinghat-0.9.0rc2/sortinghat/core/db.py
+-rw-r--r--   0        0        0     3019 2023-04-21 09:49:24.047503 sortinghat-0.9.0rc2/sortinghat/core/decorators.py
+-rw-r--r--   0        0        0     3875 2023-04-21 09:49:24.047503 sortinghat-0.9.0rc2/sortinghat/core/errors.py
+-rw-r--r--   0        0        0    41236 2023-04-21 09:49:24.047503 sortinghat-0.9.0rc2/sortinghat/core/fixtures/countries.json
+-rw-r--r--   0        0        0     7820 2023-04-21 09:49:24.047503 sortinghat-0.9.0rc2/sortinghat/core/importer/backend.py
+-rw-r--r--   0        0        0     7136 2023-04-21 09:49:24.047503 sortinghat-0.9.0rc2/sortinghat/core/importer/backends/mailmap.py
+-rw-r--r--   0        0        0     5817 2023-04-21 09:49:24.047503 sortinghat-0.9.0rc2/sortinghat/core/importer/base.py
+-rw-r--r--   0        0        0     2143 2023-04-21 09:49:24.047503 sortinghat-0.9.0rc2/sortinghat/core/importer/models.py
+-rw-r--r--   0        0        0     2059 2023-04-21 09:49:24.047503 sortinghat-0.9.0rc2/sortinghat/core/importer/utils.py
+-rw-r--r--   0        0        0    25814 2023-04-21 09:49:24.047503 sortinghat-0.9.0rc2/sortinghat/core/jobs.py
+-rw-r--r--   0        0        0     7298 2023-04-21 09:49:24.047503 sortinghat-0.9.0rc2/sortinghat/core/log.py
+-rw-r--r--   0        0        0        0 2023-04-21 09:49:24.047503 sortinghat-0.9.0rc2/sortinghat/core/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 09:49:24.047503 sortinghat-0.9.0rc2/sortinghat/core/management/commands/__init__.py
+-rw-r--r--   0        0        0     4155 2023-04-21 09:49:24.047503 sortinghat-0.9.0rc2/sortinghat/core/management/commands/create_groups.py
+-rw-r--r--   0        0        0     4354 2023-04-21 09:49:24.047503 sortinghat-0.9.0rc2/sortinghat/core/middleware.py
+-rw-r--r--   0        0        0    14035 2023-04-21 09:49:24.051503 sortinghat-0.9.0rc2/sortinghat/core/migrations/0001_sortinghat.py
+-rw-r--r--   0        0        0     1717 2023-04-21 09:49:24.051503 sortinghat-0.9.0rc2/sortinghat/core/migrations/0002_importidentitiestask.py
+-rw-r--r--   0        0        0     1502 2023-04-21 09:49:24.051503 sortinghat-0.9.0rc2/sortinghat/core/migrations/0003_multi_tenancy.py
+-rw-r--r--   0        0        0        0 2023-04-21 09:49:24.051503 sortinghat-0.9.0rc2/sortinghat/core/migrations/__init__.py
+-rw-r--r--   0        0        0    11931 2023-04-21 09:49:24.051503 sortinghat-0.9.0rc2/sortinghat/core/models.py
+-rw-r--r--   0        0        0      839 2023-04-21 09:49:24.051503 sortinghat-0.9.0rc2/sortinghat/core/recommendations/__init__.py
+-rw-r--r--   0        0        0     4272 2023-04-21 09:49:24.051503 sortinghat-0.9.0rc2/sortinghat/core/recommendations/affiliation.py
+-rw-r--r--   0        0        0     3137 2023-04-21 09:49:24.051503 sortinghat-0.9.0rc2/sortinghat/core/recommendations/engine.py
+-rw-r--r--   0        0        0     5313 2023-04-21 09:49:24.051503 sortinghat-0.9.0rc2/sortinghat/core/recommendations/exclusion.py
+-rw-r--r--   0        0        0     5642 2023-04-21 09:49:24.051503 sortinghat-0.9.0rc2/sortinghat/core/recommendations/gender.py
+-rw-r--r--   0        0        0     9134 2023-04-21 09:49:24.051503 sortinghat-0.9.0rc2/sortinghat/core/recommendations/matching.py
+-rw-r--r--   0        0        0    74254 2023-04-21 09:49:24.051503 sortinghat-0.9.0rc2/sortinghat/core/schema.py
+-rw-r--r--   0        0        0     2394 2023-04-21 09:49:24.051503 sortinghat-0.9.0rc2/sortinghat/core/tenant.py
+-rw-r--r--   0        0        0     2944 2023-04-21 09:49:24.051503 sortinghat-0.9.0rc2/sortinghat/core/views.py
+-rw-r--r--   0        0        0        0 2023-04-21 09:49:24.051503 sortinghat-0.9.0rc2/sortinghat/server/__init__.py
+-rw-r--r--   0        0        0    13705 2023-04-21 09:49:24.051503 sortinghat-0.9.0rc2/sortinghat/server/sortinghat_admin.py
+-rw-r--r--   0        0        0     2884 2023-04-21 09:49:24.051503 sortinghat-0.9.0rc2/sortinghat/server/sortinghatd.py
+-rw-r--r--   0        0        0     2365 2023-04-21 09:49:24.051503 sortinghat-0.9.0rc2/sortinghat/server/sortinghatw.py
+-rwxr-xr-x   0        0        0     9218 2023-04-21 09:49:24.051503 sortinghat-0.9.0rc2/sortinghat/server/utils/create_sh_0_7_fixture.py
+-rw-r--r--   0        0        0     3485 2023-04-21 09:49:24.051503 sortinghat-0.9.0rc2/sortinghat/utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 09:49:24.051503 sortinghat-0.9.0rc2/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 09:49:24.051503 sortinghat-0.9.0rc2/tests/cli/__init__.py
+-rw-r--r--   0        0        0       57 2023-04-21 09:49:24.051503 sortinghat-0.9.0rc2/tests/cli/config_file.cfg
+-rw-r--r--   0        0        0     7601 2023-04-21 09:49:24.051503 sortinghat-0.9.0rc2/tests/cli/test_cmd_add.py
+-rw-r--r--   0        0        0    17698 2023-04-21 09:49:24.051503 sortinghat-0.9.0rc2/tests/cli/test_cmd_config.py
+-rw-r--r--   0        0        0    10234 2023-04-21 09:49:24.051503 sortinghat-0.9.0rc2/tests/cli/test_cmd_countries.py
+-rw-r--r--   0        0        0     7597 2023-04-21 09:49:24.051503 sortinghat-0.9.0rc2/tests/cli/test_cmd_enroll.py
+-rw-r--r--   0        0        0     5397 2023-04-21 09:49:24.051503 sortinghat-0.9.0rc2/tests/cli/test_cmd_lock.py
+-rw-r--r--   0        0        0     3851 2023-04-21 09:49:24.051503 sortinghat-0.9.0rc2/tests/cli/test_cmd_merge.py
+-rw-r--r--   0        0        0     5041 2023-04-21 09:49:24.051503 sortinghat-0.9.0rc2/tests/cli/test_cmd_mv.py
+-rw-r--r--   0        0        0    13658 2023-04-21 09:49:24.051503 sortinghat-0.9.0rc2/tests/cli/test_cmd_orgs.py
+-rw-r--r--   0        0        0     9117 2023-04-21 09:49:24.051503 sortinghat-0.9.0rc2/tests/cli/test_cmd_profile.py
+-rw-r--r--   0        0        0     4599 2023-04-21 09:49:24.051503 sortinghat-0.9.0rc2/tests/cli/test_cmd_rm.py
+-rw-r--r--   0        0        0    10993 2023-04-21 09:49:24.051503 sortinghat-0.9.0rc2/tests/cli/test_cmd_show.py
+-rw-r--r--   0        0        0     5280 2023-04-21 09:49:24.051503 sortinghat-0.9.0rc2/tests/cli/test_cmd_split.py
+-rw-r--r--   0        0        0     6294 2023-04-21 09:49:24.051503 sortinghat-0.9.0rc2/tests/cli/test_cmd_withdraw.py
+-rw-r--r--   0        0        0        0 2023-04-21 09:49:24.051503 sortinghat-0.9.0rc2/tests/importer/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 09:49:24.051503 sortinghat-0.9.0rc2/tests/importer/mocked_package/__init__.py
+-rw-r--r--   0        0        0     1055 2023-04-21 09:49:24.051503 sortinghat-0.9.0rc2/tests/importer/mocked_package/backend_a.py
+-rw-r--r--   0        0        0        0 2023-04-21 09:49:24.051503 sortinghat-0.9.0rc2/tests/importer/mocked_package/nested_package/__init__.py
+-rw-r--r--   0        0        0      950 2023-04-21 09:49:24.051503 sortinghat-0.9.0rc2/tests/importer/mocked_package/nested_package/nested_backend_b.py
+-rw-r--r--   0        0        0     1050 2023-04-21 09:49:24.051503 sortinghat-0.9.0rc2/tests/importer/mocked_package/nested_package/nested_backend_c.py
+-rw-r--r--   0        0        0      865 2023-04-21 09:49:24.051503 sortinghat-0.9.0rc2/tests/importer/mocked_package/nested_package/nested_not_backend.py
+-rw-r--r--   0        0        0     4797 2023-04-21 09:49:24.051503 sortinghat-0.9.0rc2/tests/importer/test_backend.py
+-rw-r--r--   0        0        0     2416 2023-04-21 09:49:24.051503 sortinghat-0.9.0rc2/tests/importer/test_utils.py
+-rw-r--r--   0        0        0        0 2023-04-21 09:49:24.051503 sortinghat-0.9.0rc2/tests/rec/__init__.py
+-rw-r--r--   0        0        0     7474 2023-04-21 09:49:24.051503 sortinghat-0.9.0rc2/tests/rec/test_affiliations.py
+-rw-r--r--   0        0        0     2922 2023-04-21 09:49:24.051503 sortinghat-0.9.0rc2/tests/rec/test_engine.py
+-rw-r--r--   0        0        0     3937 2023-04-21 09:49:24.051503 sortinghat-0.9.0rc2/tests/rec/test_exclusion.py
+-rw-r--r--   0        0        0     8536 2023-04-21 09:49:24.051503 sortinghat-0.9.0rc2/tests/rec/test_gender.py
+-rw-r--r--   0        0        0    11764 2023-04-21 09:49:24.051503 sortinghat-0.9.0rc2/tests/rec/test_matches.py
+-rw-r--r--   0        0        0      825 2023-04-21 09:49:24.051503 sortinghat-0.9.0rc2/tests/runners.py
+-rw-r--r--   0        0        0        0 2023-04-21 09:49:24.051503 sortinghat-0.9.0rc2/tests/tenants/__init__.py
+-rw-r--r--   0        0        0     3781 2023-04-21 09:49:24.051503 sortinghat-0.9.0rc2/tests/tenants/test_jobs.py
+-rw-r--r--   0        0        0     2273 2023-04-21 09:49:24.051503 sortinghat-0.9.0rc2/tests/tenants/test_middleware.py
+-rw-r--r--   0        0        0     5872 2023-04-21 09:49:24.051503 sortinghat-0.9.0rc2/tests/tenants/test_schema.py
+-rw-r--r--   0        0        0   258794 2023-04-21 09:49:24.051503 sortinghat-0.9.0rc2/tests/test_api.py
+-rw-r--r--   0        0        0    18369 2023-04-21 09:49:24.051503 sortinghat-0.9.0rc2/tests/test_aux.py
+-rw-r--r--   0        0        0    10449 2023-04-21 09:49:24.051503 sortinghat-0.9.0rc2/tests/test_client.py
+-rw-r--r--   0        0        0   125568 2023-04-21 09:49:24.055503 sortinghat-0.9.0rc2/tests/test_db.py
+-rw-r--r--   0        0        0     9257 2023-04-21 09:49:24.055503 sortinghat-0.9.0rc2/tests/test_errors.py
+-rw-r--r--   0        0        0    54990 2023-04-21 09:49:24.055503 sortinghat-0.9.0rc2/tests/test_jobs.py
+-rw-r--r--   0        0        0    14074 2023-04-21 09:49:24.055503 sortinghat-0.9.0rc2/tests/test_log.py
+-rw-r--r--   0        0        0    47504 2023-04-21 09:49:24.055503 sortinghat-0.9.0rc2/tests/test_model.py
+-rw-r--r--   0        0        0   399040 2023-04-21 09:49:24.055503 sortinghat-0.9.0rc2/tests/test_schema.py
+-rw-r--r--   0        0        0     6316 2023-04-21 09:49:24.055503 sortinghat-0.9.0rc2/tests/test_utils.py
+-rw-r--r--   0        0        0    10402 1970-01-01 00:00:00.000000 sortinghat-0.9.0rc2/PKG-INFO
```

### Comparing `sortinghat-0.9.0rc1/LICENSE` & `sortinghat-0.9.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/NEWS` & `sortinghat-0.9.0rc2/NEWS`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/README.md` & `sortinghat-0.9.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/pyproject.toml` & `sortinghat-0.9.0rc2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sortinghat"
-version = "0.9.0-rc.1"
+version = "0.9.0-rc.2"
 description = "A tool to manage identities."
 authors = [
     "GrimoireLab Developers"
 ]
 license = "GPL-3.0+"
 
 readme = "README.md"
```

### Comparing `sortinghat-0.9.0rc1/sortinghat/app/schema.py` & `sortinghat-0.9.0rc2/sortinghat/app/schema.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/sortinghat/app/urls.py` & `sortinghat-0.9.0rc2/sortinghat/app/urls.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/sortinghat/cli/client/__init__.py` & `sortinghat-0.9.0rc2/sortinghat/cli/client/__init__.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/sortinghat/cli/client/client.py` & `sortinghat-0.9.0rc2/sortinghat/cli/client/client.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/sortinghat/cli/client/schema.py` & `sortinghat-0.9.0rc2/sortinghat/cli/client/schema.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/sortinghat/cli/cmds/add.py` & `sortinghat-0.9.0rc2/sortinghat/cli/cmds/add.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/sortinghat/cli/cmds/config.py` & `sortinghat-0.9.0rc2/sortinghat/cli/cmds/config.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/sortinghat/cli/cmds/countries.py` & `sortinghat-0.9.0rc2/sortinghat/cli/cmds/countries.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/sortinghat/cli/cmds/enroll.py` & `sortinghat-0.9.0rc2/sortinghat/cli/cmds/enroll.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/sortinghat/cli/cmds/lock.py` & `sortinghat-0.9.0rc2/sortinghat/cli/cmds/lock.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/sortinghat/cli/cmds/merge.py` & `sortinghat-0.9.0rc2/sortinghat/cli/cmds/merge.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/sortinghat/cli/cmds/mv.py` & `sortinghat-0.9.0rc2/sortinghat/cli/cmds/mv.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/sortinghat/cli/cmds/orgs.py` & `sortinghat-0.9.0rc2/sortinghat/cli/cmds/orgs.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/sortinghat/cli/cmds/profile.py` & `sortinghat-0.9.0rc2/sortinghat/cli/cmds/profile.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/sortinghat/cli/cmds/rm.py` & `sortinghat-0.9.0rc2/sortinghat/cli/cmds/rm.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/sortinghat/cli/cmds/show.py` & `sortinghat-0.9.0rc2/sortinghat/cli/cmds/show.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/sortinghat/cli/cmds/split.py` & `sortinghat-0.9.0rc2/sortinghat/cli/cmds/split.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/sortinghat/cli/cmds/withdraw.py` & `sortinghat-0.9.0rc2/sortinghat/cli/cmds/withdraw.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/sortinghat/cli/sortinghat.py` & `sortinghat-0.9.0rc2/sortinghat/cli/sortinghat.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/sortinghat/cli/templates/show.tmpl` & `sortinghat-0.9.0rc2/sortinghat/cli/templates/show.tmpl`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/sortinghat/cli/utils.py` & `sortinghat-0.9.0rc2/sortinghat/cli/utils.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/sortinghat/config/settings.py` & `sortinghat-0.9.0rc2/sortinghat/config/settings.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/sortinghat/core/admin.py` & `sortinghat-0.9.0rc2/sortinghat/core/admin.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/sortinghat/core/api.py` & `sortinghat-0.9.0rc2/sortinghat/core/api.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/sortinghat/core/apps.py` & `sortinghat-0.9.0rc2/sortinghat/core/apps.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/sortinghat/core/aux.py` & `sortinghat-0.9.0rc2/sortinghat/core/aux.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/sortinghat/core/context.py` & `sortinghat-0.9.0rc2/sortinghat/core/context.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/sortinghat/core/db.py` & `sortinghat-0.9.0rc2/sortinghat/core/db.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/sortinghat/core/decorators.py` & `sortinghat-0.9.0rc2/sortinghat/core/decorators.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/sortinghat/core/errors.py` & `sortinghat-0.9.0rc2/sortinghat/core/errors.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/sortinghat/core/fixtures/countries.json` & `sortinghat-0.9.0rc2/sortinghat/core/fixtures/countries.json`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/sortinghat/core/importer/backend.py` & `sortinghat-0.9.0rc2/sortinghat/core/importer/backend.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/sortinghat/core/importer/backends/mailmap.py` & `sortinghat-0.9.0rc2/sortinghat/core/importer/backends/mailmap.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/sortinghat/core/importer/base.py` & `sortinghat-0.9.0rc2/sortinghat/core/importer/base.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/sortinghat/core/importer/models.py` & `sortinghat-0.9.0rc2/sortinghat/core/importer/models.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/sortinghat/core/importer/utils.py` & `sortinghat-0.9.0rc2/sortinghat/core/importer/utils.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/sortinghat/core/jobs.py` & `sortinghat-0.9.0rc2/sortinghat/core/jobs.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/sortinghat/core/log.py` & `sortinghat-0.9.0rc2/sortinghat/core/log.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/sortinghat/core/management/commands/create_groups.py` & `sortinghat-0.9.0rc2/sortinghat/core/management/commands/create_groups.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/sortinghat/core/middleware.py` & `sortinghat-0.9.0rc2/sortinghat/core/middleware.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/sortinghat/core/migrations/0001_sortinghat.py` & `sortinghat-0.9.0rc2/sortinghat/core/migrations/0001_sortinghat.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/sortinghat/core/migrations/0002_importidentitiestask.py` & `sortinghat-0.9.0rc2/sortinghat/core/migrations/0002_importidentitiestask.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/sortinghat/core/migrations/0003_multi_tenancy.py` & `sortinghat-0.9.0rc2/sortinghat/core/migrations/0003_multi_tenancy.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/sortinghat/core/models.py` & `sortinghat-0.9.0rc2/sortinghat/core/models.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/sortinghat/core/recommendations/__init__.py` & `sortinghat-0.9.0rc2/sortinghat/core/recommendations/__init__.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/sortinghat/core/recommendations/affiliation.py` & `sortinghat-0.9.0rc2/sortinghat/core/recommendations/affiliation.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/sortinghat/core/recommendations/engine.py` & `sortinghat-0.9.0rc2/sortinghat/core/recommendations/engine.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/sortinghat/core/recommendations/exclusion.py` & `sortinghat-0.9.0rc2/sortinghat/core/recommendations/exclusion.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/sortinghat/core/recommendations/gender.py` & `sortinghat-0.9.0rc2/sortinghat/core/recommendations/gender.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/sortinghat/core/recommendations/matching.py` & `sortinghat-0.9.0rc2/sortinghat/core/recommendations/matching.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/sortinghat/core/schema.py` & `sortinghat-0.9.0rc2/sortinghat/core/schema.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/sortinghat/core/tenant.py` & `sortinghat-0.9.0rc2/sortinghat/core/tenant.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/sortinghat/core/views.py` & `sortinghat-0.9.0rc2/sortinghat/core/views.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/sortinghat/server/sortinghat_admin.py` & `sortinghat-0.9.0rc2/sortinghat/server/sortinghat_admin.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/sortinghat/server/sortinghatd.py` & `sortinghat-0.9.0rc2/sortinghat/server/sortinghatd.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/sortinghat/server/sortinghatw.py` & `sortinghat-0.9.0rc2/sortinghat/server/sortinghatw.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/sortinghat/server/utils/create_sh_0_7_fixture.py` & `sortinghat-0.9.0rc2/sortinghat/server/utils/create_sh_0_7_fixture.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/sortinghat/utils/__init__.py` & `sortinghat-0.9.0rc2/sortinghat/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/tests/cli/test_cmd_add.py` & `sortinghat-0.9.0rc2/tests/cli/test_cmd_add.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/tests/cli/test_cmd_config.py` & `sortinghat-0.9.0rc2/tests/cli/test_cmd_config.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/tests/cli/test_cmd_countries.py` & `sortinghat-0.9.0rc2/tests/cli/test_cmd_countries.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/tests/cli/test_cmd_enroll.py` & `sortinghat-0.9.0rc2/tests/cli/test_cmd_enroll.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/tests/cli/test_cmd_lock.py` & `sortinghat-0.9.0rc2/tests/cli/test_cmd_lock.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/tests/cli/test_cmd_merge.py` & `sortinghat-0.9.0rc2/tests/cli/test_cmd_merge.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/tests/cli/test_cmd_mv.py` & `sortinghat-0.9.0rc2/tests/cli/test_cmd_mv.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/tests/cli/test_cmd_orgs.py` & `sortinghat-0.9.0rc2/tests/cli/test_cmd_orgs.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/tests/cli/test_cmd_profile.py` & `sortinghat-0.9.0rc2/tests/cli/test_cmd_profile.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/tests/cli/test_cmd_rm.py` & `sortinghat-0.9.0rc2/tests/cli/test_cmd_rm.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/tests/cli/test_cmd_show.py` & `sortinghat-0.9.0rc2/tests/cli/test_cmd_show.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/tests/cli/test_cmd_split.py` & `sortinghat-0.9.0rc2/tests/cli/test_cmd_split.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/tests/cli/test_cmd_withdraw.py` & `sortinghat-0.9.0rc2/tests/cli/test_cmd_withdraw.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/tests/importer/mocked_package/backend_a.py` & `sortinghat-0.9.0rc2/tests/importer/mocked_package/backend_a.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/tests/importer/mocked_package/nested_package/nested_backend_b.py` & `sortinghat-0.9.0rc2/tests/importer/mocked_package/nested_package/nested_backend_b.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/tests/importer/mocked_package/nested_package/nested_backend_c.py` & `sortinghat-0.9.0rc2/tests/importer/mocked_package/nested_package/nested_backend_c.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/tests/importer/mocked_package/nested_package/nested_not_backend.py` & `sortinghat-0.9.0rc2/tests/importer/mocked_package/nested_package/nested_not_backend.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/tests/importer/test_backend.py` & `sortinghat-0.9.0rc2/tests/importer/test_backend.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/tests/importer/test_utils.py` & `sortinghat-0.9.0rc2/tests/importer/test_utils.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/tests/rec/test_affiliations.py` & `sortinghat-0.9.0rc2/tests/rec/test_affiliations.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/tests/rec/test_engine.py` & `sortinghat-0.9.0rc2/tests/rec/test_engine.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/tests/rec/test_exclusion.py` & `sortinghat-0.9.0rc2/tests/rec/test_exclusion.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/tests/rec/test_gender.py` & `sortinghat-0.9.0rc2/tests/rec/test_gender.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/tests/rec/test_matches.py` & `sortinghat-0.9.0rc2/tests/rec/test_matches.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/tests/runners.py` & `sortinghat-0.9.0rc2/tests/runners.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/tests/tenants/test_jobs.py` & `sortinghat-0.9.0rc2/tests/tenants/test_jobs.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/tests/tenants/test_middleware.py` & `sortinghat-0.9.0rc2/tests/tenants/test_middleware.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/tests/tenants/test_schema.py` & `sortinghat-0.9.0rc2/tests/tenants/test_schema.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/tests/test_api.py` & `sortinghat-0.9.0rc2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/tests/test_aux.py` & `sortinghat-0.9.0rc2/tests/test_aux.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/tests/test_client.py` & `sortinghat-0.9.0rc2/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/tests/test_db.py` & `sortinghat-0.9.0rc2/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/tests/test_errors.py` & `sortinghat-0.9.0rc2/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/tests/test_jobs.py` & `sortinghat-0.9.0rc2/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/tests/test_log.py` & `sortinghat-0.9.0rc2/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/tests/test_model.py` & `sortinghat-0.9.0rc2/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/tests/test_schema.py` & `sortinghat-0.9.0rc2/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/tests/test_utils.py` & `sortinghat-0.9.0rc2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.0rc1/PKG-INFO` & `sortinghat-0.9.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sortinghat
-Version: 0.9.0rc1
+Version: 0.9.0rc2
 Summary: A tool to manage identities.
 Home-page: https://chaoss.github.io/grimoirelab/
 License: GPL-3.0+
 Keywords: development,grimoirelab
 Author: GrimoireLab Developers
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: Development Status :: 4 - Beta
```

