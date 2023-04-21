# Comparing `tmp/planetmint-2.4.4.tar.gz` & `tmp/planetmint-2.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "planetmint-2.4.4.tar", max compression
+gzip compressed data, was "planetmint-2.4.5.tar", max compression
```

## Comparing `planetmint-2.4.4.tar` & `planetmint-2.4.5.tar`

### file list

```diff
@@ -1,80 +1,80 @@
--rw-r--r--   0        0        0    34523 2023-04-19 12:05:10.127119 planetmint-2.4.4/LICENSE
--rw-r--r--   0        0        0     1614 2023-04-19 12:05:10.127119 planetmint-2.4.4/LICENSES.md
--rw-r--r--   0        0        0     3126 2023-04-19 12:05:10.127119 planetmint-2.4.4/README.md
--rw-r--r--   0        0        0     1796 2023-04-19 12:05:10.139119 planetmint-2.4.4/planetmint/README.md
--rw-r--r--   0        0        0      205 2023-04-19 12:05:10.139119 planetmint-2.4.4/planetmint/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 12:05:10.139119 planetmint-2.4.4/planetmint/abci/__init__.py
--rw-r--r--   0        0        0    10928 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/abci/application_logic.py
--rw-r--r--   0        0        0      104 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/abci/block.py
--rw-r--r--   0        0        0     4896 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/abci/parallel_validation.py
--rw-r--r--   0        0        0     2994 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/abci/rpc.py
--rw-r--r--   0        0        0     5291 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/abci/utils.py
--rw-r--r--   0        0        0       86 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/application/__init__.py
--rw-r--r--   0        0        0      833 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/application/basevalidationrules.py
--rw-r--r--   0        0        0    23655 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/application/validator.py
--rw-r--r--   0        0        0     2319 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/backend/README.md
--rw-r--r--   0        0        0      705 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/backend/__init__.py
--rw-r--r--   0        0        0     4496 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/backend/connection.py
--rw-r--r--   0        0        0      891 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/backend/exceptions.py
--rw-r--r--   0        0        0     1192 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/backend/localmongodb/__init__.py
--rw-r--r--   0        0        0     6303 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/backend/localmongodb/connection.py
--rw-r--r--   0        0        0     9498 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/backend/localmongodb/query.py
--rw-r--r--   0        0        0     2995 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/backend/localmongodb/schema.py
--rw-r--r--   0        0        0      438 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/backend/models/__init__.py
--rw-r--r--   0        0        0      938 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/backend/models/asset.py
--rw-r--r--   0        0        0      727 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/backend/models/block.py
--rw-r--r--   0        0        0     3050 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/backend/models/dbtransaction.py
--rw-r--r--   0        0        0      446 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/backend/models/fulfills.py
--rw-r--r--   0        0        0     1971 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/backend/models/input.py
--rw-r--r--   0        0        0      603 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/backend/models/metadata.py
--rw-r--r--   0        0        0     4387 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/backend/models/output.py
--rw-r--r--   0        0        0      600 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/backend/models/script.py
--rw-r--r--   0        0        0    10645 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/backend/query.py
--rw-r--r--   0        0        0     4516 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/backend/schema.py
--rw-r--r--   0        0        0      127 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/backend/tarantool/__init__.py
--rw-r--r--   0        0        0      917 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/backend/tarantool/const.py
--rw-r--r--   0        0        0    13774 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/backend/tarantool/opt/init.lua
--rw-r--r--   0        0        0        0 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/backend/tarantool/sync_io/__init__.py
--rw-r--r--   0        0        0     2714 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/backend/tarantool/sync_io/connection.py
--rw-r--r--   0        0        0    19127 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/backend/tarantool/sync_io/query.py
--rw-r--r--   0        0        0     1154 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/backend/tarantool/sync_io/schema.py
--rw-r--r--   0        0        0      916 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/backend/tarantool/tarantool.md
--rw-r--r--   0        0        0     1123 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/backend/utils.py
--rw-r--r--   0        0        0        0 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/commands/__init__.py
--rw-r--r--   0        0        0     1015 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/commands/election_types.py
--rw-r--r--   0        0        0    14105 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/commands/planetmint.py
--rw-r--r--   0        0        0     4976 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/commands/utils.py
--rw-r--r--   0        0        0     6711 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/config.py
--rw-r--r--   0        0        0    12361 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/config_utils.py
--rw-r--r--   0        0        0      401 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/const.py
--rw-r--r--   0        0        0      390 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/ipc/__init__.py
--rw-r--r--   0        0        0      951 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/ipc/events.py
--rw-r--r--   0        0        0     2195 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/ipc/exchange.py
--rw-r--r--   0        0        0        0 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/model/__init__.py
--rw-r--r--   0        0        0    14086 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/model/dataaccessor.py
--rw-r--r--   0        0        0     3442 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/start.py
--rw-r--r--   0        0        0        0 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/utils/__init__.py
--rw-r--r--   0        0        0     1153 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/utils/lazy.py
--rw-r--r--   0        0        0     2253 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/utils/processes.py
--rw-r--r--   0        0        0      261 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/utils/python.py
--rw-r--r--   0        0        0      239 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/utils/singleton.py
--rw-r--r--   0        0        0      327 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/version.py
--rw-r--r--   0        0        0        0 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/web/__init__.py
--rw-r--r--   0        0        0     1341 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/web/routes.py
--rw-r--r--   0        0        0     3671 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/web/server.py
--rw-r--r--   0        0        0      947 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/web/strip_content_type_middleware.py
--rw-r--r--   0        0        0        0 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/web/views/__init__.py
--rw-r--r--   0        0        0     1240 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/web/views/assets.py
--rw-r--r--   0        0        0     1525 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/web/views/base.py
--rw-r--r--   0        0        0     2345 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/web/views/blocks.py
--rw-r--r--   0        0        0     1817 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/web/views/info.py
--rw-r--r--   0        0        0     1428 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/web/views/metadata.py
--rw-r--r--   0        0        0     1464 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/web/views/outputs.py
--rw-r--r--   0        0        0     1631 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/web/views/parameters.py
--rw-r--r--   0        0        0     4785 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/web/views/transactions.py
--rw-r--r--   0        0        0      677 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/web/views/validators.py
--rw-r--r--   0        0        0     3548 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/web/websocket_dispatcher.py
--rw-r--r--   0        0        0     4906 2023-04-19 12:05:10.143119 planetmint-2.4.4/planetmint/web/websocket_server.py
--rw-r--r--   0        0        0     2664 2023-04-19 12:05:10.147120 planetmint-2.4.4/pyproject.toml
--rw-r--r--   0        0        0     4976 1970-01-01 00:00:00.000000 planetmint-2.4.4/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-04-21 09:09:09.220714 planetmint-2.4.5/LICENSE
+-rw-r--r--   0        0        0     1614 2023-04-21 09:09:09.220714 planetmint-2.4.5/LICENSES.md
+-rw-r--r--   0        0        0     3126 2023-04-21 09:09:09.220714 planetmint-2.4.5/README.md
+-rw-r--r--   0        0        0     1796 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/README.md
+-rw-r--r--   0        0        0      205 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/abci/__init__.py
+-rw-r--r--   0        0        0    10928 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/abci/application_logic.py
+-rw-r--r--   0        0        0      104 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/abci/block.py
+-rw-r--r--   0        0        0     4896 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/abci/parallel_validation.py
+-rw-r--r--   0        0        0     2994 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/abci/rpc.py
+-rw-r--r--   0        0        0     5291 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/abci/utils.py
+-rw-r--r--   0        0        0       86 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/application/__init__.py
+-rw-r--r--   0        0        0      833 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/application/basevalidationrules.py
+-rw-r--r--   0        0        0    23644 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/application/validator.py
+-rw-r--r--   0        0        0     2319 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/backend/README.md
+-rw-r--r--   0        0        0      705 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/backend/__init__.py
+-rw-r--r--   0        0        0     4464 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/backend/connection.py
+-rw-r--r--   0        0        0      891 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/backend/exceptions.py
+-rw-r--r--   0        0        0     1192 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/backend/localmongodb/__init__.py
+-rw-r--r--   0        0        0     6303 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/backend/localmongodb/connection.py
+-rw-r--r--   0        0        0     9498 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/backend/localmongodb/query.py
+-rw-r--r--   0        0        0     2995 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/backend/localmongodb/schema.py
+-rw-r--r--   0        0        0      438 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/backend/models/__init__.py
+-rw-r--r--   0        0        0      938 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/backend/models/asset.py
+-rw-r--r--   0        0        0      727 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/backend/models/block.py
+-rw-r--r--   0        0        0     3050 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/backend/models/dbtransaction.py
+-rw-r--r--   0        0        0      446 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/backend/models/fulfills.py
+-rw-r--r--   0        0        0     1971 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/backend/models/input.py
+-rw-r--r--   0        0        0      603 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/backend/models/metadata.py
+-rw-r--r--   0        0        0     4387 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/backend/models/output.py
+-rw-r--r--   0        0        0      600 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/backend/models/script.py
+-rw-r--r--   0        0        0    10645 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/backend/query.py
+-rw-r--r--   0        0        0     4516 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/backend/schema.py
+-rw-r--r--   0        0        0      127 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/backend/tarantool/__init__.py
+-rw-r--r--   0        0        0      917 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/backend/tarantool/const.py
+-rw-r--r--   0        0        0    13774 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/backend/tarantool/opt/init.lua
+-rw-r--r--   0        0        0        0 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/backend/tarantool/sync_io/__init__.py
+-rw-r--r--   0        0        0     2714 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/backend/tarantool/sync_io/connection.py
+-rw-r--r--   0        0        0    19154 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/backend/tarantool/sync_io/query.py
+-rw-r--r--   0        0        0     1154 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/backend/tarantool/sync_io/schema.py
+-rw-r--r--   0        0        0      916 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/backend/tarantool/tarantool.md
+-rw-r--r--   0        0        0     1123 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/backend/utils.py
+-rw-r--r--   0        0        0        0 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/commands/__init__.py
+-rw-r--r--   0        0        0     1015 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/commands/election_types.py
+-rw-r--r--   0        0        0    14105 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/commands/planetmint.py
+-rw-r--r--   0        0        0     4976 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/commands/utils.py
+-rw-r--r--   0        0        0     6711 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/config.py
+-rw-r--r--   0        0        0    12361 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/config_utils.py
+-rw-r--r--   0        0        0      401 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/const.py
+-rw-r--r--   0        0        0      390 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/ipc/__init__.py
+-rw-r--r--   0        0        0      951 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/ipc/events.py
+-rw-r--r--   0        0        0     2195 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/ipc/exchange.py
+-rw-r--r--   0        0        0        0 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/model/__init__.py
+-rw-r--r--   0        0        0    14245 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/model/dataaccessor.py
+-rw-r--r--   0        0        0     3442 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/start.py
+-rw-r--r--   0        0        0        0 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/utils/__init__.py
+-rw-r--r--   0        0        0     1153 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/utils/lazy.py
+-rw-r--r--   0        0        0     2253 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/utils/processes.py
+-rw-r--r--   0        0        0      261 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/utils/python.py
+-rw-r--r--   0        0        0      239 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/utils/singleton.py
+-rw-r--r--   0        0        0      327 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/version.py
+-rw-r--r--   0        0        0        0 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/web/__init__.py
+-rw-r--r--   0        0        0     1341 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/web/routes.py
+-rw-r--r--   0        0        0     3671 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/web/server.py
+-rw-r--r--   0        0        0      947 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/web/strip_content_type_middleware.py
+-rw-r--r--   0        0        0        0 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/web/views/__init__.py
+-rw-r--r--   0        0        0     1240 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/web/views/assets.py
+-rw-r--r--   0        0        0     1525 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/web/views/base.py
+-rw-r--r--   0        0        0     2345 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/web/views/blocks.py
+-rw-r--r--   0        0        0     1817 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/web/views/info.py
+-rw-r--r--   0        0        0     1428 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/web/views/metadata.py
+-rw-r--r--   0        0        0     1464 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/web/views/outputs.py
+-rw-r--r--   0        0        0     1631 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/web/views/parameters.py
+-rw-r--r--   0        0        0     4785 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/web/views/transactions.py
+-rw-r--r--   0        0        0      677 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/web/views/validators.py
+-rw-r--r--   0        0        0     3548 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/web/websocket_dispatcher.py
+-rw-r--r--   0        0        0     4906 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/web/websocket_server.py
+-rw-r--r--   0        0        0     2664 2023-04-21 09:09:09.240715 planetmint-2.4.5/pyproject.toml
+-rw-r--r--   0        0        0     4976 1970-01-01 00:00:00.000000 planetmint-2.4.5/PKG-INFO
```

### Comparing `planetmint-2.4.4/LICENSE` & `planetmint-2.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.4/LICENSES.md` & `planetmint-2.4.5/LICENSES.md`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.4/README.md` & `planetmint-2.4.5/README.md`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.4/planetmint/README.md` & `planetmint-2.4.5/planetmint/README.md`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.4/planetmint/abci/application_logic.py` & `planetmint-2.4.5/planetmint/abci/application_logic.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.4/planetmint/abci/parallel_validation.py` & `planetmint-2.4.5/planetmint/abci/parallel_validation.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.4/planetmint/abci/rpc.py` & `planetmint-2.4.5/planetmint/abci/rpc.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.4/planetmint/abci/utils.py` & `planetmint-2.4.5/planetmint/abci/utils.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.4/planetmint/application/basevalidationrules.py` & `planetmint-2.4.5/planetmint/application/basevalidationrules.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.4/planetmint/application/validator.py` & `planetmint-2.4.5/planetmint/application/validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,22 +24,22 @@
 
 from planetmint.abci.utils import encode_validator, new_validator_set, key_from_base64, public_key_to_base64
 from planetmint.application.basevalidationrules import BaseValidationRules
 from planetmint.backend.models.output import Output
 from planetmint.model.dataaccessor import DataAccessor
 from planetmint.config import Config
 from planetmint.config_utils import load_validation_plugin
+from planetmint.utils.singleton import Singleton
 
 logger = logging.getLogger(__name__)
 
 
 class Validator:
-    def __init__(self, async_io: bool = False):
-        self.async_io = async_io
-        self.models = DataAccessor(async_io=async_io)
+    def __init__(self):
+        self.models = DataAccessor()
         self.validation = Validator._get_validation_method()
 
     @staticmethod
     def _get_validation_method():
         validationPlugin = Config().get().get("validation_plugin")
 
         if validationPlugin:
@@ -265,15 +265,15 @@
         return self.models.get_validator_set(latest_block["height"])
 
     def get_validator_dict(self, height=None):
         """Return a dictionary of validators with key as `public_key` and
         value as the `voting_power`
         """
         validators = {}
-        for validator in self.models.get_validators(height):
+        for validator in self.models.get_validators(height=height):
             # NOTE: we assume that Tendermint encodes public key in base64
             public_key = public_key_from_ed25519_key(key_from_base64(validator["public_key"]["value"]))
             validators[public_key] = validator["voting_power"]
 
         return validators
 
     # TODO to be moved to planetmint.commands.planetmint
@@ -489,15 +489,15 @@
         election rules. Consider the current database state to account for
         other concluded elections, if required.
         """
         if election.operation == CHAIN_MIGRATION_ELECTION:
             self.migrate_abci_chain()
         if election.operation == VALIDATOR_ELECTION:
             validator_updates = [election.assets[0].data]
-            curr_validator_set = self.models.get_validators(new_height)
+            curr_validator_set = self.models.get_validators(height=new_height)
             updated_validator_set = new_validator_set(curr_validator_set, validator_updates)
 
             updated_validator_set = [v for v in updated_validator_set if v["voting_power"] > 0]
 
             # TODO change to `new_height + 2` when upgrading to Tendermint 0.24.0.
             self.models.store_validator_set(new_height + 1, updated_validator_set)
             return encode_validator(election.assets[0].data)
```

### Comparing `planetmint-2.4.4/planetmint/backend/README.md` & `planetmint-2.4.5/planetmint/backend/README.md`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.4/planetmint/backend/__init__.py` & `planetmint-2.4.5/planetmint/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.4/planetmint/backend/connection.py` & `planetmint-2.4.5/planetmint/backend/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,14 @@
         host: str = None,
         port: int = None,
         login: str = None,
         password: str = None,
         backend: str = None,
         connection_timeout: int = None,
         max_tries: int = None,
-        async_io: bool = False,
         **kwargs
     ):
         """Create a new :class:`~.Connection` instance.
 
         Args:
             host (str): the host to connect to.
             port (int): the port to connect to.
```

### Comparing `planetmint-2.4.4/planetmint/backend/exceptions.py` & `planetmint-2.4.5/planetmint/backend/exceptions.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.4/planetmint/backend/localmongodb/__init__.py` & `planetmint-2.4.5/planetmint/backend/localmongodb/__init__.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.4/planetmint/backend/localmongodb/connection.py` & `planetmint-2.4.5/planetmint/backend/localmongodb/connection.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.4/planetmint/backend/localmongodb/query.py` & `planetmint-2.4.5/planetmint/backend/localmongodb/query.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.4/planetmint/backend/localmongodb/schema.py` & `planetmint-2.4.5/planetmint/backend/localmongodb/schema.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.4/planetmint/backend/models/asset.py` & `planetmint-2.4.5/planetmint/backend/models/asset.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.4/planetmint/backend/models/block.py` & `planetmint-2.4.5/planetmint/backend/models/block.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.4/planetmint/backend/models/dbtransaction.py` & `planetmint-2.4.5/planetmint/backend/models/dbtransaction.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.4/planetmint/backend/models/input.py` & `planetmint-2.4.5/planetmint/backend/models/input.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.4/planetmint/backend/models/metadata.py` & `planetmint-2.4.5/planetmint/backend/models/metadata.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.4/planetmint/backend/models/output.py` & `planetmint-2.4.5/planetmint/backend/models/output.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.4/planetmint/backend/models/script.py` & `planetmint-2.4.5/planetmint/backend/models/script.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.4/planetmint/backend/query.py` & `planetmint-2.4.5/planetmint/backend/query.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.4/planetmint/backend/schema.py` & `planetmint-2.4.5/planetmint/backend/schema.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.4/planetmint/backend/tarantool/const.py` & `planetmint-2.4.5/planetmint/backend/tarantool/const.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.4/planetmint/backend/tarantool/opt/init.lua` & `planetmint-2.4.5/planetmint/backend/tarantool/opt/init.lua`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.4/planetmint/backend/tarantool/sync_io/connection.py` & `planetmint-2.4.5/planetmint/backend/tarantool/sync_io/connection.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.4/planetmint/backend/tarantool/sync_io/query.py` & `planetmint-2.4.5/planetmint/backend/tarantool/sync_io/query.py`

 * *Files 0% similar despite different names*

```diff
@@ -403,19 +403,20 @@
 @register_query(TarantoolDBConnection)
 @catch_db_exception
 def store_validator_set(conn, validators_update: dict):
     _validator = (
         conn.connect().select(TARANT_TABLE_VALIDATOR_SETS, validators_update["height"], index="height", limit=1).data
     )
     unique_id = uuid4().hex if _validator is None or len(_validator) == 0 else _validator[0][0]
-    conn.connect().upsert(
+    result = conn.connect().upsert(
         TARANT_TABLE_VALIDATOR_SETS,
         (unique_id, validators_update["height"], validators_update["validators"]),
         op_list=[("=", 1, validators_update["height"]), ("=", 2, validators_update["validators"])],
     )
+    return result
 
 
 @register_query(TarantoolDBConnection)
 @catch_db_exception
 def delete_validator_set(connection, height: int):
     _validators = connection.connect().select(TARANT_TABLE_VALIDATOR_SETS, height, index="height").data
     for _valid in _validators:
```

### Comparing `planetmint-2.4.4/planetmint/backend/tarantool/sync_io/schema.py` & `planetmint-2.4.5/planetmint/backend/tarantool/sync_io/schema.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.4/planetmint/backend/tarantool/tarantool.md` & `planetmint-2.4.5/planetmint/backend/tarantool/tarantool.md`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.4/planetmint/backend/utils.py` & `planetmint-2.4.5/planetmint/backend/utils.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.4/planetmint/commands/election_types.py` & `planetmint-2.4.5/planetmint/commands/election_types.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.4/planetmint/commands/planetmint.py` & `planetmint-2.4.5/planetmint/commands/planetmint.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.4/planetmint/commands/utils.py` & `planetmint-2.4.5/planetmint/commands/utils.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.4/planetmint/config.py` & `planetmint-2.4.5/planetmint/config.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.4/planetmint/config_utils.py` & `planetmint-2.4.5/planetmint/config_utils.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.4/planetmint/ipc/events.py` & `planetmint-2.4.5/planetmint/ipc/events.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.4/planetmint/ipc/exchange.py` & `planetmint-2.4.5/planetmint/ipc/exchange.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.4/planetmint/model/dataaccessor.py` & `planetmint-2.4.5/planetmint/model/dataaccessor.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,20 +18,27 @@
     TARANT_TABLE_OUTPUT,
 )
 from planetmint.backend.models.block import Block
 from planetmint.backend.models.output import Output
 from planetmint.backend.models.asset import Asset
 from planetmint.backend.models.metadata import MetaData
 from planetmint.backend.models.dbtransaction import DbTransaction
+from planetmint.utils.singleton import Singleton
 
 
-class DataAccessor:
-    def __init__(self, database_connection=None, async_io: bool = False):
+class DataAccessor(metaclass=Singleton):
+    def __init__(self, database_connection=None):
         config_utils.autoconfigure()
-        self.connection = database_connection if database_connection is not None else Connection(async_io=async_io)
+        self.connection = database_connection if database_connection is not None else Connection()
+
+    def close_connection(self):
+        self.connection.close()
+
+    def connect(self):
+        self.connection.connect()
 
     def store_bulk_transactions(self, transactions):
         txns = []
         gov_txns = []
 
         for t in transactions:
             transaction = t.tx_dict if t.tx_dict else rapidjson.loads(rapidjson.dumps(t.to_dict()))
@@ -140,15 +147,15 @@
 
     # NOTE: moved here from Election needs to be placed somewhere else
     def get_validators_dict(self, height=None):
         """Return a dictionary of validators with key as `public_key` and
         value as the `voting_power`
         """
         validators = {}
-        for validator in self.get_validators(height):
+        for validator in self.get_validators(height=height):
             # NOTE: we assume that Tendermint encodes public key in base64
             public_key = public_key_from_ed25519_key(key_from_base64(validator["public_key"]["value"]))
             validators[public_key] = validator["voting_power"]
 
         return validators
 
     def get_spending_transaction(self, txid, output, current_transactions=[]) -> DbTransaction:
```

### Comparing `planetmint-2.4.4/planetmint/start.py` & `planetmint-2.4.5/planetmint/start.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.4/planetmint/utils/lazy.py` & `planetmint-2.4.5/planetmint/utils/lazy.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.4/planetmint/utils/processes.py` & `planetmint-2.4.5/planetmint/utils/processes.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.4/planetmint/web/routes.py` & `planetmint-2.4.5/planetmint/web/routes.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.4/planetmint/web/server.py` & `planetmint-2.4.5/planetmint/web/server.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.4/planetmint/web/strip_content_type_middleware.py` & `planetmint-2.4.5/planetmint/web/strip_content_type_middleware.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.4/planetmint/web/views/assets.py` & `planetmint-2.4.5/planetmint/web/views/assets.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.4/planetmint/web/views/base.py` & `planetmint-2.4.5/planetmint/web/views/base.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.4/planetmint/web/views/blocks.py` & `planetmint-2.4.5/planetmint/web/views/blocks.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.4/planetmint/web/views/info.py` & `planetmint-2.4.5/planetmint/web/views/info.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.4/planetmint/web/views/metadata.py` & `planetmint-2.4.5/planetmint/web/views/metadata.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.4/planetmint/web/views/outputs.py` & `planetmint-2.4.5/planetmint/web/views/outputs.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.4/planetmint/web/views/parameters.py` & `planetmint-2.4.5/planetmint/web/views/parameters.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.4/planetmint/web/views/transactions.py` & `planetmint-2.4.5/planetmint/web/views/transactions.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.4/planetmint/web/views/validators.py` & `planetmint-2.4.5/planetmint/web/views/validators.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.4/planetmint/web/websocket_dispatcher.py` & `planetmint-2.4.5/planetmint/web/websocket_dispatcher.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.4/planetmint/web/websocket_server.py` & `planetmint-2.4.5/planetmint/web/websocket_server.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.4/pyproject.toml` & `planetmint-2.4.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "planetmint"
-version = "2.4.4"
+version = "2.4.5"
 description = "Planetmint: The Blockchain Database"
 authors = ["Planetmint contributors"]
 license = "AGPLv3"
 readme = "README.md"
 classifiers = [
   "Development Status :: 4 - Beta",
   "Intended Audience :: Developers",
```

### Comparing `planetmint-2.4.4/PKG-INFO` & `planetmint-2.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planetmint
-Version: 2.4.4
+Version: 2.4.5
 Summary: Planetmint: The Blockchain Database
 License: AGPLv3
 Author: Planetmint contributors
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

