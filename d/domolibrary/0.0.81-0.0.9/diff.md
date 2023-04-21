# Comparing `tmp/domolibrary-0.0.81.tar.gz` & `tmp/domolibrary-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domolibrary-0.0.81.tar", last modified: Fri Apr 21 12:00:46 2023, max compression
+gzip compressed data, was "domolibrary-0.0.9.tar", last modified: Mon Jan 30 17:31:54 2023, max compression
```

## Comparing `domolibrary-0.0.81.tar` & `domolibrary-0.0.9.tar`

### file list

```diff
@@ -1,144 +1,122 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-21 12:00:46.714491 domolibrary-0.0.81/
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-21 12:00:46.590492 domolibrary-0.0.81/Automation/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.0.81/Automation/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6580 2023-01-05 15:38:44.000000 domolibrary-0.0.81/Automation/automation.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-21 12:00:46.602492 domolibrary-0.0.81/DataOcean/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2534 2023-01-05 15:38:44.000000 domolibrary-0.0.81/DataOcean/Transport.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.0.81/DataOcean/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2263 2023-01-05 15:38:44.000000 domolibrary-0.0.81/DataOcean/cnfg_athena_highbandwidth.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3060 2023-01-05 15:38:44.000000 domolibrary-0.0.81/DataOcean/cnfg_pgsql.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3402 2023-01-05 15:38:44.000000 domolibrary-0.0.81/DataOcean/cnfg_s3.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3514 2023-01-05 15:38:44.000000 domolibrary-0.0.81/DataOcean/cnfg_snowflake.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-21 12:00:46.638491 domolibrary-0.0.81/DomoClasses/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9543 2023-01-17 21:03:25.000000 domolibrary-0.0.81/DomoClasses/DomoAccount.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2504 2023-01-05 15:38:44.000000 domolibrary-0.0.81/DomoClasses/DomoActivityLog.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1904 2023-01-05 15:38:44.000000 domolibrary-0.0.81/DomoClasses/DomoAppDb.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4514 2023-03-02 20:34:40.000000 domolibrary-0.0.81/DomoClasses/DomoApplication.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5125 2023-01-05 15:38:44.000000 domolibrary-0.0.81/DomoClasses/DomoAuth.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1680 2023-01-17 21:03:25.000000 domolibrary-0.0.81/DomoClasses/DomoBootstrap.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1643 2023-01-05 15:38:44.000000 domolibrary-0.0.81/DomoClasses/DomoCard.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      767 2023-01-05 15:38:44.000000 domolibrary-0.0.81/DomoClasses/DomoCertification.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8511 2023-01-17 21:03:25.000000 domolibrary-0.0.81/DomoClasses/DomoDatacenter.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1789 2023-01-05 15:38:44.000000 domolibrary-0.0.81/DomoClasses/DomoDataflow.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    19304 2023-01-05 15:38:44.000000 domolibrary-0.0.81/DomoClasses/DomoDataset.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      727 2023-01-05 15:38:44.000000 domolibrary-0.0.81/DomoClasses/DomoGrant.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8797 2023-01-05 15:38:44.000000 domolibrary-0.0.81/DomoClasses/DomoGroup.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8972 2023-01-05 15:38:44.000000 domolibrary-0.0.81/DomoClasses/DomoInstanceConfig.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12851 2023-04-03 12:48:28.000000 domolibrary-0.0.81/DomoClasses/DomoJob.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8279 2023-01-05 15:38:44.000000 domolibrary-0.0.81/DomoClasses/DomoLineage.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3950 2023-01-05 15:38:44.000000 domolibrary-0.0.81/DomoClasses/DomoPDP.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15635 2023-02-08 21:41:51.000000 domolibrary-0.0.81/DomoClasses/DomoPage.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10879 2023-01-05 15:38:44.000000 domolibrary-0.0.81/DomoClasses/DomoPublish.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4464 2023-01-05 15:38:44.000000 domolibrary-0.0.81/DomoClasses/DomoRole.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2963 2023-01-05 15:38:44.000000 domolibrary-0.0.81/DomoClasses/DomoSandbox.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7127 2023-01-17 21:03:25.000000 domolibrary-0.0.81/DomoClasses/DomoStream.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3073 2023-01-05 15:38:44.000000 domolibrary-0.0.81/DomoClasses/DomoTag.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8118 2023-01-05 15:38:44.000000 domolibrary-0.0.81/DomoClasses/DomoUser.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.0.81/DomoClasses/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-21 12:00:46.650491 domolibrary-0.0.81/DomoClasses/routes/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.0.81/DomoClasses/routes/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6391 2023-01-17 21:03:25.000000 domolibrary-0.0.81/DomoClasses/routes/account_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1469 2023-01-05 15:38:44.000000 domolibrary-0.0.81/DomoClasses/routes/activity_log_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1359 2023-01-05 15:38:44.000000 domolibrary-0.0.81/DomoClasses/routes/appdb_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1294 2023-01-05 15:38:44.000000 domolibrary-0.0.81/DomoClasses/routes/application_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1763 2023-01-05 15:38:44.000000 domolibrary-0.0.81/DomoClasses/routes/auth_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      889 2023-01-05 15:38:44.000000 domolibrary-0.0.81/DomoClasses/routes/bootstrap_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2638 2023-01-05 15:38:44.000000 domolibrary-0.0.81/DomoClasses/routes/card_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3711 2023-01-05 15:38:44.000000 domolibrary-0.0.81/DomoClasses/routes/datacenter_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      830 2023-01-05 15:38:44.000000 domolibrary-0.0.81/DomoClasses/routes/dataflow_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    13688 2023-01-05 15:38:44.000000 domolibrary-0.0.81/DomoClasses/routes/dataset_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6044 2023-04-03 12:48:28.000000 domolibrary-0.0.81/DomoClasses/routes/get_data.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      977 2023-01-05 15:38:44.000000 domolibrary-0.0.81/DomoClasses/routes/grant_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4523 2023-01-05 15:38:44.000000 domolibrary-0.0.81/DomoClasses/routes/group_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2697 2023-01-05 15:38:44.000000 domolibrary-0.0.81/DomoClasses/routes/instance_config_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6434 2023-03-02 20:34:40.000000 domolibrary-0.0.81/DomoClasses/routes/job_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3183 2023-01-31 17:52:06.000000 domolibrary-0.0.81/DomoClasses/routes/page_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2470 2023-01-05 15:38:44.000000 domolibrary-0.0.81/DomoClasses/routes/pdp_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4670 2023-01-05 15:38:44.000000 domolibrary-0.0.81/DomoClasses/routes/publish_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3836 2023-01-05 15:38:44.000000 domolibrary-0.0.81/DomoClasses/routes/role_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2204 2023-01-05 15:38:44.000000 domolibrary-0.0.81/DomoClasses/routes/sandbox_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1633 2023-01-05 15:38:44.000000 domolibrary-0.0.81/DomoClasses/routes/stream_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4371 2023-01-05 15:38:44.000000 domolibrary-0.0.81/DomoClasses/routes/user_routes.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-21 12:00:46.650491 domolibrary-0.0.81/GitHub/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.0.81/GitHub/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      322 2023-01-05 15:38:44.000000 domolibrary-0.0.81/GitHub/get_github_file.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11337 2023-01-05 15:38:44.000000 domolibrary-0.0.81/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      111 2023-01-05 15:38:44.000000 domolibrary-0.0.81/MANIFEST.in
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8774 2023-04-21 12:00:46.714491 domolibrary-0.0.81/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7997 2023-04-04 23:21:28.000000 domolibrary-0.0.81/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-21 12:00:46.654491 domolibrary-0.0.81/domolibrary/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       23 2023-04-21 12:00:15.000000 domolibrary-0.0.81/domolibrary/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   145313 2023-04-21 12:00:15.000000 domolibrary-0.0.81/domolibrary/_modidx.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-21 12:00:46.674491 domolibrary-0.0.81/domolibrary/classes/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15664 2023-04-21 12:00:15.000000 domolibrary-0.0.81/domolibrary/classes/DomoAccount.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4070 2023-04-21 12:00:15.000000 domolibrary-0.0.81/domolibrary/classes/DomoActivityLog.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3015 2023-04-21 12:00:15.000000 domolibrary-0.0.81/domolibrary/classes/DomoBootstrap.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4119 2023-04-21 12:00:15.000000 domolibrary-0.0.81/domolibrary/classes/DomoDatacenter.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2706 2023-04-21 12:00:15.000000 domolibrary-0.0.81/domolibrary/classes/DomoDataflow.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    25103 2023-04-21 12:00:15.000000 domolibrary-0.0.81/domolibrary/classes/DomoDataset.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1255 2023-04-21 12:00:15.000000 domolibrary-0.0.81/domolibrary/classes/DomoGrant.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    17403 2023-04-21 12:00:15.000000 domolibrary-0.0.81/domolibrary/classes/DomoGroup.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6174 2023-04-21 12:00:15.000000 domolibrary-0.0.81/domolibrary/classes/DomoInstanceConfig.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12109 2023-04-21 12:00:15.000000 domolibrary-0.0.81/domolibrary/classes/DomoPDP.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3801 2023-04-21 12:00:15.000000 domolibrary-0.0.81/domolibrary/classes/DomoPage.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6985 2023-04-21 12:00:15.000000 domolibrary-0.0.81/domolibrary/classes/DomoPublish.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15572 2023-04-21 12:00:15.000000 domolibrary-0.0.81/domolibrary/classes/DomoRole.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11913 2023-04-21 12:00:15.000000 domolibrary-0.0.81/domolibrary/classes/DomoUser.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-21 12:00:15.000000 domolibrary-0.0.81/domolibrary/classes/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-21 12:00:46.678491 domolibrary-0.0.81/domolibrary/client/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12655 2023-04-21 12:00:15.000000 domolibrary-0.0.81/domolibrary/client/DomoAuth.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2069 2023-04-21 12:00:15.000000 domolibrary-0.0.81/domolibrary/client/DomoError.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5929 2023-04-21 12:00:15.000000 domolibrary-0.0.81/domolibrary/client/Logger.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6189 2023-04-21 12:00:15.000000 domolibrary-0.0.81/domolibrary/client/ResponseGetData.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-21 12:00:15.000000 domolibrary-0.0.81/domolibrary/client/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12027 2023-04-21 12:00:15.000000 domolibrary-0.0.81/domolibrary/client/get_data.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-21 12:00:46.678491 domolibrary-0.0.81/domolibrary/integrations/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15484 2023-04-21 12:00:15.000000 domolibrary-0.0.81/domolibrary/integrations/DomoJupyter.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-21 12:00:15.000000 domolibrary-0.0.81/domolibrary/integrations/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-21 12:00:46.686491 domolibrary-0.0.81/domolibrary/routes/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-21 12:00:15.000000 domolibrary-0.0.81/domolibrary/routes/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7968 2023-04-21 12:00:15.000000 domolibrary-0.0.81/domolibrary/routes/account.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2035 2023-04-21 12:00:15.000000 domolibrary-0.0.81/domolibrary/routes/activity_log.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2039 2023-04-21 12:00:15.000000 domolibrary-0.0.81/domolibrary/routes/bootstrap.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3425 2023-04-21 12:00:15.000000 domolibrary-0.0.81/domolibrary/routes/card.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6442 2023-04-21 12:00:15.000000 domolibrary-0.0.81/domolibrary/routes/datacenter.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      769 2023-04-21 12:00:15.000000 domolibrary-0.0.81/domolibrary/routes/dataflow.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15254 2023-04-21 12:00:15.000000 domolibrary-0.0.81/domolibrary/routes/dataset.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1682 2023-04-21 12:00:15.000000 domolibrary-0.0.81/domolibrary/routes/grant.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10945 2023-04-21 12:00:15.000000 domolibrary-0.0.81/domolibrary/routes/group.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4807 2023-04-21 12:00:15.000000 domolibrary-0.0.81/domolibrary/routes/instance_config.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2463 2023-04-21 12:00:15.000000 domolibrary-0.0.81/domolibrary/routes/page.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7214 2023-04-21 12:00:15.000000 domolibrary-0.0.81/domolibrary/routes/pdp.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4174 2023-04-21 12:00:15.000000 domolibrary-0.0.81/domolibrary/routes/publish.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8584 2023-04-21 12:00:15.000000 domolibrary-0.0.81/domolibrary/routes/role.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8693 2023-04-21 12:00:15.000000 domolibrary-0.0.81/domolibrary/routes/user.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-21 12:00:46.690491 domolibrary-0.0.81/domolibrary/utils/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1660 2023-04-21 12:00:15.000000 domolibrary-0.0.81/domolibrary/utils/DictDot.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-21 12:00:15.000000 domolibrary-0.0.81/domolibrary/utils/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      865 2023-04-21 12:00:15.000000 domolibrary-0.0.81/domolibrary/utils/chunk_execution.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1732 2023-04-21 12:00:15.000000 domolibrary-0.0.81/domolibrary/utils/convert.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1184 2023-04-21 12:00:15.000000 domolibrary-0.0.81/domolibrary/utils/read_creds_from_dotenv.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4519 2023-04-21 12:00:15.000000 domolibrary-0.0.81/domolibrary/utils/upload_data.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-21 12:00:46.662491 domolibrary-0.0.81/domolibrary.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8774 2023-04-21 12:00:46.000000 domolibrary-0.0.81/domolibrary.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3800 2023-04-21 12:00:46.000000 domolibrary-0.0.81/domolibrary.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-04-21 12:00:46.000000 domolibrary-0.0.81/domolibrary.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       65 2023-04-21 12:00:46.000000 domolibrary-0.0.81/domolibrary.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-02-17 20:52:42.000000 domolibrary-0.0.81/domolibrary.egg-info/not-zip-safe
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      105 2023-04-21 12:00:46.000000 domolibrary-0.0.81/domolibrary.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       58 2023-04-21 12:00:46.000000 domolibrary-0.0.81/domolibrary.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1083 2023-04-21 12:00:24.000000 domolibrary-0.0.81/settings.ini
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-04-21 12:00:46.714491 domolibrary-0.0.81/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2539 2023-01-06 02:41:16.000000 domolibrary-0.0.81/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-21 12:00:46.710491 domolibrary-0.0.81/utils/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      540 2023-01-05 15:38:44.000000 domolibrary-0.0.81/utils/Base.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      759 2023-01-05 15:38:44.000000 domolibrary-0.0.81/utils/DictDot.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1220 2023-01-09 21:38:41.000000 domolibrary-0.0.81/utils/Exceptions.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2578 2023-01-17 21:03:25.000000 domolibrary-0.0.81/utils/LoggerClass.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      273 2023-01-05 15:38:44.000000 domolibrary-0.0.81/utils/ResponseGetData.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.0.81/utils/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1145 2023-01-05 15:38:44.000000 domolibrary-0.0.81/utils/chunk_execution.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1133 2023-01-05 15:38:44.000000 domolibrary-0.0.81/utils/consol_get_creds.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      522 2023-01-05 15:38:44.000000 domolibrary-0.0.81/utils/convert.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1476 2023-01-05 15:38:44.000000 domolibrary-0.0.81/utils/read_creds_from_dotenv.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3671 2023-03-06 14:03:40.000000 domolibrary-0.0.81/utils/upload_data.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-01-30 17:31:54.796988 domolibrary-0.0.9/
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-01-30 17:31:54.780988 domolibrary-0.0.9/Automation/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.0.9/Automation/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6580 2023-01-05 15:38:44.000000 domolibrary-0.0.9/Automation/automation.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-01-30 17:31:54.780988 domolibrary-0.0.9/DataOcean/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2534 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DataOcean/Transport.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DataOcean/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2263 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DataOcean/cnfg_athena_highbandwidth.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3060 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DataOcean/cnfg_pgsql.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3402 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DataOcean/cnfg_s3.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3514 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DataOcean/cnfg_snowflake.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-01-30 17:31:54.784988 domolibrary-0.0.9/DomoClasses/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9543 2023-01-17 21:03:25.000000 domolibrary-0.0.9/DomoClasses/DomoAccount.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2504 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/DomoActivityLog.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1904 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/DomoAppDb.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4504 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/DomoApplication.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5125 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/DomoAuth.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1680 2023-01-17 21:03:25.000000 domolibrary-0.0.9/DomoClasses/DomoBootstrap.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1643 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/DomoCard.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      767 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/DomoCertification.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8511 2023-01-17 21:03:25.000000 domolibrary-0.0.9/DomoClasses/DomoDatacenter.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1789 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/DomoDataflow.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    19304 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/DomoDataset.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      727 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/DomoGrant.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8797 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/DomoGroup.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8972 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/DomoInstanceConfig.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12089 2023-01-17 21:03:25.000000 domolibrary-0.0.9/DomoClasses/DomoJob.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8279 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/DomoLineage.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3950 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/DomoPDP.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3370 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/DomoPage.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10879 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/DomoPublish.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4464 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/DomoRole.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2963 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/DomoSandbox.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7127 2023-01-17 21:03:25.000000 domolibrary-0.0.9/DomoClasses/DomoStream.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3073 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/DomoTag.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8118 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/DomoUser.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-01-30 17:31:54.788988 domolibrary-0.0.9/DomoClasses/routes/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/routes/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6391 2023-01-17 21:03:25.000000 domolibrary-0.0.9/DomoClasses/routes/account_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1469 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/routes/activity_log_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1359 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/routes/appdb_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1294 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/routes/application_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1763 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/routes/auth_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      889 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/routes/bootstrap_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2638 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/routes/card_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3711 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/routes/datacenter_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      830 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/routes/dataflow_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    13688 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/routes/dataset_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6036 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/routes/get_data.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      977 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/routes/grant_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4523 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/routes/group_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2697 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/routes/instance_config_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5695 2023-01-17 21:03:25.000000 domolibrary-0.0.9/DomoClasses/routes/job_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1386 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/routes/page_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2470 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/routes/pdp_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4670 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/routes/publish_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3836 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/routes/role_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2204 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/routes/sandbox_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1633 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/routes/stream_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4371 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/routes/user_routes.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-01-30 17:31:54.788988 domolibrary-0.0.9/GitHub/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.0.9/GitHub/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      322 2023-01-05 15:38:44.000000 domolibrary-0.0.9/GitHub/get_github_file.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11337 2023-01-05 15:38:44.000000 domolibrary-0.0.9/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      111 2023-01-05 15:38:44.000000 domolibrary-0.0.9/MANIFEST.in
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11131 2023-01-30 17:31:54.796988 domolibrary-0.0.9/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10355 2023-01-30 17:30:00.000000 domolibrary-0.0.9/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-01-30 17:31:54.788988 domolibrary-0.0.9/domolibrary/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       22 2023-01-30 17:29:32.000000 domolibrary-0.0.9/domolibrary/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    77437 2023-01-30 17:29:32.000000 domolibrary-0.0.9/domolibrary/_modidx.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-01-30 17:31:54.792988 domolibrary-0.0.9/domolibrary/classes/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10073 2023-01-30 17:29:32.000000 domolibrary-0.0.9/domolibrary/classes/DomoAccount.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4070 2023-01-30 17:29:32.000000 domolibrary-0.0.9/domolibrary/classes/DomoActivityLog.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3015 2023-01-30 17:29:32.000000 domolibrary-0.0.9/domolibrary/classes/DomoBootstrap.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24047 2023-01-30 17:29:32.000000 domolibrary-0.0.9/domolibrary/classes/DomoDataset.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2108 2023-01-30 17:29:32.000000 domolibrary-0.0.9/domolibrary/classes/DomoPage.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9363 2023-01-30 17:29:32.000000 domolibrary-0.0.9/domolibrary/classes/DomoUser.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-30 17:29:32.000000 domolibrary-0.0.9/domolibrary/classes/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-01-30 17:31:54.792988 domolibrary-0.0.9/domolibrary/client/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11517 2023-01-30 17:29:32.000000 domolibrary-0.0.9/domolibrary/client/DomoAuth.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5929 2023-01-30 17:29:32.000000 domolibrary-0.0.9/domolibrary/client/Logger.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4830 2023-01-30 17:29:32.000000 domolibrary-0.0.9/domolibrary/client/ResponseGetData.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-30 17:29:32.000000 domolibrary-0.0.9/domolibrary/client/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11038 2023-01-30 17:29:32.000000 domolibrary-0.0.9/domolibrary/client/get_data.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-01-30 17:31:54.792988 domolibrary-0.0.9/domolibrary/integrations/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    17028 2023-01-30 17:29:32.000000 domolibrary-0.0.9/domolibrary/integrations/DomoJupyter.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-30 17:29:32.000000 domolibrary-0.0.9/domolibrary/integrations/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-01-30 17:31:54.792988 domolibrary-0.0.9/domolibrary/routes/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-30 17:29:32.000000 domolibrary-0.0.9/domolibrary/routes/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5153 2023-01-30 17:29:32.000000 domolibrary-0.0.9/domolibrary/routes/account.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2030 2023-01-30 17:29:32.000000 domolibrary-0.0.9/domolibrary/routes/activity_log.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2116 2023-01-30 17:29:32.000000 domolibrary-0.0.9/domolibrary/routes/bootstrap.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15781 2023-01-30 17:29:32.000000 domolibrary-0.0.9/domolibrary/routes/dataset.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5783 2023-01-30 17:29:32.000000 domolibrary-0.0.9/domolibrary/routes/user.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-01-30 17:31:54.792988 domolibrary-0.0.9/domolibrary/utils/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1077 2023-01-30 17:29:32.000000 domolibrary-0.0.9/domolibrary/utils/DictDot.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-30 17:29:32.000000 domolibrary-0.0.9/domolibrary/utils/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      919 2023-01-30 17:29:32.000000 domolibrary-0.0.9/domolibrary/utils/convert.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-01-30 17:31:54.788988 domolibrary-0.0.9/domolibrary.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11131 2023-01-30 17:31:54.000000 domolibrary-0.0.9/domolibrary.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3079 2023-01-30 17:31:54.000000 domolibrary-0.0.9/domolibrary.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-01-30 17:31:54.000000 domolibrary-0.0.9/domolibrary.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       65 2023-01-30 17:31:54.000000 domolibrary-0.0.9/domolibrary.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-01-11 00:36:49.000000 domolibrary-0.0.9/domolibrary.egg-info/not-zip-safe
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       65 2023-01-30 17:31:54.000000 domolibrary-0.0.9/domolibrary.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       58 2023-01-30 17:31:54.000000 domolibrary-0.0.9/domolibrary.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1028 2023-01-30 17:31:52.000000 domolibrary-0.0.9/settings.ini
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-01-30 17:31:54.796988 domolibrary-0.0.9/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2539 2023-01-06 02:41:16.000000 domolibrary-0.0.9/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-01-30 17:31:54.796988 domolibrary-0.0.9/utils/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      540 2023-01-05 15:38:44.000000 domolibrary-0.0.9/utils/Base.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      759 2023-01-05 15:38:44.000000 domolibrary-0.0.9/utils/DictDot.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1220 2023-01-09 21:38:41.000000 domolibrary-0.0.9/utils/Exceptions.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2578 2023-01-17 21:03:25.000000 domolibrary-0.0.9/utils/LoggerClass.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      273 2023-01-05 15:38:44.000000 domolibrary-0.0.9/utils/ResponseGetData.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.0.9/utils/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1145 2023-01-05 15:38:44.000000 domolibrary-0.0.9/utils/chunk_execution.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1133 2023-01-05 15:38:44.000000 domolibrary-0.0.9/utils/consol_get_creds.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      522 2023-01-05 15:38:44.000000 domolibrary-0.0.9/utils/convert.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1476 2023-01-05 15:38:44.000000 domolibrary-0.0.9/utils/read_creds_from_dotenv.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3659 2023-01-05 15:38:44.000000 domolibrary-0.0.9/utils/upload_data.py
```

### Comparing `domolibrary-0.0.81/Automation/automation.py` & `domolibrary-0.0.9/Automation/automation.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.81/DataOcean/Transport.py` & `domolibrary-0.0.9/DataOcean/Transport.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.81/DataOcean/cnfg_athena_highbandwidth.py` & `domolibrary-0.0.9/DataOcean/cnfg_athena_highbandwidth.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.81/DataOcean/cnfg_pgsql.py` & `domolibrary-0.0.9/DataOcean/cnfg_pgsql.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.81/DataOcean/cnfg_s3.py` & `domolibrary-0.0.9/DataOcean/cnfg_s3.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.81/DataOcean/cnfg_snowflake.py` & `domolibrary-0.0.9/DataOcean/cnfg_snowflake.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.81/DomoClasses/DomoAccount.py` & `domolibrary-0.0.9/DomoClasses/DomoAccount.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.81/DomoClasses/DomoActivityLog.py` & `domolibrary-0.0.9/DomoClasses/DomoActivityLog.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.81/DomoClasses/DomoAppDb.py` & `domolibrary-0.0.9/DomoClasses/DomoAppDb.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.81/DomoClasses/DomoApplication.py` & `domolibrary-0.0.9/DomoClasses/DomoApplication.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,9 +107,9 @@
             value=0)
         schedules_interpolated.sort_values(
             ['cnt_schedule', 'hour', 'minute'], ascending=True, inplace=True)
 
         schedules_interpolated.reset_index(drop=True, inplace=True)
 
         return dmdj.DomoTrigger_Schedule(
-            hour=int(schedules_interpolated.loc[0].get('hour')),
-            minute=int(schedules_interpolated.loc[0].get('minute')))
+            hour=schedules_interpolated.loc[0].get('hour'),
+            minute=schedules_interpolated.loc[0].get('minute'))
```

### Comparing `domolibrary-0.0.81/DomoClasses/DomoAuth.py` & `domolibrary-0.0.9/DomoClasses/DomoAuth.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.81/DomoClasses/DomoBootstrap.py` & `domolibrary-0.0.9/DomoClasses/DomoBootstrap.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.81/DomoClasses/DomoCard.py` & `domolibrary-0.0.9/DomoClasses/DomoCard.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.81/DomoClasses/DomoCertification.py` & `domolibrary-0.0.9/DomoClasses/DomoCertification.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.81/DomoClasses/DomoDatacenter.py` & `domolibrary-0.0.9/DomoClasses/DomoDatacenter.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.81/DomoClasses/DomoDataflow.py` & `domolibrary-0.0.9/DomoClasses/DomoDataflow.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.81/DomoClasses/DomoDataset.py` & `domolibrary-0.0.9/DomoClasses/DomoDataset.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.81/DomoClasses/DomoGrant.py` & `domolibrary-0.0.9/DomoClasses/DomoGrant.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.81/DomoClasses/DomoGroup.py` & `domolibrary-0.0.9/DomoClasses/DomoGroup.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.81/DomoClasses/DomoInstanceConfig.py` & `domolibrary-0.0.9/DomoClasses/DomoInstanceConfig.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.81/DomoClasses/DomoJob.py` & `domolibrary-0.0.9/DomoClasses/DomoJob.py`

 * *Files 12% similar despite different names*

```diff
@@ -37,15 +37,15 @@
             schedule_type=s_type,
             schedule_text=s_text)
 
         try:
             parsed_hour =s_text.split(' ')[2]
             parsed_minute=s_text.split(' ')[1]
             
-            if "*" in parsed_hour or "/" in parsed_hour:
+            if "*" in parsed_hour:
                 sched.hour_str = parsed_hour
             else:
                 sched.hour = int(float(parsed_hour))
             if "*" in parsed_minute:
                 sched.minute_str = parsed_minute
             else:
                 sched.minute = int(float(parsed_minute))
@@ -80,15 +80,15 @@
 
 @dataclass
 class DomoJob:
     id: str
     name: str
     description :str
     remote_instance: str
-    user_id: str
+    user_id: int
     application_id: str
     customer_id: str
     execution_timeout: int
     entity_ids: list
     job_type: str
     entity_type: str
     max_indexing_time_min :int
@@ -103,14 +103,15 @@
     resources_limits: str
     
     triggers: [DomoTrigger] = None
 
     @classmethod
     def _from_json(cls, obj):
         dd = DictDot(obj)
+
         triggers_ls = obj.get('triggers', None)
 
         triggers_dj = [DomoTrigger(
             id=tg.get('triggerId'),
             job_id=tg.get('jobId'),
 
             schedule=DomoTrigger_Schedule._from_str(
@@ -123,21 +124,21 @@
                    customer_id=dd.customerId,
                    name=dd.jobName,
                    description = dd.jobDescription,
                    user_id=dd.userId,
                    remote_instance=dd.executionPayload.remoteInstance.replace(
                        '.domo.com', '') if dd.executionPayload.remoteInstance else None,
                    execution_timeout = dd.executionTimeout,
-                   entity_ids = dd.executionPayload.watcherParameters.entityIds if dd.executionPayload.watcherParameters else [],
-                   job_type = dd.executionPayload.watcherParameters.type if dd.executionPayload.watcherParameters else [],
-                   entity_type=dd.executionPayload.watcherParameters.entityType if dd.executionPayload.watcherParameters else [],
-                   max_indexing_time_min = dd.executionPayload.watcherParameters.maxIndexingTimeInMinutes if dd.executionPayload.watcherParameters else [],
-                   variance_percent = dd.executionPayload.watcherParameters.variancePercent if dd.executionPayload.watcherParameters else [],
-                   min_update_frequency_min = dd.executionPayload.watcherParameters.minDataUpdateFrequencyInMinutes if dd.executionPayload.watcherParameters else [],
-                   sql_query=dd.executionPayload.watcherParameters.sqlQuery if dd.executionPayload.watcherParameters else [],
+                   entity_ids = dd.executionPayload.watcherParameters.entityIds,
+                   job_type = dd.executionPayload.watcherParameters.type,
+                   entity_type=dd.executionPayload.watcherParameters.entityType,
+                   max_indexing_time_min = dd.executionPayload.watcherParameters.maxIndexingTimeInMinutes,
+                   variance_percent = dd.executionPayload.watcherParameters.variancePercent,
+                   min_update_frequency_min = dd.executionPayload.watcherParameters.minDataUpdateFrequencyInMinutes,
+                   sql_query=dd.executionPayload.watcherParameters.sqlQuery,
                    notify_user_ids=dd.executionPayload.notifyUserIds,
                    metrics_dataset_id=dd.executionPayload.metricsDatasetId,
                    notify_group_ids=dd.executionPayload.notifyGroupIds,
                    notify_email_addressess=dd.executionPayload.notifyEmailAddresses,
                    resources_requests =dd.resources.requests.memory,
                    resources_limits = dd.resources.limits.memory,
                    triggers=triggers_dj)
@@ -188,15 +189,15 @@
         body = job_routes.generate_body_remote_domostats(target_instance=target_instance,
                                                          report_dict=report_dict,
                                                          output_dataset_id=output_dataset_id,
                                                          account_id=account_id,
                                                          schedule_ls=[
                                                              schedule_obj],
                                                          execution_timeout=execution_timeout)
-        
+
         res = await job_routes.add_job(full_auth=full_auth,
                                        application_id=application_id,
                                        body=body,
                                        debug=debug,
                                        log_results=log_results,
                                        session=session)
         if debug:
@@ -206,52 +207,32 @@
             return False
 
         return True
 
     @classmethod
     async def create_watchdog_job(cls,
                                    full_auth: DomoFullAuth,
-                                   body : str,
-                                    application_id : str,
-                                   debug: bool = False, log_results: bool = False,
-                                   session: aiohttp.ClientSession = None):
-            
-            
-        res = await job_routes.add_job(full_auth=full_auth,
-                                       application_id=application_id,
-                                       body=body,
-                                       debug=debug,
-                                       log_results=log_results,
-                                       session=session)
-
-#         if debug:
-#             print(res)
-
-        if res.status != 200:
-            return False
-
-        return True
-    
-    @classmethod
-    async def generate_watchdog_body(cls,
                                    watchdog_report_type : WatchDogType,
                                    watchdog_schedule: DomoTrigger_Schedule,
+                                   application_id: str,
                                    job_name: str,
                                    notify_user_ids_ls: list,
                                    notify_group_ids_ls: list,
                                    notify_emails_ls: list,
                                    entity_ids_ls: list,
                                    entity_type : str,
                                    metric_dataset_id: str,
                                    sql_query :str = None,
                                    variance_percent: int = 30,
                                    max_indexing_time_mins: int = 30,
                                    execution_timeout: int = 1440,
                                    min_update_frequency_min: int = 1440,
-                           ):
+                                   debug: bool = False, log_results: bool = False,
+                                   session: aiohttp.ClientSession = None):
+
         schedule_obj = watchdog_schedule.to_schedule_obj()
 
         body = job_routes.generate_body_watchdog_generic(job_name=job_name,
                                                          notify_user_ids_ls=notify_user_ids_ls,
                                                          notify_group_ids_ls=notify_group_ids_ls,
                                                          notify_emails_ls=notify_emails_ls,
                                                          entity_ids_ls = entity_ids_ls,
@@ -260,38 +241,49 @@
                                                          schedule_ls=[
                                                              schedule_obj],
                                                          job_type = watchdog_report_type.value,
                                                          execution_timeout=execution_timeout)
         
 
         
-        if watchdog_report_type == watchdog_report_type.DATASET_INDEX_TIME:
+        if watchdog_report_type.DATASET_INDEX_TIME:
             child ={ "maxIndexingTimeInMinutes": max_indexing_time_mins }
             body["executionPayload"]["watcherParameters"].update(child)
 
   
         
-        if watchdog_report_type == watchdog_report_type.ROW_COUNT_CHANGE or watchdog_report_type == watchdog_report_type.OUTLIER_EXECUTION:
+        if watchdog_report_type.ROW_COUNT_CHANGE or watchdog_report_type.OUTLIER_EXECUTION:
             child ={ "variancePercent": variance_percent }
             body["executionPayload"]["watcherParameters"].update(child)
             
         
-        if watchdog_report_type == watchdog_report_type.CUSTOM_QUERY:
+        if watchdog_report_type.CUSTOM_QUERY:
             child ={ "sqlQuery": sql_query }
             body["executionPayload"]["watcherParameters"].update(child)
             
-        if watchdog_report_type == watchdog_report_type.LAST_UPDATED_DATA:
+        if watchdog_report_type.LAST_UPDATED_DATA:
             child ={ "minDataUpdateFrequencyInMinutes": min_update_frequency_min }
             body["executionPayload"]["watcherParameters"].update(child)
             
             
-        return body
-                            
-                            
-                            
+        res = await job_routes.add_job(full_auth=full_auth,
+                                       application_id=application_id,
+                                       body=body,
+                                       debug=debug,
+                                       log_results=log_results,
+                                       session=session)
+
+#         if debug:
+#             print(res)
+
+        if res.status != 200:
+            return False
+
+        return True
+    
     @classmethod
     async def update_job(cls,
                          full_auth: DomoFullAuth,
                          body: str,
                          job_id: str,
                          application_id: str,
                          debug: bool = False,
```

### Comparing `domolibrary-0.0.81/DomoClasses/DomoLineage.py` & `domolibrary-0.0.9/DomoClasses/DomoLineage.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.81/DomoClasses/DomoPDP.py` & `domolibrary-0.0.9/DomoClasses/DomoPDP.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.81/DomoClasses/DomoPublish.py` & `domolibrary-0.0.9/DomoClasses/DomoPublish.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.81/DomoClasses/DomoRole.py` & `domolibrary-0.0.9/DomoClasses/DomoRole.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.81/DomoClasses/DomoSandbox.py` & `domolibrary-0.0.9/DomoClasses/DomoSandbox.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.81/DomoClasses/DomoStream.py` & `domolibrary-0.0.9/DomoClasses/DomoStream.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.81/DomoClasses/DomoTag.py` & `domolibrary-0.0.9/DomoClasses/DomoTag.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.81/DomoClasses/DomoUser.py` & `domolibrary-0.0.9/DomoClasses/DomoUser.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.81/DomoClasses/routes/account_routes.py` & `domolibrary-0.0.9/DomoClasses/routes/account_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.81/DomoClasses/routes/activity_log_routes.py` & `domolibrary-0.0.9/DomoClasses/routes/activity_log_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.81/DomoClasses/routes/appdb_routes.py` & `domolibrary-0.0.9/DomoClasses/routes/appdb_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.81/DomoClasses/routes/application_routes.py` & `domolibrary-0.0.9/DomoClasses/routes/application_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.81/DomoClasses/routes/auth_routes.py` & `domolibrary-0.0.9/DomoClasses/routes/auth_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.81/DomoClasses/routes/bootstrap_routes.py` & `domolibrary-0.0.9/DomoClasses/routes/bootstrap_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.81/DomoClasses/routes/card_routes.py` & `domolibrary-0.0.9/DomoClasses/routes/card_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.81/DomoClasses/routes/datacenter_routes.py` & `domolibrary-0.0.9/DomoClasses/routes/datacenter_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.81/DomoClasses/routes/dataflow_routes.py` & `domolibrary-0.0.9/DomoClasses/routes/dataflow_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.81/DomoClasses/routes/dataset_routes.py` & `domolibrary-0.0.9/DomoClasses/routes/dataset_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.81/DomoClasses/routes/get_data.py` & `domolibrary-0.0.9/DomoClasses/routes/get_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         if debug:
             print('passing json')
 
         res = await session.request(method=method.upper(),
                                     url=url, headers=headers,
                                     json=body,
                                     params=params)
-        
+
     elif body is not None:
         res = await session.request(method=method.upper(),
                                     url=url,
                                     headers=headers,
                                     data=body,
                                     params=params)
```

### Comparing `domolibrary-0.0.81/DomoClasses/routes/grant_routes.py` & `domolibrary-0.0.9/DomoClasses/routes/grant_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.81/DomoClasses/routes/group_routes.py` & `domolibrary-0.0.9/DomoClasses/routes/group_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.81/DomoClasses/routes/instance_config_routes.py` & `domolibrary-0.0.9/DomoClasses/routes/instance_config_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.81/DomoClasses/routes/job_routes.py` & `domolibrary-0.0.9/DomoClasses/routes/job_routes.py`

 * *Files 7% similar despite different names*

```diff
@@ -179,35 +179,8 @@
         auth=full_auth,
         url=url,
         method='PUT',
         body=body,
         log_results=log_results,
         debug=debug,
         session=session
-    )
-
-#update trigger
-
-async def update_job_trigger(full_auth: DomoFullAuth,
-                  body: dict,
-                  job_id :str,
-                  trigger_id : str,  
-                  application_id: str,
-                  session: aiohttp.ClientSession = None,
-                  debug: bool = False,
-                  log_results: bool = False
-                  ):
-
-    url = f'https://{full_auth.domo_instance}.domo.com/api/executor/v1/applications/{application_id}/jobs/{job_id}/triggers/{trigger_id}'
-
-    if debug:
-        print(url)
-
-    return await get_data(
-        auth=full_auth,
-        url=url,
-        method='PUT',
-        body=body,
-        log_results=log_results,
-        debug=debug,
-        session=session
-    )
+    )
```

### Comparing `domolibrary-0.0.81/DomoClasses/routes/page_routes.py` & `domolibrary-0.0.9/DomoClasses/routes/pdp_routes.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,109 +1,94 @@
 import aiohttp
+import pandas as pd
+import io
+from pprint import pprint
 
-from .get_data import get_data
-from ..DomoAuth import DomoFullAuth
+from .get_data import get_data, looper
+from ..DomoAuth import DomoDeveloperAuth, DomoFullAuth
 from ...utils.ResponseGetData import ResponseGetData
 
 
+async def get_pdp_policies(full_auth: DomoFullAuth, dataset_id: str, debug: bool = False) -> ResponseGetData:
+    url = f'http://{full_auth.domo_instance}.domo.com/api/query/v1/data-control/{dataset_id}/filter-groups/'
+
+    if debug:
+        print(url)
 
-async def get_page_by_id(full_auth: DomoFullAuth, page_id: str,
-                         debug: bool = False, log_result: bool = False, include_layout: bool = False) -> ResponseGetData:
-    url = f'https://{full_auth.domo_instance}.domo.com/api/content/v3/stacks/{page_id}/cards'
-    if include_layout:
-        url+='?includeV4PageLayouts=true'
     res = await get_data(
         auth=full_auth,
         url=url,
         method='GET',
         debug=debug,
     )
-
-    if log_result:
-        print(res)
-
     return res
 
 
-async def get_page_definition(full_auth, page_id, debug: bool = False, session: aiohttp.ClientSession = None):
+####  PDP ####
+def generate_policy_parameter_simple(column_name, column_values_list, operator='EQUALS', ignore_case: bool = True):
+    return {
+        "type": "COLUMN",
+        "name": column_name,
+        "values": column_values_list,
+        "operator": operator,
+        "ignoreCase": ignore_case
+    }
 
-    close_session = False if session else True
 
-    if not session:
-        session = aiohttp.ClientSession()
-    try:
-        url = f"https://{full_auth.domo_instance}.domo.com/api/content/v3/stacks/{page_id}/cards"
-
-        params = {"includeV4PageLayouts": "true",
-                  "parts": "metadata,datasources,library,drillPathURNs,certification,owners,dateInfo,subscriptions,slicers"}
-
-        res = await get_data(url,
-                             method='GET',
-                             auth=full_auth,
-                             session=session,
-                             params=params, debug=debug)
-
-        return res
-    finally:
-        if close_session:
-            await session.close()
-
-async def update_page_layout(full_auth: DomoFullAuth, layout_id: str,
-                             body: dict,
-                         debug: bool = False, log_results: bool = False) -> ResponseGetData:
-    url = f'https://{full_auth.domo_instance}.domo.com/api/content/v4/pages/layouts/{layout_id}'
+def generate_policy_body(policy_name, dataset_id, parameters_list, policy_id=None, user_ids=None,
+                         group_ids=None, virtual_user_ids=None):
+    if not user_ids:
+        user_ids = []
+
+    if not group_ids:
+        group_ids = []
+    
+    if not virtual_user_ids:
+        virtual_user_ids = []
+
+    body = {
+        "name": policy_name,
+        "dataSourceId": dataset_id,
+        "userIds": user_ids,
+        "virtualUserIds": virtual_user_ids,
+        "groupIds": group_ids,
+        "dataSourcePermissions": False,
+        "parameters": parameters_list
+    }
 
+    if policy_id:
+        body.update({'filterGroupId': policy_id})
 
-    res = await get_data(
-        auth=full_auth,
-        url=url,
-        body=body,
-        method='PUT',
-        debug=debug,
-        log_results=log_results
-    )
+    return body
 
-    if log_results:
-        print(res)
 
-    return res
+async def create_policy(full_auth: DomoFullAuth, dataset_id: str, body: dict, debug: bool = False) -> ResponseGetData:
+    url = f'https://{full_auth.domo_instance}.domo.com/api/query/v1/data-control/{dataset_id}/filter-groups'
+    if debug:
+        print(url)
 
-async def put_writelock(full_auth: DomoFullAuth, layout_id: str, user_id: str,
-                             epoch_time: int,
-                         debug: bool = False, log_results: bool = False) -> ResponseGetData:
-    url = f'https://{full_auth.domo_instance}.domo.com/api/content/v4/pages/layouts/{layout_id}/writelock'
-    body= {
-        "layoutId": layout_id,
-        "lockHeartbeat": epoch_time,
-        "lockTimestamp": epoch_time,
-        "userId":user_id
-    }
-  
     res = await get_data(
         auth=full_auth,
         url=url,
+        method='POST',
         body=body,
-        method='PUT',
-        debug=debug,
-        log_results=log_results
-    )
-
-    if log_results:
-        print(res)
+        debug=debug)
 
     return res
 
-async def delete_writelock(full_auth: DomoFullAuth, layout_id: str,
-                         debug: bool = False, log_results: bool = False) -> ResponseGetData:
-    url = f'https://{full_auth.domo_instance}.domo.com/api/content/v4/pages/layouts/{layout_id}/writelock'
+
+async def update_policy(full_auth: DomoFullAuth, dataset_id: str, filter_group_id, body: dict,
+                        debug: bool = False) -> ResponseGetData:
+    url = f'https://{full_auth.domo_instance}.domo.com/api/query/v1/data-control/{dataset_id}/filter-groups/{filter_group_id}'
+    if debug:
+        print(url)
+
     res = await get_data(
         auth=full_auth,
         url=url,
-        method='DELETE',
-        debug=debug,
-        log_results=log_results
+        method='PUT',
+        body=body,
+        debug=debug
     )
 
-    if log_results:
-        print(res)
+    return res
 
-    return res
```

### Comparing `domolibrary-0.0.81/DomoClasses/routes/publish_routes.py` & `domolibrary-0.0.9/DomoClasses/routes/publish_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.81/DomoClasses/routes/role_routes.py` & `domolibrary-0.0.9/DomoClasses/routes/role_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.81/DomoClasses/routes/sandbox_routes.py` & `domolibrary-0.0.9/DomoClasses/routes/sandbox_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.81/DomoClasses/routes/stream_routes.py` & `domolibrary-0.0.9/DomoClasses/routes/stream_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.81/DomoClasses/routes/user_routes.py` & `domolibrary-0.0.9/DomoClasses/routes/user_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.81/LICENSE` & `domolibrary-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.81/PKG-INFO` & `domolibrary-0.0.9/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: domolibrary
-Version: 0.0.81
-Summary: UNKNOWN
-Home-page: https://github.com/jaewilson07/domo_library
-Author: Jae Wilson
-Author-email: jaewilson07@gmail.com
-License: Apache Software License 2.0
-Keywords: nbdev jupyter notebook python
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 domolibrary: a powerful pydomo alternative
 ================
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 ## What is it?
 
@@ -42,15 +19,15 @@
 ## Install
 
 The DataCrew team is hard at work expanding the list of available
 `classes` and `routes`. We have a ton of work completed, it’s just a
 matter of migrating and documenting the code into this library.
 
 ``` sh
-pip install domolibrary
+pip install domo_library
 ```
 
 ## How to use
 
 ### Authentication
 
 For each task, consider the appropriate
@@ -72,15 +49,15 @@
 auth objects.
 
 ``` python
 # configure an auth method
 import os
 import domolibrary.client.DomoAuth as dmda
 
-token_auth = dmda.DomoTokenAuth( domo_instance = 'domo-community', domo_access_token = os.environ['DOMO_DOJO_ACCESS_TOKEN'])
+token_auth = dmda.DomoTokenAuth( domo_instance = 'domo-dojoo', domo_access_token = os.environ['DOMO_DOJO_ACCESS_TOKEN'])
 ```
 
 ### Option 1: class based programming
 
 In this project domo entities,
 [`DomoActivityLog`](https://jaewilson07.github.io/domo_library/classes/domoactivitylog.html#domoactivitylog),
 [`DomoDataset`](https://jaewilson07.github.io/domo_library/classes/domodataset.html#domodataset)
@@ -96,21 +73,23 @@
 [`DomoDataset.get_from_id`](https://jaewilson07.github.io/domo_library/classes/domodataset.html#domodataset.get_from_id)
 is a classmethod.
 
 Note: DomoLibrary uses the asynchronous `aiohttp` requests library to
 offer users the ability to write concurrently executing code.
 
 ``` python
-# import domolibrary.classes.DomoDataset as dmds
+import domolibrary.classes.DomoDataset as dmds
 
-# # this is a class method
-# domo_ds = await dmds.DomoDataset.get_from_id(auth=token_auth, dataset_id=os.environ['DOJO_DATASET_ID'])
-# domo_ds
+# this is a class method
+domo_ds = await dmds.DomoDataset.get_from_id(auth = token_auth, dataset_id = os.environ['DOJO_DATASET_ID'])
+domo_ds
 ```
 
+    DomoDataset(id='04c1574e-c8be-4721-9846-c6ffa491144b', display_type='domo-jupyterdata', data_provider_type='domo-jupyterdata', name='domo_kbs', description=None, row_count=1185, column_count=7, stream_id=825, owner=DictDot(id='1893952720', name='Jae Wilson', type='USER', group=False), formula=DictDot(), schema=DomoDataset_Schema(dataset=..., columns=[]))
+
 Once instantiated, you can call methods to interact with that object.
 You typically won’t have to pass auth creds again because they are saved
 to the object.
 
 In the example below we are retrieving the
 [`DomoDataset_Schema`](https://jaewilson07.github.io/domo_library/classes/domodataset.html#domodataset_schema)
 which consists of subclass
@@ -120,23 +99,47 @@
 method.
 
 We take the approach of where possible converting dictionaries from Domo
 APIs into classes because it provides greater predictability when users
 are creating integrations between platforms (ex. Domo to Trello).
 
 ``` python
-# await domo_ds.schema.get()
+await domo_ds.schema.get()
 ```
 
+    [DomoDataset_Schema_Column(name='objectID', id='objectID', type='STRING'),
+     DomoDataset_Schema_Column(name='url', id='url', type='STRING'),
+     DomoDataset_Schema_Column(name='Title', id='Title', type='STRING'),
+     DomoDataset_Schema_Column(name='article', id='article', type='STRING'),
+     DomoDataset_Schema_Column(name='views', id='views', type='LONG'),
+     DomoDataset_Schema_Column(name='created_dt', id='created_dt', type='DATETIME'),
+     DomoDataset_Schema_Column(name='published_dt', id='published_dt', type='DATETIME')]
+
 Typically all information about an entity is saved in the object
 
 ``` python
-# domo_ds.__dict__
+domo_ds.__dict__
 ```
 
+    {'auth': DomoTokenAuth(domo_instance='domo-dojoo', token_name='token_auth', url_manual_login='https://domo-dojoo.domo.com/auth/index?domoManualLogin=true'),
+     'id': '04c1574e-c8be-4721-9846-c6ffa491144b',
+     'display_type': 'domo-jupyterdata',
+     'data_provider_type': 'domo-jupyterdata',
+     'name': 'domo_kbs',
+     'description': None,
+     'row_count': 1185,
+     'column_count': 7,
+     'stream_id': 825,
+     'owner': namespace(id='1893952720',
+               name='Jae Wilson',
+               type='USER',
+               group=False),
+     'formula': namespace(),
+     'schema': DomoDataset_Schema(dataset=DomoDataset(id='04c1574e-c8be-4721-9846-c6ffa491144b', display_type='domo-jupyterdata', data_provider_type='domo-jupyterdata', name='domo_kbs', description=None, row_count=1185, column_count=7, stream_id=825, owner=DictDot(id='1893952720', name='Jae Wilson', type='USER', group=False), formula=DictDot(), schema=...), columns=[DomoDataset_Schema_Column(name='objectID', id='objectID', type='STRING'), DomoDataset_Schema_Column(name='url', id='url', type='STRING'), DomoDataset_Schema_Column(name='Title', id='Title', type='STRING'), DomoDataset_Schema_Column(name='article', id='article', type='STRING'), DomoDataset_Schema_Column(name='views', id='views', type='LONG'), DomoDataset_Schema_Column(name='created_dt', id='created_dt', type='DATETIME'), DomoDataset_Schema_Column(name='published_dt', id='published_dt', type='DATETIME')])}
+
 ### Option 2 functional programming
 
 Although classes add a pretty wrapper for interacting with Domo APIs,
 users can opt to interact directly with APIs by way of `routes`.
 
 All route functions will exclusively call one API and will always return
 a
@@ -220,9 +223,7 @@
 Consider
 [`query_dataset_private`](https://jaewilson07.github.io/domo_library/routes/dataset.html#query_dataset_private)
 from the `routes.dataset`.
 
 Inside this function we are using
 [`looper`](https://jaewilson07.github.io/domo_library/client/get_data.html#looper)
 from `client.get_data` to paginate over the API response.
-
-
```

### Comparing `domolibrary-0.0.81/domolibrary/_modidx.py` & `domolibrary-0.0.9/domolibrary/_modidx.py`

 * *Files 27% similar despite different names*

```diff
@@ -17,16 +17,14 @@
                                                                                                                  'domolibrary/classes/DomoAccount.py'),
                                                  'domolibrary.classes.DomoAccount.DomoAccount.delete_account': ( 'classes/domoaccount.html#domoaccount.delete_account',
                                                                                                                  'domolibrary/classes/DomoAccount.py'),
                                                  'domolibrary.classes.DomoAccount.DomoAccount.generate_create_body': ( 'classes/domoaccount.html#domoaccount.generate_create_body',
                                                                                                                        'domolibrary/classes/DomoAccount.py'),
                                                  'domolibrary.classes.DomoAccount.DomoAccount.get_from_id': ( 'classes/domoaccount.html#domoaccount.get_from_id',
                                                                                                               'domolibrary/classes/DomoAccount.py'),
-                                                 'domolibrary.classes.DomoAccount.DomoAccount.share_account': ( 'classes/domoaccount.html#domoaccount.share_account',
-                                                                                                                'domolibrary/classes/DomoAccount.py'),
                                                  'domolibrary.classes.DomoAccount.DomoAccount.update_config': ( 'classes/domoaccount.html#domoaccount.update_config',
                                                                                                                 'domolibrary/classes/DomoAccount.py'),
                                                  'domolibrary.classes.DomoAccount.DomoAccount.update_name': ( 'classes/domoaccount.html#domoaccount.update_name',
                                                                                                               'domolibrary/classes/DomoAccount.py'),
                                                  'domolibrary.classes.DomoAccount.DomoAccount_Config': ( 'classes/domoaccount.html#domoaccount_config',
                                                                                                          'domolibrary/classes/DomoAccount.py'),
                                                  'domolibrary.classes.DomoAccount.DomoAccount_Config._from_json': ( 'classes/domoaccount.html#domoaccount_config._from_json',
@@ -35,20 +33,14 @@
                                                                                                                  'domolibrary/classes/DomoAccount.py'),
                                                  'domolibrary.classes.DomoAccount.DomoAccount_Config_AbstractCredential': ( 'classes/domoaccount.html#domoaccount_config_abstractcredential',
                                                                                                                             'domolibrary/classes/DomoAccount.py'),
                                                  'domolibrary.classes.DomoAccount.DomoAccount_Config_AbstractCredential._from_json': ( 'classes/domoaccount.html#domoaccount_config_abstractcredential._from_json',
                                                                                                                                        'domolibrary/classes/DomoAccount.py'),
                                                  'domolibrary.classes.DomoAccount.DomoAccount_Config_AbstractCredential.to_json': ( 'classes/domoaccount.html#domoaccount_config_abstractcredential.to_json',
                                                                                                                                     'domolibrary/classes/DomoAccount.py'),
-                                                 'domolibrary.classes.DomoAccount.DomoAccount_Config_AwsAthena': ( 'classes/domoaccount.html#domoaccount_config_awsathena',
-                                                                                                                   'domolibrary/classes/DomoAccount.py'),
-                                                 'domolibrary.classes.DomoAccount.DomoAccount_Config_AwsAthena._from_json': ( 'classes/domoaccount.html#domoaccount_config_awsathena._from_json',
-                                                                                                                              'domolibrary/classes/DomoAccount.py'),
-                                                 'domolibrary.classes.DomoAccount.DomoAccount_Config_AwsAthena.to_json': ( 'classes/domoaccount.html#domoaccount_config_awsathena.to_json',
-                                                                                                                           'domolibrary/classes/DomoAccount.py'),
                                                  'domolibrary.classes.DomoAccount.DomoAccount_Config_DatasetCopy': ( 'classes/domoaccount.html#domoaccount_config_datasetcopy',
                                                                                                                      'domolibrary/classes/DomoAccount.py'),
                                                  'domolibrary.classes.DomoAccount.DomoAccount_Config_DatasetCopy._from_json': ( 'classes/domoaccount.html#domoaccount_config_datasetcopy._from_json',
                                                                                                                                 'domolibrary/classes/DomoAccount.py'),
                                                  'domolibrary.classes.DomoAccount.DomoAccount_Config_DatasetCopy.to_json': ( 'classes/domoaccount.html#domoaccount_config_datasetcopy.to_json',
                                                                                                                              'domolibrary/classes/DomoAccount.py'),
                                                  'domolibrary.classes.DomoAccount.DomoAccount_Config_Governance': ( 'classes/domoaccount.html#domoaccount_config_governance',
@@ -63,32 +55,20 @@
                                                                                                                                            'domolibrary/classes/DomoAccount.py'),
                                                  'domolibrary.classes.DomoAccount.DomoAccount_Config_HighBandwidthConnector.to_json': ( 'classes/domoaccount.html#domoaccount_config_highbandwidthconnector.to_json',
                                                                                                                                         'domolibrary/classes/DomoAccount.py'),
                                                  'domolibrary.classes.DomoAccount.DomoAccount_CreateAccount_Error': ( 'classes/domoaccount.html#domoaccount_createaccount_error',
                                                                                                                       'domolibrary/classes/DomoAccount.py'),
                                                  'domolibrary.classes.DomoAccount.DomoAccount_CreateAccount_Error.__init__': ( 'classes/domoaccount.html#domoaccount_createaccount_error.__init__',
                                                                                                                                'domolibrary/classes/DomoAccount.py'),
-                                                 'domolibrary.classes.DomoAccount.DomoAccount_DataProviderType_ConfigNotDefined': ( 'classes/domoaccount.html#domoaccount_dataprovidertype_confignotdefined',
-                                                                                                                                    'domolibrary/classes/DomoAccount.py'),
-                                                 'domolibrary.classes.DomoAccount.DomoAccount_DataProviderType_ConfigNotDefined.__init__': ( 'classes/domoaccount.html#domoaccount_dataprovidertype_confignotdefined.__init__',
-                                                                                                                                             'domolibrary/classes/DomoAccount.py'),
                                                  'domolibrary.classes.DomoAccount.DomoAccount_DeleteAccount_Error': ( 'classes/domoaccount.html#domoaccount_deleteaccount_error',
                                                                                                                       'domolibrary/classes/DomoAccount.py'),
                                                  'domolibrary.classes.DomoAccount.DomoAccount_DeleteAccount_Error.__init__': ( 'classes/domoaccount.html#domoaccount_deleteaccount_error.__init__',
                                                                                                                                'domolibrary/classes/DomoAccount.py'),
                                                  'domolibrary.classes.DomoAccount.DomoAccount_UpdateName_Error': ( 'classes/domoaccount.html#domoaccount_updatename_error',
-                                                                                                                   'domolibrary/classes/DomoAccount.py'),
-                                                 'domolibrary.classes.DomoAccount.DomoAccount_UpdateName_Error.__init__': ( 'classes/domoaccount.html#domoaccount_updatename_error.__init__',
-                                                                                                                            'domolibrary/classes/DomoAccount.py'),
-                                                 'domolibrary.classes.DomoAccount.DomoAccounts': ( 'classes/domoaccount.html#domoaccounts',
-                                                                                                   'domolibrary/classes/DomoAccount.py'),
-                                                 'domolibrary.classes.DomoAccount.DomoAccounts.get_accounts': ( 'classes/domoaccount.html#domoaccounts.get_accounts',
-                                                                                                                'domolibrary/classes/DomoAccount.py'),
-                                                 'domolibrary.classes.DomoAccount.ShareAccount_AccessLevel': ( 'classes/domoaccount.html#shareaccount_accesslevel',
-                                                                                                               'domolibrary/classes/DomoAccount.py')},
+                                                                                                                   'domolibrary/classes/DomoAccount.py')},
             'domolibrary.classes.DomoActivityLog': { 'domolibrary.classes.DomoActivityLog.ActivityLog_ObjectType': ( 'classes/domoactivitylog.html#activitylog_objecttype',
                                                                                                                      'domolibrary/classes/DomoActivityLog.py'),
                                                      'domolibrary.classes.DomoActivityLog.DomoActivityLog': ( 'classes/domoactivitylog.html#domoactivitylog',
                                                                                                               'domolibrary/classes/DomoActivityLog.py'),
                                                      'domolibrary.classes.DomoActivityLog.DomoActivityLog._process_activity_log_row': ( 'classes/domoactivitylog.html#domoactivitylog._process_activity_log_row',
                                                                                                                                         'domolibrary/classes/DomoActivityLog.py'),
                                                      'domolibrary.classes.DomoActivityLog.DomoActivityLog.get_activity_log': ( 'classes/domoactivitylog.html#domoactivitylog.get_activity_log',
@@ -101,34 +81,28 @@
                                                                                                                      'domolibrary/classes/DomoBootstrap.py'),
                                                    'domolibrary.classes.DomoBootstrap.DomoBootstrap.get_pages': ( 'classes/domobootstrap.html#domobootstrap.get_pages',
                                                                                                                   'domolibrary/classes/DomoBootstrap.py'),
                                                    'domolibrary.classes.DomoBootstrap.DomoBootstrap_Feature': ( 'classes/domobootstrap.html#domobootstrap_feature',
                                                                                                                 'domolibrary/classes/DomoBootstrap.py'),
                                                    'domolibrary.classes.DomoBootstrap.DomoBootstrap_Feature._from_json_bootstrap': ( 'classes/domobootstrap.html#domobootstrap_feature._from_json_bootstrap',
                                                                                                                                      'domolibrary/classes/DomoBootstrap.py')},
-            'domolibrary.classes.DomoDatacenter': { 'domolibrary.classes.DomoDatacenter.DomoDatacenter': ( 'classes/domodatacenter.html#domodatacenter',
-                                                                                                           'domolibrary/classes/DomoDatacenter.py'),
-                                                    'domolibrary.classes.DomoDatacenter.DomoDatacenter.get_accounts': ( 'classes/domodatacenter.html#domodatacenter.get_accounts',
-                                                                                                                        'domolibrary/classes/DomoDatacenter.py'),
-                                                    'domolibrary.classes.DomoDatacenter.DomoDatacenter.search_datacenter': ( 'classes/domodatacenter.html#domodatacenter.search_datacenter',
-                                                                                                                             'domolibrary/classes/DomoDatacenter.py'),
-                                                    'domolibrary.classes.DomoDatacenter.DomoDatacenter.search_datasets': ( 'classes/domodatacenter.html#domodatacenter.search_datasets',
-                                                                                                                           'domolibrary/classes/DomoDatacenter.py')},
-            'domolibrary.classes.DomoDataflow': { 'domolibrary.classes.DomoDataflow.DomoDataflow': ( 'classes/domodataflow.html#domodataflow',
-                                                                                                     'domolibrary/classes/DomoDataflow.py'),
-                                                  'domolibrary.classes.DomoDataflow.DomoDataflow.get_from_id': ( 'classes/domodataflow.html#domodataflow.get_from_id',
-                                                                                                                 'domolibrary/classes/DomoDataflow.py'),
-                                                  'domolibrary.classes.DomoDataflow.DomoDataflow_Action': ( 'classes/domodataflow.html#domodataflow_action',
-                                                                                                            'domolibrary/classes/DomoDataflow.py'),
-                                                  'domolibrary.classes.DomoDataflow.DomoDataflow_Action._from_obj': ( 'classes/domodataflow.html#domodataflow_action._from_obj',
-                                                                                                                      'domolibrary/classes/DomoDataflow.py'),
-                                                  'domolibrary.classes.DomoDataflow.DomoDataflow_Action_Type': ( 'classes/domodataflow.html#domodataflow_action_type',
-                                                                                                                 'domolibrary/classes/DomoDataflow.py')},
-            'domolibrary.classes.DomoDataset': { 'domolibrary.classes.DomoDataset.DatasetSchema_Types': ( 'classes/domodataset.html#datasetschema_types',
+            'domolibrary.classes.DomoDataset': { 'domolibrary.classes.DomoDataset.DatasetSchema_AuthNotProvidedError': ( 'classes/domodataset.html#datasetschema_authnotprovidederror',
+                                                                                                                         'domolibrary/classes/DomoDataset.py'),
+                                                 'domolibrary.classes.DomoDataset.DatasetSchema_AuthNotProvidedError.__init__': ( 'classes/domodataset.html#datasetschema_authnotprovidederror.__init__',
+                                                                                                                                  'domolibrary/classes/DomoDataset.py'),
+                                                 'domolibrary.classes.DomoDataset.DatasetSchema_DatasetNotProvidedError': ( 'classes/domodataset.html#datasetschema_datasetnotprovidederror',
+                                                                                                                            'domolibrary/classes/DomoDataset.py'),
+                                                 'domolibrary.classes.DomoDataset.DatasetSchema_DatasetNotProvidedError.__init__': ( 'classes/domodataset.html#datasetschema_datasetnotprovidederror.__init__',
+                                                                                                                                     'domolibrary/classes/DomoDataset.py'),
+                                                 'domolibrary.classes.DomoDataset.DatasetSchema_Types': ( 'classes/domodataset.html#datasetschema_types',
                                                                                                           'domolibrary/classes/DomoDataset.py'),
+                                                 'domolibrary.classes.DomoDataset.DatasetTags_AuthNotProvidedError': ( 'classes/domodataset.html#datasettags_authnotprovidederror',
+                                                                                                                       'domolibrary/classes/DomoDataset.py'),
+                                                 'domolibrary.classes.DomoDataset.DatasetTags_AuthNotProvidedError.__init__': ( 'classes/domodataset.html#datasettags_authnotprovidederror.__init__',
+                                                                                                                                'domolibrary/classes/DomoDataset.py'),
                                                  'domolibrary.classes.DomoDataset.DatasetTags_SetTagsError': ( 'classes/domodataset.html#datasettags_settagserror',
                                                                                                                'domolibrary/classes/DomoDataset.py'),
                                                  'domolibrary.classes.DomoDataset.DatasetTags_SetTagsError.__init__': ( 'classes/domodataset.html#datasettags_settagserror.__init__',
                                                                                                                         'domolibrary/classes/DomoDataset.py'),
                                                  'domolibrary.classes.DomoDataset.DomoDataset': ( 'classes/domodataset.html#domodataset',
                                                                                                   'domolibrary/classes/DomoDataset.py'),
                                                  'domolibrary.classes.DomoDataset.DomoDataset.__post_init__': ( 'classes/domodataset.html#domodataset.__post_init__',
@@ -163,290 +137,80 @@
                                                                                                              'domolibrary/classes/DomoDataset.py'),
                                                  'domolibrary.classes.DomoDataset.DomoDataset_Schema_Column': ( 'classes/domodataset.html#domodataset_schema_column',
                                                                                                                 'domolibrary/classes/DomoDataset.py'),
                                                  'domolibrary.classes.DomoDataset.DomoDataset_Schema_Column._from_json': ( 'classes/domodataset.html#domodataset_schema_column._from_json',
                                                                                                                            'domolibrary/classes/DomoDataset.py'),
                                                  'domolibrary.classes.DomoDataset.DomoDataset_Tags': ( 'classes/domodataset.html#domodataset_tags',
                                                                                                        'domolibrary/classes/DomoDataset.py'),
+                                                 'domolibrary.classes.DomoDataset.DomoDataset_Tags._have_prereqs': ( 'classes/domodataset.html#domodataset_tags._have_prereqs',
+                                                                                                                     'domolibrary/classes/DomoDataset.py'),
                                                  'domolibrary.classes.DomoDataset.DomoDataset_Tags.add': ( 'classes/domodataset.html#domodataset_tags.add',
                                                                                                            'domolibrary/classes/DomoDataset.py'),
                                                  'domolibrary.classes.DomoDataset.DomoDataset_Tags.get': ( 'classes/domodataset.html#domodataset_tags.get',
                                                                                                            'domolibrary/classes/DomoDataset.py'),
                                                  'domolibrary.classes.DomoDataset.DomoDataset_Tags.remove': ( 'classes/domodataset.html#domodataset_tags.remove',
                                                                                                               'domolibrary/classes/DomoDataset.py'),
                                                  'domolibrary.classes.DomoDataset.DomoDataset_Tags.set': ( 'classes/domodataset.html#domodataset_tags.set',
                                                                                                            'domolibrary/classes/DomoDataset.py'),
-                                                 'domolibrary.classes.DomoDataset.DomoDataset_UploadData_CommitDatasetUploadId_Error': ( 'classes/domodataset.html#domodataset_uploaddata_commitdatasetuploadid_error',
-                                                                                                                                         'domolibrary/classes/DomoDataset.py'),
-                                                 'domolibrary.classes.DomoDataset.DomoDataset_UploadData_CommitDatasetUploadId_Error.__init__': ( 'classes/domodataset.html#domodataset_uploaddata_commitdatasetuploadid_error.__init__',
-                                                                                                                                                  'domolibrary/classes/DomoDataset.py'),
                                                  'domolibrary.classes.DomoDataset.DomoDataset_UploadData_DatasetUploadId_Error': ( 'classes/domodataset.html#domodataset_uploaddata_datasetuploadid_error',
                                                                                                                                    'domolibrary/classes/DomoDataset.py'),
                                                  'domolibrary.classes.DomoDataset.DomoDataset_UploadData_DatasetUploadId_Error.__init__': ( 'classes/domodataset.html#domodataset_uploaddata_datasetuploadid_error.__init__',
                                                                                                                                             'domolibrary/classes/DomoDataset.py'),
                                                  'domolibrary.classes.DomoDataset.DomoDataset_UploadData_Error': ( 'classes/domodataset.html#domodataset_uploaddata_error',
                                                                                                                    'domolibrary/classes/DomoDataset.py'),
                                                  'domolibrary.classes.DomoDataset.DomoDataset_UploadData_Error.__init__': ( 'classes/domodataset.html#domodataset_uploaddata_error.__init__',
                                                                                                                             'domolibrary/classes/DomoDataset.py'),
                                                  'domolibrary.classes.DomoDataset.DomoDataset_UploadData_UploadData_Error': ( 'classes/domodataset.html#domodataset_uploaddata_uploaddata_error',
                                                                                                                               'domolibrary/classes/DomoDataset.py'),
+                                                 'domolibrary.classes.DomoDataset.DomoDataset_UploadData_UploadData_Error.DomoDataset_UploadData_DatasetUploadId_Error': ( 'classes/domodataset.html#domodataset_uploaddata_uploaddata_error.domodataset_uploaddata_datasetuploadid_error',
+                                                                                                                                                                           'domolibrary/classes/DomoDataset.py'),
                                                  'domolibrary.classes.DomoDataset.DomoDataset_UploadData_UploadData_Error.__init__': ( 'classes/domodataset.html#domodataset_uploaddata_uploaddata_error.__init__',
                                                                                                                                        'domolibrary/classes/DomoDataset.py'),
                                                  'domolibrary.classes.DomoDataset.QueryExecutionError': ( 'classes/domodataset.html#queryexecutionerror',
                                                                                                           'domolibrary/classes/DomoDataset.py'),
                                                  'domolibrary.classes.DomoDataset.QueryExecutionError.__init__': ( 'classes/domodataset.html#queryexecutionerror.__init__',
-                                                                                                                   'domolibrary/classes/DomoDataset.py'),
-                                                 'domolibrary.classes.DomoDataset._have_prereqs': ( 'classes/domodataset.html#_have_prereqs',
-                                                                                                    'domolibrary/classes/DomoDataset.py')},
-            'domolibrary.classes.DomoGrant': { 'domolibrary.classes.DomoGrant.DomoGrant': ( 'classes/domogrant.html#domogrant',
-                                                                                            'domolibrary/classes/DomoGrant.py'),
-                                               'domolibrary.classes.DomoGrant.DomoGrant.__eq__': ( 'classes/domogrant.html#domogrant.__eq__',
-                                                                                                   'domolibrary/classes/DomoGrant.py'),
-                                               'domolibrary.classes.DomoGrant.DomoGrant.__post_init__': ( 'classes/domogrant.html#domogrant.__post_init__',
-                                                                                                          'domolibrary/classes/DomoGrant.py'),
-                                               'domolibrary.classes.DomoGrant.DomoGrant._from_json': ( 'classes/domogrant.html#domogrant._from_json',
-                                                                                                       'domolibrary/classes/DomoGrant.py')},
-            'domolibrary.classes.DomoGroup': { 'domolibrary.classes.DomoGroup.DomoGroup': ( 'classes/domogroup.html#domogroup',
-                                                                                            'domolibrary/classes/DomoGroup.py'),
-                                               'domolibrary.classes.DomoGroup.DomoGroup.__post_init__': ( 'classes/domogroup.html#domogroup.__post_init__',
-                                                                                                          'domolibrary/classes/DomoGroup.py'),
-                                               'domolibrary.classes.DomoGroup.DomoGroup._from_group_json': ( 'classes/domogroup.html#domogroup._from_group_json',
-                                                                                                             'domolibrary/classes/DomoGroup.py'),
-                                               'domolibrary.classes.DomoGroup.DomoGroup._from_grouplist_json': ( 'classes/domogroup.html#domogroup._from_grouplist_json',
-                                                                                                                 'domolibrary/classes/DomoGroup.py'),
-                                               'domolibrary.classes.DomoGroup.DomoGroup._groups_to_domo_group': ( 'classes/domogroup.html#domogroup._groups_to_domo_group',
-                                                                                                                  'domolibrary/classes/DomoGroup.py'),
-                                               'domolibrary.classes.DomoGroup.DomoGroup.create_from_name': ( 'classes/domogroup.html#domogroup.create_from_name',
-                                                                                                             'domolibrary/classes/DomoGroup.py'),
-                                               'domolibrary.classes.DomoGroup.DomoGroup.get_by_id': ( 'classes/domogroup.html#domogroup.get_by_id',
-                                                                                                      'domolibrary/classes/DomoGroup.py'),
-                                               'domolibrary.classes.DomoGroup.DomoGroup.search_by_name': ( 'classes/domogroup.html#domogroup.search_by_name',
-                                                                                                           'domolibrary/classes/DomoGroup.py'),
-                                               'domolibrary.classes.DomoGroup.DomoGroup.update_metadata': ( 'classes/domogroup.html#domogroup.update_metadata',
-                                                                                                            'domolibrary/classes/DomoGroup.py'),
-                                               'domolibrary.classes.DomoGroup.DomoGroup.upsert': ( 'classes/domogroup.html#domogroup.upsert',
-                                                                                                   'domolibrary/classes/DomoGroup.py'),
-                                               'domolibrary.classes.DomoGroup.DomoGroups': ( 'classes/domogroup.html#domogroups',
-                                                                                             'domolibrary/classes/DomoGroup.py'),
-                                               'domolibrary.classes.DomoGroup.DomoGroups.__init__': ( 'classes/domogroup.html#domogroups.__init__',
-                                                                                                      'domolibrary/classes/DomoGroup.py'),
-                                               'domolibrary.classes.DomoGroup.DomoGroups._groups_to_domo_group': ( 'classes/domogroup.html#domogroups._groups_to_domo_group',
-                                                                                                                   'domolibrary/classes/DomoGroup.py'),
-                                               'domolibrary.classes.DomoGroup.DomoGroups.get_all_groups': ( 'classes/domogroup.html#domogroups.get_all_groups',
-                                                                                                            'domolibrary/classes/DomoGroup.py'),
-                                               'domolibrary.classes.DomoGroup.GroupMembership': ( 'classes/domogroup.html#groupmembership',
-                                                                                                  'domolibrary/classes/DomoGroup.py'),
-                                               'domolibrary.classes.DomoGroup.GroupMembership.__init__': ( 'classes/domogroup.html#groupmembership.__init__',
-                                                                                                           'domolibrary/classes/DomoGroup.py'),
-                                               'domolibrary.classes.DomoGroup.GroupMembership._add_member': ( 'classes/domogroup.html#groupmembership._add_member',
-                                                                                                              'domolibrary/classes/DomoGroup.py'),
-                                               'domolibrary.classes.DomoGroup.GroupMembership._add_owner': ( 'classes/domogroup.html#groupmembership._add_owner',
-                                                                                                             'domolibrary/classes/DomoGroup.py'),
-                                               'domolibrary.classes.DomoGroup.GroupMembership._add_to_list': ( 'classes/domogroup.html#groupmembership._add_to_list',
-                                                                                                               'domolibrary/classes/DomoGroup.py'),
-                                               'domolibrary.classes.DomoGroup.GroupMembership._remove_member': ( 'classes/domogroup.html#groupmembership._remove_member',
-                                                                                                                 'domolibrary/classes/DomoGroup.py'),
-                                               'domolibrary.classes.DomoGroup.GroupMembership._remove_owner': ( 'classes/domogroup.html#groupmembership._remove_owner',
-                                                                                                                'domolibrary/classes/DomoGroup.py'),
-                                               'domolibrary.classes.DomoGroup.GroupMembership._reset_obj': ( 'classes/domogroup.html#groupmembership._reset_obj',
-                                                                                                             'domolibrary/classes/DomoGroup.py'),
-                                               'domolibrary.classes.DomoGroup.GroupMembership._update_group_access': ( 'classes/domogroup.html#groupmembership._update_group_access',
-                                                                                                                       'domolibrary/classes/DomoGroup.py'),
-                                               'domolibrary.classes.DomoGroup.GroupMembership.add_members': ( 'classes/domogroup.html#groupmembership.add_members',
-                                                                                                              'domolibrary/classes/DomoGroup.py'),
-                                               'domolibrary.classes.DomoGroup.GroupMembership.add_owners': ( 'classes/domogroup.html#groupmembership.add_owners',
-                                                                                                             'domolibrary/classes/DomoGroup.py'),
-                                               'domolibrary.classes.DomoGroup.GroupMembership.get_members': ( 'classes/domogroup.html#groupmembership.get_members',
-                                                                                                              'domolibrary/classes/DomoGroup.py'),
-                                               'domolibrary.classes.DomoGroup.GroupMembership.get_owners': ( 'classes/domogroup.html#groupmembership.get_owners',
-                                                                                                             'domolibrary/classes/DomoGroup.py'),
-                                               'domolibrary.classes.DomoGroup.GroupMembership.remove_members': ( 'classes/domogroup.html#groupmembership.remove_members',
-                                                                                                                 'domolibrary/classes/DomoGroup.py'),
-                                               'domolibrary.classes.DomoGroup.GroupMembership.remove_owners': ( 'classes/domogroup.html#groupmembership.remove_owners',
-                                                                                                                'domolibrary/classes/DomoGroup.py'),
-                                               'domolibrary.classes.DomoGroup.GroupMembership.set_members': ( 'classes/domogroup.html#groupmembership.set_members',
-                                                                                                              'domolibrary/classes/DomoGroup.py'),
-                                               'domolibrary.classes.DomoGroup.GroupMembership.set_owners': ( 'classes/domogroup.html#groupmembership.set_owners',
-                                                                                                             'domolibrary/classes/DomoGroup.py'),
-                                               'domolibrary.classes.DomoGroup.UpdateGroupMembership': ( 'classes/domogroup.html#updategroupmembership',
-                                                                                                        'domolibrary/classes/DomoGroup.py'),
-                                               'domolibrary.classes.DomoGroup.UpdateGroupMembership.__init__': ( 'classes/domogroup.html#updategroupmembership.__init__',
-                                                                                                                 'domolibrary/classes/DomoGroup.py')},
-            'domolibrary.classes.DomoInstanceConfig': { 'domolibrary.classes.DomoInstanceConfig.DomoInstanceConfig': ( 'classes/domoinstanceconfig.html#domoinstanceconfig',
-                                                                                                                       'domolibrary/classes/DomoInstanceConfig.py'),
-                                                        'domolibrary.classes.DomoInstanceConfig.DomoInstanceConfig.get_allowlist': ( 'classes/domoinstanceconfig.html#domoinstanceconfig.get_allowlist',
-                                                                                                                                     'domolibrary/classes/DomoInstanceConfig.py'),
-                                                        'domolibrary.classes.DomoInstanceConfig.DomoInstanceConfig.get_authorized_domains': ( 'classes/domoinstanceconfig.html#domoinstanceconfig.get_authorized_domains',
-                                                                                                                                              'domolibrary/classes/DomoInstanceConfig.py'),
-                                                        'domolibrary.classes.DomoInstanceConfig.DomoInstanceConfig.get_grants': ( 'classes/domoinstanceconfig.html#domoinstanceconfig.get_grants',
-                                                                                                                                  'domolibrary/classes/DomoInstanceConfig.py'),
-                                                        'domolibrary.classes.DomoInstanceConfig.DomoInstanceConfig.get_roles': ( 'classes/domoinstanceconfig.html#domoinstanceconfig.get_roles',
-                                                                                                                                 'domolibrary/classes/DomoInstanceConfig.py'),
-                                                        'domolibrary.classes.DomoInstanceConfig.DomoInstanceConfig.set_allowlist': ( 'classes/domoinstanceconfig.html#domoinstanceconfig.set_allowlist',
-                                                                                                                                     'domolibrary/classes/DomoInstanceConfig.py'),
-                                                        'domolibrary.classes.DomoInstanceConfig.DomoInstanceConfig.upsert_allowlist': ( 'classes/domoinstanceconfig.html#domoinstanceconfig.upsert_allowlist',
-                                                                                                                                        'domolibrary/classes/DomoInstanceConfig.py')},
-            'domolibrary.classes.DomoPDP': { 'domolibrary.classes.DomoPDP.Dataset_PDP_Policies': ( 'classes/domopdp.html#dataset_pdp_policies',
-                                                                                                   'domolibrary/classes/DomoPDP.py'),
-                                             'domolibrary.classes.DomoPDP.Dataset_PDP_Policies.__init__': ( 'classes/domopdp.html#dataset_pdp_policies.__init__',
-                                                                                                            'domolibrary/classes/DomoPDP.py'),
-                                             'domolibrary.classes.DomoPDP.Dataset_PDP_Policies.get_policies': ( 'classes/domopdp.html#dataset_pdp_policies.get_policies',
-                                                                                                                'domolibrary/classes/DomoPDP.py'),
-                                             'domolibrary.classes.DomoPDP.Dataset_PDP_Policies.search_pdp_policies': ( 'classes/domopdp.html#dataset_pdp_policies.search_pdp_policies',
-                                                                                                                       'domolibrary/classes/DomoPDP.py'),
-                                             'domolibrary.classes.DomoPDP.Dataset_PDP_Policies.toggle_dataset_pdp': ( 'classes/domopdp.html#dataset_pdp_policies.toggle_dataset_pdp',
-                                                                                                                      'domolibrary/classes/DomoPDP.py'),
-                                             'domolibrary.classes.DomoPDP.PDP_Parameter': ( 'classes/domopdp.html#pdp_parameter',
-                                                                                            'domolibrary/classes/DomoPDP.py'),
-                                             'domolibrary.classes.DomoPDP.PDP_Parameter.generate_parameter_simple': ( 'classes/domopdp.html#pdp_parameter.generate_parameter_simple',
-                                                                                                                      'domolibrary/classes/DomoPDP.py'),
-                                             'domolibrary.classes.DomoPDP.PDP_Policy': ( 'classes/domopdp.html#pdp_policy',
-                                                                                         'domolibrary/classes/DomoPDP.py'),
-                                             'domolibrary.classes.DomoPDP.PDP_Policy._from_json': ( 'classes/domopdp.html#pdp_policy._from_json',
-                                                                                                    'domolibrary/classes/DomoPDP.py'),
-                                             'domolibrary.classes.DomoPDP.PDP_Policy.add_parameter': ( 'classes/domopdp.html#pdp_policy.add_parameter',
-                                                                                                       'domolibrary/classes/DomoPDP.py'),
-                                             'domolibrary.classes.DomoPDP.PDP_Policy.delete_policy': ( 'classes/domopdp.html#pdp_policy.delete_policy',
-                                                                                                       'domolibrary/classes/DomoPDP.py'),
-                                             'domolibrary.classes.DomoPDP.PDP_Policy.generate_body': ( 'classes/domopdp.html#pdp_policy.generate_body',
-                                                                                                       'domolibrary/classes/DomoPDP.py'),
-                                             'domolibrary.classes.DomoPDP.PDP_Policy.upsert_policy': ( 'classes/domopdp.html#pdp_policy.upsert_policy',
-                                                                                                       'domolibrary/classes/DomoPDP.py'),
-                                             'domolibrary.classes.DomoPDP.SearchPDP_NotFound': ( 'classes/domopdp.html#searchpdp_notfound',
-                                                                                                 'domolibrary/classes/DomoPDP.py'),
-                                             'domolibrary.classes.DomoPDP.SearchPDP_NotFound.__init__': ( 'classes/domopdp.html#searchpdp_notfound.__init__',
-                                                                                                          'domolibrary/classes/DomoPDP.py')},
+                                                                                                                   'domolibrary/classes/DomoDataset.py')},
             'domolibrary.classes.DomoPage': { 'domolibrary.classes.DomoPage.DomoPage': ( 'classes/domopage.html#domopage',
                                                                                          'domolibrary/classes/DomoPage.py'),
                                               'domolibrary.classes.DomoPage.DomoPage._from_bootstrap': ( 'classes/domopage.html#domopage._from_bootstrap',
                                                                                                          'domolibrary/classes/DomoPage.py'),
-                                              'domolibrary.classes.DomoPage.DomoPage._from_content_stacks_v3': ( 'classes/domopage.html#domopage._from_content_stacks_v3',
-                                                                                                                 'domolibrary/classes/DomoPage.py'),
+                                              'domolibrary.classes.DomoPage.DomoPage._ol_fn': ( 'classes/domopage.html#domopage._ol_fn',
+                                                                                                'domolibrary/classes/DomoPage.py'),
                                               'domolibrary.classes.DomoPage.DomoPage.display_url': ( 'classes/domopage.html#domopage.display_url',
-                                                                                                     'domolibrary/classes/DomoPage.py'),
-                                              'domolibrary.classes.DomoPage.DomoPage.get_accesslist': ( 'classes/domopage.html#domopage.get_accesslist',
-                                                                                                        'domolibrary/classes/DomoPage.py'),
-                                              'domolibrary.classes.DomoPage.DomoPage.get_by_id': ( 'classes/domopage.html#domopage.get_by_id',
-                                                                                                   'domolibrary/classes/DomoPage.py')},
-            'domolibrary.classes.DomoPublish': { 'domolibrary.classes.DomoPublish.DomoPublication': ( 'classes/domopublish.html#domopublication',
-                                                                                                      'domolibrary/classes/DomoPublish.py'),
-                                                 'domolibrary.classes.DomoPublish.DomoPublication._from_json': ( 'classes/domopublish.html#domopublication._from_json',
-                                                                                                                 'domolibrary/classes/DomoPublish.py'),
-                                                 'domolibrary.classes.DomoPublish.DomoPublication.get_from_id': ( 'classes/domopublish.html#domopublication.get_from_id',
-                                                                                                                  'domolibrary/classes/DomoPublish.py'),
-                                                 'domolibrary.classes.DomoPublish.DomoPublication_Content': ( 'classes/domopublish.html#domopublication_content',
-                                                                                                              'domolibrary/classes/DomoPublish.py'),
-                                                 'domolibrary.classes.DomoPublish.DomoPublication_Content._from_json': ( 'classes/domopublish.html#domopublication_content._from_json',
-                                                                                                                         'domolibrary/classes/DomoPublish.py'),
-                                                 'domolibrary.classes.DomoPublish.DomoPublication_Content.to_api_json': ( 'classes/domopublish.html#domopublication_content.to_api_json',
-                                                                                                                          'domolibrary/classes/DomoPublish.py'),
-                                                 'domolibrary.classes.DomoPublish.DomoPublication_Subscription': ( 'classes/domopublish.html#domopublication_subscription',
-                                                                                                                   'domolibrary/classes/DomoPublish.py'),
-                                                 'domolibrary.classes.DomoPublish.DomoPublication_Subscription._from_json': ( 'classes/domopublish.html#domopublication_subscription._from_json',
-                                                                                                                              'domolibrary/classes/DomoPublish.py'),
-                                                 'domolibrary.classes.DomoPublish.DomoPublication_UnexpectedContentType': ( 'classes/domopublish.html#domopublication_unexpectedcontenttype',
-                                                                                                                            'domolibrary/classes/DomoPublish.py'),
-                                                 'domolibrary.classes.DomoPublish.DomoPublication_UnexpectedContentType.__init__': ( 'classes/domopublish.html#domopublication_unexpectedcontenttype.__init__',
-                                                                                                                                     'domolibrary/classes/DomoPublish.py'),
-                                                 'domolibrary.classes.DomoPublish.DomoPublications': ( 'classes/domopublish.html#domopublications',
-                                                                                                       'domolibrary/classes/DomoPublish.py'),
-                                                 'domolibrary.classes.DomoPublish.DomoPublications.get_subscription_summaries': ( 'classes/domopublish.html#domopublications.get_subscription_summaries',
-                                                                                                                                  'domolibrary/classes/DomoPublish.py'),
-                                                 'domolibrary.classes.DomoPublish.DomoPublications.search_publications': ( 'classes/domopublish.html#domopublications.search_publications',
-                                                                                                                           'domolibrary/classes/DomoPublish.py')},
-            'domolibrary.classes.DomoRole': { 'domolibrary.classes.DomoRole.AddUser_Error': ( 'classes/domorole.html#adduser_error',
-                                                                                              'domolibrary/classes/DomoRole.py'),
-                                              'domolibrary.classes.DomoRole.AddUser_Error.__init__': ( 'classes/domorole.html#adduser_error.__init__',
-                                                                                                       'domolibrary/classes/DomoRole.py'),
-                                              'domolibrary.classes.DomoRole.CreateRole_Error': ( 'classes/domorole.html#createrole_error',
-                                                                                                 'domolibrary/classes/DomoRole.py'),
-                                              'domolibrary.classes.DomoRole.CreateRole_Error.__init__': ( 'classes/domorole.html#createrole_error.__init__',
-                                                                                                          'domolibrary/classes/DomoRole.py'),
-                                              'domolibrary.classes.DomoRole.DeleteRole_Error': ( 'classes/domorole.html#deleterole_error',
-                                                                                                 'domolibrary/classes/DomoRole.py'),
-                                              'domolibrary.classes.DomoRole.DeleteRole_Error.__init__': ( 'classes/domorole.html#deleterole_error.__init__',
-                                                                                                          'domolibrary/classes/DomoRole.py'),
-                                              'domolibrary.classes.DomoRole.DomoRole': ( 'classes/domorole.html#domorole',
-                                                                                         'domolibrary/classes/DomoRole.py'),
-                                              'domolibrary.classes.DomoRole.DomoRole.__post_init__': ( 'classes/domorole.html#domorole.__post_init__',
-                                                                                                       'domolibrary/classes/DomoRole.py'),
-                                              'domolibrary.classes.DomoRole.DomoRole._from_json': ( 'classes/domorole.html#domorole._from_json',
-                                                                                                    'domolibrary/classes/DomoRole.py'),
-                                              'domolibrary.classes.DomoRole.DomoRole._valid_grant_ls': ( 'classes/domorole.html#domorole._valid_grant_ls',
-                                                                                                         'domolibrary/classes/DomoRole.py'),
-                                              'domolibrary.classes.DomoRole.DomoRole.add_user': ( 'classes/domorole.html#domorole.add_user',
-                                                                                                  'domolibrary/classes/DomoRole.py'),
-                                              'domolibrary.classes.DomoRole.DomoRole.delete_role': ( 'classes/domorole.html#domorole.delete_role',
-                                                                                                     'domolibrary/classes/DomoRole.py'),
-                                              'domolibrary.classes.DomoRole.DomoRole.get_grants': ( 'classes/domorole.html#domorole.get_grants',
-                                                                                                    'domolibrary/classes/DomoRole.py'),
-                                              'domolibrary.classes.DomoRole.DomoRole.get_membership': ( 'classes/domorole.html#domorole.get_membership',
-                                                                                                        'domolibrary/classes/DomoRole.py'),
-                                              'domolibrary.classes.DomoRole.DomoRole.set_as_default_role': ( 'classes/domorole.html#domorole.set_as_default_role',
-                                                                                                             'domolibrary/classes/DomoRole.py'),
-                                              'domolibrary.classes.DomoRole.DomoRole.set_grants': ( 'classes/domorole.html#domorole.set_grants',
-                                                                                                    'domolibrary/classes/DomoRole.py'),
-                                              'domolibrary.classes.DomoRole.DomoRole.update_role_metadata': ( 'classes/domorole.html#domorole.update_role_metadata',
-                                                                                                              'domolibrary/classes/DomoRole.py'),
-                                              'domolibrary.classes.DomoRole.DomoRoles': ( 'classes/domorole.html#domoroles',
-                                                                                          'domolibrary/classes/DomoRole.py'),
-                                              'domolibrary.classes.DomoRole.DomoRoles.create_role': ( 'classes/domorole.html#domoroles.create_role',
-                                                                                                      'domolibrary/classes/DomoRole.py'),
-                                              'domolibrary.classes.DomoRole.DomoRoles.get_roles': ( 'classes/domorole.html#domoroles.get_roles',
-                                                                                                    'domolibrary/classes/DomoRole.py'),
-                                              'domolibrary.classes.DomoRole.DomoRoles.search_role': ( 'classes/domorole.html#domoroles.search_role',
-                                                                                                      'domolibrary/classes/DomoRole.py'),
-                                              'domolibrary.classes.DomoRole.DomoRoles.upsert_role': ( 'classes/domorole.html#domoroles.upsert_role',
-                                                                                                      'domolibrary/classes/DomoRole.py'),
-                                              'domolibrary.classes.DomoRole.SearchRole_NotFound': ( 'classes/domorole.html#searchrole_notfound',
-                                                                                                    'domolibrary/classes/DomoRole.py'),
-                                              'domolibrary.classes.DomoRole.SearchRole_NotFound.__init__': ( 'classes/domorole.html#searchrole_notfound.__init__',
-                                                                                                             'domolibrary/classes/DomoRole.py'),
-                                              'domolibrary.classes.DomoRole.SetRoleGrants_MissingGrants': ( 'classes/domorole.html#setrolegrants_missinggrants',
-                                                                                                            'domolibrary/classes/DomoRole.py'),
-                                              'domolibrary.classes.DomoRole.SetRoleGrants_MissingGrants.__init__': ( 'classes/domorole.html#setrolegrants_missinggrants.__init__',
-                                                                                                                     'domolibrary/classes/DomoRole.py')},
-            'domolibrary.classes.DomoUser': { 'domolibrary.classes.DomoUser.CreateUser_MissingRole': ( 'classes/domouser.html#createuser_missingrole',
-                                                                                                       'domolibrary/classes/DomoUser.py'),
-                                              'domolibrary.classes.DomoUser.CreateUser_MissingRole.__init__': ( 'classes/domouser.html#createuser_missingrole.__init__',
-                                                                                                                'domolibrary/classes/DomoUser.py'),
-                                              'domolibrary.classes.DomoUser.DomoUser': ( 'classes/domouser.html#domouser',
+                                                                                                     'domolibrary/classes/DomoPage.py')},
+            'domolibrary.classes.DomoUser': { 'domolibrary.classes.DomoUser.DomoUser': ( 'classes/domouser.html#domouser',
                                                                                          'domolibrary/classes/DomoUser.py'),
-                                              'domolibrary.classes.DomoUser.DomoUser.__eq__': ( 'classes/domouser.html#domouser.__eq__',
-                                                                                                'domolibrary/classes/DomoUser.py'),
-                                              'domolibrary.classes.DomoUser.DomoUser.__post_init__': ( 'classes/domouser.html#domouser.__post_init__',
-                                                                                                       'domolibrary/classes/DomoUser.py'),
                                               'domolibrary.classes.DomoUser.DomoUser._from_bootstrap_json': ( 'classes/domouser.html#domouser._from_bootstrap_json',
                                                                                                               'domolibrary/classes/DomoUser.py'),
                                               'domolibrary.classes.DomoUser.DomoUser._from_search_json': ( 'classes/domouser.html#domouser._from_search_json',
                                                                                                            'domolibrary/classes/DomoUser.py'),
                                               'domolibrary.classes.DomoUser.DomoUser._from_virtual_json': ( 'classes/domouser.html#domouser._from_virtual_json',
                                                                                                             'domolibrary/classes/DomoUser.py'),
+                                              'domolibrary.classes.DomoUser.DomoUser.create_user': ( 'classes/domouser.html#domouser.create_user',
+                                                                                                     'domolibrary/classes/DomoUser.py'),
                                               'domolibrary.classes.DomoUser.DomoUser.request_password_reset': ( 'classes/domouser.html#domouser.request_password_reset',
                                                                                                                 'domolibrary/classes/DomoUser.py'),
                                               'domolibrary.classes.DomoUser.DomoUser.reset_password': ( 'classes/domouser.html#domouser.reset_password',
                                                                                                         'domolibrary/classes/DomoUser.py'),
+                                              'domolibrary.classes.DomoUser.DomoUser.set_user_landing_page': ( 'classes/domouser.html#domouser.set_user_landing_page',
+                                                                                                               'domolibrary/classes/DomoUser.py'),
                                               'domolibrary.classes.DomoUser.DomoUsers': ( 'classes/domouser.html#domousers',
                                                                                           'domolibrary/classes/DomoUser.py'),
                                               'domolibrary.classes.DomoUser.DomoUsers._generate_logger': ( 'classes/domouser.html#domousers._generate_logger',
                                                                                                            'domolibrary/classes/DomoUser.py'),
                                               'domolibrary.classes.DomoUser.DomoUsers._users_to_domo_user': ( 'classes/domouser.html#domousers._users_to_domo_user',
                                                                                                               'domolibrary/classes/DomoUser.py'),
                                               'domolibrary.classes.DomoUser.DomoUsers._users_to_virtual_user': ( 'classes/domouser.html#domousers._users_to_virtual_user',
                                                                                                                  'domolibrary/classes/DomoUser.py'),
                                               'domolibrary.classes.DomoUser.DomoUsers.all_users': ( 'classes/domouser.html#domousers.all_users',
                                                                                                     'domolibrary/classes/DomoUser.py'),
                                               'domolibrary.classes.DomoUser.DomoUsers.by_email': ( 'classes/domouser.html#domousers.by_email',
                                                                                                    'domolibrary/classes/DomoUser.py'),
                                               'domolibrary.classes.DomoUser.DomoUsers.by_id': ( 'classes/domouser.html#domousers.by_id',
                                                                                                 'domolibrary/classes/DomoUser.py'),
-                                              'domolibrary.classes.DomoUser.DomoUsers.create_user': ( 'classes/domouser.html#domousers.create_user',
-                                                                                                      'domolibrary/classes/DomoUser.py'),
-                                              'domolibrary.classes.DomoUser.DomoUsers.upsert_user': ( 'classes/domouser.html#domousers.upsert_user',
-                                                                                                      'domolibrary/classes/DomoUser.py'),
                                               'domolibrary.classes.DomoUser.DomoUsers.util_match_domo_users_to_emails': ( 'classes/domouser.html#domousers.util_match_domo_users_to_emails',
                                                                                                                           'domolibrary/classes/DomoUser.py'),
                                               'domolibrary.classes.DomoUser.DomoUsers.util_match_users_obj_to_emails': ( 'classes/domouser.html#domousers.util_match_users_obj_to_emails',
                                                                                                                          'domolibrary/classes/DomoUser.py'),
                                               'domolibrary.classes.DomoUser.DomoUsers.virtual_user_by_subscriber_instance': ( 'classes/domouser.html#domousers.virtual_user_by_subscriber_instance',
                                                                                                                               'domolibrary/classes/DomoUser.py')},
             'domolibrary.client.DomoAuth': { 'domolibrary.client.DomoAuth.DomoAuth': ( 'client/domoauth.html#domoauth',
@@ -455,42 +219,38 @@
                                                                                                 'domolibrary/client/DomoAuth.py'),
                                              'domolibrary.client.DomoAuth.DomoDeveloperAuth.__init__': ( 'client/domoauth.html#domodeveloperauth.__init__',
                                                                                                          'domolibrary/client/DomoAuth.py'),
                                              'domolibrary.client.DomoAuth.DomoDeveloperAuth.generate_auth_header': ( 'client/domoauth.html#domodeveloperauth.generate_auth_header',
                                                                                                                      'domolibrary/client/DomoAuth.py'),
                                              'domolibrary.client.DomoAuth.DomoDeveloperAuth.get_auth_token': ( 'client/domoauth.html#domodeveloperauth.get_auth_token',
                                                                                                                'domolibrary/client/DomoAuth.py'),
+                                             'domolibrary.client.DomoAuth.DomoErrror': ( 'client/domoauth.html#domoerrror',
+                                                                                         'domolibrary/client/DomoAuth.py'),
+                                             'domolibrary.client.DomoAuth.DomoErrror.__init__': ( 'client/domoauth.html#domoerrror.__init__',
+                                                                                                  'domolibrary/client/DomoAuth.py'),
                                              'domolibrary.client.DomoAuth.DomoFullAuth': ( 'client/domoauth.html#domofullauth',
                                                                                            'domolibrary/client/DomoAuth.py'),
                                              'domolibrary.client.DomoAuth.DomoFullAuth.generate_auth_header': ( 'client/domoauth.html#domofullauth.generate_auth_header',
                                                                                                                 'domolibrary/client/DomoAuth.py'),
                                              'domolibrary.client.DomoAuth.DomoFullAuth.get_auth_token': ( 'client/domoauth.html#domofullauth.get_auth_token',
                                                                                                           'domolibrary/client/DomoAuth.py'),
                                              'domolibrary.client.DomoAuth.DomoTokenAuth': ( 'client/domoauth.html#domotokenauth',
                                                                                             'domolibrary/client/DomoAuth.py'),
                                              'domolibrary.client.DomoAuth.DomoTokenAuth.generate_auth_header': ( 'client/domoauth.html#domotokenauth.generate_auth_header',
                                                                                                                  'domolibrary/client/DomoAuth.py'),
                                              'domolibrary.client.DomoAuth.DomoTokenAuth.get_auth_token': ( 'client/domoauth.html#domotokenauth.get_auth_token',
                                                                                                            'domolibrary/client/DomoAuth.py'),
-                                             'domolibrary.client.DomoAuth.InvalidAuthTypeError': ( 'client/domoauth.html#invalidauthtypeerror',
-                                                                                                   'domolibrary/client/DomoAuth.py'),
-                                             'domolibrary.client.DomoAuth.InvalidAuthTypeError.__init__': ( 'client/domoauth.html#invalidauthtypeerror.__init__',
-                                                                                                            'domolibrary/client/DomoAuth.py'),
                                              'domolibrary.client.DomoAuth.InvalidCredentialsError': ( 'client/domoauth.html#invalidcredentialserror',
                                                                                                       'domolibrary/client/DomoAuth.py'),
                                              'domolibrary.client.DomoAuth.InvalidCredentialsError.__init__': ( 'client/domoauth.html#invalidcredentialserror.__init__',
                                                                                                                'domolibrary/client/DomoAuth.py'),
                                              'domolibrary.client.DomoAuth.InvalidInstanceError': ( 'client/domoauth.html#invalidinstanceerror',
                                                                                                    'domolibrary/client/DomoAuth.py'),
                                              'domolibrary.client.DomoAuth.InvalidInstanceError.__init__': ( 'client/domoauth.html#invalidinstanceerror.__init__',
                                                                                                             'domolibrary/client/DomoAuth.py'),
-                                             'domolibrary.client.DomoAuth.NoAccessTokenReturned': ( 'client/domoauth.html#noaccesstokenreturned',
-                                                                                                    'domolibrary/client/DomoAuth.py'),
-                                             'domolibrary.client.DomoAuth.NoAccessTokenReturned.__init__': ( 'client/domoauth.html#noaccesstokenreturned.__init__',
-                                                                                                             'domolibrary/client/DomoAuth.py'),
                                              'domolibrary.client.DomoAuth._DomoAuth_Optional': ( 'client/domoauth.html#_domoauth_optional',
                                                                                                  'domolibrary/client/DomoAuth.py'),
                                              'domolibrary.client.DomoAuth._DomoAuth_Optional.generate_auth_header': ( 'client/domoauth.html#_domoauth_optional.generate_auth_header',
                                                                                                                       'domolibrary/client/DomoAuth.py'),
                                              'domolibrary.client.DomoAuth._DomoAuth_Optional.get_auth_token': ( 'client/domoauth.html#_domoauth_optional.get_auth_token',
                                                                                                                 'domolibrary/client/DomoAuth.py'),
                                              'domolibrary.client.DomoAuth._DomoAuth_Optional.print_is_token': ( 'client/domoauth.html#_domoauth_optional.print_is_token',
@@ -509,26 +269,14 @@
                                                                                                       'domolibrary/client/DomoAuth.py'),
                                              'domolibrary.client.DomoAuth.get_developer_auth': ( 'client/domoauth.html#get_developer_auth',
                                                                                                  'domolibrary/client/DomoAuth.py'),
                                              'domolibrary.client.DomoAuth.get_full_auth': ( 'client/domoauth.html#get_full_auth',
                                                                                             'domolibrary/client/DomoAuth.py'),
                                              'domolibrary.client.DomoAuth.test_access_token': ( 'client/domoauth.html#test_access_token',
                                                                                                 'domolibrary/client/DomoAuth.py')},
-            'domolibrary.client.DomoError': { 'domolibrary.client.DomoError.AuthNotProvidedError': ( 'client/domoerror.html#authnotprovidederror',
-                                                                                                     'domolibrary/client/DomoError.py'),
-                                              'domolibrary.client.DomoError.AuthNotProvidedError.__init__': ( 'client/domoerror.html#authnotprovidederror.__init__',
-                                                                                                              'domolibrary/client/DomoError.py'),
-                                              'domolibrary.client.DomoError.DatasetNotProvidedError': ( 'client/domoerror.html#datasetnotprovidederror',
-                                                                                                        'domolibrary/client/DomoError.py'),
-                                              'domolibrary.client.DomoError.DatasetNotProvidedError.__init__': ( 'client/domoerror.html#datasetnotprovidederror.__init__',
-                                                                                                                 'domolibrary/client/DomoError.py'),
-                                              'domolibrary.client.DomoError.DomoError': ( 'client/domoerror.html#domoerror',
-                                                                                          'domolibrary/client/DomoError.py'),
-                                              'domolibrary.client.DomoError.DomoError.__init__': ( 'client/domoerror.html#domoerror.__init__',
-                                                                                                   'domolibrary/client/DomoError.py')},
             'domolibrary.client.Logger': { 'domolibrary.client.Logger.Logger': ( 'client/logger.html#logger',
                                                                                  'domolibrary/client/Logger.py'),
                                            'domolibrary.client.Logger.Logger.__init__': ( 'client/logger.html#logger.__init__',
                                                                                           'domolibrary/client/Logger.py'),
                                            'domolibrary.client.Logger.Logger._add_crumb': ( 'client/logger.html#logger._add_crumb',
                                                                                             'domolibrary/client/Logger.py'),
                                            'domolibrary.client.Logger.Logger._add_log': ( 'client/logger.html#logger._add_log',
@@ -545,68 +293,58 @@
                                                                                           'domolibrary/client/Logger.py'),
                                            'domolibrary.client.Logger.Logger.log_warning': ( 'client/logger.html#logger.log_warning',
                                                                                              'domolibrary/client/Logger.py'),
                                            'domolibrary.client.Logger.Logger.output_log': ( 'client/logger.html#logger.output_log',
                                                                                             'domolibrary/client/Logger.py'),
                                            'domolibrary.client.Logger.TracebackDetails': ( 'client/logger.html#tracebackdetails',
                                                                                            'domolibrary/client/Logger.py')},
-            'domolibrary.client.ResponseGetData': { 'domolibrary.client.ResponseGetData.BlockedByVPN': ( 'client/responsegetdata.html#blockedbyvpn',
-                                                                                                         'domolibrary/client/ResponseGetData.py'),
-                                                    'domolibrary.client.ResponseGetData.BlockedByVPN.__init__': ( 'client/responsegetdata.html#blockedbyvpn.__init__',
-                                                                                                                  'domolibrary/client/ResponseGetData.py'),
-                                                    'domolibrary.client.ResponseGetData.ResponseGetData': ( 'client/responsegetdata.html#responsegetdata',
+            'domolibrary.client.ResponseGetData': { 'domolibrary.client.ResponseGetData.ResponseGetData': ( 'client/responsegetdata.html#responsegetdata',
                                                                                                             'domolibrary/client/ResponseGetData.py'),
                                                     'domolibrary.client.ResponseGetData.ResponseGetData._from_aiohttp_response': ( 'client/responsegetdata.html#responsegetdata._from_aiohttp_response',
                                                                                                                                    'domolibrary/client/ResponseGetData.py'),
                                                     'domolibrary.client.ResponseGetData.ResponseGetData._from_httpx_response': ( 'client/responsegetdata.html#responsegetdata._from_httpx_response',
                                                                                                                                  'domolibrary/client/ResponseGetData.py'),
                                                     'domolibrary.client.ResponseGetData.ResponseGetData._from_looper': ( 'client/responsegetdata.html#responsegetdata._from_looper',
                                                                                                                          'domolibrary/client/ResponseGetData.py'),
                                                     'domolibrary.client.ResponseGetData.ResponseGetData._from_requests_response': ( 'client/responsegetdata.html#responsegetdata._from_requests_response',
                                                                                                                                     'domolibrary/client/ResponseGetData.py'),
                                                     'domolibrary.client.ResponseGetData.ResponseGetData.set_response': ( 'client/responsegetdata.html#responsegetdata.set_response',
                                                                                                                          'domolibrary/client/ResponseGetData.py'),
                                                     'domolibrary.client.ResponseGetData._read_stream': ( 'client/responsegetdata.html#_read_stream',
                                                                                                          'domolibrary/client/ResponseGetData.py'),
                                                     'domolibrary.client.ResponseGetData._write_stream': ( 'client/responsegetdata.html#_write_stream',
-                                                                                                          'domolibrary/client/ResponseGetData.py'),
-                                                    'domolibrary.client.ResponseGetData.find_ip': ( 'client/responsegetdata.html#find_ip',
-                                                                                                    'domolibrary/client/ResponseGetData.py')},
-            'domolibrary.client.get_data': { 'domolibrary.client.get_data.GetData_Error': ( 'client/get_data.html#getdata_error',
-                                                                                            'domolibrary/client/get_data.py'),
-                                             'domolibrary.client.get_data.GetData_Error.__init__': ( 'client/get_data.html#getdata_error.__init__',
-                                                                                                     'domolibrary/client/get_data.py'),
-                                             'domolibrary.client.get_data.LooperError': ( 'client/get_data.html#loopererror',
+                                                                                                          'domolibrary/client/ResponseGetData.py')},
+            'domolibrary.client.get_data': { 'domolibrary.client.get_data.LooperError': ( 'client/get_data.html#loopererror',
                                                                                           'domolibrary/client/get_data.py'),
                                              'domolibrary.client.get_data.LooperError.__init__': ( 'client/get_data.html#loopererror.__init__',
                                                                                                    'domolibrary/client/get_data.py'),
                                              'domolibrary.client.get_data.get_data': ( 'client/get_data.html#get_data',
                                                                                        'domolibrary/client/get_data.py'),
                                              'domolibrary.client.get_data.get_data_aiohttp': ( 'client/get_data.html#get_data_aiohttp',
                                                                                                'domolibrary/client/get_data.py'),
                                              'domolibrary.client.get_data.looper': ( 'client/get_data.html#looper',
                                                                                      'domolibrary/client/get_data.py'),
                                              'domolibrary.client.get_data.looper_aiohttp': ( 'client/get_data.html#looper_aiohttp',
                                                                                              'domolibrary/client/get_data.py')},
-            'domolibrary.integrations.DomoJupyter': { 'domolibrary.integrations.DomoJupyter.DomoJupyterAccount_InstanceAuth': ( 'integrations/domojupyter.html#domojupyteraccount_instanceauth',
-                                                                                                                                'domolibrary/integrations/DomoJupyter.py'),
-                                                      'domolibrary.integrations.DomoJupyter.DomoJupyterAccount_InstanceAuth.__post_init__': ( 'integrations/domojupyter.html#domojupyteraccount_instanceauth.__post_init__',
-                                                                                                                                              'domolibrary/integrations/DomoJupyter.py'),
-                                                      'domolibrary.integrations.DomoJupyter.DomoJupyterAccount_InstanceAuth._clean_account_admin_accounts': ( 'integrations/domojupyter.html#domojupyteraccount_instanceauth._clean_account_admin_accounts',
-                                                                                                                                                              'domolibrary/integrations/DomoJupyter.py'),
-                                                      'domolibrary.integrations.DomoJupyter.DomoJupyterAccount_InstanceAuth._generate_auth': ( 'integrations/domojupyter.html#domojupyteraccount_instanceauth._generate_auth',
-                                                                                                                                               'domolibrary/integrations/DomoJupyter.py'),
-                                                      'domolibrary.integrations.DomoJupyter.DomoJupyterAccount_InstanceAuth._set_display_name': ( 'integrations/domojupyter.html#domojupyteraccount_instanceauth._set_display_name',
-                                                                                                                                                  'domolibrary/integrations/DomoJupyter.py'),
-                                                      'domolibrary.integrations.DomoJupyter.DomoJupyterAccount_InstanceAuth._test_regex_mask': ( 'integrations/domojupyter.html#domojupyteraccount_instanceauth._test_regex_mask',
-                                                                                                                                                 'domolibrary/integrations/DomoJupyter.py'),
-                                                      'domolibrary.integrations.DomoJupyter.DomoJupyterAccount_InstanceAuth.generate_auth_ls': ( 'integrations/domojupyter.html#domojupyteraccount_instanceauth.generate_auth_ls',
-                                                                                                                                                 'domolibrary/integrations/DomoJupyter.py'),
-                                                      'domolibrary.integrations.DomoJupyter.DomoJupyterAccount_InstanceAuth.get_domo_instance_auth_account': ( 'integrations/domojupyter.html#domojupyteraccount_instanceauth.get_domo_instance_auth_account',
-                                                                                                                                                               'domolibrary/integrations/DomoJupyter.py'),
+            'domolibrary.integrations.DomoJupyter': { 'domolibrary.integrations.DomoJupyter.DojoAccount_InstanceAuth': ( 'integrations/domojupyter.html#dojoaccount_instanceauth',
+                                                                                                                         'domolibrary/integrations/DomoJupyter.py'),
+                                                      'domolibrary.integrations.DomoJupyter.DojoAccount_InstanceAuth.__post_init__': ( 'integrations/domojupyter.html#dojoaccount_instanceauth.__post_init__',
+                                                                                                                                       'domolibrary/integrations/DomoJupyter.py'),
+                                                      'domolibrary.integrations.DomoJupyter.DojoAccount_InstanceAuth._clean_account_admin_accounts': ( 'integrations/domojupyter.html#dojoaccount_instanceauth._clean_account_admin_accounts',
+                                                                                                                                                       'domolibrary/integrations/DomoJupyter.py'),
+                                                      'domolibrary.integrations.DomoJupyter.DojoAccount_InstanceAuth._generate_auth': ( 'integrations/domojupyter.html#dojoaccount_instanceauth._generate_auth',
+                                                                                                                                        'domolibrary/integrations/DomoJupyter.py'),
+                                                      'domolibrary.integrations.DomoJupyter.DojoAccount_InstanceAuth._set_display_name': ( 'integrations/domojupyter.html#dojoaccount_instanceauth._set_display_name',
+                                                                                                                                           'domolibrary/integrations/DomoJupyter.py'),
+                                                      'domolibrary.integrations.DomoJupyter.DojoAccount_InstanceAuth._test_regex_mask': ( 'integrations/domojupyter.html#dojoaccount_instanceauth._test_regex_mask',
+                                                                                                                                          'domolibrary/integrations/DomoJupyter.py'),
+                                                      'domolibrary.integrations.DomoJupyter.DojoAccount_InstanceAuth.generate_auth_ls': ( 'integrations/domojupyter.html#dojoaccount_instanceauth.generate_auth_ls',
+                                                                                                                                          'domolibrary/integrations/DomoJupyter.py'),
+                                                      'domolibrary.integrations.DomoJupyter.DojoAccount_InstanceAuth.get_domo_instance_auth_account': ( 'integrations/domojupyter.html#dojoaccount_instanceauth.get_domo_instance_auth_account',
+                                                                                                                                                        'domolibrary/integrations/DomoJupyter.py'),
                                                       'domolibrary.integrations.DomoJupyter.GenerateAuth_CredentialsNotProvided': ( 'integrations/domojupyter.html#generateauth_credentialsnotprovided',
                                                                                                                                     'domolibrary/integrations/DomoJupyter.py'),
                                                       'domolibrary.integrations.DomoJupyter.GenerateAuth_CredentialsNotProvided.__init__': ( 'integrations/domojupyter.html#generateauth_credentialsnotprovided.__init__',
                                                                                                                                              'domolibrary/integrations/DomoJupyter.py'),
                                                       'domolibrary.integrations.DomoJupyter.GenerateAuth_InvalidDomoInstanceList': ( 'integrations/domojupyter.html#generateauth_invaliddomoinstancelist',
                                                                                                                                      'domolibrary/integrations/DomoJupyter.py'),
                                                       'domolibrary.integrations.DomoJupyter.GenerateAuth_InvalidDomoInstanceList.__init__': ( 'integrations/domojupyter.html#generateauth_invaliddomoinstancelist.__init__',
@@ -651,86 +389,42 @@
                                                                                                                               'domolibrary/integrations/DomoJupyter.py'),
                                                       'domolibrary.integrations.DomoJupyter.get_jupyter_account': ( 'integrations/domojupyter.html#get_jupyter_account',
                                                                                                                     'domolibrary/integrations/DomoJupyter.py')},
             'domolibrary.routes.account': { 'domolibrary.routes.account.AccountConfig_InvalidDataProvider': ( 'routes/account.html#accountconfig_invaliddataprovider',
                                                                                                               'domolibrary/routes/account.py'),
                                             'domolibrary.routes.account.AccountConfig_InvalidDataProvider.__init__': ( 'routes/account.html#accountconfig_invaliddataprovider.__init__',
                                                                                                                        'domolibrary/routes/account.py'),
-                                            'domolibrary.routes.account.GetAccount_NoMatch': ( 'routes/account.html#getaccount_nomatch',
-                                                                                               'domolibrary/routes/account.py'),
-                                            'domolibrary.routes.account.GetAccount_NoMatch.__init__': ( 'routes/account.html#getaccount_nomatch.__init__',
-                                                                                                        'domolibrary/routes/account.py'),
-                                            'domolibrary.routes.account.ShareAccount_V1_AccessLevel': ( 'routes/account.html#shareaccount_v1_accesslevel',
-                                                                                                        'domolibrary/routes/account.py'),
-                                            'domolibrary.routes.account.ShareAccount_V2_AccessLevel': ( 'routes/account.html#shareaccount_v2_accesslevel',
-                                                                                                        'domolibrary/routes/account.py'),
                                             'domolibrary.routes.account.create_account': ( 'routes/account.html#create_account',
                                                                                            'domolibrary/routes/account.py'),
                                             'domolibrary.routes.account.delete_account': ( 'routes/account.html#delete_account',
                                                                                            'domolibrary/routes/account.py'),
-                                            'domolibrary.routes.account.generate_share_account_payload_v1': ( 'routes/account.html#generate_share_account_payload_v1',
-                                                                                                              'domolibrary/routes/account.py'),
-                                            'domolibrary.routes.account.generate_share_account_payload_v2': ( 'routes/account.html#generate_share_account_payload_v2',
-                                                                                                              'domolibrary/routes/account.py'),
                                             'domolibrary.routes.account.get_account_config': ( 'routes/account.html#get_account_config',
                                                                                                'domolibrary/routes/account.py'),
                                             'domolibrary.routes.account.get_account_from_id': ( 'routes/account.html#get_account_from_id',
                                                                                                 'domolibrary/routes/account.py'),
                                             'domolibrary.routes.account.get_accounts': ( 'routes/account.html#get_accounts',
                                                                                          'domolibrary/routes/account.py'),
-                                            'domolibrary.routes.account.share_account_v1': ( 'routes/account.html#share_account_v1',
-                                                                                             'domolibrary/routes/account.py'),
-                                            'domolibrary.routes.account.share_account_v2': ( 'routes/account.html#share_account_v2',
-                                                                                             'domolibrary/routes/account.py'),
                                             'domolibrary.routes.account.update_account_config': ( 'routes/account.html#update_account_config',
                                                                                                   'domolibrary/routes/account.py'),
                                             'domolibrary.routes.account.update_account_name': ( 'routes/account.html#update_account_name',
                                                                                                 'domolibrary/routes/account.py')},
             'domolibrary.routes.activity_log': { 'domolibrary.routes.activity_log.get_activity_log_object_types': ( 'routes/activity_log.html#get_activity_log_object_types',
                                                                                                                     'domolibrary/routes/activity_log.py'),
                                                  'domolibrary.routes.activity_log.search_activity_log': ( 'routes/activity_log.html#search_activity_log',
                                                                                                           'domolibrary/routes/activity_log.py')},
-            'domolibrary.routes.bootstrap': { 'domolibrary.routes.bootstrap.get_bootstrap': ( 'routes/bootstrap.html#get_bootstrap',
+            'domolibrary.routes.bootstrap': { 'domolibrary.routes.bootstrap.GetBootstrap_InvalidAuthMethod': ( 'routes/bootstrap.html#getbootstrap_invalidauthmethod',
+                                                                                                               'domolibrary/routes/bootstrap.py'),
+                                              'domolibrary.routes.bootstrap.GetBootstrap_InvalidAuthMethod.__init__': ( 'routes/bootstrap.html#getbootstrap_invalidauthmethod.__init__',
+                                                                                                                        'domolibrary/routes/bootstrap.py'),
+                                              'domolibrary.routes.bootstrap.get_bootstrap': ( 'routes/bootstrap.html#get_bootstrap',
                                                                                               'domolibrary/routes/bootstrap.py'),
                                               'domolibrary.routes.bootstrap.get_bootstrap_features': ( 'routes/bootstrap.html#get_bootstrap_features',
                                                                                                        'domolibrary/routes/bootstrap.py'),
                                               'domolibrary.routes.bootstrap.get_bootstrap_pages': ( 'routes/bootstrap.html#get_bootstrap_pages',
                                                                                                     'domolibrary/routes/bootstrap.py')},
-            'domolibrary.routes.card': { 'domolibrary.routes.card.generate_body_search_cards_admin_summary': ( 'routes/card.html#generate_body_search_cards_admin_summary',
-                                                                                                               'domolibrary/routes/card.py'),
-                                         'domolibrary.routes.card.get_card_metadata': ( 'routes/card.html#get_card_metadata',
-                                                                                        'domolibrary/routes/card.py'),
-                                         'domolibrary.routes.card.get_kpi_definition': ( 'routes/card.html#get_kpi_definition',
-                                                                                         'domolibrary/routes/card.py'),
-                                         'domolibrary.routes.card.search_cards_admin_summary': ( 'routes/card.html#search_cards_admin_summary',
-                                                                                                 'domolibrary/routes/card.py')},
-            'domolibrary.routes.datacenter': { 'domolibrary.routes.datacenter.Datacenter_Enum': ( 'routes/datacenter.html#datacenter_enum',
-                                                                                                  'domolibrary/routes/datacenter.py'),
-                                               'domolibrary.routes.datacenter.Datacenter_Filter_Field_Enum': ( 'routes/datacenter.html#datacenter_filter_field_enum',
-                                                                                                               'domolibrary/routes/datacenter.py'),
-                                               'domolibrary.routes.datacenter.Dataflow_Type_Filter_Enum': ( 'routes/datacenter.html#dataflow_type_filter_enum',
-                                                                                                            'domolibrary/routes/datacenter.py'),
-                                               'domolibrary.routes.datacenter.SearchDatacenter_NoResultsFound': ( 'routes/datacenter.html#searchdatacenter_noresultsfound',
-                                                                                                                  'domolibrary/routes/datacenter.py'),
-                                               'domolibrary.routes.datacenter.SearchDatacenter_NoResultsFound.__init__': ( 'routes/datacenter.html#searchdatacenter_noresultsfound.__init__',
-                                                                                                                           'domolibrary/routes/datacenter.py'),
-                                               'domolibrary.routes.datacenter.generate_search_datacenter_account_body': ( 'routes/datacenter.html#generate_search_datacenter_account_body',
-                                                                                                                          'domolibrary/routes/datacenter.py'),
-                                               'domolibrary.routes.datacenter.generate_search_datacenter_body': ( 'routes/datacenter.html#generate_search_datacenter_body',
-                                                                                                                  'domolibrary/routes/datacenter.py'),
-                                               'domolibrary.routes.datacenter.generate_search_datacenter_filter': ( 'routes/datacenter.html#generate_search_datacenter_filter',
-                                                                                                                    'domolibrary/routes/datacenter.py'),
-                                               'domolibrary.routes.datacenter.generate_search_datacenter_filter_search_term': ( 'routes/datacenter.html#generate_search_datacenter_filter_search_term',
-                                                                                                                                'domolibrary/routes/datacenter.py'),
-                                               'domolibrary.routes.datacenter.get_lineage_upstream': ( 'routes/datacenter.html#get_lineage_upstream',
-                                                                                                       'domolibrary/routes/datacenter.py'),
-                                               'domolibrary.routes.datacenter.search_datacenter': ( 'routes/datacenter.html#search_datacenter',
-                                                                                                    'domolibrary/routes/datacenter.py')},
-            'domolibrary.routes.dataflow': { 'domolibrary.routes.dataflow.get_dataflow_by_id': ( 'routes/dataflow.html#get_dataflow_by_id',
-                                                                                                 'domolibrary/routes/dataflow.py')},
             'domolibrary.routes.dataset': { 'domolibrary.routes.dataset.DatasetNotFoundError': ( 'routes/dataset.html#datasetnotfounderror',
                                                                                                  'domolibrary/routes/dataset.py'),
                                             'domolibrary.routes.dataset.DatasetNotFoundError.__init__': ( 'routes/dataset.html#datasetnotfounderror.__init__',
                                                                                                           'domolibrary/routes/dataset.py'),
                                             'domolibrary.routes.dataset.QueryRequestError': ( 'routes/dataset.html#queryrequesterror',
                                                                                               'domolibrary/routes/dataset.py'),
                                             'domolibrary.routes.dataset.QueryRequestError.__init__': ( 'routes/dataset.html#queryrequesterror.__init__',
@@ -767,148 +461,16 @@
                                                                                                    'domolibrary/routes/dataset.py'),
                                             'domolibrary.routes.dataset.upload_dataset_stage_2_df': ( 'routes/dataset.html#upload_dataset_stage_2_df',
                                                                                                       'domolibrary/routes/dataset.py'),
                                             'domolibrary.routes.dataset.upload_dataset_stage_2_file': ( 'routes/dataset.html#upload_dataset_stage_2_file',
                                                                                                         'domolibrary/routes/dataset.py'),
                                             'domolibrary.routes.dataset.upload_dataset_stage_3': ( 'routes/dataset.html#upload_dataset_stage_3',
                                                                                                    'domolibrary/routes/dataset.py')},
-            'domolibrary.routes.grant': { 'domolibrary.routes.grant.GetGrants_Error': ( 'routes/grant.html#getgrants_error',
-                                                                                        'domolibrary/routes/grant.py'),
-                                          'domolibrary.routes.grant.GetGrants_Error.__init__': ( 'routes/grant.html#getgrants_error.__init__',
-                                                                                                 'domolibrary/routes/grant.py'),
-                                          'domolibrary.routes.grant.get_grants': ( 'routes/grant.html#get_grants',
-                                                                                   'domolibrary/routes/grant.py')},
-            'domolibrary.routes.group': { 'domolibrary.routes.group.CreateGroup_Error': ( 'routes/group.html#creategroup_error',
-                                                                                          'domolibrary/routes/group.py'),
-                                          'domolibrary.routes.group.CreateGroup_Error.__init__': ( 'routes/group.html#creategroup_error.__init__',
-                                                                                                   'domolibrary/routes/group.py'),
-                                          'domolibrary.routes.group.GroupType_Enum': ( 'routes/group.html#grouptype_enum',
-                                                                                       'domolibrary/routes/group.py'),
-                                          'domolibrary.routes.group.SearchGroups_Error': ( 'routes/group.html#searchgroups_error',
-                                                                                           'domolibrary/routes/group.py'),
-                                          'domolibrary.routes.group.SearchGroups_Error.__init__': ( 'routes/group.html#searchgroups_error.__init__',
-                                                                                                    'domolibrary/routes/group.py'),
-                                          'domolibrary.routes.group.create_group': ( 'routes/group.html#create_group',
-                                                                                     'domolibrary/routes/group.py'),
-                                          'domolibrary.routes.group.generate_body_create_group': ( 'routes/group.html#generate_body_create_group',
-                                                                                                   'domolibrary/routes/group.py'),
-                                          'domolibrary.routes.group.generate_body_update_group_membership': ( 'routes/group.html#generate_body_update_group_membership',
-                                                                                                              'domolibrary/routes/group.py'),
-                                          'domolibrary.routes.group.generate_body_update_group_membership_entity': ( 'routes/group.html#generate_body_update_group_membership_entity',
-                                                                                                                     'domolibrary/routes/group.py'),
-                                          'domolibrary.routes.group.get_all_groups': ( 'routes/group.html#get_all_groups',
-                                                                                       'domolibrary/routes/group.py'),
-                                          'domolibrary.routes.group.get_group_by_id': ( 'routes/group.html#get_group_by_id',
-                                                                                        'domolibrary/routes/group.py'),
-                                          'domolibrary.routes.group.get_group_membership': ( 'routes/group.html#get_group_membership',
-                                                                                             'domolibrary/routes/group.py'),
-                                          'domolibrary.routes.group.get_group_owners': ( 'routes/group.html#get_group_owners',
-                                                                                         'domolibrary/routes/group.py'),
-                                          'domolibrary.routes.group.search_groups_by_name': ( 'routes/group.html#search_groups_by_name',
-                                                                                              'domolibrary/routes/group.py'),
-                                          'domolibrary.routes.group.update_group': ( 'routes/group.html#update_group',
-                                                                                     'domolibrary/routes/group.py'),
-                                          'domolibrary.routes.group.update_group_membership': ( 'routes/group.html#update_group_membership',
-                                                                                                'domolibrary/routes/group.py')},
-            'domolibrary.routes.instance_config': { 'domolibrary.routes.instance_config.Allowlist_UnableToUpdate': ( 'routes/instance_config.html#allowlist_unabletoupdate',
-                                                                                                                     'domolibrary/routes/instance_config.py'),
-                                                    'domolibrary.routes.instance_config.Allowlist_UnableToUpdate.__init__': ( 'routes/instance_config.html#allowlist_unabletoupdate.__init__',
-                                                                                                                              'domolibrary/routes/instance_config.py'),
-                                                    'domolibrary.routes.instance_config.GetDomains_NotFound': ( 'routes/instance_config.html#getdomains_notfound',
-                                                                                                                'domolibrary/routes/instance_config.py'),
-                                                    'domolibrary.routes.instance_config.GetDomains_NotFound.__init__': ( 'routes/instance_config.html#getdomains_notfound.__init__',
-                                                                                                                         'domolibrary/routes/instance_config.py'),
-                                                    'domolibrary.routes.instance_config.get_allowlist': ( 'routes/instance_config.html#get_allowlist',
-                                                                                                          'domolibrary/routes/instance_config.py'),
-                                                    'domolibrary.routes.instance_config.get_authorized_domains': ( 'routes/instance_config.html#get_authorized_domains',
-                                                                                                                   'domolibrary/routes/instance_config.py'),
-                                                    'domolibrary.routes.instance_config.set_allowlist': ( 'routes/instance_config.html#set_allowlist',
-                                                                                                          'domolibrary/routes/instance_config.py'),
-                                                    'domolibrary.routes.instance_config.set_authorized_domains': ( 'routes/instance_config.html#set_authorized_domains',
-                                                                                                                   'domolibrary/routes/instance_config.py')},
-            'domolibrary.routes.page': { 'domolibrary.routes.page.get_page_accesslist': ( 'routes/page.html#get_page_accesslist',
-                                                                                          'domolibrary/routes/page.py'),
-                                         'domolibrary.routes.page.get_page_by_id': ( 'routes/page.html#get_page_by_id',
-                                                                                     'domolibrary/routes/page.py'),
-                                         'domolibrary.routes.page.get_page_definition': ( 'routes/page.html#get_page_definition',
-                                                                                          'domolibrary/routes/page.py')},
-            'domolibrary.routes.pdp': { 'domolibrary.routes.pdp.CreatePolicy_Error': ( 'routes/pdp.html#createpolicy_error',
-                                                                                       'domolibrary/routes/pdp.py'),
-                                        'domolibrary.routes.pdp.CreatePolicy_Error.__init__': ( 'routes/pdp.html#createpolicy_error.__init__',
-                                                                                                'domolibrary/routes/pdp.py'),
-                                        'domolibrary.routes.pdp.PDP_NotRetrieved': ( 'routes/pdp.html#pdp_notretrieved',
-                                                                                     'domolibrary/routes/pdp.py'),
-                                        'domolibrary.routes.pdp.PDP_NotRetrieved.__init__': ( 'routes/pdp.html#pdp_notretrieved.__init__',
-                                                                                              'domolibrary/routes/pdp.py'),
-                                        'domolibrary.routes.pdp.create_policy': ( 'routes/pdp.html#create_policy',
-                                                                                  'domolibrary/routes/pdp.py'),
-                                        'domolibrary.routes.pdp.delete_policy': ( 'routes/pdp.html#delete_policy',
-                                                                                  'domolibrary/routes/pdp.py'),
-                                        'domolibrary.routes.pdp.generate_policy_body': ( 'routes/pdp.html#generate_policy_body',
-                                                                                         'domolibrary/routes/pdp.py'),
-                                        'domolibrary.routes.pdp.generate_policy_parameter_simple': ( 'routes/pdp.html#generate_policy_parameter_simple',
-                                                                                                     'domolibrary/routes/pdp.py'),
-                                        'domolibrary.routes.pdp.get_pdp_policies': ( 'routes/pdp.html#get_pdp_policies',
-                                                                                     'domolibrary/routes/pdp.py'),
-                                        'domolibrary.routes.pdp.toggle_pdp': ('routes/pdp.html#toggle_pdp', 'domolibrary/routes/pdp.py'),
-                                        'domolibrary.routes.pdp.update_policy': ( 'routes/pdp.html#update_policy',
-                                                                                  'domolibrary/routes/pdp.py')},
-            'domolibrary.routes.publish': { 'domolibrary.routes.publish.accept_invite_by_id': ( 'routes/publish.html#accept_invite_by_id',
-                                                                                                'domolibrary/routes/publish.py'),
-                                            'domolibrary.routes.publish.get_publication_by_id': ( 'routes/publish.html#get_publication_by_id',
-                                                                                                  'domolibrary/routes/publish.py'),
-                                            'domolibrary.routes.publish.get_subscription_invititations': ( 'routes/publish.html#get_subscription_invititations',
-                                                                                                           'domolibrary/routes/publish.py'),
-                                            'domolibrary.routes.publish.get_subscription_summaries': ( 'routes/publish.html#get_subscription_summaries',
-                                                                                                       'domolibrary/routes/publish.py'),
-                                            'domolibrary.routes.publish.refresh_publish_jobs': ( 'routes/publish.html#refresh_publish_jobs',
-                                                                                                 'domolibrary/routes/publish.py'),
-                                            'domolibrary.routes.publish.search_publications': ( 'routes/publish.html#search_publications',
-                                                                                                'domolibrary/routes/publish.py')},
-            'domolibrary.routes.role': { 'domolibrary.routes.role.Role_NotRetrieved': ( 'routes/role.html#role_notretrieved',
-                                                                                        'domolibrary/routes/role.py'),
-                                         'domolibrary.routes.role.Role_NotRetrieved.__init__': ( 'routes/role.html#role_notretrieved.__init__',
-                                                                                                 'domolibrary/routes/role.py'),
-                                         'domolibrary.routes.role.create_role': ( 'routes/role.html#create_role',
-                                                                                  'domolibrary/routes/role.py'),
-                                         'domolibrary.routes.role.delete_role': ( 'routes/role.html#delete_role',
-                                                                                  'domolibrary/routes/role.py'),
-                                         'domolibrary.routes.role.get_default_role': ( 'routes/role.html#get_default_role',
-                                                                                       'domolibrary/routes/role.py'),
-                                         'domolibrary.routes.role.get_role_grants': ( 'routes/role.html#get_role_grants',
-                                                                                      'domolibrary/routes/role.py'),
-                                         'domolibrary.routes.role.get_role_membership': ( 'routes/role.html#get_role_membership',
-                                                                                          'domolibrary/routes/role.py'),
-                                         'domolibrary.routes.role.get_roles': ('routes/role.html#get_roles', 'domolibrary/routes/role.py'),
-                                         'domolibrary.routes.role.role_membership_add_users': ( 'routes/role.html#role_membership_add_users',
-                                                                                                'domolibrary/routes/role.py'),
-                                         'domolibrary.routes.role.set_default_role': ( 'routes/role.html#set_default_role',
-                                                                                       'domolibrary/routes/role.py'),
-                                         'domolibrary.routes.role.set_role_grants': ( 'routes/role.html#set_role_grants',
-                                                                                      'domolibrary/routes/role.py'),
-                                         'domolibrary.routes.role.update_role_metadata': ( 'routes/role.html#update_role_metadata',
-                                                                                           'domolibrary/routes/role.py')},
-            'domolibrary.routes.user': { 'domolibrary.routes.user.SearchUser_NoResults': ( 'routes/user.html#searchuser_noresults',
-                                                                                           'domolibrary/routes/user.py'),
-                                         'domolibrary.routes.user.SearchUser_NoResults.__init__': ( 'routes/user.html#searchuser_noresults.__init__',
-                                                                                                    'domolibrary/routes/user.py'),
-                                         'domolibrary.routes.user.UserProperty': ( 'routes/user.html#userproperty',
-                                                                                   'domolibrary/routes/user.py'),
-                                         'domolibrary.routes.user.UserProperty.__init__': ( 'routes/user.html#userproperty.__init__',
-                                                                                            'domolibrary/routes/user.py'),
-                                         'domolibrary.routes.user.UserProperty._valid_value': ( 'routes/user.html#userproperty._valid_value',
-                                                                                                'domolibrary/routes/user.py'),
-                                         'domolibrary.routes.user.UserProperty.to_json': ( 'routes/user.html#userproperty.to_json',
-                                                                                           'domolibrary/routes/user.py'),
-                                         'domolibrary.routes.user.UserProperty_Type': ( 'routes/user.html#userproperty_type',
-                                                                                        'domolibrary/routes/user.py'),
-                                         'domolibrary.routes.user.create_user': ( 'routes/user.html#create_user',
+            'domolibrary.routes.user': { 'domolibrary.routes.user.create_user': ( 'routes/user.html#create_user',
                                                                                   'domolibrary/routes/user.py'),
-                                         'domolibrary.routes.user.generate_patch_user_property_body': ( 'routes/user.html#generate_patch_user_property_body',
-                                                                                                        'domolibrary/routes/user.py'),
                                          'domolibrary.routes.user.generate_search_users_body_by_email': ( 'routes/user.html#generate_search_users_body_by_email',
                                                                                                           'domolibrary/routes/user.py'),
                                          'domolibrary.routes.user.generate_search_users_body_by_id': ( 'routes/user.html#generate_search_users_body_by_id',
                                                                                                        'domolibrary/routes/user.py'),
                                          'domolibrary.routes.user.get_all_users': ( 'routes/user.html#get_all_users',
                                                                                     'domolibrary/routes/user.py'),
                                          'domolibrary.routes.user.process_v1_search_users': ( 'routes/user.html#process_v1_search_users',
@@ -918,44 +480,20 @@
                                          'domolibrary.routes.user.reset_password': ( 'routes/user.html#reset_password',
                                                                                      'domolibrary/routes/user.py'),
                                          'domolibrary.routes.user.search_users': ( 'routes/user.html#search_users',
                                                                                    'domolibrary/routes/user.py'),
                                          'domolibrary.routes.user.search_virtual_user_by_subscriber_instance': ( 'routes/user.html#search_virtual_user_by_subscriber_instance',
                                                                                                                  'domolibrary/routes/user.py'),
                                          'domolibrary.routes.user.set_user_landing_page': ( 'routes/user.html#set_user_landing_page',
-                                                                                            'domolibrary/routes/user.py'),
-                                         'domolibrary.routes.user.update_user': ( 'routes/user.html#update_user',
-                                                                                  'domolibrary/routes/user.py')},
+                                                                                            'domolibrary/routes/user.py')},
             'domolibrary.utils.DictDot': { 'domolibrary.utils.DictDot.DictDot': ( 'utils/dictdot.html#dictdot',
                                                                                   'domolibrary/utils/DictDot.py'),
                                            'domolibrary.utils.DictDot.DictDot.__getattr__': ( 'utils/dictdot.html#dictdot.__getattr__',
                                                                                               'domolibrary/utils/DictDot.py'),
                                            'domolibrary.utils.DictDot.DictDot.__init__': ( 'utils/dictdot.html#dictdot.__init__',
-                                                                                           'domolibrary/utils/DictDot.py'),
-                                           'domolibrary.utils.DictDot.split_str_to_obj': ( 'utils/dictdot.html#split_str_to_obj',
                                                                                            'domolibrary/utils/DictDot.py')},
-            'domolibrary.utils.chunk_execution': { 'domolibrary.utils.chunk_execution.chunk_list': ( 'utils/chunk_execution.html#chunk_list',
-                                                                                                     'domolibrary/utils/chunk_execution.py'),
-                                                   'domolibrary.utils.chunk_execution.run_sequence': ( 'utils/chunk_execution.html#run_sequence',
-                                                                                                       'domolibrary/utils/chunk_execution.py')},
-            'domolibrary.utils.convert': { 'domolibrary.utils.convert.ConcatDataframe_InvalidElement': ( 'utils/convert.html#concatdataframe_invalidelement',
-                                                                                                         'domolibrary/utils/convert.py'),
-                                           'domolibrary.utils.convert.ConcatDataframe_InvalidElement.__init__': ( 'utils/convert.html#concatdataframe_invalidelement.__init__',
-                                                                                                                  'domolibrary/utils/convert.py'),
-                                           'domolibrary.utils.convert.concat_list_dataframe': ( 'utils/convert.html#concat_list_dataframe',
-                                                                                                'domolibrary/utils/convert.py'),
-                                           'domolibrary.utils.convert.convert_datetime_to_epoch_millisecond': ( 'utils/convert.html#convert_datetime_to_epoch_millisecond',
+            'domolibrary.utils.convert': { 'domolibrary.utils.convert.convert_datetime_to_epoch_millisecond': ( 'utils/convert.html#convert_datetime_to_epoch_millisecond',
                                                                                                                 'domolibrary/utils/convert.py'),
                                            'domolibrary.utils.convert.convert_epoch_millisecond_to_datetime': ( 'utils/convert.html#convert_epoch_millisecond_to_datetime',
                                                                                                                 'domolibrary/utils/convert.py'),
                                            'domolibrary.utils.convert.convert_snake_to_pascal': ( 'utils/convert.html#convert_snake_to_pascal',
-                                                                                                  'domolibrary/utils/convert.py')},
-            'domolibrary.utils.read_creds_from_dotenv': { 'domolibrary.utils.read_creds_from_dotenv.ReadCreds_EnvFileNotExist': ( 'utils/read_creds_from_dotenv.html#readcreds_envfilenotexist',
-                                                                                                                                  'domolibrary/utils/read_creds_from_dotenv.py'),
-                                                          'domolibrary.utils.read_creds_from_dotenv.ReadCreds_EnvFileNotExist.__init__': ( 'utils/read_creds_from_dotenv.html#readcreds_envfilenotexist.__init__',
-                                                                                                                                           'domolibrary/utils/read_creds_from_dotenv.py'),
-                                                          'domolibrary.utils.read_creds_from_dotenv.read_creds_from_dotenv': ( 'utils/read_creds_from_dotenv.html#read_creds_from_dotenv',
-                                                                                                                               'domolibrary/utils/read_creds_from_dotenv.py')},
-            'domolibrary.utils.upload_data': { 'domolibrary.utils.upload_data.loop_upload': ( 'utils/upload_data.html#loop_upload',
-                                                                                              'domolibrary/utils/upload_data.py'),
-                                               'domolibrary.utils.upload_data.upload_data': ( 'utils/upload_data.html#upload_data',
-                                                                                              'domolibrary/utils/upload_data.py')}}}
+                                                                                                  'domolibrary/utils/convert.py')}}}
```

### Comparing `domolibrary-0.0.81/domolibrary/classes/DomoAccount.py` & `domolibrary-0.0.9/domolibrary/integrations/DomoJupyter.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,573 +1,437 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/classes/50_DomoAccount.ipynb.
+# AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/integrations/DomoJupyter.ipynb.
 
 # %% auto 0
-__all__ = ['DomoAccount_Config', 'DomoAccount_Config_AbstractCredential', 'DomoAccount_Config_DatasetCopy',
-           'DomoAccount_Config_Governance', 'DomoAccount_Config_HighBandwidthConnector', 'DomoAccount_Config_AwsAthena',
-           'AccountConfig', 'DomoAccount', 'DomoAccount_DataProviderType_ConfigNotDefined',
-           'DomoAccount_UpdateName_Error', 'DomoAccount_CreateAccount_Error', 'DomoAccount_DeleteAccount_Error',
-           'ShareAccount_AccessLevel', 'DomoAccounts']
+__all__ = ['NoConfigCompanyError', 'GetInstanceConfig', 'GetDomains_Query_Exception_PW_Col_Error',
+           'GetDomains_Query_AuthMatch_Error', 'GetJupyter_ErrorRetrievingAccount',
+           'GetJupyter_ErrorRetrievingAccountProperty', 'get_jupyter_account', 'InvalidAccountTypeError',
+           'DojoAccount_InstanceAuth', 'InvalidAccountNameError', 'GenerateAuth_InvalidDomoInstanceList',
+           'GenerateAuth_CredentialsNotProvided']
 
-# %% ../../nbs/classes/50_DomoAccount.ipynb 3
-from enum import Enum
+# %% ../../nbs/integrations/DomoJupyter.ipynb 2
 from dataclasses import dataclass, field
-from abc import ABC, abstractmethod
+from typing import Optional
+from enum import Enum
 
-from typing import Union
 
-import datetime as dt
 import re
+import pandas as pd
+import importlib
+import datetime as dt
+import time
 
+import json
 
-import httpx
-
-from fastcore.basics import patch_to
+# import domojupyter as dj
 
-import domolibrary.utils.convert as cd
-import domolibrary.utils.DictDot as util_dd
 import domolibrary.client.DomoAuth as dmda
-import domolibrary.client.DomoError as de
-import domolibrary.routes.account as account_routes
-
-# %% ../../nbs/classes/50_DomoAccount.ipynb 5
-class DomoAccount_Config(ABC):
-    """DomoAccount Config abstract base class"""
+import domolibrary.client.Logger as lc
+import domolibrary.classes.DomoDataset as dmds
 
-    data_provider_type: str
+from nbdev.showdoc import show_doc
+from fastcore.basics import patch_to
 
-    @classmethod
-    @abstractmethod
-    def _from_json(cls, obj):
-        """convert accounts API response into a class object"""
-        pass
 
-    @abstractmethod
-    def to_json(self):
-        """convert class object into a format the accounts API expects"""
-        pass
+# %% ../../nbs/integrations/DomoJupyter.ipynb 3
+class NoConfigCompanyError(Exception):
+    def __init__(self, sql, domo_instance):
+        message = f'SQL "{sql}" returned no results in {domo_instance}'
+        self.message = message
+        super().__init__(self.message)
+
+
+class GetInstanceConfig:
+    config: pd.DataFrame = None
+    logger: lc.Logger = None
+
+    def __init__(self, logger: Optional[lc.Logger] = None):
+
+        self.logger = logger or lc.Logger(app_name='GetInstanceConfig')
+
+    async def _retrieve_company_ds(self,
+                                   config_auth: dmda.DomoAuth,
+                                   dataset_id: str,
+                                   sql: str,
+                                   debug_prn: bool = False,
+                                   debug_api: bool = False,
+                                   debug_log: bool = False,
+            
+                                   ) -> pd.DataFrame:
+
+        ds = await dmds.DomoDataset.get_from_id(auth=config_auth,
+                                                dataset_id=dataset_id, debug_api=debug_api)
+
+        message = f"⚙️ START - Retrieving company list \n{ds.display_url()} using \n{sql}"
+
+        if debug_prn:
+            print(message)
+
+        self.logger.log_info(message, debug_log=debug_log)
+
+        df = await ds.query_dataset_private(auth=config_auth,
+                                            dataset_id=dataset_id,
+                                            sql=sql,
+                                            debug_api=debug_api)
+        if len(df.index) == 0:
+            raise NoConfigCompanyError(
+                sql, domo_instance=config_auth.domo_instance)
+
+        self.config = df
+
+        message = f"\n⚙️ SUCCESS 🎉 Retrieved company list \nThere are {len(df.index)} companies to update"
+
+        if debug_prn:
+            print(message)
+        self.logger.log_info(message, debug_log=debug_log)
+
+        return df
+
+
+# %% ../../nbs/integrations/DomoJupyter.ipynb 6
+class GetDomains_Query_Exception_PW_Col_Error(Exception):
+    """raise if SQL query fails to return column named 'config_exception_pw'"""
+
+    def __init__(self, sql :str = None, domo_instance : str = None, message : str = None):
+        message = message or f"Query failed to return a column 'config_exception_pw' sql = {sql} in {domo_instance}"
+        super().__init__(self, message)
+
+
+@patch_to(GetInstanceConfig, cls_method=True)
+async def get_domains_with_global_config_auth(cls: GetInstanceConfig,
+
+                                              config_dataset_id: str,
+                                              config_auth: dmda.DomoAuth, # which instance to retrieve configuration data from
+                                              
+                                              global_auth: dmda.DomoAuth, # global authentication credentials
+                                              global_exception_auth: dmda.DomoAuth, # exception credentials (ex 24 char password)
+                                              # must return a column named domo_instance, if there is an exception_auth, must return a column 'config_exception_pw'
+                                              
+                                              config_sql: str = "select domain as domo_instance, config_exception_pw from table",
+                                              
+                                              debug_api: bool = False,
+                                              debug_log: bool = False,
+                                              debug_prn: bool = False,
+                                              
+                                              logger: lc.Logger = None) -> pd.DataFrame:
+    if not logger:
+        logger = lc.Logger(app_name='get_domains_with_global_config_auth')
+
+    gic = cls(logger = logger)
+
+    df = await gic._retrieve_company_ds(config_auth=config_auth,
+                                        dataset_id=config_dataset_id,
+                                        sql=config_sql,
+                                       debug_prn=debug_prn,
+                                       debug_log=debug_log,
+                                       debug_api=debug_api)
+    
+    if 'config_exception_pw' not in df.columns:
+        message = f"Query failed to return a column 'config_exception_pw' sql = {config_sql} in {config_auth.domo_instance}"
+        gic.logger.log_error(message)
+        raise GetDomains_Query_Exception_PW_Col_Error(message= message)
+
+    for index, instance in df.iterrows():
+        creds = global_auth
+
+        if instance['config_exception_pw'] == 1:
+            creds = global_exception_auth
+
+        creds.domo_instance=instance['domo_instance']
+
+        try:
+            await creds.get_auth_token()
+            df.at[index, 'is_valid'] = 1
+
+        except dmda.InvalidCredentialsError as e:
+            if debug_prn:
+                print(e)
+            
+            logger.log_error(str(e))
+            df.at[index, 'is_valid'] = 0
+        
+        finally:
+            df.at[index, 'instance_auth'] = creds
+
+    return df
+
+
+# %% ../../nbs/integrations/DomoJupyter.ipynb 10
+class GetDomains_Query_AuthMatch_Error(Exception):
+    """raise if SQL query fails to return column named 'auth_match_col'"""
+    def __init__(self, sql : str = None, domo_instance : str = None ,message : str = None):
+        self.message = message or f"Query failed to return a column 'auth_match_col' sql = {sql} in {domo_instance}"
+        super().__init__( self.message)
+
+@patch_to(GetInstanceConfig, cls_method=True)
+async def get_domains_with_instance_auth(cls: GetInstanceConfig,
+                                         config_dataset_id: str, # dataset_id to run config_sql query against
+                                         config_auth: dmda.DomoAuth,  # which instance to retrieve configuration data from
+                                         
+                                         default_auth : dmda.DomoAuth, # default auth to use with each row
+                                         auth_enum : Enum, # Enum where enum_name should match to `auth_match_col` from config_sql query and enum_value is the appropriate DomoAuth object
+                                         
+                                         config_sql: str = "select domain as domo_instance,concat(config_useprod, '-', project) as auth_match_col from table",
+                                         
+                                         debug_api: bool = False,
+                                         debug_log: bool = False,
+                                         debug_prn: bool = False,
+                                         logger: lc.Logger = None # pass in Logger class
+                                         ) -> pd.DataFrame: # returns a dataframe with domo_instance, instance_auth, and binary column is_valid 
+    """uses a sql query to retrieve a list of domo_instances and map authentication object to each instance"""
+    
+    if not logger:
+        logger = lc.Logger(app_name='get_domains_with_instance_auth')
+
+    gic = cls(logger=logger)
+
+    df = await gic._retrieve_company_ds(config_auth=config_auth,
+                                        dataset_id=config_dataset_id,
+                                        sql=config_sql,
+                                        debug_prn=debug_prn,
+                                        debug_log=debug_log,
+                                        debug_api=debug_api)
+
+    if 'auth_match_col' not in df.columns:
+        message = f"Query failed to return a column 'auth_match_col' sql = {config_sql} in {config_auth.domo_instance}"
+        raise GetDomains_Query_AuthMatch_Error(message)
+
+    for index, instance in df.iterrows():
+        
+        creds = default_auth
+
+        match_auth = next(
+            (member.value for member in auth_enum if member.name == instance['auth_match_col']))
+
+        if match_auth:
+            creds = match_auth
+
+        creds.domo_instance=instance['domo_instance']
+
+        try:
+            await creds.get_auth_token(debug_api = debug_api)
+            df.at[index, 'is_valid'] = 1
+
+        except dmda.InvalidCredentialsError as e:
+            if debug_prn:
+                print(e)
+            
+            logger.log_error(str(e))
+            df.at[index, 'is_valid'] = 0
+        
+        finally:
+            df.at[index, 'instance_auth'] = creds
+
+    return df
+
+
+# %% ../../nbs/integrations/DomoJupyter.ipynb 14
+class GetJupyter_ErrorRetrievingAccount(Exception):
+    def __init__(self, account_name):
+        self.message = f'failure to retrieve DomoDojo Account {account_name}'
+        super().__init__(self.message)
+
+
+class GetJupyter_ErrorRetrievingAccountProperty(Exception):
+    def __init__(self, account_name, property_name):
+        self.message = f'failure to retrieve {property_name} DomoDojo Account {account_name}'
+        super().__init__(self.message)
+
+def get_jupyter_account(account_name: str,  # name of account as it appears in the
+                        domojupyter_fn : callable,
+                        maximum_retry: int = 10
+                        ) -> (list, dict):  # returns account properties list and a dictionary of the properties.
+    """import a domojupyter account, will loop until success"""
+    account_properties = None
+
+    retry_attempt = 0
+    while not account_properties and retry_attempt <= maximum_retry:
+        try:
+            account_properties = domojupyter_fn.get_account_property_keys(
+                account_name)
+            retry_attempt += 1
+
+        except Exception as e:
+            print(f"Error:  retry attempt {retry_attempt} - {account_name}")
+            time.sleep(2)
+    
+    if not account_properties:
+        raise GetJupyter_ErrorRetrievingAccount(
+            account_name=account_name)
+
+    obj = {}
+
+    retry_attempt = 0
+    for index, prop in enumerate(account_properties):
+        value = None
+
+        while not value and retry_attempt <= maximum_retry:
+            try:
+                value = domojupyter_fn.get_account_property_value(
+                    account_name, account_properties[index])
+            
+            except Exception as e:
+                print(f"trying again - {prop}")
+                time.sleep(2)
+
+        if not value:
+            raise GetJupyter_ErrorRetrievingAccountProperty(account_name=account_name, property_name = prop)
+            
+        obj.update({prop: value})
+
+    return account_properties, obj
+
+# %% ../../nbs/integrations/DomoJupyter.ipynb 15
+class InvalidAccountTypeError(Exception):
+    """raised when account type is not expected type"""
 
+    def __init__(self, account_name, account_type):
 
-# %% ../../nbs/classes/50_DomoAccount.ipynb 6
-@dataclass
-class DomoAccount_Config_AbstractCredential(DomoAccount_Config):
-    data_provider_type = "abstract-credential-store"
-    credentials: dict
+        self.message = f"account: {account_name} is not {account_type}"
 
-    @classmethod
-    def _from_json(cls, obj):
+        super().__init__(self.message)
+    pass
 
-        dd = util_dd.DictDot(obj)
+@dataclass
+class DojoAccount_InstanceAuth:
 
-        return cls(
-            credentials=dd.credentials,
-        )
+    account_name: str
 
-    def to_json(self):
-        return {"credentials": self.credentials}
+    domo_username: str = None
 
+    display_name: str = field(repr=False, default=None)
 
-# %% ../../nbs/classes/50_DomoAccount.ipynb 7
-@dataclass
-class DomoAccount_Config_DatasetCopy(DomoAccount_Config):
-    domo_instance: str
-    access_token: str = field(repr=False)
+    domo_instance: str = field(repr=False, default=None)
+    domo_instance_ls: list = field(repr=False, default=None)
 
-    data_provider_type = "dataset-copy"
+    raw_cred: dict = field(repr=False, default=None)
+    domo_password: str = field(repr=False, default=None)
+    domo_access_token : str = field(repr = False, default = None)
 
-    @classmethod
-    def _from_json(cls, obj):
+    auth_ls: list = field(repr=False, default=None)
 
-        dd = util_dd.DictDot(obj)
+    account_name_mask = '^dj_.*_acc'
 
-        return cls(access_token=dd.accessToken, domo_instance=dd.instance)
+    def __post_init__(self):
+        if not self.display_name and self.domo_username:
+            self._set_display_name()
 
-    def to_json(self):
-        return {"accessToken": self.access_token, "instance": self.domo_instance}
+    def _set_display_name(self ):
+        clean_text = re.sub('@.*$', '', self.domo_username)
+        self.display_name = clean_text
 
 
-# %% ../../nbs/classes/50_DomoAccount.ipynb 8
-@dataclass
-class DomoAccount_Config_Governance(DomoAccount_Config):
-    domo_instance: str
-    access_token: str = field(repr=False)
-
-    data_provider_type = "domo-governance-d14c2fef-49a8-4898-8ddd-f64998005600"
+    @staticmethod
+    def _test_regex_mask(test_string: str  # the string to test
+                         , regex_mask: str  # the regex expression to test
+                         ) -> bool:  # boolean of the re match
+        """tests if a string matches the regex pattern"""
 
-    @classmethod
-    def _from_json(cls, obj):
+        return bool(re.match(regex_mask, test_string))
 
-        dd = util_dd.DictDot(obj)
+    @staticmethod
+    def _clean_account_admin_accounts(account_name):
 
-        return cls(access_token=dd.apikey, domo_instance=dd.customer)
+        clean_str = re.sub('^dj_', '', account_name)
+        clean_str = re.sub('_acc$', '', clean_str)
 
-    def to_json(self):
-        return {"apikey": self.access_token, "customer": self.domo_instance}
+        return clean_str
 
+# %% ../../nbs/integrations/DomoJupyter.ipynb 16
+class InvalidAccountNameError(Exception):
+    """raised when account name does not follow format string"""
 
-# %% ../../nbs/classes/50_DomoAccount.ipynb 9
-@dataclass
-class DomoAccount_Config_HighBandwidthConnector(DomoAccount_Config):
-    aws_access_key: str
-    aws_secret_key: str = field(repr=False)
-    s3_staging_dir: str
-
-    region: str = "us-west-2"
-    data_provider_type = "amazon-athena-high-bandwidth"
-
-    @classmethod
-    def _from_json(cls, obj):
-
-        dd = util_dd.DictDot(obj)
-
-        return cls(
-            aws_access_key=dd.awsAccessKey,
-            aws_secret_key=dd.awsSecretKey,
-            s3_staging_dir=dd.s3StagingDir,
-            region=dd.region,
-        )
-
-    def to_json(self):
-        return {
-            "awsAccessKey": self.aws_access_key,
-            "awsSecretKey": self.aws_secret_key,
-            "s3StagingDir": self.s3_staging_dir,
-            "region": self.region,
-        }
+    def __init__(self, account_name=None, regex_pattern=None):
+        account_str = f'"{account_name}" '
+        regex_str = f'"{regex_pattern}"'
 
+        message = f"string {account_str if account_name else ''}does not match regex pattern {regex_str or ''}"
+        self.message = message
 
-# %% ../../nbs/classes/50_DomoAccount.ipynb 10
-@dataclass
-class DomoAccount_Config_AwsAthena(DomoAccount_Config):
-    aws_access_key: str
-    aws_secret_key: str = field(repr=False)
-    s3_staging_dir: str
-    workgroup: str
-
-    region: str = "us-west-2"
-    data_provider_type = "aws-athena"
-
-    @classmethod
-    def _from_json(cls, obj):
-
-        dd = util_dd.DictDot(obj)
-
-        return cls(
-            aws_access_key=dd.awsAccessKey,
-            aws_secret_key=dd.awsSecretKey,
-            s3_staging_dir=dd.s3StagingDir,
-            region=dd.region,
-            workgroup=dd.workgroup,
-        )
-
-    def to_json(self):
-        return {
-            "awsAccessKey": self.aws_access_key,
-            "awsSecretKey": self.aws_secret_key,
-            "s3StagingDir": self.s3_staging_dir,
-            "region": self.region,
-            "workgroup": self.workgroup,
-        }
+        super().__init__(self.message)
 
-# %% ../../nbs/classes/50_DomoAccount.ipynb 11
-class AccountConfig(Enum):
+@patch_to(DojoAccount_InstanceAuth, cls_method=True)
+def get_domo_instance_auth_account(cls: DojoAccount_InstanceAuth, account_name: str,  # domojupyter account to retrieve
+                     # Domo's domojupyter module, pass in b/c can only be retrieved inside Domo jupyter notebook environment
+                     domojupyter_fn: callable,
+                     # set the domo_instance or retrieve from the domojupyter_account credential store
+                     domo_instance=None
+                     ):
     """
-    Enum provides appropriate spelling for data_provider_type and config object.
-    The name of the enum should correspond with the data_provider_type with hyphens replaced with underscores.
+    retrieves Abstract Credential Store from DomoJupyter environment.
+    expects credentials property to contain DOMO_USERNAME, DOMO_PASSWORD, or DOMO_ACCESS_TOKEN, and (optional) DOMO_INSTANCE
     """
 
-    amazon_athena_high_bandwidth = DomoAccount_Config_HighBandwidthConnector
-
-    abstract_credential_store = DomoAccount_Config_AbstractCredential
-
-    dataset_copy = DomoAccount_Config_DatasetCopy
-
-    domo_governance_d14c2fef_49a8_4898_8ddd_f64998005600 = DomoAccount_Config_Governance
-
-    aws_athena = DomoAccount_Config_AwsAthena
-
-# %% ../../nbs/classes/50_DomoAccount.ipynb 13
-@dataclass
-class DomoAccount:
-    name: str
-    data_provider_type: str
-
-    id: int = None
-    created_dt: dt.datetime = None
-    modified_dt: dt.datetime = None
-    auth: dmda.DomoAuth = field(repr=False, default=None)
-
-    config: DomoAccount_Config = None
-
-    @classmethod
-    def _from_json(cls, obj: dict, auth: dmda.DomoAuth = None):
-        """converts data_v1_accounts API response into an accounts class object"""
-
-        dd = util_dd.DictDot(obj)
-
-        return cls(
-            id=dd.id,
-            name=dd.displayName,
-            data_provider_type=dd.dataProviderType,
-            created_dt=cd.convert_epoch_millisecond_to_datetime(dd.createdAt),
-            modified_dt=cd.convert_epoch_millisecond_to_datetime(dd.modifiedAt),
-            auth=auth,
-        )
-
-# %% ../../nbs/classes/50_DomoAccount.ipynb 14
-class DomoAccount_DataProviderType_ConfigNotDefined(de.DomoError):
-    def __init__(
-        self, account_id, data_provider_type, domo_instance, function_name="_get_config"
-    ):
-
-        message = f"🛑 data provider type {data_provider_type} for account_id {account_id} not defined yet.  Extend the AccountConfig class"
-
-        super().__init__(
-            message=message, function_name=function_name, domo_instance=domo_instance
-        )
-
-
-@patch_to(DomoAccount)
-async def _get_config(
-    self: DomoAccount, session=None, debug_api: bool = None, return_raw: bool = False
-):
-
-    res_config = await account_routes.get_account_config(
-        auth=self.auth,
-        account_id=self.id,
-        data_provider_type=self.data_provider_type,
-        session=session,
-        debug_api=debug_api,
-    )
-
-    if return_raw:
-        return res_config
-
-    enum_clean = re.sub("-", "_", self.data_provider_type)
-
-    if not enum_clean in AccountConfig.__members__:
-        raise DomoAccount_DataProviderType_ConfigNotDefined(
-            account_id=self.id,
-            data_provider_type=self.data_provider_type,
-            domo_instance=self.auth.domo_instance,
-        )
-
-    self.config = AccountConfig[enum_clean].value._from_json(res_config.response)
-
-    return self.config
-
-# %% ../../nbs/classes/50_DomoAccount.ipynb 15
-@patch_to(DomoAccount, cls_method=True)
-async def get_from_id(
-    cls,
-    auth: dmda.DomoAuth,
-    account_id: int,
-    session: httpx.AsyncClient = None,
-    return_raw: bool = False,
-    debug_api: bool = False,
-):
-
-    res = await account_routes.get_account_from_id(
-        auth=auth, account_id=account_id, session=session, debug_api=debug_api
-    )
-
-    if return_raw:
-        return res
-
-    if not res.is_success:
-        return None
-
-    obj = res.response
-    acc = cls._from_json(obj, auth)
-
-    try:
-        await acc._get_config(session=session, debug_api=debug_api)
-
-    except DomoAccount_DataProviderType_ConfigNotDefined as e:
-        print(e)
-
-    finally:
-        return acc
-
-# %% ../../nbs/classes/50_DomoAccount.ipynb 19
-@patch_to(DomoAccount)
-async def update_config(
-    self: DomoAccount,
-    auth: dmda.DomoAuth = None,
-    debug_api: bool = False,
-    config: DomoAccount_Config = None,
-    session: httpx.AsyncClient = None,
-    return_raw: bool = False,
-):
-
-    auth = auth or self.auth
-
-    config = config or self.config
-
-    res = await account_routes.update_account_config(
-        auth=auth,
-        account_id=self.id,
-        data_provider_type=self.data_provider_type,
-        config_body=config.to_json(),
-        debug_api=debug_api,
-        session=session,
-    )
-
-    if return_raw:
-        return res
-
-    await self._get_config(session=session, debug_api=debug_api)
-
-    return self
-
-
-# %% ../../nbs/classes/50_DomoAccount.ipynb 22
-class DomoAccount_UpdateName_Error(de.DomoError):
-    def __init__(
-        self,
-        domo_instance,
-        status,
-        message,
-        entity_id,
-        function_name="update_name",
-    ):
-
-        super().__init__(
-            function_name=function_name,
-            entity_id=entity_id,
-            domo_instance=domo_instance,
-            status=status,
-            message=message,
-        )
-
-
-@patch_to(DomoAccount)
-async def update_name(
-    self: DomoAccount,
-    account_name: str = None,
-    auth: dmda.DomoAuth = None,
-    debug_api: bool = False,
-    session: httpx.AsyncClient = None,
-    return_raw: bool = False,
-):
-
-    auth = auth or self.auth
-
-    # print(auth, self.id, self.data_provider_type, self.config.to_json())
-
-    res = await account_routes.update_account_name(
-        auth=auth,
-        account_id=self.id,
-        account_name=account_name or self.name,
-        debug_api=debug_api,
-        session=session,
-    )
-
-    if return_raw:
-        return res
-
-    if not res.is_success:
-        raise DomoAccount_UpdateName_Error(
-            entity_id=self.id,
-            domo_instance=auth.domo_instance,
-            status=res.status,
-            message=res.response,
-        )
-
-    self = await self.get_from_id(auth=auth, account_id=self.id)
-
-    return self
-
-# %% ../../nbs/classes/50_DomoAccount.ipynb 26
-class DomoAccount_CreateAccount_Error(de.DomoError):
-    def __init__(
-        self,
-        entity_id,
-        domo_instance,
-        status,
-        message,
-        function_name="create_account",
-    ):
-
-        super().__init__(
-            function_name=function_name,
-            entity_id=entity_id,
-            domo_instance=domo_instance,
-            status=status,
-            message=message,
-        )
-
-# %% ../../nbs/classes/50_DomoAccount.ipynb 27
-@patch_to(DomoAccount, cls_method=True)
-def generate_create_body(cls, account_name, config):
-    return {
-        "displayName": account_name,
-        "dataProviderType": config.data_provider_type,
-        "name": config.data_provider_type,
-        "configurations": config.to_json(),
-    }
-
-
-@patch_to(DomoAccount, cls_method=True)
-async def create_account(
-    cls: DomoAccount,
-    account_name: str,
-    config: DomoAccount_Config,
-    auth: dmda.DomoAuth,
-    debug_api: bool = False,
-    session: httpx.AsyncClient = None,
-):
-
-    body = cls.generate_create_body(account_name=account_name, config=config)
-
-    res = await account_routes.create_account(
-        auth=auth, config_body=body, debug_api=debug_api, session=session
-    )
-
-    if not res.is_success:
-        raise DomoAccount_CreateAccount_Error(
-            entity_id=account_name,
-            domo_instance=auth.domo_instance,
-            status=res.status,
-            message=res.response,
-        )
-
-    return await cls.get_from_id(auth=auth, account_id=res.response.get("id"))
-
-# %% ../../nbs/classes/50_DomoAccount.ipynb 28
-class DomoAccount_DeleteAccount_Error(de.DomoError):
-    def __init__(
-        self,
-        entity_id,
-        domo_instance,
-        status,
-        message,
-        function_name="delete_account",
-    ):
-
-        super().__init__(
-            function_name=function_name,
-            entity_id=entity_id,
-            domo_instance=domo_instance,
-            status=status,
-            message=message,
-        )
-
-
-@patch_to(DomoAccount)
-async def delete_account(
-    self: DomoAccount,
-    auth: dmda.DomoAuth = None,
-    debug_api: bool = False,
-    session: httpx.AsyncClient = None,
-):
-
-    auth = auth or self.auth
-
-    res = await account_routes.delete_account(
-        auth=auth, account_id=self.id, debug_api=debug_api, session=session
-    )
-
-    if not res.is_success:
-
-        raise DomoAccount_DeleteAccount_Error(
-            entity_id=self.id,
-            domo_instance=auth.domo_instance,
-            status=res.status,
-            message=res.response,
-        )
-
-    return True
-
-# %% ../../nbs/classes/50_DomoAccount.ipynb 29
-class ShareAccount_AccessLevel(Enum):
-    "enumerates access levels for Domo Users and Domo Accounts"
-    CAN_VIEW = "CAN_VIEW"
-    CAN_EDIT = "CAN_EDIT" # only available with accounts_v2 feature switch (group ownership beta)
-    CAN_SHARE = "CAN_SHARE" # only available with accounts_v2 feature switch (group ownership beta)
-
-
-@patch_to(DomoAccount)
-async def share_account(
-    self,
-    auth: dmda.DomoAuth,
-    user_id: int,
-    is_v2: bool = False,
-    access_level: ShareAccount_AccessLevel = ShareAccount_AccessLevel.CAN_VIEW,
-    debug_api: bool = False,
-    session: httpx.AsyncClient = None,
-):
-    if is_v2:
-        share_payload = account_routes.generate_share_account_payload_v2(
-            user_id=user_id, access_level=access_level.value
-        )
-
-        return await account_routes.share_account_v2(
-            auth=auth,
-            account_id=self.id,
-            share_payload=share_payload,
-            debug_api=debug_api,
-            session=session,
-        )
-
-    share_payload = account_routes.generate_share_account_payload_v1(
-        user_id=user_id, access_level=access_level.value
-    )
-
-    return await account_routes.share_account_v1(
-        auth=auth,
-        account_id=self.id,
-        share_payload=share_payload,
-        debug_api=debug_api,
-        session=session,
-    )
-
-
-# %% ../../nbs/classes/50_DomoAccount.ipynb 31
-@dataclass
-class DomoAccounts:
-    auth: dmda.DomoAuth
+    if not cls._test_regex_mask(account_name, cls.account_name_mask):
+        raise InvalidAccountNameError(account_name = account_name, regex_pattern = cls.account_name_mask)
 
-# %% ../../nbs/classes/50_DomoAccount.ipynb 32
-@patch_to(DomoAccounts, cls_method=True)
-async def get_accounts(
-    cls: DomoAccounts,
-    auth: dmda.DomoAuth,
-    account_name: str = None, # account string to search for, must be an exact match in spelling.  case insensitive
-    account_type: AccountConfig = None, #to retrieve a specific account type
-    debug_api: bool = False,
-    session: httpx.AsyncClient = None,
-    return_raw: bool = False,
-):
+    account_properties, dj_account = get_jupyter_account(
+        account_name, domojupyter_fn=domojupyter_fn)
 
-    res = await account_routes.get_accounts(
-        auth=auth, debug_api=debug_api, session=session
+    if account_properties != ['credentials']:
+        raise InvalidAccountTypeError(
+            account_name=account_name, account_type="abstract_credential_store")
+
+    creds = json.loads(dj_account.get('credentials'))
+
+    return cls(
+        account_name=account_name,
+        raw_cred=creds,
+        domo_username=creds.get('DOMO_USERNAME'),
+        domo_password=creds.get('DOMO_PASSWORD'),
+        domo_access_token=creds.get('DOMO_ACCESS_TOKEN'),
+        domo_instance=domo_instance or creds.get('DOMO_INSTANCE')
     )
 
-    if return_raw:
-        return res
 
-    if not res.is_success:
-        return None
+# %% ../../nbs/integrations/DomoJupyter.ipynb 18
+class GenerateAuth_InvalidDomoInstanceList(Exception):
+    def __init__(self):
+        message = f"provide a list of domo_instances"
+        super().__init__(message)
+
+
+class GenerateAuth_CredentialsNotProvided(Exception):
+    def __init__(self):
+        message = f"object does not have a valid combination of credentials (access_token or username and password)"
+        super().__init__(message)
+
+
+@patch_to(DojoAccount_InstanceAuth)
+def _generate_auth(self, domo_instance):
+    if self.domo_access_token:
+            auth = dmda.DomoTokenAuth(
+                domo_instance=domo_instance, domo_access_token=self.domo_access_token)
+
+    elif self.domo_username and self.domo_password:
+
+        auth = dmda.DomoFullAuth(domo_instance=domo_instance,
+                                    domo_username=self.domo_username,
+                                    domo_password=self.domo_password)
+    
+    else:
+            raise GenerateAuth_CredentialsNotProvided()
+    
+    return auth
+
+@patch_to(DojoAccount_InstanceAuth)
+def generate_auth_ls(self : DojoAccount_InstanceAuth,
+                          domo_instance_ls: list[str] = None # list of domo_instances
+                          ) -> list[dmda.DomoAuth]: # list of domo auth objects
+                          
+    """for every domo_instance in domo_instance_ls generates an DomoAuth object"""
+
+    # reset internal lists
+    self.domo_instance = None
+
+    self.domo_instance_ls = list(
+        set(domo_instance_ls or self.domo_instance_ls))
+
+    if not self.domo_instance_ls:
+        raise GenerateAuth_InvalidDomoInstanceList()
+
+    self.auth_ls = []
+    for domo_instance in self.domo_instance_ls:
+        auth = self._generate_auth(domo_instance)
 
-    domo_account_ls = [
-        DomoAccount._from_json(account_obj, auth=auth) for account_obj in res.response
-    ]
-
-    if not account_name and not account_type:
-        return domo_account_ls
-
-    filtered_account_ls = domo_account_ls
-    if account_name:
-        filtered_account_ls = [
-            domo_account
-            for domo_account in filtered_account_ls
-            if domo_account.name.lower() == account_name.lower()
-        ]
-
-    if account_type:
-        filtered_account_ls = [
-            domo_account
-            for domo_account in filtered_account_ls
-            if domo_account.data_provider_type == account_type.value.data_provider_type
-        ]
+        self.auth_ls.append(auth)
 
-    return filtered_account_ls
+    return self.auth_ls
```

### Comparing `domolibrary-0.0.81/domolibrary/classes/DomoActivityLog.py` & `domolibrary-0.0.9/domolibrary/classes/DomoActivityLog.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.81/domolibrary/classes/DomoBootstrap.py` & `domolibrary-0.0.9/domolibrary/classes/DomoBootstrap.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.81/domolibrary/classes/DomoDataset.py` & `domolibrary-0.0.9/domolibrary/classes/DomoDataset.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/classes/50_DomoDataset.ipynb.
 
 # %% auto 0
-__all__ = ['DatasetSchema_Types', 'DomoDataset_Schema_Column', 'DomoDataset_Schema', 'DatasetTags_SetTagsError',
-           'DomoDataset_Tags', 'DomoDataset', 'QueryExecutionError', 'DomoDataset_DeleteDataset_Error',
-           'DomoDataset_UploadData_Error', 'DomoDataset_UploadData_DatasetUploadId_Error',
-           'DomoDataset_UploadData_UploadData_Error', 'DomoDataset_UploadData_CommitDatasetUploadId_Error',
+__all__ = ['DatasetSchema_Types', 'DatasetSchema_AuthNotProvidedError', 'DatasetSchema_DatasetNotProvidedError',
+           'DomoDataset_Schema_Column', 'DomoDataset_Schema', 'DatasetTags_AuthNotProvidedError',
+           'DatasetTags_SetTagsError', 'DomoDataset_Tags', 'DomoDataset', 'QueryExecutionError',
+           'DomoDataset_DeleteDataset_Error', 'DomoDataset_UploadData_Error',
+           'DomoDataset_UploadData_DatasetUploadId_Error', 'DomoDataset_UploadData_UploadData_Error',
            'DomoDataset_CreateDataset_Error']
 
 # %% ../../nbs/classes/50_DomoDataset.ipynb 4
 from fastcore.basics import patch_to
 import pandas as pd
 
 # %% ../../nbs/classes/50_DomoDataset.ipynb 5
 from dataclasses import dataclass, field
-from typing import List, Optional
-from enum import Enum
+from typing import Any, List, Optional
+from enum import Enum, auto
 
 import json
 import io
 
 import httpx
 import asyncio
 
@@ -27,65 +28,51 @@
 
 # import importlib
 # import json
 # from pprint import pprint
 
 # import pandas as pd
 
-
+# from ..utils import Exceptions as ex
 # from ..utils.Base import Base
 # from ..utils.chunk_execution import chunk_list
 # from . import DomoCertification as dmdc
 # from . import DomoPDP as dmpdp
 # from . import DomoTag as dmtg
 
 
 import domolibrary.utils.DictDot as util_dd
 import domolibrary.client.DomoAuth as dmda
-import domolibrary.client.DomoError as de
 import domolibrary.routes.dataset as dataset_routes
 
 # %% ../../nbs/classes/50_DomoDataset.ipynb 7
-async def _have_prereqs(self, auth, dataset_id, function_name):
-    """tests if have a parent dataset or prerequsite dataset_id and auth object"""
-
-    auth_from_self_dataset = getattr(self.dataset, 'auth', None) if getattr(self, 'dataset', None) else None
-    auth_from_self = getattr(self , 'auth', None)
-
-    auth = auth or auth_from_self or auth_from_self_dataset
-
-    await auth.get_auth_token()
-
-    if not auth or not auth.token:
-        raise de.AuthNotProvidedError(
-            function_name=function_name,
-            entity_id = self.dataset.id)
-
-    id_from_self = getattr(self, 'id', None)
-    id_from_self_parent = getattr(self.dataset, 'id', None ) if getattr(self, 'dataset', None) else None
-    
-    dataset_id = dataset_id or id_from_self or id_from_self_parent
-    
-    if not dataset_id:
-        raise de.DatasetNotProvidedError(
-            function_name = function_name, 
-            domo_instance = auth.domo_instance
-        )
-
-    return auth, dataset_id
-
-# %% ../../nbs/classes/50_DomoDataset.ipynb 8
 class DatasetSchema_Types(Enum):
     STRING = 'STRING'
     DOUBLE = 'DOUBLE'
     LONG = 'LONG'
     DATE = 'DATE'
     DATETIME = 'DATETIME'
 
 
+class DatasetSchema_AuthNotProvidedError(Exception):
+    """return if DatasetSchema request cannot access an auth object"""
+
+    def __init__(self, dataset_id):
+        message = f"valid Auth object not provided to dataset - {dataset_id}"
+        super().__init__(message)
+
+
+class DatasetSchema_DatasetNotProvidedError(Exception):
+    """return if DatasetSchema request does not have a dataset id"""
+
+    def __init__(self):
+        message = f"dataset_id not provided"
+        super().__init__(message)
+
+
 @dataclass
 class DomoDataset_Schema_Column:
     name: str
     id: str
     type: DatasetSchema_Types
 
     @classmethod
@@ -107,15 +94,23 @@
         dataset_id: str = None,
         debug_api: bool = False,
         return_raw_res: bool = False,  # return the raw response
     ) -> List[DomoDataset_Schema_Column]:
 
         """method that retrieves schema for a dataset"""
 
-        auth, dataset_id = await _have_prereqs(self = self, auth = auth, dataset_id = dataset_id, function_name = "DomoDataset_Schema.get")
+        if self.dataset and (not self.dataset.auth and not auth):
+            raise DatasetSchema_AuthNotProvidedError(dataset_id = self.dataset.id)
+
+        auth = auth or self.dataset.auth
+
+        if not self.dataset and not dataset_id:
+            raise DatasetSchema_DatasetNotProvidedError()
+
+        dataset_id = dataset_id or self.dataset.id
 
         res = await dataset_routes.get_schema(
             auth=auth, dataset_id=dataset_id, debug_api=debug_api
         )
 
         if return_raw_res:
             return res.response
@@ -126,16 +121,23 @@
             self.columns = [
                 DomoDataset_Schema_Column._from_json(json_obj=json_obj)
                 for json_obj in json_list
             ]
 
             return self.columns
 
+# %% ../../nbs/classes/50_DomoDataset.ipynb 12
+class DatasetTags_AuthNotProvidedError(Exception):
+    """return if DatasetTags request cannot access an auth object"""
+
+    def __init__(self, dataset_id):
+        message = f"valid Auth object not provided to dataset - {dataset_id}"
+        super().__init__(message)
+
 
-# %% ../../nbs/classes/50_DomoDataset.ipynb 13
 class DatasetTags_SetTagsError(Exception):
     """return if DatasetTags request is not successfull"""
 
     def __init__(self, dataset_id, domo_instance):
         message = f"failed to set tags on dataset - {dataset_id} in {domo_instance}"
         super().__init__(message)
 
@@ -143,53 +145,65 @@
 @dataclass
 class DomoDataset_Tags:
     """class for interacting with dataset tags"""
 
     dataset: any = None
     tag_ls: List[str] = field(default_factory=list)
 
+    def _have_prereqs(self, auth, dataset_id):
+        """tests if have a parent dataset or prerequsite dataset_id and auth object"""
+
+        if self.dataset and (not self.dataset.auth and not auth):
+            raise DatasetTags_AuthNotProvidedError(self.dataset.id)
+
+        auth = auth or self.dataset.auth
+
+        if not self.dataset and not auth:
+            raise DatasetTags_AuthNotProvidedError(self.dataset.id)
+
+        dataset_id = dataset_id or self.dataset.id
+
+        return auth, dataset_id
+
     async def get(
         self,
         dataset_id: str = None,
         auth: Optional[dmda.DomoAuth] = None,
         debug_api: bool = False,
         session: Optional[httpx.AsyncClient] = None,
     ) -> List[str]:  # returns a list of tags
         """gets the existing list of dataset_tags"""
 
-        auth, dataset_id = await _have_prereqs(self = self, auth=auth, dataset_id=dataset_id, function_name="DomoDataset_Tages.get")
+        auth, dataset_id = self._have_prereqs(auth=auth, dataset_id=dataset_id)
 
         res = await dataset_routes.get_dataset_by_id(
             dataset_id=dataset_id, auth=auth, debug_api=debug_api, session=session
         )
 
         if res.is_success == False:
             print(res)
             return None
 
-        tag_ls = []
-
-        if res.response.get("tags"):
+        if res.is_success == True:
             tag_ls = json.loads(res.response.get("tags"))
-        
-        self.tag_ls = tag_ls
+            self.tag_ls = tag_ls
 
-        return tag_ls
+            return tag_ls
 
     async def set(
         self,
         tag_ls: [str],
         dataset_id: str = None,
         auth: Optional[dmda.DomoAuth] = None,
         debug_api: bool = False,
         session: Optional[httpx.AsyncClient] = None,
     ) -> List[str]: # returns a list of tags
         """replaces all tags with a new list of dataset_tags"""
 
-        auth, dataset_id = await _have_prereqs(self = self , auth=auth, dataset_id=dataset_id, function_name="DomoDatasetTags.set")
+        auth, dataset_id = self._have_prereqs(auth=auth, dataset_id=dataset_id)
 
         res = await dataset_routes.set_dataset_tags(
             auth=auth,
             tag_ls=list(set(tag_ls)),
             dataset_id=dataset_id,
             debug_api=debug_api,
             session=session,
@@ -200,65 +214,65 @@
                 dataset_id=dataset_id, domo_instance=auth.domo_instance
             )
 
         await self.get(dataset_id=dataset_id, auth=auth)
 
         return self.tag_ls
 
-# %% ../../nbs/classes/50_DomoDataset.ipynb 16
+# %% ../../nbs/classes/50_DomoDataset.ipynb 15
 @patch_to(DomoDataset_Tags)
 async def add(
     self: DomoDataset_Tags,
     add_tag_ls: [str],
     dataset_id: str = None,
     auth: Optional[dmda.DomoAuth] = None,
     debug_api: bool = False,
     session: Optional[httpx.AsyncClient] = None,
 ) -> List[str]:  # returns a list of tags
     """appends tags to the list of existing dataset_tags"""
 
-    auth, dataset_id = await _have_prereqs(self = self, auth=auth, dataset_id=dataset_id, function_name = "DomoDataset_Tags.add")
+    auth, dataset_id = self._have_prereqs(auth=auth, dataset_id=dataset_id)
 
-    existing_tag_ls = await self.get(dataset_id=dataset_id, auth=auth) or []
+    existing_tag_ls = await self.get(dataset_id=dataset_id, auth=auth)
     
     add_tag_ls += existing_tag_ls
 
     return await self.set(
         auth=auth,
         dataset_id=dataset_id,
         tag_ls=list(set(add_tag_ls)),
         debug_api=debug_api,
         session=session,
     )
 
-# %% ../../nbs/classes/50_DomoDataset.ipynb 18
+# %% ../../nbs/classes/50_DomoDataset.ipynb 17
 @patch_to(DomoDataset_Tags)
 async def remove(self: DomoDataset_Tags,
                  remove_tag_ls: [str],
                  dataset_id: str = None,
                  auth: dmda.DomoFullAuth = None,
                  debug_api: bool = False,
                  session: Optional[httpx.AsyncClient] = None
                  ) -> List[str]:  # returns a list of tags
     """removes tags from the existing list of dataset_tags"""
 
-    auth, dataset_id = await _have_prereqs(self = self, auth=auth, dataset_id=dataset_id, function_name = "DomoDataset_Tags.remove")
+    auth, dataset_id = self._have_prereqs(auth=auth, dataset_id=dataset_id)
 
     existing_tag_ls = await self.get(dataset_id=dataset_id, auth=auth)
 
     existing_tag_ls = [
         ex for ex in existing_tag_ls if ex not in remove_tag_ls]
 
     return await self.set(auth=auth,
                           dataset_id=dataset_id,
                           tag_ls=list(set(existing_tag_ls)),
                           debug_api=debug_api, session=session)
 
 
-# %% ../../nbs/classes/50_DomoDataset.ipynb 22
+# %% ../../nbs/classes/50_DomoDataset.ipynb 21
 @dataclass
 class DomoDataset:
     "interacts with domo datasets"
 
     auth: dmda.DomoAuth = field(repr=False, default=None)
 
     id: str = ""
@@ -271,174 +285,140 @@
 
     stream_id: int = None
 
     owner: dict = field(default_factory=dict)
     formula: dict = field(default_factory=dict)
 
     schema: DomoDataset_Schema = field(default=None)
-    tags: DomoDataset_Tags = field(default=None)
+    # tags: Dataset_Tags = field(default = None)
 
     # certification: dmdc.DomoCertification = None
     # PDPPolicies: dmpdp.Dataset_PDP_Policies = None
 
     def __post_init__(self):
         self.schema = DomoDataset_Schema(dataset=self)
-        self.tags = DomoDataset_Tags(dataset=self)
+        # self.tags = Dataset_Tags(dataset=self)
 
-        # self.PDPPolicies = dmpdp.Dataset_PDP_Policies(dataset=self)
+        # self.PDPPolicies = dmpdp.Dataset_PDP_Policies(self)
 
     def display_url(self):
         return f"https://{self.auth.domo_instance }.domo.com/datasources/{self.id}/details/overview"
 
-# %% ../../nbs/classes/50_DomoDataset.ipynb 26
+# %% ../../nbs/classes/50_DomoDataset.ipynb 25
 @patch_to(DomoDataset, cls_method=True)
 async def get_from_id(
     cls: DomoDataset,
     dataset_id: str,
     auth: dmda.DomoAuth,
     debug_api: bool = False,
     return_raw_res: bool = False,
-    session : httpx.AsyncClient = None,
 ):
 
     """retrieves dataset metadata"""
 
     res = await dataset_routes.get_dataset_by_id(
-        auth=auth, dataset_id=dataset_id, debug_api=debug_api, session = session
+        auth=auth, dataset_id=dataset_id, debug_api=debug_api
     )
 
     if return_raw_res:
         return res.response
 
     dd = util_dd.DictDot(res.response)
     ds = cls(
         auth=auth,
         id=dd.id,
         display_type=dd.displayType,
         data_provider_type=dd.dataProviderType,
         name=dd.name,
         description=dd.description,
-        owner=res.response.get('owner'),
+        owner=dd.owner,
+        formula=dd.properties.formulas.formulas,
         stream_id=dd.streamId,
         row_count=int(dd.rowCount),
         column_count=int(dd.columnCount),
     )
-    
-    if dd.properties.formulas.formulas.__dict__ :
-        # print(dd.properties.formulas.formulas.__dict__)
-        ds.formula=res.response.get('properties').get('formulas').get('formulas')
 
-    if dd.tags:
-        ds.tags.tag_ls = json.loads(dd.tags)
+    # if dd.tags:
+    #     ds.tags.tag_ls = json.loads(dd.tags)
 
     # if dd.certification:
     #     # print('class def certification', dd.certification)
     #     ds.certification = dmdc.DomoCertification._from_json(
     #         dd.certification)
 
     return ds
 
 
-# %% ../../nbs/classes/50_DomoDataset.ipynb 30
-class QueryExecutionError(de.DomoError):
-    def __init__(self,
-                 sql, dataset_id,
-                 domo_instance,
-                 status, message,
-                 function_name=None ):
-        
-        self.message = f"error executing {sql}: {message}"
-
-        super().__init__(entity_id=dataset_id,
-                         function_name=function_name,
-                         status=status,
-                         message=message,
-                         domo_instance=domo_instance)
+# %% ../../nbs/classes/50_DomoDataset.ipynb 29
+class QueryExecutionError(Exception):
+    def __init__(self, sql, dataset_id, domo_instance):
+        self.message = f"error executing {sql} against dataset {dataset_id} in {domo_instance}"
+        super().__init__(self, self.message)
 
 
 @patch_to(DomoDataset, cls_method=True)
 async def query_dataset_private(cls: DomoDataset,
                                 auth: dmda.DomoAuth,  # DomoFullAuth or DomoTokenAuth
                                 dataset_id: str,
                                 sql: str,
                                 session: Optional[httpx.AsyncClient] = None,
                                 loop_until_end: bool = False,  # retrieve all available rows
                                 limit=100,  # maximum rows to return per request.  refers to PAGINATION
                                 skip=0,
                                 maximum=100,  # equivalent to the LIMIT or TOP clause in SQL, the number of rows to return total
                                 debug_api: bool = False,
                                 debug_loop: bool = False,
-                                timeout = 10 # larger API requests may require a longer response time
                                 ) -> pd.DataFrame:
 
     res = await dataset_routes.query_dataset_private(auth=auth,
                                                      dataset_id=dataset_id,
                                                      sql=sql,
                                                      maximum=maximum,
                                                      skip=skip,
                                                      limit=limit,
                                                      loop_until_end=loop_until_end,
                                                      session=session,
                                                      debug_loop=debug_loop,
-                                                     debug_api=debug_api,
-                                                     timeout = timeout
+                                                     debug_api=debug_api
                                                      )
 
     if not res.is_success:
-        raise QueryExecutionError(
-            status=res.status, message=res.response,
-            function_name="query_dataset_private", 
-            sql=sql, dataset_id=dataset_id, domo_instance=auth.domo_instance)
+        raise QueryExecutionError(sql=sql, dataset_id=dataset_id, domo_instance=auth.domo_instance)
 
     return pd.DataFrame(res.response)
 
 
-# %% ../../nbs/classes/50_DomoDataset.ipynb 31
-class DomoDataset_DeleteDataset_Error(de.DomoError):
-    def __init__(self,
-                 dataset_id,
-                 status, reason,
-                 domo_instance,
-                 function_name
-                 ):
-
-        super().__init__(entity_id=dataset_id,
-                         function_name=function_name,
-                         status=status,
-                         message=reason,
-                         domo_instance=domo_instance)
-
+# %% ../../nbs/classes/50_DomoDataset.ipynb 30
+class DomoDataset_DeleteDataset_Error(Exception):
+    def __init__(self, status, reason, dataset_id, domo_instance):
+        message = f"Error deleting {dataset_id} from {domo_instance}: {status} - {reason}"
+        super().__init__(message)
 
 @patch_to(DomoDataset)
-async def delete(self: DomoDataset,
-                 dataset_id=None,
-                 auth: dmda.DomoAuth = None,
-                 debug_api: bool = False,
-                 session: httpx.AsyncClient = None):
+async def delete(self : DomoDataset,
+                    dataset_id=None,
+                    auth: dmda.DomoAuth = None,
+                    debug_api: bool = False,
+                    session: httpx.AsyncClient = None):
 
     dataset_id = dataset_id or self.id
     auth = auth or self.auth
 
     res = await dataset_routes.delete(
         auth=auth,
         dataset_id=dataset_id,
         debug_api=debug_api,
         session=session)
 
     if not res.is_success:
-        raise DomoDataset_DeleteDataset_Error(
-            dataset_id=dataset_id, 
-            function_name="DomoDataset.delete",
-            domo_instance=auth.domo_instance, 
-            status=res.status, reason=res.response)
-
+        raise DomoDataset_DeleteDataset_Error(domo_instance = auth.domo_instance, dataset_id = dataset_id, status = res.status, reason = res.response )
+    
     return res
 
-
-# %% ../../nbs/classes/50_DomoDataset.ipynb 34
+# %% ../../nbs/classes/50_DomoDataset.ipynb 33
 class DomoDataset_UploadData_Error(Exception):
 
     def __init__(self,
                  message_error: str,
                  domo_instance: str,
                  dataset_id: str,
                  stage: int,
@@ -478,43 +458,43 @@
         message_error = "while uploading data"
 
         super().__init__(message_error=message_error,
                          domo_instance=domo_instance, dataset_id=dataset_id,
                          stage=stage, status=status, reason=reason,
                          partition_key=partition_key)
 
-class DomoDataset_UploadData_CommitDatasetUploadId_Error(DomoDataset_UploadData_Error):
-    def __init__(self, domo_instance: str, dataset_id: str,
-                    stage: int = 3, status="", reason="",
-                    partition_key: str = None):
-
-        message_error = "while commiting dataset_upload_id"
-
-        super().__init__(message_error=message_error,
-                            domo_instance=domo_instance, dataset_id=dataset_id,
-                            stage=stage, status=status, reason=reason,
-                            partition_key=partition_key)
+    class DomoDataset_UploadData_DatasetUploadId_Error(DomoDataset_UploadData_Error):
+        def __init__(self, domo_instance: str, dataset_id: str,
+                     stage: int = 3, status="", reason="",
+                     partition_key: str = None):
+
+            message_error = "while commiting dataset_upload_id"
+
+            super().__init__(message_error=message_error,
+                              domo_instance=domo_instance, dataset_id=dataset_id,
+                              stage=stage, status=status, reason=reason,
+                              partition_key=partition_key)
 
 
-# %% ../../nbs/classes/50_DomoDataset.ipynb 35
+# %% ../../nbs/classes/50_DomoDataset.ipynb 34
 @patch_to(DomoDataset)
 async def index_dataset(self: DomoDataset,
                         auth: dmda.DomoAuth = None,
                         dataset_id: str = None,
                         debug_api: bool = False,
                         session: httpx.AsyncClient = None
                         ):
 
     auth = auth or self.auth
     dataset_id = dataset_id or self.id
     return await dataset_routes.index_dataset(auth=auth, dataset_id=dataset_id, debug_api=debug_api,
                                               session=session)
 
 
-# %% ../../nbs/classes/50_DomoDataset.ipynb 36
+# %% ../../nbs/classes/50_DomoDataset.ipynb 35
 @patch_to(DomoDataset)
 async def upload_data(self : DomoDataset,
                       upload_df: pd.DataFrame = None,
                       upload_df_ls: list[pd.DataFrame] = None,
                       upload_file: io.TextIOWrapper = None,
 
                       upload_method: str = 'REPLACE',  # APPEND or REPLACE
@@ -528,78 +508,77 @@
                       auth: dmda.DomoAuth = None,
 
                       session: httpx.AsyncClient = None,
                       debug_api: bool = False,
                       debug_prn: bool = False
                       ):
 
-    auth, dataset_id = await _have_prereqs(self = self, auth = auth, dataset_id=dataset_id, function_name= "upload_data")
+    auth = auth or self.auth
+    dataset_id = dataset_id or self.id
 
     upload_df_ls = upload_df_ls or [upload_df]
 
-    status_message = f"{dataset_id} {partition_key} | {auth.domo_instance}"
-
     # stage 1 get uploadId
     if not dataset_upload_id:
         if debug_prn:
-            print(f"\n\n🎭 starting Stage 1 - {status_message}")
+            print(f"\n\n🎭 starting Stage 1")
 
         stage_1_res = await dataset_routes.upload_dataset_stage_1(auth=auth,
                                                                   dataset_id=dataset_id,
                                                                   session=session,
                                                                   partition_tag=partition_key,
                                                                   debug_api=debug_api
                                                                   )
         if debug_prn:
-            print(f"\n\n🎭 Stage 1 response -- {stage_1_res.status} for {status_message}")
+            print(f"\n\n🎭 Stage 1 response -- {stage_1_res.status}")
 
         dataset_upload_id = stage_1_res.response.get('uploadId')
 
     if not dataset_upload_id:
         raise DomoDataset_UploadData_DatasetUploadId_Error(
             domo_instance=auth.domo_instance,  dataset_id=dataset_id, stage=1, partition_key=partition_key,
             status=stage_1_res.status, reason=stage_1_res.response)
 
     # stage 2 upload_dataset
     stage_2_res = None
 
     if upload_file:
         if debug_prn:
-            print(f"\n\n🎭 starting Stage 2 - upload file for {status_message}")
+            print(f"\n\n🎭 starting Stage 2 - upload file")
 
         stage_2_res = await asyncio.gather(*[dataset_routes.upload_dataset_stage_2_file(auth=auth,
                                                                                         dataset_id=dataset_id,
                                                                                         upload_id=dataset_upload_id,
                                                                                         part_id=1,
                                                                                         data_file=upload_file,
                                                                                         session=session, debug_api=debug_api)])
 
     else:
         if debug_prn:
             print(
-                f"\n\n🎭 starting Stage 2 - {len(upload_df_ls)} - number of parts for {status_message}")
+                f"\n\n🎭 starting Stage 2 - {len(upload_df_ls)} - number of parts")
         stage_2_res = await asyncio.gather(*[dataset_routes.upload_dataset_stage_2_df(auth=auth,
                                                                                       dataset_id=dataset_id,
                                                                                       upload_id=dataset_upload_id,
                                                                                       part_id=index + 1,
                                                                                       upload_df=df,
                                                                                       session=session, debug_api=debug_api) for index, df in enumerate(upload_df_ls)])
 
     for res in stage_2_res:
         if not res.is_success:
             raise DomoDataset_UploadData_UploadData_Error(
                 domo_instance=auth.domo_instance, dataset_id=dataset_id, stage=2, partition_key=partition_key,
                 status=res.status, reason=res.response)
 
     if debug_prn:
-        print(f"🎭 Stage 2 - upload data: complete for {status_message}")
+        print(f"🎭 Stage 2 - upload data: complete")
 
     # stage 3 commit_data
     if debug_prn:
-        print(f"\n\n🎭 starting Stage 3 - commit dataset_upload_id for {status_message}")
+        print(f"\n\n🎭 starting Stage 3 - commit dataset_upload_id")
 
     await asyncio.sleep(10)  # wait for uploads to finish
     stage3_res = await dataset_routes.upload_dataset_stage_3(auth=auth,
                                                              dataset_id=dataset_id,
                                                              upload_id=dataset_upload_id,
                                                              update_method=upload_method,
                                                              partition_tag=partition_key,
@@ -609,27 +588,27 @@
 
     if not stage3_res.is_success:
         raise DomoDataset_UploadData_CommitDatasetUploadId_Error(
             domo_instance=auth.domo_instance, dataset_id=dataset_id, partition_key=partition_key, stage=3,
             status=stage3_res.status, reason=stage3_res.response)
 
     if debug_prn:
-        print(f"\n🎭 stage 3 - commit dataset: complete for {status_message} ")
+        print(f"\n🎭 stage 3 - commit dataset: complete")
 
     if is_index:
         await asyncio.sleep(3)
         return await self.index_dataset(auth=auth,
                                         dataset_id=dataset_id,
                                         debug_api=debug_api,
                                         session=session)
 
     return stage3_res
 
 
-# %% ../../nbs/classes/50_DomoDataset.ipynb 38
+# %% ../../nbs/classes/50_DomoDataset.ipynb 37
 @patch_to(DomoDataset)
 async def list_partitions(self : DomoDataset,
                             auth: dmda.DomoAuth = None,
                             dataset_id: str = None,
                             debug_api: bool = False,
                             session: httpx.AsyncClient = None
                             ):
@@ -640,35 +619,33 @@
     res = await dataset_routes.list_partitions(auth=auth, dataset_id=dataset_id, debug_api=debug_api,
                                                 session=session)
     if res.status != 200:
         return None
 
     return res.response
 
-# %% ../../nbs/classes/50_DomoDataset.ipynb 40
+# %% ../../nbs/classes/50_DomoDataset.ipynb 39
 class DomoDataset_CreateDataset_Error(Exception):
     def __init__(self, domo_instance: str, dataset_name: str, status: int, reason: str):
         message = f"Failure to create dataset {dataset_name} in {domo_instance} :: {status} - {reason}"
-        super().__init__(message)
 
 
 @patch_to(DomoDataset, cls_method=True)
 async def create(cls: DomoDataset,
                  dataset_name: str,
                  dataset_type='api',
 
-                 schema=None,
+                 schema={"columns": [
+                     {"name": 'col1', "type": 'LONG', "upsertKey": False},
+                     {"name": 'col2', "type": 'STRING', "upsertKey": False}
+                 ]},
                  auth: dmda.DomoAuth = None,
                  debug_api: bool = False, 
                  session : httpx.AsyncClient = None
                  ):
-    schema = schema or {"columns": [
-        {"name": 'col1', "type": 'LONG', "upsertKey": False},
-        {"name": 'col2', "type": 'STRING', "upsertKey": False}
-    ]}
     
 
     res = await dataset_routes.create(dataset_name=dataset_name,
                                       dataset_type=dataset_type,
                                       schema=schema, auth=auth, debug_api=debug_api, session=session
                                       )
```

### Comparing `domolibrary-0.0.81/domolibrary/classes/DomoPage.py` & `domolibrary-0.0.9/domolibrary/classes/DomoPage.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/classes/50_DomoPage.ipynb.
 
 # %% auto 0
 __all__ = ['DomoPage']
 
 # %% ../../nbs/classes/50_DomoPage.ipynb 2
 from fastcore.basics import patch_to
+
+# %% ../../nbs/classes/50_DomoPage.ipynb 3
 from dataclasses import dataclass, field
 
-import asyncio
-import httpx
+# import asyncio
+# import httpx
 
 import domolibrary.client.DomoAuth as dmda
 import domolibrary.classes.DomoUser as dmdu
 import domolibrary.utils.DictDot as util_dd
 
-import domolibrary.routes.page as page_routes
-
+# from .routes import page_routes
+# from ..utils.Base import Base
 
-# %% ../../nbs/classes/50_DomoPage.ipynb 3
+# %% ../../nbs/classes/50_DomoPage.ipynb 4
 @dataclass
 class DomoPage:
     id: str
     title: str = None
     parent_page_id: str = None
     auth: dmda.DomoAuth = field(default = None , repr = False)
     owners: list = field(default_factory=list)
     cards: list = field(default_factory=list)
     collections: list = field(default_factory=list)
     children: list = field(default_factory=list)
 
     def display_url(self):
         return f"https://{self.auth.domo_instance}.domo.com/page/{self.id}"
 
-# %% ../../nbs/classes/50_DomoPage.ipynb 4
+# %% ../../nbs/classes/50_DomoPage.ipynb 5
 @patch_to(DomoPage, cls_method=True)
 def _from_bootstrap(cls: DomoPage, page_obj, auth: dmda.DomoAuth = None):
 
     dd = page_obj
     if isinstance(page_obj, dict):
         dd = util_dd.DictDot(page_obj)
 
@@ -62,72 +64,11 @@
         [print(other_dd) for other_dd in dd.children
             if other_dd.type != "page"]
 
     return domo_page
 
 
 # %% ../../nbs/classes/50_DomoPage.ipynb 7
-@patch_to(DomoPage, cls_method=True)
-async def _from_content_stacks_v3(cls: DomoPage, page_obj, auth: dmda.DomoAuth = None):
-    # import domolibrary.classes.DomoCard as dc
-
-    dd = page_obj
-    if isinstance(page_obj, dict):
-        dd = util_dd.DictDot(page_obj)
-
-    pg = cls(
-        id=dd.id,
-        title=dd.title,
-        parent_page_id=dd.page.parentPageId,
-        owners=dd.page.owners,
-        collections=dd.collections,
-        auth=auth
-    )
-
-    # if dd.cards and len(dd.cards) > 0:
-    #     pg.cards = await asyncio.gather(
-    #         *[dc.DomoCard.get_from_id(id=card.id, auth=auth) for card in dd.cards])
-
-    return pg
-
-
-@patch_to(DomoPage, cls_method=True)
-async def get_by_id(cls: DomoPage,
-                    page_id: str,
-                    auth: dmda.DomoAuth,
-                    return_raw: bool = False, 
-                    debug_api: bool = False):
-
-    res = await page_routes.get_page_by_id(auth=auth, page_id=page_id, debug_api=debug_api)
-
-    if return_raw:
-        return res
-        
-    if not res.status == 200:
-        return
-
-    pg = await cls._from_content_stacks_v3(page_obj=res.response, auth=auth)
-
-    return pg
-
-
-# %% ../../nbs/classes/50_DomoPage.ipynb 10
 @patch_to(DomoPage)
-async def get_accesslist(self,
-                         auth: dmda.DomoAuth = None,
-                         return_raw: bool = False,
-                         debug_api: bool = False):
-
-    auth = auth or self.auth
-
-    res = await page_routes.get_page_accesslist(auth=auth,
-                                                page_id=self.id, 
-                                                debug_api=debug_api
-                                                )
-    
-    if return_raw:
-        return res
-
-    import domolibrary.classes.DomoUser as dmu
-    
-    return res
+def _ol_fn():
+    pass
```

### Comparing `domolibrary-0.0.81/domolibrary/classes/DomoUser.py` & `domolibrary-0.0.9/domolibrary/classes/DomoUser.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,68 +1,50 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/classes/50_DomoUser.ipynb.
 
 # %% auto 0
-__all__ = ['DomoUser', 'DomoUsers', 'CreateUser_MissingRole']
+__all__ = ['DomoUser', 'DomoUsers']
 
 # %% ../../nbs/classes/50_DomoUser.ipynb 3
-from fastcore.basics import patch_to
-
+from fastcore.basics import patch, patch_to
 
 # %% ../../nbs/classes/50_DomoUser.ipynb 4
-import datetime as dt
 from dataclasses import dataclass, field
-from typing import Optional
-import httpx
-
-from pprint import pprint
+from typing import List, Optional
 
 import domolibrary.utils.DictDot as util_dd
 import domolibrary.client.DomoAuth as dmda
 import domolibrary.client.Logger as lc
-import domolibrary.client.DomoError as de
 import domolibrary.routes.user as user_routes
 
+
 # %% ../../nbs/classes/50_DomoUser.ipynb 6
 @dataclass
 class DomoUser:
     """a class for interacting with a Domo User"""
 
     id: str
-    title: str = None
-    department: str = None
     display_name: str = None
     email_address: str = None
     role_id: str = None
 
     publisher_domain: str = None
     subscriber_domain: str = None
     virtual_user_id: str = None
 
     auth: Optional[dmda.DomoAuth] = field(repr=False, default=None)
 
-    def __post_init__(self):
-        self.id = str(self.id)
-
-    def __eq__(self, other):
-        if not isinstance(other, DomoUser):
-            return False
-        
-        return self.id == other.id
-
     @classmethod
     def _from_search_json(cls, auth, user_obj):
         user_dd = util_dd.DictDot(user_obj)
 
         return cls(
             auth=auth,
-            id=str(user_dd.id or user_dd.userId),
+            id=str(user_dd.id) or str(user_dd.userId),
             display_name=user_dd.displayName,
-            title = user_dd.title,
-            department = user_dd.department,
-            email_address=user_dd.emailAddress or user_dd.email,
+            email_address=user_dd.emailAddress,
             role_id=user_dd.roleId,
         )
 
     @classmethod
     def _from_virtual_json(cls, auth, user_obj):
         user_dd = util_dd.DictDot(user_obj)
 
@@ -74,18 +56,22 @@
             virtual_user_id=user_dd.virtualUserId,
         )
 
     @classmethod
     def _from_bootstrap_json(cls, auth, user_obj):
 
         dd = user_obj
-        if isinstance(user_obj, dict):
+        if isinstance( user_obj, dict):
             dd = util_dd.DictDot(user_obj)
 
-        return cls(id=dd.id, display_name=dd.displayName, auth=auth)
+
+        return cls(
+            id = dd.id,
+            display_name = dd.displayName
+        )
 
 # %% ../../nbs/classes/50_DomoUser.ipynb 8
 @patch_to(DomoUser)
 async def reset_password(self: DomoUser, new_password: str, debug_api: bool = False):
     """reset your password, will respect password restrictions set up in the Domo UI"""
 
     res = await user_routes.reset_password(
@@ -93,125 +79,180 @@
     )
 
     return res
 
 # %% ../../nbs/classes/50_DomoUser.ipynb 9
 @patch_to(DomoUser, cls_method=True)
 async def request_password_reset(
-    cls,
-    domo_instance: str,
-    email: str,
-    locale: str = "en-us",
-    debug_api: bool = False,
-    session: httpx.AsyncClient = None,
+    cls, domo_instance: str, email: str, locale: str = "en-us", debug_api: bool = False
 ):
     """request password reset email.  Note: does not require authentication."""
 
     return await user_routes.request_password_reset(
-        domo_instance=domo_instance,
+        domo_instance=domo_instance, email=email, locale=locale, debug_api=debug_api
+    )
+
+# %% ../../nbs/classes/50_DomoUser.ipynb 10
+@patch_to(DomoUser, cls_method=True)
+async def create_user(
+    cls: DomoUser,
+    auth: dmda.DomoAuth,
+    display_name,
+    email,
+    role_id,
+    password: str = None,
+    send_password_reset_email: bool = False,
+    debug: bool = False,
+    log_results: bool = False,
+):
+    """class method that creates a new Domo user"""
+
+    res = await user_routes.create_user(
+        full_auth=full_auth,
+        display_name=display_name,
         email=email,
-        locale=locale,
+        role_id=role_id,
+        debug=debug,
+        log_results=log_results,
+    )
+
+    if debug:
+        print(res)
+
+    if res.status != 200:
+        return None
+
+    dd = util_dd.DictDot(res.response)
+    u = cls(
+        domo_instance=full_auth.domo_instance,
+        full_auth=full_auth,
+        id=dd.id or dd.userId,
+        display_name=dd.displayName,
+        email_address=dd.emailAddress,
+    )
+
+    if password:
+        await u.reset_password(new_password=password)
+
+    if send_password_reset_email:
+        await u.request_password_reset(
+            domo_instance=full_auth.domo_instance, email=u.email_address
+        )
+
+    return u
+
+
+@patch_to(DomoUser)
+async def set_user_landing_page(
+    self: DomoUser,
+    page_id: str,
+    user_id: str = None,
+    auth: dmda.DomoAuth = None,
+    debug_api: bool = False,
+):
+
+    res = await user_routes.set_user_landing_page(
+        auth=auth or self.auth,
+        page_id=page_id,
+        user_id=self.id or user_id,
         debug_api=debug_api,
-        session=session,
     )
 
-# %% ../../nbs/classes/50_DomoUser.ipynb 13
+    if res.status != 200:
+        return False
+
+    return True
+
+# %% ../../nbs/classes/50_DomoUser.ipynb 12
 @dataclass
 class DomoUsers:
     """a class for searching for Users"""
 
     logger: Optional[lc.Logger] = None
 
-    @classmethod
-    def _users_to_domo_user(cls, user_ls, auth: dmda.DomoAuth):
+    def _users_to_domo_user(user_ls, auth: dmda.DomoAuth):
         return [
             DomoUser._from_search_json(auth=auth, user_obj=user_obj)
             for user_obj in user_ls
         ]
 
-    @classmethod
-    def _users_to_virtual_user(cls, user_ls, auth: dmda.DomoAuth):
+    def _users_to_virtual_user(user_ls, auth: dmda.DomoAuth):
         return [
             DomoUser._from_virtual_json(auth=auth, user_obj=user_obj)
             for user_obj in user_ls
         ]
 
     def _generate_logger(self, logger: Optional[lc.Logger] = None):
-        self.logger = logger or self.logger or lc.Logger(app_name = "domo_users")
+        self.logger = logger or self.logger or lc.loger()
 
-# %% ../../nbs/classes/50_DomoUser.ipynb 15
+# %% ../../nbs/classes/50_DomoUser.ipynb 13
 @patch_to(DomoUsers, cls_method=True)
 async def all_users(
     cls: DomoUsers,
     auth: dmda.DomoAuth,
-    return_raw: bool = False,
     debug_api: bool = False,
     debug_prn: bool = False,
     debug_log: bool = False,
     logger: Optional[lc.Logger] = None,
 ) -> [DomoUser]:
     """retrieves all users from Domo"""
 
     logger = logger or lc.Logger(app_name="all_users")
 
     res = await user_routes.get_all_users(auth=auth, debug_api=debug_api)
 
-    if return_raw:
-        return res
-
     if not res.is_success:
         return None
 
     users_ls = res.response
 
     message = f"{len(users_ls)} users retrieved from {auth.domo_instance}"
 
     if debug_prn:
         print(message)
     logger.log_info(message=message, debug_log=debug_log)
 
     return cls._users_to_domo_user(user_ls=users_ls, auth=auth)
 
-
-# %% ../../nbs/classes/50_DomoUser.ipynb 18
+# %% ../../nbs/classes/50_DomoUser.ipynb 16
 @patch_to(DomoUsers, cls_method=True)
 async def by_id(
     cls: DomoUsers,
     user_ids: list[str],  # can search for one or multiple users
     auth: dmda.DomoAuth,
     only_allow_one: bool = True,
     debug_api: bool = False,
     return_raw: bool = False,
 ) -> list:
 
     body = user_routes.generate_search_users_body_by_id(user_ids)
 
-    try:
-        res = await user_routes.search_users(
-            return_raw=False,
-            body=body,
-            debug_api=debug_api,
-            auth=auth,
-        )
-
-    except user_routes.SearchUser_NoResults as e:
-        print(e)
-        return None
+    res = await user_routes.search_users(
+        process_users=False,
+        body=body,
+        debug_api=debug_api,
+        auth=auth,
+    )
 
     if return_raw:
         return res
 
-    domo_users = cls._users_to_domo_user(user_ls=res.response, auth=auth)
+    if not res.is_success:
+        return None
+
+    user_ls = res.response.get("users")
+
+    domo_users = cls._users_to_domo_user(user_ls=user_ls, auth=auth)
 
     if only_allow_one:
         return domo_users[0]
 
     return domo_users
 
-# %% ../../nbs/classes/50_DomoUser.ipynb 21
+# %% ../../nbs/classes/50_DomoUser.ipynb 20
 @patch_to(DomoUsers, cls_method=True)
 def util_match_domo_users_to_emails(
     cls: DomoUsers, domo_users: list[DomoUser], user_email_ls: list[str]
 ) -> list:
     """pass in an array of user emails to match against an array of Domo User"""
 
     matches = []
@@ -249,48 +290,47 @@
             matches.append(match_user)
     return matches
 
 
 @patch_to(DomoUsers, cls_method=True)
 async def by_email(
     cls: DomoUsers,
-    email_ls: list[str],
+    user_email_ls: list,
     auth: dmda.DomoAuth,
     only_allow_one: bool = True,
     debug_api: bool = False,
-    debug_prn: bool = False,
     return_raw: bool = False,
 ) -> list:
 
-    body = user_routes.generate_search_users_body_by_email(
-        user_email_ls=email_ls)
-
-    if debug_prn:
-        pprint(body)
+    body = user_routes.generate_search_users_body_by_email(user_email_ls=user_email_ls)
 
     res = await user_routes.search_users(
-        body=body, auth=auth, return_raw=False, debug_api=debug_api
+        body=body, auth=auth, process_users=False, debug_api=debug_api
     )
 
     if return_raw:
         if only_allow_one:
             res.response = cls.util_match_users_obj_to_emails(
-                res.response, email_ls
+                res.response.get("users"), user_email_ls
             )[0]
         return res
 
-    domo_users = cls._users_to_domo_user(res.response, auth=auth)
+    if res.status != 200:
+        return None
+
+    user_ls = res.response.get("users")
+
+    domo_users = cls._users_to_domo_user(user_ls, auth=auth)
 
     if only_allow_one:
-        return cls.util_match_domo_users_to_emails(domo_users, email_ls)[0]
+        return cls.util_match_domo_users_to_emails(domo_users, user_email_ls)[0]
 
     return domo_users
 
-
-# %% ../../nbs/classes/50_DomoUser.ipynb 24
+# %% ../../nbs/classes/50_DomoUser.ipynb 23
 @patch_to(DomoUsers, cls_method=True)
 async def virtual_user_by_subscriber_instance(
     cls: DomoUsers,
     subscriber_instance_ls: str,
     auth: dmda.DomoAuth,
     debug_api: bool = False,
     return_raw: bool = False,
@@ -307,117 +347,7 @@
     if not res.is_success:
         return None
 
     user_ls = res.response
 
     domo_users = cls._users_to_virtual_user(user_ls, auth=auth)
     return domo_users[0]
-
-
-# %% ../../nbs/classes/50_DomoUser.ipynb 28
-class CreateUser_MissingRole(de.DomoError):
-    def __init__(self, domo_instance, email_address):
-        super().__init__(domo_instance= domo_instance, message = f"error creating user {email_address} missing role_id")
-
-@patch_to(DomoUsers, cls_method=True)
-async def create_user(
-    cls: DomoUsers,
-    auth: dmda.DomoAuth,
-    display_name,
-    email_address,
-    role_id,
-    password: str = None,
-    send_password_reset_email: bool = False,
-    debug_api: bool = False,
-    session : httpx.AsyncClient = None
-):
-    """class method that creates a new Domo user"""
-
-    res = await user_routes.create_user(
-        auth=auth,
-        display_name=display_name,
-        email_address=email_address,
-        role_id=role_id,
-        debug_api=debug_api,
-        session = session
-    )
-
-    if not res.is_success:
-        return None
-
-    dd = util_dd.DictDot(res.response)
-    u = DomoUser(
-        auth=auth,
-        id=dd.id or dd.userId,
-        display_name=dd.displayName,
-        email_address=dd.emailAddress,
-    )
-
-    if password:
-        await u.reset_password(new_password=password)
-
-    if send_password_reset_email:
-        await u.request_password_reset(
-            domo_instance=auth.domo_instance, email=u.email_address
-        )
-
-    return u
-
-
-# %% ../../nbs/classes/50_DomoUser.ipynb 30
-@patch_to(DomoUsers, cls_method=True)
-async def upsert_user(cls: DomoUsers,
-                      auth: dmda.DomoAuth,
-                      email_address: str,
-                      display_name: str = None,
-                      role_id: str = None,
-                      debug_api: bool = False,
-                      debug_prn: bool = False,
-                      session: httpx.AsyncClient = None
-                      ):
-
-    try:
-        domo_user = await cls.by_email(
-            email_ls=[email_address],
-            auth=auth,
-            only_allow_one=True,
-            debug_api=debug_api,
-        )
-
-        if domo_user:
-            user_property_ls = []
-            if display_name:
-                user_property_ls.append(user_routes.UserProperty(
-                    user_routes.UserProperty_Type.display_name, display_name))
-
-            if role_id:
-                user_property_ls.append(user_routes.UserProperty(
-                    user_routes.UserProperty_Type.role_id, role_id))
-
-            return await user_routes.update_user(
-                user_id=domo_user.id,
-                user_property_ls=user_property_ls,
-                auth=auth,
-                debug_api=debug_api
-            )
-
-    except user_routes.SearchUser_NoResults as e:
-        if debug_prn:
-            print(
-                f'No user match -- creating new user in {auth.domo_instance}')
-
-        if not role_id:
-            raise CreateUser_MissingRole(
-                domo_instance=auth.domo_instance, email_address=email_address)
-
-        return await cls.create_user(auth=auth,
-                                     display_name=display_name or f"{email_address} - via dl {dt.date.today()}",
-                                     email_address=email_address,
-                                     role_id=role_id,
-                                     debug_api=debug_api, 
-                                     session=session)
-
-    # finally:
-    #     if grant_ls:
-    #         grant_ls = domo_role._valid_grant_ls(grant_ls)
-    #         await domo_role.set_grants(grant_ls=grant_ls)
-
```

### Comparing `domolibrary-0.0.81/domolibrary/client/DomoAuth.py` & `domolibrary-0.0.9/domolibrary/client/DomoAuth.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/client/95_DomoAuth.ipynb.
 
 # %% auto 0
 __all__ = ['get_full_auth', 'get_developer_auth', 'test_access_token', 'DomoAuth', 'InvalidCredentialsError',
-           'InvalidAuthTypeError', 'InvalidInstanceError', 'NoAccessTokenReturned', 'DomoFullAuth', 'DomoTokenAuth',
-           'DomoDeveloperAuth']
+           'InvalidInstanceError', 'DomoFullAuth', 'DomoTokenAuth', 'DomoDeveloperAuth']
 
 # %% ../../nbs/client/95_DomoAuth.ipynb 3
 from dataclasses import dataclass, field
+from abc import abstractmethod
 from typing import Optional, Union
 
 import httpx
 
 import domolibrary.client.ResponseGetData as rgd
-import domolibrary.client.DomoError as de
 
 # %% ../../nbs/client/95_DomoAuth.ipynb 5
 async def get_full_auth(
     domo_instance: str,  # domo_instance.domo.com
     domo_username: str,  # email address
     domo_password: str,
     session: Optional[httpx.AsyncClient] = None,
@@ -65,15 +64,15 @@
 
     if not session:
         is_close_session = True
         session = httpx.AsyncClient(
             auth=httpx.BasicAuth(domo_client_id, domo_client_secret)
         )
 
-    url = "https://api.domo.com/oauth/token?grant_type=client_credentials"
+    url = f"https://api.domo.com/oauth/token?grant_type=client_credentials"
 
     if debug_api:
         print(url, domo_client_id, domo_client_secret)
 
     res = await session.request(method="GET", url=url)
 
     if is_close_session:
@@ -135,16 +134,14 @@
     """parameters are defined after initialization"""
 
     token: Optional[str] = field(default=None, repr=False)
     token_name: Optional[str] = field(default=None)
     user_id: Optional[str] = field(default=None, repr=False)
     auth_header: dict = field(default_factory=dict, repr=False)
 
-    is_valid_token: bool = None
-
     url_manual_login: Optional[str] = None
 
     async def get_auth_token(self) -> Union[str, None]:
         """placeholder method"""
         pass
 
     async def generate_auth_header(self) -> Union[dict, None]:
@@ -171,74 +168,64 @@
 
 # %% ../../nbs/client/95_DomoAuth.ipynb 21
 @dataclass
 class DomoAuth(_DomoAuth_Optional, _DomoAuth_Required):
     """abstract DomoAuth class"""
 
 # %% ../../nbs/client/95_DomoAuth.ipynb 25
-class InvalidCredentialsError(de.DomoError):
-    """return invalid credentials sent to API"""
+class DomoErrror(Exception):
+    """base exception"""
 
     def __init__(
         self,
-        function_name: Optional[str] = None,
         status: Optional[int] = None,  # API request status
-        message="invalid credentials",
+        message: str = "error",  # <domo_instance>.domo.com
         domo_instance: Optional[str] = None,
     ):
 
-        super().__init__(status=status, message=message, domo_instance=domo_instance)
+        instance_str = f" at {domo_instance}" if domo_instance else ""
+        status_str = f"Status {status} - " if status else ""
+        self.message = f"{status_str}{message}{instance_str}"
+        super().__init__(self.message)
 
-
-class InvalidAuthTypeError(de.DomoError):
-    """return invalid Auth type sent to API"""
+# %% ../../nbs/client/95_DomoAuth.ipynb 26
+class InvalidCredentialsError(DomoErrror):
+    """return invalid credentials sent to API"""
 
     def __init__(
         self,
-        required_auth_type :DomoAuth ,
-        function_name: Optional[str] = None,
+        status: Optional[int] = None,  # API request status
+        message="invalid credentials",
         domo_instance: Optional[str] = None,
     ):
-        message = f"This API rquires {required_auth_type.__name__}"
 
-        super().__init__(message=message, domo_instance=domo_instance, function_name = function_name)
+        super().__init__(status=status, message=message, domo_instance=domo_instance)
+
 
-class InvalidInstanceError(de.DomoError):
+class InvalidInstanceError(DomoErrror):
     """return if invalid domo_instance sent to API"""
 
     def __init__(
         self,
-        function_name: Optional[str] = None,
         status: Optional[int] = None,
         message="invalid instance",
         domo_instance: Optional[str] = None,
     ):
         super().__init__(status=status, message=message, domo_instance=domo_instance)
-    
 
-class NoAccessTokenReturned(de.DomoError):
-    def __init__(
-        self,
-        function_name: Optional[str] = None,
-        status: Optional[int] = None,
-        message :str = "No AccessToken returned",
-        domo_instance: Optional[str] = None,
-    ):
-        super().__init__(status = status, message = message, domo_instance = domo_instance)
-
-# %% ../../nbs/client/95_DomoAuth.ipynb 28
+# %% ../../nbs/client/95_DomoAuth.ipynb 29
 @dataclass
 class _DomoFullAuth_Required(_DomoAuth_Required):
     """mix requied parameters for DomoFullAuth"""
 
     domo_username: str
     domo_password: str = field(repr=False)
 
 
-# %% ../../nbs/client/95_DomoAuth.ipynb 29
+# %% ../../nbs/client/95_DomoAuth.ipynb 30
 @dataclass
 class DomoFullAuth(_DomoAuth_Optional, _DomoFullAuth_Required):
     """use for full authentication token"""
 
     def generate_auth_header(self, token: str) -> dict:
         self.auth_header = {"x-domo-authentication": token}
         return self.auth_header
@@ -255,63 +242,48 @@
             domo_username=self.domo_username,
             domo_password=self.domo_password,
             session=session,
             debug_api = debug_api
         )
 
         if res.is_success and res.response.get("reason") == "INVALID_CREDENTIALS":
-            self.is_valid_token = False
             raise InvalidCredentialsError(
-                function_name = "get_auth_token",
                 status=res.status,
                 message=str(res.response.get("reason")),
                 domo_instance=self.domo_instance,
             )
 
         if res.status == 403:
-            self.is_valid_token = False
             raise InvalidInstanceError(
-                function_name = "get_auth_token",
                 status=res.status,
                 message="INVALID INSTANCE",
                 domo_instance=self.domo_instance,
             )
-        
-        if res.is_success and res.response == {}:
-            self.is_valid_token = False
-            raise NoAccessTokenReturned(
-                function_name="get_auth_token",
-                status=res.status, 
-                domo_instance=self.domo_instance)
-        
-        self.is_valid_token = True
 
         token = str(res.response.get("sessionToken"))
         self.token = token
         self.user_id = str(res.response.get("userId"))
 
         self.auth_header = self.generate_auth_header(token=token)
 
         if not self.token_name:
             self.token_name = "full_auth"
 
         return self.token
 
-# %% ../../nbs/client/95_DomoAuth.ipynb 36
+# %% ../../nbs/client/95_DomoAuth.ipynb 37
 @dataclass
 class _DomoTokenAuth_Required(_DomoAuth_Required):
     """mix requied parameters for DomoFullAuth"""
 
     domo_access_token: str = field(repr=False)
 
-# %% ../../nbs/client/95_DomoAuth.ipynb 37
+# %% ../../nbs/client/95_DomoAuth.ipynb 38
 @dataclass
 class DomoTokenAuth(_DomoAuth_Optional, _DomoTokenAuth_Required):
-    
-
     """
     use for access_token authentication.
     Tokens are generated in domo > admin > access token
     Necessary in cases where direct sign on is not permitted
     """
 
     def generate_auth_header(self, token: str) -> dict:
@@ -331,43 +303,39 @@
             domo_instance=self.domo_instance,
             domo_access_token=self.domo_access_token,
             session=session,
             debug_api = debug_api
         )
 
         if res.status == 401 and res.response == "Unauthorized":
-            self.is_valid_token = False
             raise InvalidCredentialsError(
                 status=res.status,
                 message=res.response,
                 domo_instance=self.domo_instance,
             )
 
-        if res.status == 200:
-            self.is_valid_token = True
-
         self.token = self.domo_access_token
         self.user_id = res.response.get("id")
 
         self.auth_header = self.generate_auth_header(token=self.token)
 
         if not self.token_name:
             self.token_name = "token_auth"
 
         return self.token
 
-# %% ../../nbs/client/95_DomoAuth.ipynb 41
+# %% ../../nbs/client/95_DomoAuth.ipynb 42
 @dataclass
 class _DomoDeveloperAuth_Required(_DomoAuth_Required):
     """mix requied parameters for DomoFullAuth"""
 
     domo_client_id: str
     domo_client_secret: str = field(repr=False)
 
-# %% ../../nbs/client/95_DomoAuth.ipynb 42
+# %% ../../nbs/client/95_DomoAuth.ipynb 43
 @dataclass(init=False)
 class DomoDeveloperAuth(_DomoAuth_Optional, _DomoDeveloperAuth_Required):
     """use for full authentication token"""
 
     def __init__(self, domo_client_id: str, domo_client_secret: str):
         self.domo_client_id = domo_client_id
         self.domo_client_secret = domo_client_secret
@@ -387,23 +355,20 @@
             domo_client_id=self.domo_client_id,
             domo_client_secret=self.domo_client_secret,
             session=session,
             debug_api = debug_api
         )
 
         if res.status == 401:
-            self.is_valid_token = False
             raise InvalidCredentialsError(
                 status=res.status,
                 message=str(res.response),
                 domo_instance=self.domo_instance,
             )
 
-        self.is_valid_token = True
-
         token = str(res.response.get("access_token"))
         self.token = token
         self.user_id = res.response.get("userId")
         self.domo_instance = res.response.get("domain")
         self.set_manual_login()
 
         self.auth_header = self.generate_auth_header(token=token)
```

### Comparing `domolibrary-0.0.81/domolibrary/client/Logger.py` & `domolibrary-0.0.9/domolibrary/client/Logger.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.81/domolibrary/client/ResponseGetData.py` & `domolibrary-0.0.9/domolibrary/client/ResponseGetData.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,46 +1,28 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/client/99_ResponseGetData.ipynb.
 
 # %% auto 0
-__all__ = ['API_Response', 'STREAM_FILE_PATH', 'BlockedByVPN', 'ResponseGetData', 'find_ip']
+__all__ = ['API_Response', 'STREAM_FILE_PATH', 'ResponseGetData']
 
 # %% ../../nbs/client/99_ResponseGetData.ipynb 2
 # pylint: disable=no-member
 
-import re
-from bs4 import BeautifulSoup
-
 from dataclasses import dataclass, field
 from typing import Optional
 
 import orjson
 
 import asyncio
 import requests
 import httpx
 import aiohttp
 
 from fastcore.utils import patch_to
-import domolibrary.client.DomoError as de
-
-# %% ../../nbs/client/99_ResponseGetData.ipynb 5
-class BlockedByVPN(de.DomoError):
-    def __init__(
-        self,
-        domo_instance: Optional[str] = None,
-        ip_address : str = None,
-        function_name: str = "get_data"
-    ):
-        ip_address_str = f"from {ip_address}" if ip_address else ""
-        message = f"request blocked {ip_address_str} - check VPN settings"
-
-        super().__init__(message=message, domo_instance=domo_instance, function_name=function_name)
 
-
-# %% ../../nbs/client/99_ResponseGetData.ipynb 6
+# %% ../../nbs/client/99_ResponseGetData.ipynb 4
 API_Response = any
 
 
 @dataclass
 class ResponseGetData:
     """preferred response class for all API Requests"""
 
@@ -48,15 +30,15 @@
     response: API_Response
     is_success: bool
     auth: dict = field(repr = False, default=None)
 
     def set_response(self, response):
         self.response = response
 
-# %% ../../nbs/client/99_ResponseGetData.ipynb 11
+# %% ../../nbs/client/99_ResponseGetData.ipynb 8
 @patch_to(ResponseGetData, cls_method=True)
 def _from_requests_response(
     cls, res: requests.Response  # requests response object
 ) -> ResponseGetData:
     """returns ResponseGetData"""
 
     # JSON responses
@@ -66,56 +48,38 @@
     # default text responses
     elif res.ok:
         return cls(status=res.status_code, response=res.text, is_success=True)
 
     # errors
     return cls(status=res.status_code, response=res.reason, is_success=False)
 
-# %% ../../nbs/client/99_ResponseGetData.ipynb 16
-def find_ip(html,   html_tag: str = 'p'):
-    ip_address_regex = r'(\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3})'
-    soup = BeautifulSoup(html, 'html.parser')
-
-    return re.findall(ip_address_regex, str(soup.find(html_tag)))[0]
-                                 
-
-# %% ../../nbs/client/99_ResponseGetData.ipynb 17
+# %% ../../nbs/client/99_ResponseGetData.ipynb 12
 @patch_to(ResponseGetData, cls_method=True)
 def _from_httpx_response(
-    cls, 
-    res: requests.Response,  # requests response object
+    cls, res: requests.Response,  # requests response object
     auth : Optional[any] = None,
+    debug_api : bool = False
 ) -> ResponseGetData:
     """returns ResponseGetData"""
 
-
     # JSON responses
-    ok = True if res.status_code <= 399 and res.status_code >= 200 else False
-
-    if ok and '<title>Domo - Blocked</title>' in res.text:
-        ip_address = find_ip(res.text)
-        
-        raise BlockedByVPN(auth.domo_instance, ip_address)
+    ok = True if res.status_code <= 299 and res.status_code >= 200 else False
     
     if ok and "application/json" in res.headers.get("Content-Type", {}):
-        try:
-            return cls(status=res.status_code, response=res.json(), is_success=True, auth = auth)
-
-        except Exception as e:
-            return cls(status=res.status_code, response=res.text, is_success=True, auth=auth)
+        return cls(status=res.status_code, response=res.json(), is_success=True, auth = auth)
 
     # default text responses
     elif ok:
         return cls(status=res.status_code, response=res.text, is_success=True, auth = auth)
 
     # errors
     return cls(status=res.status_code, response=res.reason_phrase, is_success=False, auth=auth)
 
 
-# %% ../../nbs/client/99_ResponseGetData.ipynb 19
+# %% ../../nbs/client/99_ResponseGetData.ipynb 15
 STREAM_FILE_PATH = '__large-file.json'
 
 async def _write_stream(res: httpx.Response,
                         file_name: str = STREAM_FILE_PATH,
                         stream_chunks=10):
     
     print(type(res), type(res.content), stream_chunks)
@@ -130,71 +94,64 @@
             print(res.content.at_eof())
         
     print('done writing stream')
     
     return None
 
 
-async def _read_stream(file_name : str):
-    with open(file_name, "rb") as f:
+async def _read_stream(file_name : str = STREAM_FILE_PATH):
+    with open(STREAM_FILE_PATH, "rb") as f:
         return f.read()
 
 
-# %% ../../nbs/client/99_ResponseGetData.ipynb 20
+# %% ../../nbs/client/99_ResponseGetData.ipynb 16
 @patch_to(ResponseGetData, cls_method=True)
 async def _from_aiohttp_response(
     cls: ResponseGetData, 
     res: aiohttp.ClientResponse,  # requests response object
     auth : Optional[any] = None,
     process_stream: bool = False,
     stream_chunks : int = 10,
-    debug_api : bool = False,
-    response_file_name: str = None
+    debug_api : bool = False
 ) -> ResponseGetData:
 
     """async method returns ResponseGetData"""
     if debug_api:
         print( f"ResponseGetData: res.ok = {res.ok} , res.status = {res.status}" )
     
 
     try:
         data = None
 
         if process_stream:
             await _write_stream(res = res, stream_chunks = stream_chunks)
-            data = await _read_stream(response_file_name)
+            data =await _read_stream()
         
         else:        
             data = await res.text()
     
         if debug_api:
             print('converting to text complete')
     
     except asyncio.TimeoutError as e:
         print(f"ResponseGetDataError: {str(e)} , trying content.read")
 
         data = await res.content.read()
-    
 
     if res.ok and "application/json" in res.headers.get("Content-Type", {}):
-        try:
-            return cls(status=res.status, response= orjson.loads(data), is_success=True, auth = auth)
-        except Exception as e:
-            return cls(status=res.status, response=data, is_success=True, auth=auth)
+        return cls(status=res.status, response= orjson.loads(data), is_success=True, auth = auth)
 
     elif res.ok:
         return cls(status=res.status, response= data, is_success=True, auth = auth)
 
     # response is error
     else:
         return cls(status=res.status, response=res.reason, is_success=False, auth = auth)
 
-
-
-# %% ../../nbs/client/99_ResponseGetData.ipynb 24
+# %% ../../nbs/client/99_ResponseGetData.ipynb 20
 @patch_to(ResponseGetData, cls_method=True)
 async def _from_looper(cls: ResponseGetData,
                        res: ResponseGetData,  # requests response object
                        array: list
                        ) -> ResponseGetData:
 
     """async method returns ResponseGetData"""
```

### Comparing `domolibrary-0.0.81/domolibrary/client/get_data.py` & `domolibrary-0.0.9/domolibrary/client/get_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,38 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/client/10_get_data.ipynb.
 
 # %% auto 0
-__all__ = ['get_data_aiohttp', 'GetData_Error', 'get_data', 'LooperError', 'looper', 'looper_aiohttp']
+__all__ = ['get_data_aiohttp', 'get_data', 'LooperError', 'looper', 'looper_aiohttp']
 
 # %% ../../nbs/client/10_get_data.ipynb 2
 from typing import Optional, Union
 
 from pprint import pprint
 
 import httpx
 import aiohttp
-import asyncio
 
 import domolibrary.client.DomoAuth as dmda
 import domolibrary.client.ResponseGetData as rgd
-import domolibrary.client.DomoError as de
-import time
 
 
 # %% ../../nbs/client/10_get_data.ipynb 3
 async def get_data_aiohttp(
     url: str,
     method: str,
     auth: dmda.DomoAuth,
     content_type: Optional[dict] = None,
     headers: Optional[dict] = None,
     # if no session passed by default will create and close session during execution
     session: Optional[aiohttp.ClientSession] = None,
     body: Union[dict, str, None] = None,
     params: Optional[dict] = None,
     debug_api: bool = False,
-    process_stream: bool = False,
-    stream_chunks: int = 10
+    process_stream : bool = False,
+    stream_chunks : int = 10
 ) -> rgd.ResponseGetData:
     """async wrapper for asyncio requests"""
 
     if auth and not auth.token:
         await auth.get_auth_token()
 
     if headers is None:
@@ -87,49 +84,42 @@
                 params=params,
             )
 
         else:
             res = await session.request(
                 method=method.upper(), url=url, headers=headers, params=params
             )
-        return await rgd.ResponseGetData._from_aiohttp_response(res, auth=auth, process_stream=process_stream, stream_chunks=stream_chunks)
 
     except Exception as e:
         print(e)
 
     finally:
         if is_close_session:
             await session.close()
+        
+    return await rgd.ResponseGetData._from_aiohttp_response(res, auth=auth, debug_api=debug_api, process_stream=process_stream, stream_chunks=stream_chunks)
 
 
 # %% ../../nbs/client/10_get_data.ipynb 6
-class GetData_Error(de.DomoError):
-    def __init__(self, message, url):
-        super().__init__( message = message, domo_instance = url)
-        
-
-# %% ../../nbs/client/10_get_data.ipynb 7
 async def get_data(
     url: str,
     method: str,
     auth: dmda.DomoAuth,
     content_type: Optional[dict] = None,
     headers: Optional[dict] = None,
     body: Union[dict, str, None] = None,
     params: Optional[dict] = None,
     debug_api: bool = False,
-    session: httpx.AsyncClient = None,
-    return_raw: bool = False,
-    is_follow_redirects: bool = False,
-    timeout = 5
-) -> rgd.ResponseGetData:
+    session : httpx.AsyncClient = None ,
+    return_raw : bool = False
+    ) -> rgd.ResponseGetData:
     """async wrapper for asyncio requests"""
 
     if debug_api:
-        print("🐛 debugging get_data")
+        print( f"🐛 debugging get_data")
 
     if auth and not auth.token:
         await auth.get_auth_token()
 
     if headers is None:
         headers = {}
 
@@ -149,128 +139,101 @@
                 "method": method,
                 "url": url,
                 "headers": headers,
                 "body": body,
                 "params": params,
             }
         )
-
+    
     is_close_session = False if session else True
-
+        
     session = session or httpx.AsyncClient()
 
-
-    attempt = 1
-    max_attempt = 4
-    
-    while attempt <= max_attempt:
-        try:
-            if isinstance(body, dict) or isinstance(body, list):
-                if debug_api:
-                    print("get_data: sending json")
-                res = await getattr(session, method.lower())(
-                    url=url,
-                    headers=headers,
-                    json=body,
-                    params=params,
-                    follow_redirects=is_follow_redirects,
-                    timeout = timeout
-                )
-
-            elif body:
-                if debug_api:
-                    print("get_data: sending data")
-
-                res = await getattr(session, method.lower())(
-                    url=url,
-                    headers=headers,
-                    data=body,
-                    params=params,
-                    follow_redirects=is_follow_redirects,
-                    timeout = timeout
-                )
-
-            else:
-                if debug_api:
-                    print("get_data: no body")
-
-                res = await getattr(session, method.lower())(
-                    url=url,
-                    headers=headers,
-                    params=params,
-                    follow_redirects=is_follow_redirects,
-                    timeout = timeout
-                )
-
+    res = None
+    try:
+        if isinstance(body, dict) or isinstance(body, list):
+            if debug_api:
+                print("get_data: sending json")
+            res = await getattr(session, method.lower())(url=url,
+                                                 headers=headers,
+                                                 json=body,
+                                                 params=params)
+        
+        elif body:
             if debug_api:
-                print("get_data_response", res)
+                print("get_data: sending data")
 
-            if return_raw:
-                return res
+            res = await getattr(session, method.lower())(url=url,
+                                                 headers=headers,
+                                                 data=body,
+                                                 params=params)
 
-            return rgd.ResponseGetData._from_httpx_response(res, auth=auth)
-        
-        except httpx.TransportError as e:
-            print(f"ℹ️ get_data error - {e} at {url}")
-            attempt +=1
 
-            if attempt == max_attempt:
-                raise GetData_Error(url=url, message=e)
+        else:
+            if debug_api:
+                print("get_data: no body")
 
-            await asyncio.sleep(5)
+            res = await getattr(session, method.lower())(
+                url=url, headers=headers, params=params)
 
+    except Exception as e:
+        print(e)
 
-        finally:
-            if is_close_session:
-                await session.aclose()
+    finally:
+        if debug_api:
+            print('get_data_response', res)
+        if is_close_session:
+            await session.aclose()
+    
+    if return_raw:
+        return res
 
 
+    return rgd.ResponseGetData._from_httpx_response(res, auth=auth, debug_api=debug_api)
 
-# %% ../../nbs/client/10_get_data.ipynb 10
+
+# %% ../../nbs/client/10_get_data.ipynb 9
 class LooperError(Exception):
-    def __init__(self, loop_stage: str, message):
+    def __init__(self, loop_stage: str, message ):
 
         super().__init__(f"{loop_stage} - {message}")
 
-# %% ../../nbs/client/10_get_data.ipynb 11
+# %% ../../nbs/client/10_get_data.ipynb 10
 async def looper(
     auth: dmda.DomoAuth,
     session: httpx.AsyncClient,
     url,
     offset_params,
     arr_fn: callable,
     loop_until_end: bool = False,
     method="POST",
     body: dict = None,
     fixed_params: dict = None,
     offset_params_in_body: bool = False,
     body_fn=None,
     limit=1000,
-    skip=0,
+    skip = 0,
     maximum=2000,
     debug_api: bool = False,
-    debug_loop: bool = False,
-    timeout : bool = 10,
-    wait_sleep : int = 0
+    debug_loop: bool = False
 ) -> rgd.ResponseGetData:
 
-    maximum = maximum or 0
-
     is_close_session = False
-
+    
     if not session:
         session = httpx.AsyncClient()
         is_close_session = True
 
+
     allRows = []
     isLoop = True
 
     res = None
 
-    if maximum < limit and not loop_until_end:
+    if maximum < limit:
         limit = maximum
 
     while isLoop:
         params = fixed_params or {}
 
         if offset_params_in_body:
             body[offset_params.get("offset")] = skip
@@ -279,105 +242,104 @@
         else:
             params[offset_params.get("offset")] = skip
             params[offset_params.get("limit")] = limit
 
         if body_fn:
             try:
                 body = body_fn(skip, limit)
-
+            
             except Exception as e:
                 await session.aclose()
-                raise LooperError(
-                    loop_stage="processing body_fn", message=str(e)
-                ) from e
+                raise LooperError(loop_stage = "processing body_fn", message = str(e))
+            
 
         if debug_loop:
-            print(f"\n🚀 Retrieving records {skip} through {skip + limit} via {url}")
+            print(
+                f"\n🚀 Retrieving records {skip} through {skip + limit} via {url}")
             # pprint(params)
 
+        
         res = await get_data(
             auth=auth,
             url=url,
             method=method,
             params=params,
             session=session,
             body=body,
             debug_api=debug_api,
-            timeout = timeout
         )
 
         if not res.is_success:
             if is_close_session:
                 await session.aclose()
             return res
 
+
         try:
             newRecords = arr_fn(res)
-
+        
         except Exception as e:
             await session.aclose()
-            raise LooperError(loop_stage="processing arr_fn", message=str(e)) from e
-
+            raise LooperError(loop_stage = "processing arr_fn", message = str(e))
+        
         allRows += newRecords
 
         if loop_until_end and len(newRecords) != 0:
             maximum = maximum + limit
 
         if debug_loop:
             print({"all_rows": len(allRows), "new_records": len(newRecords)})
 
         if len(allRows) >= maximum or len(newRecords) == 0:
             if debug_loop:
                 print(
-                    f"\n🎉 Success - {len(allRows)} records retrieved from {url} in query looper\n"
-                )
+                    f"\n🎉 Success - {len(allRows)} records retrieved from {url} in query looper\n")
 
             break
 
         skip += len(newRecords)
-
+        
         if skip + limit > maximum:
             limit = maximum - len(allRows)
 
-        if debug_loop:
-            print(f"skip: {skip}, limit: {limit}")
-        
-        time.sleep(wait_sleep)
-
+            if debug_loop:
+                print(f"skip: {skip}, limit: {limit}")
+    
     if is_close_session:
         await session.aclose()
 
-    return await rgd.ResponseGetData._from_looper(res=res, array=allRows)
+    return await rgd.ResponseGetData._from_looper(res = res, array = allRows)
 
-# %% ../../nbs/client/10_get_data.ipynb 15
+# %% ../../nbs/client/10_get_data.ipynb 14
 async def looper_aiohttp(
     auth: dmda.DomoAuth,
     session: aiohttp.ClientSession,
     url,
     offset_params,
     arr_fn: callable,
     loop_until_end: bool = False,
     method="POST",
     body: dict = None,
     fixed_params: dict = None,
     offset_params_in_body: bool = False,
     body_fn=None,
     limit=1000,
-    skip=0,
+    skip = 0,
     maximum=2000,
     debug_api: bool = False,
-    debug_loop: bool = False,
+    debug_loop: bool = False
 ) -> rgd.ResponseGetData:
 
     is_close_session = False
-
+    
     if not session:
         session = aiohttp.ClientSession()
         is_close_session = True
 
+
     allRows = []
     isLoop = True
 
     res = None
 
     if maximum < limit:
         limit = maximum
@@ -392,25 +354,26 @@
         else:
             params[offset_params.get("offset")] = skip
             params[offset_params.get("limit")] = limit
 
         if body_fn:
             try:
                 body = body_fn(skip, limit)
-
+            
             except Exception as e:
                 await session.aclose()
-                raise LooperError(
-                    loop_stage="processing body_fn", message=str(e)
-                ) from e
+                raise LooperError(loop_stage = "processing body_fn", message = str(e))
+            
 
         if debug_loop:
-            print(f"\n🚀 Retrieving records {skip} through {skip + limit} via {url}")
+            print(
+                f"\n🚀 Retrieving records {skip} through {skip + limit} via {url}")
             # pprint(params)
 
+        
         res = await get_data_aiohttp(
             auth=auth,
             url=url,
             method=method,
             params=params,
             session=session,
             body=body,
@@ -418,42 +381,42 @@
         )
 
         if not res.is_success:
             if is_close_session:
                 await session.aclose()
             return res
 
+
         try:
             newRecords = arr_fn(res)
-
+        
         except Exception as e:
             await session.close()
-            raise LooperError(loop_stage="processing arr_fn", message=str(e)) from e
-
+            raise LooperError(loop_stage = "processing arr_fn", message = str(e))
+        
         allRows += newRecords
 
         if loop_until_end and len(newRecords) != 0:
             maximum = maximum + limit
 
         if debug_loop:
             print({"all_rows": len(allRows), "new_records": len(newRecords)})
 
         if len(allRows) >= maximum or len(newRecords) == 0:
             if debug_loop:
                 print(
-                    f"\n🎉 Success - {len(allRows)} records retrieved from {url} in query looper\n"
-                )
+                    f"\n🎉 Success - {len(allRows)} records retrieved from {url} in query looper\n")
 
             break
 
         skip += len(newRecords)
-
+        
         if skip + limit > maximum:
             limit = maximum - len(allRows)
 
             if debug_loop:
                 print(f"skip: {skip}, limit: {limit}")
-
+    
     if is_close_session:
         await session.close()
 
-    return await rgd.ResponseGetData._from_looper(res=res, array=allRows)
+    return await rgd.ResponseGetData._from_looper(res = res, array = allRows)
```

### Comparing `domolibrary-0.0.81/domolibrary/routes/account.py` & `domolibrary-0.0.9/domolibrary/routes/account.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,86 +1,67 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/routes/account.ipynb.
 
 # %% auto 0
-__all__ = ['get_accounts', 'GetAccount_NoMatch', 'get_account_from_id', 'AccountConfig_InvalidDataProvider', 'get_account_config',
-           'update_account_config', 'update_account_name', 'create_account', 'delete_account',
-           'ShareAccount_V1_AccessLevel', 'ShareAccount_V2_AccessLevel', 'generate_share_account_payload_v1',
-           'generate_share_account_payload_v2', 'share_account_v2', 'share_account_v1']
+__all__ = ['get_accounts', 'get_account_from_id', 'AccountConfig_InvalidDataProvider', 'get_account_config',
+           'update_account_config', 'update_account_name', 'create_account', 'delete_account']
 
 # %% ../../nbs/routes/account.ipynb 3
 from typing import Union
-from enum import Enum
+import httpx
 import httpx
 
 import domolibrary.client.get_data as gd
 import domolibrary.client.ResponseGetData as rgd
 import domolibrary.client.DomoAuth as dmda
-import domolibrary.client.DomoError as de
 
 # %% ../../nbs/routes/account.ipynb 4
 async def get_accounts(auth: dmda.DomoAuth,
                        debug_api: bool = False, 
-                       session: Union[httpx.AsyncClient, httpx.AsyncClient, None] = None) -> rgd.ResponseGetData:
+                       session: Union[httpx.AsyncClient, httpx.AsyncClient, None] = None):
     """retrieve a list of all the accounts the user has read access to.  Note users with "Manage all accounts" will retrieve all account objects"""
     
     url = f"https://{auth.domo_instance}.domo.com/api/data/v1/accounts"
 
     return await gd.get_data(
         auth=auth,
         url=url,
         method='GET',
         debug_api=debug_api,
         session=session
     )
 
 # %% ../../nbs/routes/account.ipynb 7
-class GetAccount_NoMatch(de.DomoError):
-    def __init__(self, account_id, domo_instance, status, function_name = 'get_account_from_id'):
-
-        message = f"account_id {account_id} not found"
-        
-        super().__init__(message = message, status = status, function_name = function_name , domo_instance = domo_instance)
-    
 async def get_account_from_id(auth: dmda.DomoAuth, account_id: int,
-                              debug_api: bool = False, session: httpx.AsyncClient = None) -> rgd.ResponseGetData:
+                              debug_api: bool = False, session: httpx.AsyncClient = None):
     """retrieves metadata about an account"""
 
     url = f"https://{auth.domo_instance}.domo.com/api/data/v1/accounts/{account_id}?unmask=true"
 
     if debug_api:
         print(url)
 
-    res = await gd.get_data(
+    return await gd.get_data(
         auth=auth,
         url=url,
         method='GET',
         debug_api=debug_api,
         session=session
     )
 
-    if not res.is_success and (res.response == 'Forbidden' or res.response == 'Not Found'):
-        raise GetAccount_NoMatch(
-            account_id=account_id, domo_instance=auth.domo_instance, status=res.status)
-    
-    return res
-
-
-
-
 # %% ../../nbs/routes/account.ipynb 11
 class AccountConfig_InvalidDataProvider(Exception):
     def __init__(self, account_id:str, data_provider_type:str, domo_instance: str):
         message = f"Account - {account_id}, could not be retrieved with data_provider_type, '{data_provider_type}' from {domo_instance}"
         super().__init__( message)
 
 async def get_account_config(auth: dmda.DomoAuth,
                              account_id: int,
                              data_provider_type: str ,
                              debug_api: bool = False, 
-                             session: Union[httpx.AsyncClient, httpx.AsyncClient, None] = None) -> rgd.ResponseGetData:
+                             session: Union[httpx.AsyncClient, httpx.AsyncClient, None] = None):
 
     url = f"https://{auth.domo_instance}.domo.com/api/data/v1/providers/{data_provider_type}/account/{account_id}?unmask=true"
 
     if debug_api:
         print(url)
 
     res = await gd.get_data(
@@ -98,15 +79,15 @@
 
 # %% ../../nbs/routes/account.ipynb 14
 async def update_account_config(auth: dmda.DomoAuth,
                                 account_id: int,
                                 config_body: dict,
                                 data_provider_type: str,
                                 debug_api: bool = False, 
-                                session: httpx.AsyncClient = None) -> rgd.ResponseGetData:
+                                session: httpx.AsyncClient = None):
 
     url = f"https://{auth.domo_instance}.domo.com/api/data/v1/providers/{data_provider_type}/account/{account_id}"
 
     if debug_api:
         print(url)
 
     return await gd.get_data(
@@ -119,15 +100,15 @@
     )
 
 # %% ../../nbs/routes/account.ipynb 15
 async def update_account_name(auth: dmda.DomoAuth,
                               account_id: int,
                               account_name: str,
                               debug_api: bool = False, 
-                              session: httpx.AsyncClient = None) -> rgd.ResponseGetData:
+                              session: httpx.AsyncClient = None):
 
     url = f"https://{auth.domo_instance}.domo.com/api/data/v1/accounts/{account_id}/name"
     
     if debug_api:
         print(url)
 
     return await gd.get_data(
@@ -138,15 +119,15 @@
         content_type = "text/plain",
         debug_api=debug_api,
         session=session
     )
 
 # %% ../../nbs/routes/account.ipynb 16
 async def create_account(auth:dmda.DomoAuth, config_body:dict,
-                         debug_api: bool = False, session: httpx.AsyncClient = None) -> rgd.ResponseGetData:
+                         debug_api: bool = False, session: httpx.AsyncClient = None):
 
     url = f"https://{auth.domo_instance}.domo.com/api/data/v1/accounts"
 
     if debug_api:
         print(url)
 
     return await gd.get_data(
@@ -158,82 +139,21 @@
         session=session
     )
 
 # %% ../../nbs/routes/account.ipynb 17
 async def delete_account(auth:dmda.DomoAuth,
                          account_id: str,
                          debug_api: bool = False, 
-                         session: httpx.AsyncClient = None) -> rgd.ResponseGetData:
+                         session: httpx.AsyncClient = None):
     
     url = f"https://{auth.domo_instance}.domo.com/api/data/v1/accounts/{account_id}"
 
     if debug_api:
         print(url)
 
     return await gd.get_data(
         auth=auth,
         url=url,
         method='DELETE',
         debug_api=debug_api,
         session=session
     )
-
-# %% ../../nbs/routes/account.ipynb 19
-class ShareAccount_V1_AccessLevel(Enum):
-    CAN_VIEW = 'READ'
-
-
-class ShareAccount_V2_AccessLevel(Enum):
-    CAN_VIEW = 'CAN_VIEW'
-    CAN_EDIT = 'CAN_EDIT'
-    CAN_SHARE = 'CAN_SHARE'
-
-
-def generate_share_account_payload_v1(user_id: int, access_level: str):
-    return {"type": "USER", "id": user_id, "permissions": [ShareAccount_V1_AccessLevel[access_level].value]}
-
-
-def generate_share_account_payload_v2(user_id: int,
-                                      access_level: str
-                                      ):
-
-    return {"type": "USER", "id": user_id, "accessLevel": ShareAccount_V2_AccessLevel[access_level].value}
-
-
-# %% ../../nbs/routes/account.ipynb 21
-async def share_account_v2(auth: dmda.DomoAuth,
-                           account_id: str,
-                           share_payload: dict,
-                           debug_api: bool = False,
-                           session: httpx.AsyncClient = None
-                           ):
-
-    url = f"https://{auth.domo_instance}.domo.com/api/data/v2/accounts/share/{account_id}"
-
-    return await gd.get_data(
-        auth=auth,
-        url=url,
-        method='PUT',
-        body=share_payload,
-        debug_api=debug_api,
-        session=session
-    )
-
-
-async def share_account_v1(auth: dmda.DomoAuth,
-                           account_id: str,
-                           share_payload: dict,
-                           debug_api: bool = False,
-                           session: httpx.AsyncClient = None
-                           ):
-
-    url = f"https://{auth.domo_instance}.domo.com/api/data/v1/accounts/{account_id}/share"
-
-    return await gd.get_data(
-        auth=auth,
-        url=url,
-        method='PUT',
-        body=share_payload,
-        debug_api=debug_api,
-        session=session
-    )
-
```

### Comparing `domolibrary-0.0.81/domolibrary/routes/activity_log.py` & `domolibrary-0.0.9/domolibrary/routes/activity_log.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import domolibrary.client.DomoAuth as dmda
 
 
 # %% ../../nbs/routes/activity_log.ipynb 4
 async def get_activity_log_object_types(auth: dmda.DomoAuth) -> rgd.ResponseGetData:
     """retrieves a list of valid objectTypes that can be used to search the activity_log API"""
 
-    url = "https://domo-community.domo.com/api/audit/v1/user-audits/objectTypes"
+    url = "https://domo-dojo.domo.com/api/audit/v1/user-audits/objectTypes"
 
     return await gd.get_data(url=url, method="GET", auth=auth)
 
 # %% ../../nbs/routes/activity_log.ipynb 7
 async def search_activity_log(
     auth: dmda.DomoAuth,
     start_time: int,  # epoch time in milliseconds
```

### Comparing `domolibrary-0.0.81/domolibrary/routes/bootstrap.py` & `domolibrary-0.0.9/domolibrary/routes/bootstrap.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,48 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/routes/bootstrap.ipynb.
 
 # %% auto 0
-__all__ = ['get_bootstrap', 'get_bootstrap_features', 'get_bootstrap_pages']
+__all__ = ['GetBootstrap_InvalidAuthMethod', 'get_bootstrap', 'get_bootstrap_features', 'get_bootstrap_pages']
 
 # %% ../../nbs/routes/bootstrap.ipynb 3
 import httpx
 
 import domolibrary.client.get_data as gd
 import domolibrary.client.ResponseGetData as rgd
 import domolibrary.client.DomoAuth as dmda
 
 # %% ../../nbs/routes/bootstrap.ipynb 4
+class GetBootstrap_InvalidAuthMethod(Exception):
+    def __init__(self, domo_instance):
+        message = f"invalid auth method sent to {domo_instance} bootstrap API, use DomoFullAuth (username and password) authentication"
+        super().__init__(message)
+
 async def get_bootstrap(
     auth: dmda.DomoFullAuth, ## only works with DomoFullAuth authentication, do not use TokenAuth
     debug_api: bool = False, session: httpx.AsyncClient = None
 ) -> rgd.ResponseGetData:
     """get bootstrap data"""
 
-    if auth.__class__.__name__ != 'DomoFullAuth':
-        raise dmda.InvalidAuthTypeError(function_name='get_bootstrap',
-                                        domo_instance=auth.domo_instance, 
-                                        required_auth_type =  dmda.DomoFullAuth )
-
     # url = f"https://{auth.domo_instance}.domo.com/api/domoweb/bootstrap?v2Navigation=false"
     url = f"https://{auth.domo_instance}.domo.com/api/domoweb/bootstrap?v2Navigation=true"
 
     res = await gd.get_data(
-        url=url, method="GET", auth=auth, debug_api=debug_api, session=session, is_follow_redirects = True
+        url=url, method="GET", auth=auth, debug_api=debug_api, session=session
     )
 
+    if res.status == 302:
+        raise GetBootstrap_InvalidAuthMethod(auth.domo_instance)
+
     return res
 
 
 # %% ../../nbs/routes/bootstrap.ipynb 8
 async def get_bootstrap_features(   
     auth: dmda.DomoAuth, session: httpx.AsyncClient = None, debug_api: bool = False
 ) -> rgd.ResponseGetData:
-
     res = await get_bootstrap(auth=auth, session=session, debug_api=debug_api)
 
     if not res.is_success:
         return None
 
     res.response = res.response.get("data").get("features")
     return res
```

### Comparing `domolibrary-0.0.81/domolibrary/routes/datacenter.py` & `domolibrary-0.0.9/domolibrary/routes/user.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,225 +1,191 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/routes/datacenter.ipynb.
+# AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/routes/user.ipynb.
 
 # %% auto 0
-__all__ = ['Datacenter_Enum', 'Dataflow_Type_Filter_Enum', 'Datacenter_Filter_Field_Enum', 'generate_search_datacenter_filter',
-           'generate_search_datacenter_filter_search_term', 'generate_search_datacenter_body',
-           'generate_search_datacenter_account_body', 'SearchDatacenter_NoResultsFound', 'search_datacenter',
-           'get_lineage_upstream']
-
-# %% ../../nbs/routes/datacenter.ipynb 2
-from enum import Enum
-from typing import Union
-import httpx
+__all__ = ['get_all_users', 'generate_search_users_body_by_id', 'generate_search_users_body_by_email', 'process_v1_search_users',
+           'search_users', 'search_virtual_user_by_subscriber_instance', 'create_user', 'set_user_landing_page',
+           'reset_password', 'request_password_reset']
 
+# %% ../../nbs/routes/user.ipynb 3
+import utils.DictDot as dd
 import domolibrary.client.get_data as gd
 import domolibrary.client.ResponseGetData as rgd
-import domolibrary.client.DomoError as de
 import domolibrary.client.DomoAuth as dmda
 
 
-# %% ../../nbs/routes/datacenter.ipynb 3
-class Datacenter_Enum(Enum):
-    ACCOUNT = "ACCOUNT"
-    CARD = "CARD"
-    DATAFLOW = "DATAFLOW"
-    DATASET = "DATASET"
-    GROUP = "GROUP"
-    PAGE = "PAGE"
-    USER = "USER"
-
-class Dataflow_Type_Filter_Enum(Enum):
-    ADR = {
-        "filterType": "term",
-        "field": "data_flow_type",
-        "value": "ADR",
-        "name": "ADR",
-        "not": False,
-    }
+# %% ../../nbs/routes/user.ipynb 5
+async def get_all_users(
+    auth: dmda.DomoAuth, debug_api: bool = False
+) -> rgd.ResponseGetData:
 
-    MYSQL = {
-        "filterType": "term",
-        "field": "data_flow_type",
-        "value": "MYSQL",
-        "name": "MYSQL",
-        "not": False,
-    }
+    """retrieves all users from Domo"""
+    url = f"https://{ auth.domo_instance}.domo.com/api/content/v2/users"
 
-    REDSHIFT = {
-        "filterType": "term",
-        "field": "data_flow_type",
-        "value": "MYSQL",
-        "name": "MYSQL",
-        "not": False,
-    }
+    return await gd.get_data(url=url, method="GET", auth=auth, debug_api=debug_api)
 
-    MAGICV2 = {
-        "filterType": "term",
-        "field": "data_flow_type",
-        "value": "MAGIC",
-        "name": "Magic ETL v2",
-        "not": False,
-    }
+# %% ../../nbs/routes/user.ipynb 9
+def generate_search_users_body_by_id(
+    user_ids: list[str],  # list of user ids to search
+) -> dict:  # dict to pass to search v1_users_search_api
+    """search v1_users_search_api"""
 
-    MAGIC = {
-        "filterType": "term",
-        "field": "data_flow_type",
-        "value": "ETL",
-        "name": "Magic ETL",
-        "not": False,
+    return {
+        # "showCount": true,
+        # "count": false,
+        "includeDeleted": False,
+        "includeSupport": False,
+        "filters": [
+            {"field": "id", "filterType": "value", "values": user_ids, "operator": "EQ"}
+        ],
     }
 
-# %% ../../nbs/routes/datacenter.ipynb 4
-class Datacenter_Filter_Field_Enum(Enum):
-    DATAPROVIDER = "dataprovidername_facet"
-
-
-def generate_search_datacenter_filter(field,  # use Datacenter_Filter_Field_Enum
-                                      value,
-                                      is_not: bool = False  # to handle exclusion
-                                      ):
+# %% ../../nbs/routes/user.ipynb 10
+def generate_search_users_body_by_email(
+    user_email_ls: list[ str ],  # list of user emails to search.  Note:  search does not appear to be case sensitive
+) -> dict:  # dict to pass to search v1_users_search_api
+    """search v1_users_search_api"""
 
     return {
-        "filterType": "term",
-        "field": field,
-        "value": value,
-        "not": is_not,
+        # "showCount": true,
+        # "count": false,
+        "includeDeleted": False,
+        "includeSupport": False,
+        "limit": 200,
+        "offset": 0,
+        "sort": {"field": "displayName", "order": "ASC"},
+        "filters": [
+            {
+                "filterType": "text",
+                "field": "emailAddress",
+                "text": " ".join(user_email_ls),
+            }
+        ],
     }
 
+# %% ../../nbs/routes/user.ipynb 11
+def process_v1_search_users(v1_user_ls: list[dict] # list of users from v1_users_search API
+) -> list[dict]: # sanitized list of users.
+    """sanitizes the response from v1_users_search API and removes unecessary attributes"""
 
-# %% ../../nbs/routes/datacenter.ipynb 6
-def generate_search_datacenter_filter_search_term(search_term):
-    # if not "*" in search_term:
-    #     search_term = f"*{search_term}*"
-
-    return {"field": "name_sort", "filterType": "wildcard", "query": search_term}
-
-
-# %% ../../nbs/routes/datacenter.ipynb 9
-def generate_search_datacenter_body(
-    search_text : str = None,
-    entity_type: Union[str, list] = "DATASET",  # can accept one entity_type or a list of entity_types
-    additional_filters_ls: list[dict] = None,
-    combineResults: bool = True,
-    limit: int = 100,
-    offset: int = 0,
-):
-    filters_ls = [generate_search_datacenter_filter_search_term(search_text)] if search_text else []
-    
-    if not isinstance(entity_type, list):
-        entity_type = [entity_type]
-
-    if additional_filters_ls:
-        if not isinstance(additional_filters_ls, list):
-            additional_filters_ls = [additional_filters_ls]
+    clean_users = []
+
+    for obj_user in v1_user_ls:
         
-        filters_ls += additional_filters_ls
-    
-    return {
-        "entities": entity_type,
-        "filters": filters_ls or [],
-        "combineResults": combineResults,
-        "query": "*",
-        "count": limit,
-        "offset": offset,
-    }
+        dd_user = dd.DictDot(obj_user)
 
-# %% ../../nbs/routes/datacenter.ipynb 12
-def generate_search_datacenter_account_body(
-    search_str: str, 
-    is_exact_match: bool = True
-):
-    return {
-        "count": 100,
-        "offset": 0,
-        "combineResults": False,
-        "query": search_str if is_exact_match else f"*{search_str}*",
-        "filters": [],
-        "facetValuesToInclude": [
-            "DATAPROVIDERNAME",
-            "OWNED_BY_ID",
-            "VALID",
-            "USED",
-            "LAST_MODIFIED_DATE",
-        ],
-        "queryProfile": "GLOBAL",
-        "entityList": [["account"]],
-        "sort": {"fieldSorts": [{"field": "display_name_sort", "sortOrder": "ASC"}]},
-    }
+        clean_users.append( {
+            "id": dd_user.id,
+            "displayName": dd_user.displayName,
+            "roleId": dd_user.roleId,
+            "userName": dd_user.userName,
+            "emailAddress": dd_user.emailAddress,
+        })
 
-# %% ../../nbs/routes/datacenter.ipynb 13
-class SearchDatacenter_NoResultsFound(de.DomoError):
-    def __init__(self, body, domo_instance):
-        super().__init__(message = body, domo_instance = domo_instance)
 
-async def search_datacenter(
+# %% ../../nbs/routes/user.ipynb 12
+async def search_users(
     auth: dmda.DomoAuth,
-    maximum: int = None,
-    
-    body: dict = None, # either pass a body or generate a body in the function using search_text, entity_type, and additional_filters parameters
-    
-    search_text = None,
-    entity_type: Union[str, list] = "dataset", # can accept one value or a list of values
-    additional_filters_ls = None,
-    
-    arr_fn: callable = None,
-    session: httpx.AsyncClient = None,
+    body: dict,
     debug_api: bool = False,
+    process_users: bool = True,
 ) -> rgd.ResponseGetData:
 
-    limit = 100  # api enforced limit
+    url = f"https://{auth.domo_instance}.domo.com/api/identity/v1/users/search"
 
-    if not body:
-        body = generate_search_datacenter_body(
-            entity_type=entity_type,
-            additional_filters_ls= additional_filters_ls,
-            search_text=search_text,
-            combineResults=False,
-            limit = limit 
-        )
-
-    if not arr_fn:
-        def arr_fn(res):
-            return res.response.get("searchObjects")
-
-    url = f"https://{auth.domo_instance}.domo.com/api/search/v1/query"
-
-    res = await gd.looper(
-        auth=auth,
-        session=session,
+    res = await gd.get_data(
         url=url,
-        body=body,
-        offset_params_in_body=True,
-        offset_params={"offset": "offset", "limit": "count"},
-        arr_fn=arr_fn,
         method="POST",
-        loop_until_end= True if not maximum else False,
-        maximum = maximum,
-        limit=limit,
+        auth=auth,
+        body=body,
         debug_api=debug_api,
     )
 
-    if res.is_success and len(res.response) == 0:
-        raise SearchDatacenter_NoResultsFound(body = body, domo_instance = auth.domo_instance)
+    if process_users and res.is_success:
+        res.response = process_v1_search_users(res.response.get('users'))
 
     return res
 
-# %% ../../nbs/routes/datacenter.ipynb 16
-async def get_lineage_upstream(
+
+# %% ../../nbs/routes/user.ipynb 16
+async def search_virtual_user_by_subscriber_instance(
+    auth: dmda.DomoAuth, # domo auth object
+    subscriber_instance_ls : list[str], # list of subscriber domo instances
+    debug_api: bool = False, # debug API requests
+) -> rgd.ResponseGetData: # list of virtual domo users
+    """retrieve virtual users for subscriber instances tied to one publisher"""
+
+    url = f"https://{auth.domo_instance}.domo.com/api/publish/v2/proxy_user/domain/"
+
+    body = {"domains": [f"{subscriber_instance}.domo.com"
+                        for subscriber_instance in subscriber_instance_ls]}
+
+    return await gd.get_data(
+        url=url,
+        method="POST",
+        auth=auth,
+        body=body,
+        debug_api=debug_api,
+    )
+
+# %% ../../nbs/routes/user.ipynb 20
+async def create_user(
     auth: dmda.DomoAuth,
-    entity_type: str,
-    entity_id: str,
-    session: httpx.AsyncClient = None,
+    display_name: str,
+    email: str,
+    role_id: int,
     debug_api: bool = False,
+) -> rgd.ResponseGetData:
+
+    url = f"https://{auth.domo_instance}.domo.com/api/content/v3/users"
+
+    body = {"displayName": display_name, "detail": {"email": email}, "roleId": role_id}
+
+    return await gd.get_data(
+        url=url, method="POST", body=body, auth=auth, debug_api=debug_api
+    )
+
+# %% ../../nbs/routes/user.ipynb 21
+async def set_user_landing_page(
+    auth: dmda.DomoAuth, user_id: str, page_id: str, debug_api: bool = False
 ):
-    url = f"https://{auth.domo_instance}.domo.com/api/data/v1/lineage/{entity_type}/{entity_id}"
 
-    params = {"traverseDown": "false"}
+    url = f"https://{auth.domo_instance}.domo.com/api/content/v1/landings/target/DESKTOP/entity/PAGE/id/{page_id}/{user_id}"
 
     return await gd.get_data(
+        url=url,
+        method="PUT",
         auth=auth,
-        method="GET",
+        # body = body,
+        debug=debug,
+    )
+
+# %% ../../nbs/routes/user.ipynb 22
+async def reset_password(
+    auth: dmda.DomoAuth,
+    user_id: str,
+    new_password: str,
+    debug_api: bool = False,
+) -> rgd.ResponseGetData:
+
+    url = f"https://{auth.domo_instance}.domo.com/api/identity/v1/password"
+
+    body = {"domoUserId": user_id, "password": new_password}
+
+    return await gd.get_data(
         url=url,
-        params=params,
-        session=session,
+        method="PUT",
+        auth=auth,
+        body=body,
         debug_api=debug_api,
     )
+
+# %% ../../nbs/routes/user.ipynb 23
+async def request_password_reset(
+    domo_instance: str, email: str, locale="en-us", debug_api: bool = False
+):
+    url = f"https://{domo_instance}.domo.com/api/domoweb/auth/sendReset"
+
+    params = {"email": email, "local": locale}
+
+    return await gd.get_data(
+        url=url, method="GET", params=params, auth=None, debug_api=debug_api
+    )
```

### Comparing `domolibrary-0.0.81/domolibrary/routes/dataset.py` & `domolibrary-0.0.9/domolibrary/routes/dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,30 +14,28 @@
 
 import httpx
 
 import domolibrary.client.get_data as gd
 import domolibrary.client.ResponseGetData as rgd
 import domolibrary.client.DomoAuth as dmda
 
-
 # %% ../../nbs/routes/dataset.ipynb 5
 class DatasetNotFoundError(Exception):
     def __init__(self, dataset_id, domo_instance):
         message = f"dataset - {dataset_id} not found in {domo_instance}"
 
         super().__init__(message)
 
 # %% ../../nbs/routes/dataset.ipynb 6
 class QueryRequestError(Exception):
     def __init__(self, dataset_id, domo_instance, sql):
         message = f"dataset - {dataset_id} in {domo_instance} received a bad request.  Check your SQL \n {sql}"
 
         super().__init__(message)
 
-
 # typically do not use
 async def query_dataset_public(
     dev_auth: dmda.DomoDeveloperAuth,
     dataset_id: str,
     sql: str,
     session: httpx.AsyncClient,
     debug_api: bool = False,
@@ -46,35 +44,29 @@
     """query for hitting public apis, requires client_id and secret authentication"""
 
     url = f"https://api.domo.com/v1/datasets/query/execute/{dataset_id}?IncludeHeaders=true"
 
     body = {"sql": sql}
 
     return await gd.get_data(
-        auth=dev_auth,
-        url=url,
-        method="POST",
-        body=body,
-        session=session,
-        debug_api=debug_api,
-    )
-
+        auth=dev_auth, url=url, method="POST", body=body, session=session, debug_api=debug_api)
+        
 
+        
 async def query_dataset_private(
     auth: dmda.DomoAuth,  # DomoFullAuth or DomoTokenAuth
     dataset_id: str,
     sql: str,
     session: Optional[httpx.AsyncClient] = None,
     loop_until_end: bool = False,  # retrieve all available rows
     limit=100,  # maximum rows to return per request.  refers to PAGINATION
     skip=0,
     maximum=100,  # equivalent to the LIMIT or TOP clause in SQL, the number of rows to return total
     debug_api: bool = False,
     debug_loop: bool = False,
-    timeout :int = 10
 ):
     """execute SQL queries against private APIs, requires DomoFullAuth or DomoTokenAuth"""
 
     url = f"https://{auth.domo_instance}.domo.com/api/query/v1/execute/{dataset_id}"
 
     offset_params = {
         "offset": "offset",
@@ -105,145 +97,140 @@
         limit=limit,
         skip=skip,
         maximum=maximum,
         session=session,
         body_fn=body_fn,
         debug_api=debug_api,
         debug_loop=debug_loop,
-        loop_until_end=loop_until_end,
-        timeout = timeout
+        loop_until_end=loop_until_end
     )
 
-    if res.status == 404 and res.response == "Not Found":
-        raise DatasetNotFoundError(
-            dataset_id=dataset_id, domo_instance=auth.domo_instance
-        )
-
-    if res.status == 400 and res.response == "Bad Request":
-        raise QueryRequestError(
-            dataset_id=dataset_id, domo_instance=auth.domo_instance, sql=sql
-        )
-
+    if res.status == 404 and res.response == 'Not Found':
+        raise DatasetNotFoundError(dataset_id=dataset_id , domo_instance=auth.domo_instance)
+    
+    if res.status == 400 and res.response == 'Bad Request':
+        raise QueryRequestError(dataset_id=dataset_id , domo_instance=auth.domo_instance, sql = sql)
+    
     return res
 
+
 # %% ../../nbs/routes/dataset.ipynb 9
 async def get_dataset_by_id(
-    dataset_id: str,  # dataset id from URL
-    auth: Optional[dmda.DomoAuth] = None,  # requires full authentication
-    debug_api: bool = False,  # for troubleshooting API request
-    session: Optional[httpx.AsyncClient] = None,
-) -> rgd.ResponseGetData:  # returns metadata about a dataset
+    dataset_id: str, # dataset id from URL
+    auth: Optional[dmda.DomoAuth] = None, # requires full authentication
+    debug_api: bool = False, # for troubleshooting API request
+    session: Optional[httpx.AsyncClient] = None
+) -> rgd.ResponseGetData: # returns metadata about a dataset
     """retrieve dataset metadata"""
 
     url = f"https://{auth.domo_instance}.domo.com/api/data/v3/datasources/{dataset_id}"
 
-    res = await gd.get_data(
-        auth=auth, url=url, method="GET", debug_api=debug_api, session=session
+    res= await gd.get_data(
+        auth=auth,
+        url=url,
+        method="GET",
+        debug_api=debug_api, session = session
     )
 
-    if res.status == 404 and res.response == "Not Found":
-        raise DatasetNotFoundError(
-            dataset_id=dataset_id, domo_instance=auth.domo_instance
-        )
+    if res.status == 404 and res.response == 'Not Found':
+        raise DatasetNotFoundError(dataset_id=dataset_id, domo_instance=auth.domo_instance)
 
     return res
 
 # %% ../../nbs/routes/dataset.ipynb 12
 async def get_schema(
     auth: dmda.DomoAuth, dataset_id: str, debug_api: bool = False
 ) -> rgd.ResponseGetData:
     """retrieve the schema for a dataset"""
 
     url = f"https://{auth.domo_instance}.domo.com/api/query/v1/datasources/{dataset_id}/schema/indexed?includeHidden=false"
 
     return await gd.get_data(auth=auth, url=url, method="GET", debug_api=debug_api)
 
-# %% ../../nbs/routes/dataset.ipynb 16
-async def set_dataset_tags(
-    auth: dmda.DomoFullAuth,
-    tag_ls: [str],  # complete list of tags for dataset
-    dataset_id: str,
-    debug_api: bool = False,
-    session: Optional[httpx.AsyncClient] = None,
-    return_raw: bool = False,
-):
 
+# %% ../../nbs/routes/dataset.ipynb 16
+async def set_dataset_tags(auth: dmda.DomoFullAuth,
+                           tag_ls: [str], # complete list of tags for dataset
+                           dataset_id: str,
+                           debug_api: bool = False,
+                           session: Optional[httpx.AsyncClient] = None,
+                           return_raw : bool = False
+                           ):
+    
     """REPLACE tags on this dataset with a new list"""
 
     url = f"https://{auth.domo_instance}.domo.com/api/data/ui/v3/datasources/{dataset_id}/tags"
 
     res = await gd.get_data(
         auth=auth,
         url=url,
-        method="POST",
+        method='POST',
         debug_api=debug_api,
         body=tag_ls,
         session=session,
-        return_raw=return_raw,
+        return_raw = return_raw
     )
 
     if return_raw:
         return res
 
     if res.status == 200:
-        res.set_response(
-            response=f'Dataset {dataset_id} tags updated to [{ ", ".join(tag_ls) }]'
-        )
-
+        res.set_response (response = f'Dataset {dataset_id} tags updated to [{ ", ".join(tag_ls) }]')
+    
     return res
 
+
 # %% ../../nbs/routes/dataset.ipynb 19
 class UploadDataError(Exception):
     """raise if unable to upload data to Domo"""
-
-    def __init__(self, stage_num: int, dataset_id: str, domo_instance: str):
+    
+    def __init__(self, stage_num : int, dataset_id : str, domo_instance : str):
         message = f"error uploading data to {dataset_id} during Stage { stage_num} in {domo_instance}"
         super().__init__(message)
 
 # %% ../../nbs/routes/dataset.ipynb 20
-async def upload_dataset_stage_1(
-    auth: dmda.DomoAuth,
-    dataset_id: str,
-    #  restate_data_tag: str = None, # deprecated
-    partition_tag: str = None,  # synonymous with data_tag
-    session: Optional[httpx.AsyncClient] = None,
-    debug_api: bool = False,
-) -> rgd.ResponseGetData:
+async def upload_dataset_stage_1(auth: dmda.DomoAuth,
+                                 dataset_id: str,
+                                 #  restate_data_tag: str = None, # deprecated
+                                 partition_tag: str = None,  # synonymous with data_tag
+                                 session: Optional[httpx.AsyncClient] = None,
+                                 debug_api: bool = False,
+                                 ) -> rgd.ResponseGetData:
 
     """preps dataset for upload by creating an upload_id (upload session key) pass to stage 2 as a parameter"""
 
     url = f"https://{auth.domo_instance}.domo.com/api/data/v3/datasources/{dataset_id}/uploads"
 
     # base body assumes no paritioning
-    body = {"action": None, "appendId": None}
+    body = {
+        "action": None,
+        "appendId": None
+    }
 
     params = None
 
     if partition_tag:
         # params = {'dataTag': restate_data_tag or data_tag} # deprecated
-        params = {"dataTag": partition_tag}
-        body.update({"appendId": "latest"})
+        params = {'dataTag': partition_tag}
+        body.update({'appendId': 'latest'})
 
-    res = await gd.get_data(
-        auth=auth,
-        url=url,
-        method="POST",
-        body=body,
-        session=session,
-        debug_api=debug_api,
-        params=params,
-    )
+    res = await gd.get_data(auth=auth,
+                         url=url, method='POST',
+                         body=body,
+                         session=session,
+                         debug_api=debug_api,
+                         params=params)
 
     if not res.is_success:
         raise UploadDataError(
-            stage_num=1, dataset_id=dataset_id, domo_instance=auth.domo_instance
-        )
+            stage_num=1, dataset_id=dataset_id, domo_instance=auth.domo_instance)
 
     return res
 
+
 # %% ../../nbs/routes/dataset.ipynb 21
 async def upload_dataset_stage_2_file(
     auth: dmda.DomoAuth,
     dataset_id: str,
     upload_id: str,  # must originate from  a stage_1 upload response
     data_file: Optional[io.TextIOWrapper] = None,
     session: Optional[httpx.AsyncClient] = None,
@@ -262,17 +249,15 @@
         auth=auth,
         content_type="text/csv",
         body=body,
         session=session,
         debug_api=debug_api,
     )
     if not res.is_success:
-        raise UploadDataError(
-            stage_num=2, dataset_id=dataset_id, domo_instance=auth.domo_instance
-        )
+        raise UploadDataError(stage_num = 2 , dataset_id = dataset_id, domo_instance = auth.domo_instance)
 
     res.upload_id = upload_id
     res.dataset_id = dataset_id
     res.part_id = part_id
 
     return res
 
@@ -301,17 +286,15 @@
         content_type="text/csv",
         body=body,
         session=session,
         debug_api=debug_api,
     )
 
     if not res.is_success:
-        raise UploadDataError(
-            stage_num=2, dataset_id=dataset_id, domo_instance=auth.domo_instance
-        )
+        raise UploadDataError(stage_num = 2 , dataset_id = dataset_id, domo_instance = auth.domo_instance)
 
     res.upload_id = upload_id
     res.dataset_id = dataset_id
     res.part_id = part_id
 
     return res
 
@@ -346,173 +329,161 @@
                 "dataTag": partition_tag,
                 "appendId": "latest" if partition_tag else None,
                 "index": is_index,
             }
         )
 
     res = await gd.get_data(
-        auth=auth,
-        method="PUT",
-        url=url,
-        body=body,
-        session=session,
-        debug_api=debug_api,
+        auth=auth, method="PUT", url=url, body=body, session=session, debug_api=debug_api
     )
 
     if not res.is_success:
-        raise UploadDataError(
-            stage_num=3, dataset_id=dataset_id, domo_instance=auth.domo_instance
-        )
+        raise UploadDataError(stage_num = 3 , dataset_id = dataset_id, domo_instance = auth.domo_instance)
 
     res.upload_id = upload_id
     res.dataset_id = dataset_id
 
     return res
 
-# %% ../../nbs/routes/dataset.ipynb 25
+# %% ../../nbs/routes/dataset.ipynb 24
 async def index_dataset(
     auth: dmda.DomoAuth,
     dataset_id: str,
     session: Optional[httpx.AsyncClient] = None,
     debug_api: bool = False,
 ) -> rgd.ResponseGetData:
     """manually index a dataset"""
 
     url = f"https://{auth.domo_instance}.domo.com/api/data/v3/datasources/{dataset_id}/indexes"
 
     body = {"dataIds": []}
 
     return await gd.get_data(
-        auth=auth,
-        method="POST",
-        body=body,
-        url=url,
-        session=session,
-        debug_api=debug_api,
+        auth=auth, method="POST", body=body, url=url, session=session, debug_api = debug_api
     )
 
-# %% ../../nbs/routes/dataset.ipynb 26
+# %% ../../nbs/routes/dataset.ipynb 25
 async def index_status(
     auth: dmda.DomoAuth,
     dataset_id: str,
     index_id: str,
     session: Optional[httpx.AsyncClient] = None,
     debug_api: bool = False,
 ) -> rgd.ResponseGetData:
     """get the completion status of an index"""
 
     url = f"https://{auth.domo_instance}.domo.com/api/data/v3/datasources/{dataset_id}/indexes/{index_id}/statuses"
 
     return await gd.get_data(
-        auth=auth, method="GET", url=url, session=session, debug_api=debug_api
+        auth=auth, 
+        method="GET", url=url, 
+        session=session, debug_api=debug_api
     )
 
-# %% ../../nbs/routes/dataset.ipynb 28
+
+# %% ../../nbs/routes/dataset.ipynb 27
 def generate_list_partitions_body(limit=100, offset=0):
     return {
-        "paginationFields": [
-            {
-                "fieldName": "datecompleted",
-                "sortOrder": "DESC",
-                "filterValues": {"MIN": None, "MAX": None},
+        "paginationFields": [{
+            "fieldName": "datecompleted",
+            "sortOrder": "DESC",
+            "filterValues": {
+                "MIN": None,
+                "MAX": None
             }
-        ],
-        "limit": limit,
-        "offset": offset,
+        }],
+        "limit": 1000,
+        "offset": 0
     }
 
 
-async def list_partitions(
-    auth: dmda.DomoAuth,
-    dataset_id: str,
-    body: dict = None,
-    session: httpx.AsyncClient = None,
-    debug_api: bool = False,
-    debug_loop: bool = False,
-):
+async def list_partitions(auth: dmda.DomoAuth,
+                          dataset_id: str,
+                          body: dict = None,
+                          session: httpx.AsyncClient = None,
+                          debug_api: bool = False,
+                          debug_loop: bool = False,
+
+
+                          ):
 
     body = body or generate_list_partitions_body()
 
     url = f"https://{auth.domo_instance}.domo.com/api/query/v1/datasources/{dataset_id}/partition/list"
 
     offset_params = {
-        "offset": "offset",
-        "limit": "limit",
+        'offset': 'offset',
+        'limit': 'limit',
     }
 
     def arr_fn(res) -> list[dict]:
         return res.response
 
-    res = await gd.looper(
-        auth=auth,
-        method="POST",
-        url=url,
-        arr_fn=arr_fn,
-        body=body,
-        offset_params_in_body=True,
-        offset_params=offset_params,
-        loop_until_end=True,
-        session=session,
-        debug_loop=debug_loop,
-        debug_api=debug_api,
-    )
+    res = await gd.looper(auth=auth,
+                       method='POST',
+                       url=url,
+                       arr_fn=arr_fn,
+                       body=body,
+                       offset_params_in_body=True,
+                       offset_params=offset_params,
+                       loop_until_end=True,
+                       session=session,
+                       debug_loop=debug_loop,
+                       debug_api = debug_api)
 
-    if res.status == 404 and res.response == "Not Found":
+    if res.status == 404 and res.response == 'Not Found':
         raise DatasetNotFoundError(
-            dataset_id=dataset_id, domo_instance=auth.domo_instance
-        )
+            dataset_id=dataset_id, domo_instance=auth.domo_instance)
     return res
 
-# %% ../../nbs/routes/dataset.ipynb 30
-def generate_create_dataset_body(
-    dataset_name: str, dataset_type: str = "API", schema: dict = None
+
+# %% ../../nbs/routes/dataset.ipynb 29
+def generate_create_dataset_body(dataset_name: str, dataset_type: str = 'API', schema: dict = {
+    "columns": [
+        {"type": "STRING", "name": "Friend"},
+        {"type": "STRING",  "name": "Attending"}
+    ]}
 ):
-    schema = schema or {
-        "columns": [
-            {"type": "STRING", "name": "Friend"},
-            {"type": "STRING", "name": "Attending"},
-        ]
-    }
 
     return {
         "userDefinedType": dataset_type,
         "dataSourceName": dataset_name,
-        "schema": schema,
+        "schema": schema
     }
 
 
-async def create(
-    auth: dmda.DomoAuth,
-    dataset_name: str,
-    dataset_type: str = "api",
-    session: httpx.AsyncClient = None,
-    schema: dict = None,
-    debug_api: bool = False,
-):
-
-    body = generate_create_dataset_body(
-        dataset_name=dataset_name, dataset_type=dataset_type, schema=schema
-    )
+async def create(auth: dmda.DomoAuth,
+                 dataset_name: str,
+                 dataset_type: str = 'api',
+                 session: httpx.AsyncClient = None,
+                 schema: dict = None,
+                 debug_api: bool = False):
+
+    body = generate_create_dataset_body(dataset_name=dataset_name,
+                                        dataset_type=dataset_type,
+                                        schema=schema)
 
     url = f"https://{auth.domo_instance}.domo.com/api/data/v2/datasources"
 
     return await gd.get_data(
         auth=auth,
         method="POST",
         url=url,
         body=body,
         session=session,
-        debug_api=debug_api,
+        debug_api=debug_api
     )
 
-# %% ../../nbs/routes/dataset.ipynb 35
-async def delete(
-    auth: dmda.DomoAuth,
-    dataset_id: str,
-    session: httpx.AsyncClient = None,
-    debug_api: bool = False,
-):
+
+# %% ../../nbs/routes/dataset.ipynb 34
+async def delete(auth: dmda.DomoAuth,
+                 dataset_id: str, session: httpx.AsyncClient = None, debug_api: bool = False):
     url = f"https://{auth.domo_instance}.domo.com/api/data/v3/datasources/{dataset_id}?deleteMethod=hard"
 
     return await gd.get_data(
-        auth=auth, method="DELETE", url=url, session=session, debug_api=debug_api
+        auth=auth,
+        method="DELETE",
+        url=url,
+        session=session,
+        debug_api=debug_api
     )
+
```

### Comparing `domolibrary-0.0.81/domolibrary.egg-info/PKG-INFO` & `domolibrary-0.0.9/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domolibrary
-Version: 0.0.81
+Version: 0.0.9
 Summary: UNKNOWN
 Home-page: https://github.com/jaewilson07/domo_library
 Author: Jae Wilson
 Author-email: jaewilson07@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
@@ -42,15 +42,15 @@
 ## Install
 
 The DataCrew team is hard at work expanding the list of available
 `classes` and `routes`. We have a ton of work completed, it’s just a
 matter of migrating and documenting the code into this library.
 
 ``` sh
-pip install domolibrary
+pip install domo_library
 ```
 
 ## How to use
 
 ### Authentication
 
 For each task, consider the appropriate
@@ -72,15 +72,15 @@
 auth objects.
 
 ``` python
 # configure an auth method
 import os
 import domolibrary.client.DomoAuth as dmda
 
-token_auth = dmda.DomoTokenAuth( domo_instance = 'domo-community', domo_access_token = os.environ['DOMO_DOJO_ACCESS_TOKEN'])
+token_auth = dmda.DomoTokenAuth( domo_instance = 'domo-dojoo', domo_access_token = os.environ['DOMO_DOJO_ACCESS_TOKEN'])
 ```
 
 ### Option 1: class based programming
 
 In this project domo entities,
 [`DomoActivityLog`](https://jaewilson07.github.io/domo_library/classes/domoactivitylog.html#domoactivitylog),
 [`DomoDataset`](https://jaewilson07.github.io/domo_library/classes/domodataset.html#domodataset)
@@ -96,21 +96,23 @@
 [`DomoDataset.get_from_id`](https://jaewilson07.github.io/domo_library/classes/domodataset.html#domodataset.get_from_id)
 is a classmethod.
 
 Note: DomoLibrary uses the asynchronous `aiohttp` requests library to
 offer users the ability to write concurrently executing code.
 
 ``` python
-# import domolibrary.classes.DomoDataset as dmds
+import domolibrary.classes.DomoDataset as dmds
 
-# # this is a class method
-# domo_ds = await dmds.DomoDataset.get_from_id(auth=token_auth, dataset_id=os.environ['DOJO_DATASET_ID'])
-# domo_ds
+# this is a class method
+domo_ds = await dmds.DomoDataset.get_from_id(auth = token_auth, dataset_id = os.environ['DOJO_DATASET_ID'])
+domo_ds
 ```
 
+    DomoDataset(id='04c1574e-c8be-4721-9846-c6ffa491144b', display_type='domo-jupyterdata', data_provider_type='domo-jupyterdata', name='domo_kbs', description=None, row_count=1185, column_count=7, stream_id=825, owner=DictDot(id='1893952720', name='Jae Wilson', type='USER', group=False), formula=DictDot(), schema=DomoDataset_Schema(dataset=..., columns=[]))
+
 Once instantiated, you can call methods to interact with that object.
 You typically won’t have to pass auth creds again because they are saved
 to the object.
 
 In the example below we are retrieving the
 [`DomoDataset_Schema`](https://jaewilson07.github.io/domo_library/classes/domodataset.html#domodataset_schema)
 which consists of subclass
@@ -120,23 +122,47 @@
 method.
 
 We take the approach of where possible converting dictionaries from Domo
 APIs into classes because it provides greater predictability when users
 are creating integrations between platforms (ex. Domo to Trello).
 
 ``` python
-# await domo_ds.schema.get()
+await domo_ds.schema.get()
 ```
 
+    [DomoDataset_Schema_Column(name='objectID', id='objectID', type='STRING'),
+     DomoDataset_Schema_Column(name='url', id='url', type='STRING'),
+     DomoDataset_Schema_Column(name='Title', id='Title', type='STRING'),
+     DomoDataset_Schema_Column(name='article', id='article', type='STRING'),
+     DomoDataset_Schema_Column(name='views', id='views', type='LONG'),
+     DomoDataset_Schema_Column(name='created_dt', id='created_dt', type='DATETIME'),
+     DomoDataset_Schema_Column(name='published_dt', id='published_dt', type='DATETIME')]
+
 Typically all information about an entity is saved in the object
 
 ``` python
-# domo_ds.__dict__
+domo_ds.__dict__
 ```
 
+    {'auth': DomoTokenAuth(domo_instance='domo-dojoo', token_name='token_auth', url_manual_login='https://domo-dojoo.domo.com/auth/index?domoManualLogin=true'),
+     'id': '04c1574e-c8be-4721-9846-c6ffa491144b',
+     'display_type': 'domo-jupyterdata',
+     'data_provider_type': 'domo-jupyterdata',
+     'name': 'domo_kbs',
+     'description': None,
+     'row_count': 1185,
+     'column_count': 7,
+     'stream_id': 825,
+     'owner': namespace(id='1893952720',
+               name='Jae Wilson',
+               type='USER',
+               group=False),
+     'formula': namespace(),
+     'schema': DomoDataset_Schema(dataset=DomoDataset(id='04c1574e-c8be-4721-9846-c6ffa491144b', display_type='domo-jupyterdata', data_provider_type='domo-jupyterdata', name='domo_kbs', description=None, row_count=1185, column_count=7, stream_id=825, owner=DictDot(id='1893952720', name='Jae Wilson', type='USER', group=False), formula=DictDot(), schema=...), columns=[DomoDataset_Schema_Column(name='objectID', id='objectID', type='STRING'), DomoDataset_Schema_Column(name='url', id='url', type='STRING'), DomoDataset_Schema_Column(name='Title', id='Title', type='STRING'), DomoDataset_Schema_Column(name='article', id='article', type='STRING'), DomoDataset_Schema_Column(name='views', id='views', type='LONG'), DomoDataset_Schema_Column(name='created_dt', id='created_dt', type='DATETIME'), DomoDataset_Schema_Column(name='published_dt', id='published_dt', type='DATETIME')])}
+
 ### Option 2 functional programming
 
 Although classes add a pretty wrapper for interacting with Domo APIs,
 users can opt to interact directly with APIs by way of `routes`.
 
 All route functions will exclusively call one API and will always return
 a
```

### Comparing `domolibrary-0.0.81/domolibrary.egg-info/SOURCES.txt` & `domolibrary-0.0.9/domolibrary.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -69,56 +69,34 @@
 domolibrary.egg-info/entry_points.txt
 domolibrary.egg-info/not-zip-safe
 domolibrary.egg-info/requires.txt
 domolibrary.egg-info/top_level.txt
 domolibrary/classes/DomoAccount.py
 domolibrary/classes/DomoActivityLog.py
 domolibrary/classes/DomoBootstrap.py
-domolibrary/classes/DomoDatacenter.py
-domolibrary/classes/DomoDataflow.py
 domolibrary/classes/DomoDataset.py
-domolibrary/classes/DomoGrant.py
-domolibrary/classes/DomoGroup.py
-domolibrary/classes/DomoInstanceConfig.py
-domolibrary/classes/DomoPDP.py
 domolibrary/classes/DomoPage.py
-domolibrary/classes/DomoPublish.py
-domolibrary/classes/DomoRole.py
 domolibrary/classes/DomoUser.py
 domolibrary/classes/__init__.py
 domolibrary/client/DomoAuth.py
-domolibrary/client/DomoError.py
 domolibrary/client/Logger.py
 domolibrary/client/ResponseGetData.py
 domolibrary/client/__init__.py
 domolibrary/client/get_data.py
 domolibrary/integrations/DomoJupyter.py
 domolibrary/integrations/__init__.py
 domolibrary/routes/__init__.py
 domolibrary/routes/account.py
 domolibrary/routes/activity_log.py
 domolibrary/routes/bootstrap.py
-domolibrary/routes/card.py
-domolibrary/routes/datacenter.py
-domolibrary/routes/dataflow.py
 domolibrary/routes/dataset.py
-domolibrary/routes/grant.py
-domolibrary/routes/group.py
-domolibrary/routes/instance_config.py
-domolibrary/routes/page.py
-domolibrary/routes/pdp.py
-domolibrary/routes/publish.py
-domolibrary/routes/role.py
 domolibrary/routes/user.py
 domolibrary/utils/DictDot.py
 domolibrary/utils/__init__.py
-domolibrary/utils/chunk_execution.py
 domolibrary/utils/convert.py
-domolibrary/utils/read_creds_from_dotenv.py
-domolibrary/utils/upload_data.py
 utils/Base.py
 utils/DictDot.py
 utils/Exceptions.py
 utils/LoggerClass.py
 utils/ResponseGetData.py
 utils/__init__.py
 utils/chunk_execution.py
```

### Comparing `domolibrary-0.0.81/settings.ini` & `domolibrary-0.0.9/settings.ini`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = domo_library
 lib_name = domolibrary
-version = 0.0.81
+version = 0.0.9
 min_python = 3.7
 license = apache2
 
 ### nbdev ###
 doc_path = _docs
 lib_path = domolibrary
 nbs_path = nbs
@@ -21,23 +21,23 @@
 branch = main
 custom_sidebar = False
 doc_host = https://%(user)s.github.io
 doc_baseurl = /%(repo)s
 git_url = https://github.com/%(user)s/%(repo)s
 title = %(lib_name)s
 
-### PyPI ###git add.
+### PyPI ###
 audience = Developers
 author = Jae Wilson
 author_email = jaewilson07@gmail.com
-copyright = 2022 onwards, %(author)sjaewi
+copyright = 2022 onwards, %(author)s
 description = 
 keywords = nbdev jupyter notebook python
 language = English
 status = 3
 user = jaewilson07
 
 ### Optional ###
-requirements = nbdev fastcore pandas aiohttp requests twine orjson httpx python-dotenv sqlparse sql_metadata bs4
+requirements = nbdev fastcore pandas aiohttp requests twine orjson httpx
 conda_requirements = https://domo-conda-prod.s3.amazonaws.com/domo::domojupyter
 # dev_requirements = 
-# console_scripts =
+# console_scripts =
```

### Comparing `domolibrary-0.0.81/setup.py` & `domolibrary-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.81/utils/Base.py` & `domolibrary-0.0.9/utils/Base.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.81/utils/DictDot.py` & `domolibrary-0.0.9/utils/DictDot.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.81/utils/Exceptions.py` & `domolibrary-0.0.9/utils/Exceptions.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.81/utils/LoggerClass.py` & `domolibrary-0.0.9/utils/LoggerClass.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.81/utils/chunk_execution.py` & `domolibrary-0.0.9/utils/chunk_execution.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.81/utils/consol_get_creds.py` & `domolibrary-0.0.9/utils/consol_get_creds.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.81/utils/convert.py` & `domolibrary-0.0.9/utils/convert.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.81/utils/read_creds_from_dotenv.py` & `domolibrary-0.0.9/utils/read_creds_from_dotenv.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.81/utils/upload_data.py` & `domolibrary-0.0.9/utils/upload_data.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,26 @@
-import asyncio
-
 import aiohttp
 import pandas as pd
+import asyncio
 
-import domolibrary.client.Logger as lc
-
+import Library.utils.LoggerClass as lc
 
 async def upload_data(instance_auth,
                       consol_auth,
                       data_fn,
                       consol_ds,
                       is_index: bool = False,
                       debug: bool = False,
                       debug_prn: bool = False,
-                      logger: lc.Logger = None):
+                      logger: lc.MyLogger = None):
 
     try:
         # await asyncio.sleep(randrange(5))
-        if logger:
-            logger.log_info(
-                f" Upload_data function - starting {instance_auth.domo_instance} - {data_fn.__name__}")
+        if logger : 
+            logger.log_info (f" Upload_data function - starting {instance_auth.domo_instance} - {data_fn.__name__}")
         if debug_prn:
             print(
                 f"starting {instance_auth.domo_instance} - {data_fn.__name__}")
 
         instance_session = aiohttp.ClientSession()
 
         upload_df = await data_fn(instance_auth, instance_session)
@@ -37,15 +34,15 @@
                                           full_auth=consol_auth,
                                           upload_method='APPEND',
                                           partition_key=instance_auth.domo_instance,
                                           is_index=is_index)
 
     except Exception as e:
         print(f"upload_data : unexpected error: {e}")
-        if logger:
+        if logger : 
             logger.log_error(f"upload_data : unexpected error: {e}")
         return None
 
     finally:
         await instance_session.close()
```

