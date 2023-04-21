# Comparing `tmp/dbm-agent-8.32.8.tar.gz` & `tmp/dbm-agent-8.33.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbm-agent-8.32.8.tar", last modified: Tue Apr 11 08:47:11 2023, max compression
+gzip compressed data, was "dbm-agent-8.33.0.tar", last modified: Fri Apr 21 09:08:54 2023, max compression
```

## Comparing `dbm-agent-8.32.8.tar` & `dbm-agent-8.33.0.tar`

### file list

```diff
@@ -1,96 +1,100 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 08:47:11.970536 dbm-agent-8.32.8/
--rw-r--r--   0 root         (0) root         (0)      651 2023-04-11 08:47:11.970536 dbm-agent-8.32.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4333 2023-04-07 08:20:26.000000 dbm-agent-8.32.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 08:47:11.955536 dbm-agent-8.32.8/bin/
--rw-r--r--   0 root         (0) root         (0)      898 2023-04-11 03:20:19.000000 dbm-agent-8.32.8/bin/dbm-agent
--rw-r--r--   0 root         (0) root         (0)      322 2023-04-06 12:14:18.000000 dbm-agent-8.32.8/bin/dbm-bt-conn-stack
--rw-r--r--   0 root         (0) root         (0)      794 2023-04-11 03:20:38.000000 dbm-agent-8.32.8/bin/dbma-cli-init
--rw-r--r--   0 root         (0) root         (0)     2613 2023-04-11 08:35:08.000000 dbm-agent-8.32.8/bin/dbma-cli-single-instance
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 08:47:11.956536 dbm-agent-8.32.8/dbm_agent.egg-info/
--rw-r--r--   0 root         (0) root         (0)      651 2023-04-11 08:47:11.000000 dbm-agent-8.32.8/dbm_agent.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2455 2023-04-11 08:47:11.000000 dbm-agent-8.32.8/dbm_agent.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 08:47:11.000000 dbm-agent-8.32.8/dbm_agent.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      106 2023-04-11 08:47:11.000000 dbm-agent-8.32.8/dbm_agent.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      162 2023-04-11 08:47:11.000000 dbm-agent-8.32.8/dbm_agent.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 08:47:11.956536 dbm-agent-8.32.8/dbma/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 02:17:13.000000 dbm-agent-8.32.8/dbma/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 08:47:11.957536 dbm-agent-8.32.8/dbma/bil/
--rw-r--r--   0 root         (0) root         (0)      104 2023-04-07 07:23:15.000000 dbm-agent-8.32.8/dbma/bil/__init__.py
--rw-r--r--   0 root         (0) root         (0)      411 2023-04-07 07:23:15.000000 dbm-agent-8.32.8/dbma/bil/cmdexecutor.py
--rw-r--r--   0 root         (0) root         (0)     3740 2023-04-07 07:23:16.000000 dbm-agent-8.32.8/dbma/bil/daemon.py
--rw-r--r--   0 root         (0) root         (0)     1891 2023-04-07 07:23:16.000000 dbm-agent-8.32.8/dbma/bil/fs.py
--rw-r--r--   0 root         (0) root         (0)      225 2023-04-07 07:23:16.000000 dbm-agent-8.32.8/dbma/bil/fun.py
--rw-r--r--   0 root         (0) root         (0)      700 2023-04-10 03:49:50.000000 dbm-agent-8.32.8/dbma/bil/net.py
--rw-r--r--   0 root         (0) root         (0)     5900 2023-04-07 07:23:16.000000 dbm-agent-8.32.8/dbma/bil/osuser.py
--rw-r--r--   0 root         (0) root         (0)      542 2023-04-07 07:23:16.000000 dbm-agent-8.32.8/dbma/bil/sudos.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 08:47:11.958536 dbm-agent-8.32.8/dbma/components/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-28 02:20:28.000000 dbm-agent-8.32.8/dbma/components/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 08:47:11.959536 dbm-agent-8.32.8/dbma/components/mysql/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-28 02:20:47.000000 dbm-agent-8.32.8/dbma/components/mysql/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5674 2023-04-11 08:23:03.000000 dbm-agent-8.32.8/dbma/components/mysql/commons.py
--rw-r--r--   0 root         (0) root         (0)    20949 2023-04-11 03:12:09.000000 dbm-agent-8.32.8/dbma/components/mysql/config.py
--rw-r--r--   0 root         (0) root         (0)      473 2023-04-07 07:23:16.000000 dbm-agent-8.32.8/dbma/components/mysql/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    15140 2023-04-11 07:41:26.000000 dbm-agent-8.32.8/dbma/components/mysql/install.py
--rw-r--r--   0 root         (0) root         (0)      646 2023-04-07 07:23:16.000000 dbm-agent-8.32.8/dbma/components/mysql/instance.py
--rw-r--r--   0 root         (0) root         (0)     3996 2023-04-11 08:39:21.000000 dbm-agent-8.32.8/dbma/components/mysql/replica.py
--rw-r--r--   0 root         (0) root         (0)      849 2023-04-11 08:19:15.000000 dbm-agent-8.32.8/dbma/components/mysql/source.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 08:47:11.960536 dbm-agent-8.32.8/dbma/components/mysql/views/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-29 08:25:42.000000 dbm-agent-8.32.8/dbma/components/mysql/views/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9589 2023-04-11 07:58:31.000000 dbm-agent-8.32.8/dbma/components/mysql/views/defaultsview.py
--rw-r--r--   0 root         (0) root         (0)     3519 2023-04-11 08:12:23.000000 dbm-agent-8.32.8/dbma/components/mysql/views/handlers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 08:47:11.960536 dbm-agent-8.32.8/dbma/components/redis/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-28 02:21:47.000000 dbm-agent-8.32.8/dbma/components/redis/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 08:47:11.961536 dbm-agent-8.32.8/dbma/core/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-11 07:21:13.000000 dbm-agent-8.32.8/dbma/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 08:47:11.962536 dbm-agent-8.32.8/dbma/core/agent/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-10 06:58:11.000000 dbm-agent-8.32.8/dbma/core/agent/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2094 2023-04-07 07:23:16.000000 dbm-agent-8.32.8/dbma/core/agent/init.py
--rw-r--r--   0 root         (0) root         (0)      117 2023-04-07 07:23:16.000000 dbm-agent-8.32.8/dbma/core/agent/upgrade.py
--rw-r--r--   0 root         (0) root         (0)     3535 2023-04-07 07:23:17.000000 dbm-agent-8.32.8/dbma/core/configs.py
--rw-r--r--   0 root         (0) root         (0)      103 2023-04-07 07:23:16.000000 dbm-agent-8.32.8/dbma/core/exception.py
--rw-r--r--   0 root         (0) root         (0)     2263 2023-04-07 07:23:17.000000 dbm-agent-8.32.8/dbma/core/httpserver.py
--rw-r--r--   0 root         (0) root         (0)      688 2023-04-07 07:23:17.000000 dbm-agent-8.32.8/dbma/core/messages.py
--rw-r--r--   0 root         (0) root         (0)      102 2023-04-07 07:23:17.000000 dbm-agent-8.32.8/dbma/core/router.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 08:47:11.963536 dbm-agent-8.32.8/dbma/core/threads/
--rw-r--r--   0 root         (0) root         (0)       90 2023-04-07 07:23:17.000000 dbm-agent-8.32.8/dbma/core/threads/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1987 2023-04-07 07:23:17.000000 dbm-agent-8.32.8/dbma/core/threads/backends.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 08:47:11.965536 dbm-agent-8.32.8/dbma/core/views/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-09 09:18:42.000000 dbm-agent-8.32.8/dbma/core/views/__init__.py
--rw-r--r--   0 root         (0) root         (0)      455 2023-04-07 07:23:17.000000 dbm-agent-8.32.8/dbma/core/views/dbmagentview.py
--rw-r--r--   0 root         (0) root         (0)      466 2023-04-07 07:23:17.000000 dbm-agent-8.32.8/dbma/core/views/response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 08:47:11.954536 dbm-agent-8.32.8/dbma/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 08:47:11.970536 dbm-agent-8.32.8/dbma/static/cnfs/
--rw-r--r--   0 root         (0) root         (0)     1396 2023-03-09 09:18:42.000000 dbm-agent-8.32.8/dbma/static/cnfs/auto-inseption-db.sql
--rw-r--r--   0 root         (0) root         (0)      168 2023-03-09 09:18:42.000000 dbm-agent-8.32.8/dbma/static/cnfs/create-innodb-cluster.js
--rw-r--r--   0 root         (0) root         (0)      286 2023-03-09 09:18:42.000000 dbm-agent-8.32.8/dbma/static/cnfs/dbm-backup-proxyd.service.jinja
--rw-r--r--   0 root         (0) root         (0)      385 2023-03-09 09:18:42.000000 dbm-agent-8.32.8/dbma/static/cnfs/dbm-monitor-gatewayd.service.jinja
--rw-r--r--   0 root         (0) root         (0)      514 2023-04-06 08:26:15.000000 dbm-agent-8.32.8/dbma/static/cnfs/init-5.7.x.sql
--rw-r--r--   0 root         (0) root         (0)      514 2023-04-06 09:18:43.000000 dbm-agent-8.32.8/dbma/static/cnfs/init-8.0.x.sql
--rw-r--r--   0 root         (0) root         (0)     6681 2023-03-09 09:18:42.000000 dbm-agent-8.32.8/dbma/static/cnfs/init-users.sql.jinja
--rw-r--r--   0 root         (0) root         (0)    10685 2023-04-03 07:33:25.000000 dbm-agent-8.32.8/dbma/static/cnfs/mysql-5.7-init-only.jinja
--rw-r--r--   0 root         (0) root         (0)    10847 2023-04-03 07:45:13.000000 dbm-agent-8.32.8/dbma/static/cnfs/mysql-5.7.25.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    14716 2023-04-03 03:33:55.000000 dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0-init-only.jinja
--rw-r--r--   0 root         (0) root         (0)    17621 2023-03-09 09:18:42.000000 dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0.17.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17631 2023-03-09 09:18:42.000000 dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0.18.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17687 2023-03-09 09:18:42.000000 dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0.19.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17766 2023-03-09 09:18:42.000000 dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0.20.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17766 2023-03-09 09:18:42.000000 dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0.21.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17767 2023-03-09 09:18:42.000000 dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0.22.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17767 2023-03-09 09:18:42.000000 dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0.23.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17767 2023-03-09 09:18:42.000000 dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0.25.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17767 2023-03-09 09:18:42.000000 dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0.26.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17528 2023-03-09 09:18:42.000000 dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0.27.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17528 2023-03-09 09:18:42.000000 dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0.28.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17528 2023-03-09 09:18:42.000000 dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0.29.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17799 2023-03-09 09:18:42.000000 dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0.30.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    18705 2023-04-11 03:16:31.000000 dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0.31.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    18707 2023-04-11 03:16:16.000000 dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0.32.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)      465 2023-03-29 06:32:45.000000 dbm-agent-8.32.8/dbma/static/cnfs/mysqld.service.jinja
--rw-r--r--   0 root         (0) root         (0)      362 2023-03-09 09:18:42.000000 dbm-agent-8.32.8/dbma/static/cnfs/zabbix-agentd.service
--rw-r--r--   0 root         (0) root         (0)    10464 2023-03-09 09:18:42.000000 dbm-agent-8.32.8/dbma/static/cnfs/zabbix_agentd.conf.jinja
--rw-r--r--   0 root         (0) root         (0)      258 2023-03-09 09:18:42.000000 dbm-agent-8.32.8/dbma/static/cnfs/zoo.cnf.jinja
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 08:47:11.970536 dbm-agent-8.32.8/dbma/static/sql-scripts/
--rw-r--r--   0 root         (0) root         (0)     9468 2023-03-09 09:18:42.000000 dbm-agent-8.32.8/dbma/static/sql-scripts/常用SQL.md
--rw-r--r--   0 root         (0) root         (0)      346 2023-04-11 08:44:13.000000 dbm-agent-8.32.8/dbma/version.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-11 08:47:11.970536 dbm-agent-8.32.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1856 2023-04-11 03:20:04.000000 dbm-agent-8.32.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 09:08:54.321970 dbm-agent-8.33.0/
+-rw-r--r--   0 root         (0) root         (0)      651 2023-04-21 09:08:54.321970 dbm-agent-8.33.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4453 2023-04-11 12:20:06.000000 dbm-agent-8.33.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 09:08:54.308970 dbm-agent-8.33.0/bin/
+-rw-r--r--   0 root         (0) root         (0)      898 2023-04-11 03:20:19.000000 dbm-agent-8.33.0/bin/dbm-agent
+-rw-r--r--   0 root         (0) root         (0)      322 2023-04-06 12:14:18.000000 dbm-agent-8.33.0/bin/dbm-bt-conn-stack
+-rw-r--r--   0 root         (0) root         (0)      794 2023-04-11 03:20:38.000000 dbm-agent-8.33.0/bin/dbma-cli-init
+-rw-r--r--   0 root         (0) root         (0)     2613 2023-04-11 08:35:08.000000 dbm-agent-8.33.0/bin/dbma-cli-single-instance
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 09:08:54.309970 dbm-agent-8.33.0/dbm_agent.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      651 2023-04-21 09:08:54.000000 dbm-agent-8.33.0/dbm_agent.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2582 2023-04-21 09:08:54.000000 dbm-agent-8.33.0/dbm_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 09:08:54.000000 dbm-agent-8.33.0/dbm_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      106 2023-04-21 09:08:54.000000 dbm-agent-8.33.0/dbm_agent.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      192 2023-04-21 09:08:54.000000 dbm-agent-8.33.0/dbm_agent.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 09:08:54.309970 dbm-agent-8.33.0/dbma/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 02:17:13.000000 dbm-agent-8.33.0/dbma/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 09:08:54.311970 dbm-agent-8.33.0/dbma/bil/
+-rw-r--r--   0 root         (0) root         (0)      104 2023-04-07 07:23:15.000000 dbm-agent-8.33.0/dbma/bil/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      411 2023-04-07 07:23:15.000000 dbm-agent-8.33.0/dbma/bil/cmdexecutor.py
+-rw-r--r--   0 root         (0) root         (0)     3740 2023-04-07 07:23:16.000000 dbm-agent-8.33.0/dbma/bil/daemon.py
+-rw-r--r--   0 root         (0) root         (0)     1891 2023-04-07 07:23:16.000000 dbm-agent-8.33.0/dbma/bil/fs.py
+-rw-r--r--   0 root         (0) root         (0)      225 2023-04-07 07:23:16.000000 dbm-agent-8.33.0/dbma/bil/fun.py
+-rw-r--r--   0 root         (0) root         (0)      700 2023-04-10 03:49:50.000000 dbm-agent-8.33.0/dbma/bil/net.py
+-rw-r--r--   0 root         (0) root         (0)     5900 2023-04-07 07:23:16.000000 dbm-agent-8.33.0/dbma/bil/osuser.py
+-rw-r--r--   0 root         (0) root         (0)      542 2023-04-07 07:23:16.000000 dbm-agent-8.33.0/dbma/bil/sudos.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 09:08:54.311970 dbm-agent-8.33.0/dbma/components/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-28 02:20:28.000000 dbm-agent-8.33.0/dbma/components/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 09:08:54.312970 dbm-agent-8.33.0/dbma/components/mysql/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-28 02:20:47.000000 dbm-agent-8.33.0/dbma/components/mysql/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 09:08:54.312970 dbm-agent-8.33.0/dbma/components/mysql/backups/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 08:54:14.000000 dbm-agent-8.33.0/dbma/components/mysql/backups/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1665 2023-04-11 11:19:32.000000 dbm-agent-8.33.0/dbma/components/mysql/backups/cloneplugin.py
+-rw-r--r--   0 root         (0) root         (0)     5674 2023-04-11 08:23:03.000000 dbm-agent-8.33.0/dbma/components/mysql/commons.py
+-rw-r--r--   0 root         (0) root         (0)    21000 2023-04-13 09:44:10.000000 dbm-agent-8.33.0/dbma/components/mysql/config.py
+-rw-r--r--   0 root         (0) root         (0)      473 2023-04-07 07:23:16.000000 dbm-agent-8.33.0/dbma/components/mysql/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    15140 2023-04-11 07:41:26.000000 dbm-agent-8.33.0/dbma/components/mysql/install.py
+-rw-r--r--   0 root         (0) root         (0)      646 2023-04-07 07:23:16.000000 dbm-agent-8.33.0/dbma/components/mysql/instance.py
+-rw-r--r--   0 root         (0) root         (0)     3996 2023-04-11 08:39:21.000000 dbm-agent-8.33.0/dbma/components/mysql/replica.py
+-rw-r--r--   0 root         (0) root         (0)      849 2023-04-11 08:19:15.000000 dbm-agent-8.33.0/dbma/components/mysql/source.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 09:08:54.313970 dbm-agent-8.33.0/dbma/components/mysql/views/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-29 08:25:42.000000 dbm-agent-8.33.0/dbma/components/mysql/views/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13670 2023-04-12 08:33:24.000000 dbm-agent-8.33.0/dbma/components/mysql/views/defaultsview.py
+-rw-r--r--   0 root         (0) root         (0)     4375 2023-04-11 11:43:08.000000 dbm-agent-8.33.0/dbma/components/mysql/views/handlers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 09:08:54.313970 dbm-agent-8.33.0/dbma/components/redis/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-28 02:21:47.000000 dbm-agent-8.33.0/dbma/components/redis/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 09:08:54.314970 dbm-agent-8.33.0/dbma/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-11 07:21:13.000000 dbm-agent-8.33.0/dbma/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 09:08:54.314970 dbm-agent-8.33.0/dbma/core/agent/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-10 06:58:11.000000 dbm-agent-8.33.0/dbma/core/agent/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2094 2023-04-07 07:23:16.000000 dbm-agent-8.33.0/dbma/core/agent/init.py
+-rw-r--r--   0 root         (0) root         (0)      117 2023-04-07 07:23:16.000000 dbm-agent-8.33.0/dbma/core/agent/upgrade.py
+-rw-r--r--   0 root         (0) root         (0)     3595 2023-04-21 09:07:34.000000 dbm-agent-8.33.0/dbma/core/configs.py
+-rw-r--r--   0 root         (0) root         (0)      103 2023-04-07 07:23:16.000000 dbm-agent-8.33.0/dbma/core/exception.py
+-rw-r--r--   0 root         (0) root         (0)     2263 2023-04-07 07:23:17.000000 dbm-agent-8.33.0/dbma/core/httpserver.py
+-rw-r--r--   0 root         (0) root         (0)      829 2023-04-12 03:16:26.000000 dbm-agent-8.33.0/dbma/core/messages.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-04-07 07:23:17.000000 dbm-agent-8.33.0/dbma/core/router.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 09:08:54.315970 dbm-agent-8.33.0/dbma/core/threads/
+-rw-r--r--   0 root         (0) root         (0)       90 2023-04-07 07:23:17.000000 dbm-agent-8.33.0/dbma/core/threads/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1987 2023-04-07 07:23:17.000000 dbm-agent-8.33.0/dbma/core/threads/backends.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 09:08:54.315970 dbm-agent-8.33.0/dbma/core/views/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-09 09:18:42.000000 dbm-agent-8.33.0/dbma/core/views/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      455 2023-04-07 07:23:17.000000 dbm-agent-8.33.0/dbma/core/views/dbmagentview.py
+-rw-r--r--   0 root         (0) root         (0)      466 2023-04-07 07:23:17.000000 dbm-agent-8.33.0/dbma/core/views/response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 09:08:54.307970 dbm-agent-8.33.0/dbma/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 09:08:54.320970 dbm-agent-8.33.0/dbma/static/cnfs/
+-rw-r--r--   0 root         (0) root         (0)     1396 2023-03-09 09:18:42.000000 dbm-agent-8.33.0/dbma/static/cnfs/auto-inseption-db.sql
+-rw-r--r--   0 root         (0) root         (0)      168 2023-03-09 09:18:42.000000 dbm-agent-8.33.0/dbma/static/cnfs/create-innodb-cluster.js
+-rw-r--r--   0 root         (0) root         (0)      286 2023-03-09 09:18:42.000000 dbm-agent-8.33.0/dbma/static/cnfs/dbm-backup-proxyd.service.jinja
+-rw-r--r--   0 root         (0) root         (0)      385 2023-03-09 09:18:42.000000 dbm-agent-8.33.0/dbma/static/cnfs/dbm-monitor-gatewayd.service.jinja
+-rw-r--r--   0 root         (0) root         (0)      514 2023-04-06 08:26:15.000000 dbm-agent-8.33.0/dbma/static/cnfs/init-5.7.x.sql
+-rw-r--r--   0 root         (0) root         (0)      514 2023-04-06 09:18:43.000000 dbm-agent-8.33.0/dbma/static/cnfs/init-8.0.x.sql
+-rw-r--r--   0 root         (0) root         (0)     6681 2023-03-09 09:18:42.000000 dbm-agent-8.33.0/dbma/static/cnfs/init-users.sql.jinja
+-rw-r--r--   0 root         (0) root         (0)    10685 2023-04-03 07:33:25.000000 dbm-agent-8.33.0/dbma/static/cnfs/mysql-5.7-init-only.jinja
+-rw-r--r--   0 root         (0) root         (0)    10847 2023-04-03 07:45:13.000000 dbm-agent-8.33.0/dbma/static/cnfs/mysql-5.7.25.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    14716 2023-04-03 03:33:55.000000 dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0-init-only.jinja
+-rw-r--r--   0 root         (0) root         (0)    17621 2023-03-09 09:18:42.000000 dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.17.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17631 2023-03-09 09:18:42.000000 dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.18.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17687 2023-03-09 09:18:42.000000 dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.19.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17766 2023-03-09 09:18:42.000000 dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.20.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17766 2023-03-09 09:18:42.000000 dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.21.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17767 2023-03-09 09:18:42.000000 dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.22.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17767 2023-03-09 09:18:42.000000 dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.23.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17767 2023-03-09 09:18:42.000000 dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.25.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17767 2023-03-09 09:18:42.000000 dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.26.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17528 2023-03-09 09:18:42.000000 dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.27.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17528 2023-03-09 09:18:42.000000 dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.28.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17528 2023-03-09 09:18:42.000000 dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.29.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17799 2023-03-09 09:18:42.000000 dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.30.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    18787 2023-04-13 09:47:14.000000 dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.31.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    18789 2023-04-13 09:47:41.000000 dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.32.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    18789 2023-04-21 09:06:42.000000 dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.33.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)      465 2023-03-29 06:32:45.000000 dbm-agent-8.33.0/dbma/static/cnfs/mysqld.service.jinja
+-rw-r--r--   0 root         (0) root         (0)      362 2023-03-09 09:18:42.000000 dbm-agent-8.33.0/dbma/static/cnfs/zabbix-agentd.service
+-rw-r--r--   0 root         (0) root         (0)    10464 2023-03-09 09:18:42.000000 dbm-agent-8.33.0/dbma/static/cnfs/zabbix_agentd.conf.jinja
+-rw-r--r--   0 root         (0) root         (0)      258 2023-03-09 09:18:42.000000 dbm-agent-8.33.0/dbma/static/cnfs/zoo.cnf.jinja
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 09:08:54.320970 dbm-agent-8.33.0/dbma/static/sql-scripts/
+-rw-r--r--   0 root         (0) root         (0)     9468 2023-03-09 09:18:42.000000 dbm-agent-8.33.0/dbma/static/sql-scripts/常用SQL.md
+-rw-r--r--   0 root         (0) root         (0)      346 2023-04-21 09:07:07.000000 dbm-agent-8.33.0/dbma/version.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-21 09:08:54.321970 dbm-agent-8.33.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1897 2023-04-11 09:42:31.000000 dbm-agent-8.33.0/setup.py
```

### Comparing `dbm-agent-8.32.8/PKG-INFO` & `dbm-agent-8.33.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbm-agent
-Version: 8.32.8
+Version: 8.33.0
 Summary: dbm-agent 数据库管理中心客户端程序
 Home-page: https://github.com/Neeky/dbm-agent
 Author: Neeky
 Author-email: neeky@live.com
 Maintainer: Neeky
 Maintainer-email: neeky@live.com
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dbm-agent-8.32.8/README.md` & `dbm-agent-8.33.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 ## 目录
 ---
 - [目录](#目录)
 - [dbm-愿景](#dbm-愿景)
 - [安装-dbm-agent](#安装-dbm-agent)
-- [安装配置-MySQL](#安装配置-mysql)
+- [安装-MySQL](#安装-mysql)
+- [备份-MySQL](#备份-mysql)
 - [关闭-dbm-agent](#关闭-dbm-agent)
 - [规范](#规范)
 - [官方微信公众平台](#官方微信公众平台)
 
 
 ---
 
@@ -78,16 +79,21 @@
    {
      "name": "dbm-agent",
      "version": "8.31.9"
    }
    ```
    ---
 
-## 安装配置-MySQL
-请查看 `dev-docs/01-auto-install-MySQL.md` [安装配置-MySQL](./dev-docs/01-auto-install-MySQL.md) 。
+## 安装-MySQL
+请查看 `docs/01-auto-install-MySQL.md` [安装配置-MySQL](./docs/01-auto-install-MySQL.md) 。
+
+---
+
+## 备份-MySQL
+请查看 `docs/02-auto-backup-MySQL.md` [备份-MySQL](./docs/02-auto-backup-MySQL.md) 。
 
 
 ## 关闭-dbm-agent
    **关闭 dbm-agent 守护进程**
    ```bash
    dbm-agent stop                                                              
    Successful exit
```

### Comparing `dbm-agent-8.32.8/bin/dbm-agent` & `dbm-agent-8.33.0/bin/dbm-agent`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.8/bin/dbma-cli-init` & `dbm-agent-8.33.0/bin/dbma-cli-init`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.8/bin/dbma-cli-single-instance` & `dbm-agent-8.33.0/bin/dbma-cli-single-instance`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.8/dbm_agent.egg-info/PKG-INFO` & `dbm-agent-8.33.0/dbm_agent.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbm-agent
-Version: 8.32.8
+Version: 8.33.0
 Summary: dbm-agent 数据库管理中心客户端程序
 Home-page: https://github.com/Neeky/dbm-agent
 Author: Neeky
 Author-email: neeky@live.com
 Maintainer: Neeky
 Maintainer-email: neeky@live.com
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dbm-agent-8.32.8/dbm_agent.egg-info/SOURCES.txt` & `dbm-agent-8.33.0/dbm_agent.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 dbma/components/mysql/commons.py
 dbma/components/mysql/config.py
 dbma/components/mysql/exceptions.py
 dbma/components/mysql/install.py
 dbma/components/mysql/instance.py
 dbma/components/mysql/replica.py
 dbma/components/mysql/source.py
+dbma/components/mysql/backups/__init__.py
+dbma/components/mysql/backups/cloneplugin.py
 dbma/components/mysql/views/__init__.py
 dbma/components/mysql/views/defaultsview.py
 dbma/components/mysql/views/handlers.py
 dbma/components/redis/__init__.py
 dbma/core/__init__.py
 dbma/core/configs.py
 dbma/core/exception.py
@@ -67,12 +69,13 @@
 dbma/static/cnfs/mysql-8.0.26.cnf.jinja
 dbma/static/cnfs/mysql-8.0.27.cnf.jinja
 dbma/static/cnfs/mysql-8.0.28.cnf.jinja
 dbma/static/cnfs/mysql-8.0.29.cnf.jinja
 dbma/static/cnfs/mysql-8.0.30.cnf.jinja
 dbma/static/cnfs/mysql-8.0.31.cnf.jinja
 dbma/static/cnfs/mysql-8.0.32.cnf.jinja
+dbma/static/cnfs/mysql-8.0.33.cnf.jinja
 dbma/static/cnfs/mysqld.service.jinja
 dbma/static/cnfs/zabbix-agentd.service
 dbma/static/cnfs/zabbix_agentd.conf.jinja
 dbma/static/cnfs/zoo.cnf.jinja
 dbma/static/sql-scripts/常用SQL.md
```

### Comparing `dbm-agent-8.32.8/dbma/bil/daemon.py` & `dbm-agent-8.33.0/dbma/bil/daemon.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.8/dbma/bil/fs.py` & `dbm-agent-8.33.0/dbma/bil/fs.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.8/dbma/bil/net.py` & `dbm-agent-8.33.0/dbma/bil/net.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.8/dbma/bil/osuser.py` & `dbm-agent-8.33.0/dbma/bil/osuser.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.8/dbma/bil/sudos.py` & `dbm-agent-8.33.0/dbma/bil/sudos.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.8/dbma/components/mysql/commons.py` & `dbm-agent-8.33.0/dbma/components/mysql/commons.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.8/dbma/components/mysql/config.py` & `dbm-agent-8.33.0/dbma/components/mysql/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,15 +139,16 @@
     binlog_row_image: str = "FULL"
     binlog_row_metadata: str = "FULL"
     binlog_rows_query_log_events: str = "ON"
     binlog_stmt_cache_size: int = 32768
     log_replica_updates: str = "ON"
     binlog_transaction_compression: str = "ON"
     binlog_transaction_dependency_history_size: int = 25000
-    binlog_transaction_dependency_tracking: str = "COMMIT_ORDER"
+    binlog_transaction_dependency_tracking: str = "WRITESET"
+    transaction_write_set_extraction: str = "XXHASH64"
     sync_binlog: int = 1
     binlog_cache_size: int = 32768
     binlog_group_commit_sync_delay: int = 0
     binlog_group_commit_sync_no_delay_count: int = 0
     # endregion binlogs
 
     # region gtids
```

### Comparing `dbm-agent-8.32.8/dbma/components/mysql/install.py` & `dbm-agent-8.33.0/dbma/components/mysql/install.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.8/dbma/components/mysql/instance.py` & `dbm-agent-8.33.0/dbma/components/mysql/instance.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.8/dbma/components/mysql/replica.py` & `dbm-agent-8.33.0/dbma/components/mysql/replica.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.8/dbma/components/mysql/source.py` & `dbm-agent-8.33.0/dbma/components/mysql/source.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.8/dbma/components/mysql/views/handlers.py` & `dbm-agent-8.33.0/dbma/components/mysql/views/handlers.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """dbm-agent 收到操作请求(task)之后，如果请求中没有带 task_id ，说明要求同步执行；如果有带 task_id 那么我们要把 task 放到后台线程中执行。
 
 """
 
 import logging
 from pathlib import Path
 from dbma.bil.sudos import sudo
+from dbma.components.mysql.backups.cloneplugin import clone_local_data
 from dbma.components.mysql.source import install_mysql_source
 from dbma.components.mysql.replica import install_mysql_replica
 
 
 def update_task_state_callback(
     task_id: int = None, state: str = None, message: str = None
 ):
@@ -111,7 +112,31 @@
             update_task_state_callback(
                 task_id, 200, "install mysql 'slave|replica' complete"
             )
 
     except Exception as err:
         logging.error("install mysql 'slave|replica' task handler got error ")
     logging.info("ends install mysql 'slave|replica' task handler .")
+
+
+def clone_local_data_task_handler(
+    port: int = 3306, backup_type: str = None, task_id: int = None
+):
+    """ """
+    logging.info("starts clone local data task handler .")
+    try:
+        with sudo("starts clone local data task handler"):
+            clone_local_data(port)
+    except Exception as err:
+        logging.error("starts clone local data task handler got error {}".format(err))
+
+    # 是否更新任务信息到 dbm-center
+    if not task_id is None:
+        logging.warn(
+            "starts clone local data task handler's callback function is None, skip callback"
+        )
+    else:
+        update_task_state_callback(
+            task_id, 200, "starts clone local data task handler complete"
+        )
+
+    logging.info("ends clone local data task handler .")
```

### Comparing `dbm-agent-8.32.8/dbma/core/agent/init.py` & `dbm-agent-8.33.0/dbma/core/agent/init.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.8/dbma/core/configs.py` & `dbm-agent-8.33.0/dbma/core/configs.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,16 +38,17 @@
 
     # 单例模式
     _instance = None
 
     # MySQL 相关的默认配置
     mysql_datadir_parent: str = "/database/mysql/data/"
     mysql_binlogdir_parent: str = "/database/mysql/binlog/"
+    mysql_backupdir_parent: str = "/database/mysql/backup/"
     mysql_user_prefix: str = "mysql"
-    mysql_default_version: str = "8.0.32"
+    mysql_default_version: str = "8.0.33"
 
     mysql_dbma_user: str = "dbma"
     mysql_dbma_password: str = "dbma@0352"
     # mysql_consts
     mysql_repl_user: str = "repl"
     mysql_repl_password: str = "2-4nw9A0-459st36"
     mysql_init_cnf: str = "/tmp/mysql-init.cnf"
```

### Comparing `dbm-agent-8.32.8/dbma/core/httpserver.py` & `dbm-agent-8.33.0/dbma/core/httpserver.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.8/dbma/core/messages.py` & `dbm-agent-8.33.0/dbma/core/messages.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 """代码写到一定的量之后发现，实在是太多的字符串常量了。另人难过的差不多的语境，不同时期的拼写还不一致。
 作者: 蒋乐兴|neeky
 时间: 2023-03
 """
 
 # 函数开执行
 FUN_STARTS = "starts {} ."
-
-
 # 函数执行完成(return 之前)
 FUN_ENDS = "ends {} ."
+VIEW_FUN_STARTS = "view-request-starts: {}"
+VIEW_FUN_ENDS = "view-requests-ends: {}"
 
 
 # 文件不存在
 FILE_NOT_EXISTS = "file '{}' not exists ."
 
 
 # 执行命令
@@ -26,7 +26,10 @@
 DIR_EXISTS = "dir '{}' exists ."
 DIR_NOT_EXISTS = "dir '{}' not exists ."
 MOVE_FILE_TO = "move '{}' to '{}' "
 
 
 # MySQL MESSAGES
 MYSQL_INSTANCE_HAS_EXISTS = "mysql instance '{}' has exists ."
+
+
+ARG_NOT_IN_POST_DICT = "argument '{}' not in post dict"
```

### Comparing `dbm-agent-8.32.8/dbma/core/threads/backends.py` & `dbm-agent-8.33.0/dbma/core/threads/backends.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.8/dbma/static/cnfs/auto-inseption-db.sql` & `dbm-agent-8.33.0/dbma/static/cnfs/auto-inseption-db.sql`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.8/dbma/static/cnfs/init-5.7.x.sql` & `dbm-agent-8.33.0/dbma/static/cnfs/init-5.7.x.sql`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.8/dbma/static/cnfs/init-8.0.x.sql` & `dbm-agent-8.33.0/dbma/static/cnfs/init-8.0.x.sql`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.8/dbma/static/cnfs/init-users.sql.jinja` & `dbm-agent-8.33.0/dbma/static/cnfs/init-users.sql.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.8/dbma/static/cnfs/mysql-5.7-init-only.jinja` & `dbm-agent-8.33.0/dbma/static/cnfs/mysql-5.7-init-only.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.8/dbma/static/cnfs/mysql-5.7.25.cnf.jinja` & `dbm-agent-8.33.0/dbma/static/cnfs/mysql-5.7.25.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0-init-only.jinja` & `dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0-init-only.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0.17.cnf.jinja` & `dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.17.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0.18.cnf.jinja` & `dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.18.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0.19.cnf.jinja` & `dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.19.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0.20.cnf.jinja` & `dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.20.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0.21.cnf.jinja` & `dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.21.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0.22.cnf.jinja` & `dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.22.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0.23.cnf.jinja` & `dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.23.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0.25.cnf.jinja` & `dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.25.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0.26.cnf.jinja` & `dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.26.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0.27.cnf.jinja` & `dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.27.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0.28.cnf.jinja` & `dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.28.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0.29.cnf.jinja` & `dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.29.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0.30.cnf.jinja` & `dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.30.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0.31.cnf.jinja` & `dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.33.cnf.jinja`

 * *Files 0% similar despite different names*

```diff
@@ -89,14 +89,15 @@
 binlog_row_metadata                        = {{binlog_row_metadata}}
 binlog_rows_query_log_events               = {{binlog_rows_query_log_events}}
 binlog_stmt_cache_size                     = {{binlog_stmt_cache_size}}
 log_replica_updates                        = ON
 binlog_transaction_compression             = {{binlog_transaction_compression}}
 binlog_transaction_dependency_history_size = {{binlog_transaction_dependency_history_size}}
 binlog_transaction_dependency_tracking     = {{binlog_transaction_dependency_tracking}}
+transaction_write_set_extraction           = {{transaction_write_set_extraction}}
 sync_binlog                                = {{sync_binlog}}
 binlog_cache_size                          = {{binlog_cache_size}}
 binlog_group_commit_sync_delay             = {{binlog_group_commit_sync_delay}}
 binlog_group_commit_sync_no_delay_count    = {{binlog_group_commit_sync_no_delay_count}}
 
 
 #### for replication
@@ -124,16 +125,16 @@
 gtid_mode                                = {{gtid_mode}}
 binlog_gtid_simple_recovery              = {{binlog_gtid_simple_recovery}}
 enforce_gtid_consistency                 = {{enforce_gtid_consistency}}
 gtid_executed_compression_period         = {{gtid_executed_compression_period}}
 
 
 #### for clone 
-plugin-load-add                          = mysql_clone.so
-clone                                    = FORCE_PLUS_PERMANENT
+plugin-load-add                           = mysql_clone.so
+clone                                     = FORCE_PLUS_PERMANENT
 clone_autotune_concurrency                = {{ clone_autotune_concurrency}}
 clone_buffer_size                         = {{ clone_buffer_size}}
 clone_block_ddl                           = {{ clone_block_ddl}}
 clone_delay_after_data_drop               = {{ clone_delay_after_data_drop}}
 clone_ddl_timeout                         = {{ clone_ddl_timeout}}
 clone_donor_timeout_after_network_failure = {{ clone_donor_timeout_after_network_failure}}
 clone_enable_compression                  = {{ clone_enable_compression}}
@@ -292,13 +293,13 @@
 performance_schema_consumer_events_waits_current                        =ON  
 performance_schema_consumer_events_waits_history                        =ON  
 performance_schema_consumer_events_waits_history_long                   =OFF 
 performance-schema-instrument                                           ='memory/%=COUNTED'
 
 
 # -- ~ _ ~    ~ _ ~     ~ _ ~ -- 
-# base on mysql-8.0.31
-# generated by https://www.sqlpy.com 2022年11月11日 23:45
+# base on mysql-8.0.33
+# generated by https://www.sqlpy.com 2023年04月21日 23:45
 # wechat: jianglegege
 # email: 1721900707@qq.com
 # -- ~ _ ~ --
```

### Comparing `dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0.32.cnf.jinja` & `dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.31.cnf.jinja`

 * *Files 0% similar despite different names*

```diff
@@ -89,14 +89,15 @@
 binlog_row_metadata                        = {{binlog_row_metadata}}
 binlog_rows_query_log_events               = {{binlog_rows_query_log_events}}
 binlog_stmt_cache_size                     = {{binlog_stmt_cache_size}}
 log_replica_updates                        = ON
 binlog_transaction_compression             = {{binlog_transaction_compression}}
 binlog_transaction_dependency_history_size = {{binlog_transaction_dependency_history_size}}
 binlog_transaction_dependency_tracking     = {{binlog_transaction_dependency_tracking}}
+transaction_write_set_extraction           = {{transaction_write_set_extraction}}
 sync_binlog                                = {{sync_binlog}}
 binlog_cache_size                          = {{binlog_cache_size}}
 binlog_group_commit_sync_delay             = {{binlog_group_commit_sync_delay}}
 binlog_group_commit_sync_no_delay_count    = {{binlog_group_commit_sync_no_delay_count}}
 
 
 #### for replication
@@ -124,16 +125,16 @@
 gtid_mode                                = {{gtid_mode}}
 binlog_gtid_simple_recovery              = {{binlog_gtid_simple_recovery}}
 enforce_gtid_consistency                 = {{enforce_gtid_consistency}}
 gtid_executed_compression_period         = {{gtid_executed_compression_period}}
 
 
 #### for clone 
-plugin-load-add                           = mysql_clone.so
-clone                                     = FORCE_PLUS_PERMANENT
+plugin-load-add                          = mysql_clone.so
+clone                                    = FORCE_PLUS_PERMANENT
 clone_autotune_concurrency                = {{ clone_autotune_concurrency}}
 clone_buffer_size                         = {{ clone_buffer_size}}
 clone_block_ddl                           = {{ clone_block_ddl}}
 clone_delay_after_data_drop               = {{ clone_delay_after_data_drop}}
 clone_ddl_timeout                         = {{ clone_ddl_timeout}}
 clone_donor_timeout_after_network_failure = {{ clone_donor_timeout_after_network_failure}}
 clone_enable_compression                  = {{ clone_enable_compression}}
@@ -292,13 +293,13 @@
 performance_schema_consumer_events_waits_current                        =ON  
 performance_schema_consumer_events_waits_history                        =ON  
 performance_schema_consumer_events_waits_history_long                   =OFF 
 performance-schema-instrument                                           ='memory/%=COUNTED'
 
 
 # -- ~ _ ~    ~ _ ~     ~ _ ~ -- 
-# base on mysql-8.0.32
-# generated by https://www.sqlpy.com 2023年03月30日 23:45
+# base on mysql-8.0.31
+# generated by https://www.sqlpy.com 2022年11月11日 23:45
 # wechat: jianglegege
 # email: 1721900707@qq.com
 # -- ~ _ ~ --
```

### Comparing `dbm-agent-8.32.8/dbma/static/cnfs/zabbix_agentd.conf.jinja` & `dbm-agent-8.33.0/dbma/static/cnfs/zabbix_agentd.conf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.8/dbma/static/sql-scripts/常用SQL.md` & `dbm-agent-8.33.0/dbma/static/sql-scripts/常用SQL.md`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.8/setup.py` & `dbm-agent-8.33.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,14 +41,15 @@
         "dbma/core/agent",
         "dbma/core/threads",
         "dbma/bil",
         "dbma/components",
         "dbma/components/mysql",
         "dbma/components/redis",
         "dbma/components/mysql/views",
+        "dbma/components/mysql/backups",
     ],
     package_data={"dbma": ["static/cnfs/*", "static/sql-scripts/*"]},
     url="https://github.com/Neeky/dbm-agent",
     install_requires=[
         "Jinja2>=2.10.1",
         "mysql-connector-python>=8.0.31",
         "psutil>=5.6.6",
```

