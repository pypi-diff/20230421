# Comparing `tmp/snowflake-connector-python-3.0.2.tar.gz` & `tmp/snowflake-connector-python-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snowflake-connector-python-3.0.2.tar", last modified: Thu Mar 23 18:13:34 2023, max compression
+gzip compressed data, was "snowflake-connector-python-3.0.3.tar", last modified: Thu Apr 20 20:32:57 2023, max compression
```

## Comparing `snowflake-connector-python-3.0.2.tar` & `snowflake-connector-python-3.0.3.tar`

### file list

```diff
@@ -1,200 +1,200 @@
-drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-03-23 18:13:34.872110 snowflake-connector-python-3.0.2/
--rw-r--r--   0 user      (1005) user      (1005)     1480 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/CONTRIBUTING.md
--rw-r--r--   0 user      (1005) user      (1005)    45719 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/DESCRIPTION.md
--rw-r--r--   0 user      (1005) user      (1005)    11365 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/LICENSE.txt
--rw-r--r--   0 user      (1005) user      (1005)      578 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/MANIFEST.in
--rw-r--r--   0 user      (1005) user      (1005)      457 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/NOTICE
--rw-r--r--   0 user      (1005) user      (1005)    47777 2023-03-23 18:13:34.872110 snowflake-connector-python-3.0.2/PKG-INFO
--rw-r--r--   0 user      (1005) user      (1005)     3045 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/README.md
--rw-r--r--   0 user      (1005) user      (1005)      308 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/SECURITY.md
--rw-r--r--   0 user      (1005) user      (1005)      696 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/pyproject.toml
--rw-r--r--   0 user      (1005) user      (1005)     2996 2023-03-23 18:13:34.872110 snowflake-connector-python-3.0.2/setup.cfg
--rw-r--r--   0 user      (1005) user      (1005)     8264 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/setup.py
-drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-03-23 18:13:34.824110 snowflake-connector-python-3.0.2/src/
-drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-03-23 18:13:34.824110 snowflake-connector-python-3.0.2/src/snowflake/
-drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-03-23 18:13:34.840110 snowflake-connector-python-3.0.2/src/snowflake/connector/
--rw-r--r--   0 user      (1005) user      (1005)     1693 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/__init__.py
--rw-r--r--   0 user      (1005) user      (1005)     1521 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/_sql_util.py
--rw-r--r--   0 user      (1005) user      (1005)     4888 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/arrow_context.py
--rw-r--r--   0 user      (1005) user      (1005)     6959 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/arrow_iterator.pyx
-drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-03-23 18:13:34.844110 snowflake-connector-python-3.0.2/src/snowflake/connector/auth/
--rw-r--r--   0 user      (1005) user      (1005)      991 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/auth/__init__.py
--rw-r--r--   0 user      (1005) user      (1005)    27245 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/auth/_auth.py
--rw-r--r--   0 user      (1005) user      (1005)     6999 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/auth/by_plugin.py
--rw-r--r--   0 user      (1005) user      (1005)     1016 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/auth/default.py
--rw-r--r--   0 user      (1005) user      (1005)     2006 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/auth/idtoken.py
--rw-r--r--   0 user      (1005) user      (1005)     6369 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/auth/keypair.py
--rw-r--r--   0 user      (1005) user      (1005)     1470 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/auth/oauth.py
--rw-r--r--   0 user      (1005) user      (1005)    10609 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/auth/okta.py
--rw-r--r--   0 user      (1005) user      (1005)     1955 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/auth/usrpwdmfa.py
--rw-r--r--   0 user      (1005) user      (1005)    14011 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/auth/webbrowser.py
--rw-r--r--   0 user      (1005) user      (1005)     9873 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/azure_storage_client.py
--rw-r--r--   0 user      (1005) user      (1005)     2355 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/bind_upload_agent.py
--rw-r--r--   0 user      (1005) user      (1005)    20410 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/cache.py
--rw-r--r--   0 user      (1005) user      (1005)     2894 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/compat.py
--rw-r--r--   0 user      (1005) user      (1005)    63767 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/connection.py
--rw-r--r--   0 user      (1005) user      (1005)    30347 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/connection_diagnostic.py
--rw-r--r--   0 user      (1005) user      (1005)     8703 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/constants.py
--rw-r--r--   0 user      (1005) user      (1005)    25717 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/converter.py
--rw-r--r--   0 user      (1005) user      (1005)     2822 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/converter_issue23517.py
--rw-r--r--   0 user      (1005) user      (1005)      437 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/converter_null.py
--rw-r--r--   0 user      (1005) user      (1005)     7633 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/converter_snowsql.py
-drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-03-23 18:13:34.824110 snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/
-drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-03-23 18:13:34.848110 snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/
--rw-r--r--   0 user      (1005) user      (1005)      651 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/BinaryConverter.cpp
--rw-r--r--   0 user      (1005) user      (1005)      555 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/BinaryConverter.hpp
--rw-r--r--   0 user      (1005) user      (1005)      565 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/BooleanConverter.cpp
--rw-r--r--   0 user      (1005) user      (1005)      512 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/BooleanConverter.hpp
--rw-r--r--   0 user      (1005) user      (1005)    14375 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/CArrowChunkIterator.cpp
--rw-r--r--   0 user      (1005) user      (1005)     2308 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/CArrowChunkIterator.hpp
--rw-r--r--   0 user      (1005) user      (1005)      443 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/CArrowIterator.cpp
--rw-r--r--   0 user      (1005) user      (1005)     1793 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/CArrowIterator.hpp
--rw-r--r--   0 user      (1005) user      (1005)    34612 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/CArrowTableIterator.cpp
--rw-r--r--   0 user      (1005) user      (1005)     5606 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/CArrowTableIterator.hpp
--rw-r--r--   0 user      (1005) user      (1005)     1601 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/DateConverter.cpp
--rw-r--r--   0 user      (1005) user      (1005)     1036 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/DateConverter.hpp
--rw-r--r--   0 user      (1005) user      (1005)     1625 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/DecimalConverter.cpp
--rw-r--r--   0 user      (1005) user      (1005)     2769 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/DecimalConverter.hpp
--rw-r--r--   0 user      (1005) user      (1005)     1032 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/FloatConverter.cpp
--rw-r--r--   0 user      (1005) user      (1005)      800 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/FloatConverter.hpp
--rw-r--r--   0 user      (1005) user      (1005)      472 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/IColumnConverter.hpp
--rw-r--r--   0 user      (1005) user      (1005)      240 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/IntConverter.cpp
--rw-r--r--   0 user      (1005) user      (1005)     1687 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/IntConverter.hpp
-drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-03-23 18:13:34.852110 snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/Python/
--rw-r--r--   0 user      (1005) user      (1005)      218 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/Python/Common.cpp
--rw-r--r--   0 user      (1005) user      (1005)     2335 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/Python/Common.hpp
--rw-r--r--   0 user      (1005) user      (1005)     1457 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/Python/Helpers.cpp
--rw-r--r--   0 user      (1005) user      (1005)      939 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/Python/Helpers.hpp
--rw-r--r--   0 user      (1005) user      (1005)     1287 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/SnowflakeType.cpp
--rw-r--r--   0 user      (1005) user      (1005)      884 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/SnowflakeType.hpp
--rw-r--r--   0 user      (1005) user      (1005)      649 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/StringConverter.cpp
--rw-r--r--   0 user      (1005) user      (1005)      555 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/StringConverter.hpp
--rw-r--r--   0 user      (1005) user      (1005)      241 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/TimeConverter.cpp
--rw-r--r--   0 user      (1005) user      (1005)     1838 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/TimeConverter.hpp
--rw-r--r--   0 user      (1005) user      (1005)     9470 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/TimeStampConverter.cpp
--rw-r--r--   0 user      (1005) user      (1005)     4063 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/TimeStampConverter.hpp
-drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-03-23 18:13:34.852110 snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/Util/
--rw-r--r--   0 user      (1005) user      (1005)      470 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/Util/macros.hpp
--rw-r--r--   0 user      (1005) user      (1005)     2013 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/Util/time.cpp
--rw-r--r--   0 user      (1005) user      (1005)     2269 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/Util/time.hpp
-drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-03-23 18:13:34.852110 snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/Logging/
--rw-r--r--   0 user      (1005) user      (1005)     3008 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/Logging/logging.cpp
--rw-r--r--   0 user      (1005) user      (1005)     1280 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/Logging/logging.hpp
--rw-r--r--   0 user      (1005) user      (1005)    54238 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/cursor.py
--rw-r--r--   0 user      (1005) user      (1005)     1268 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/dbapi.py
--rw-r--r--   0 user      (1005) user      (1005)      615 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/description.py
--rw-r--r--   0 user      (1005) user      (1005)     9376 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/encryption_util.py
--rw-r--r--   0 user      (1005) user      (1005)     2646 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/errorcode.py
--rw-r--r--   0 user      (1005) user      (1005)    19004 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/errors.py
--rw-r--r--   0 user      (1005) user      (1005)      184 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/feature.py
--rw-r--r--   0 user      (1005) user      (1005)     3246 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/file_compression_type.py
--rw-r--r--   0 user      (1005) user      (1005)    46365 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/file_transfer_agent.py
--rw-r--r--   0 user      (1005) user      (1005)     5427 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/file_util.py
--rw-r--r--   0 user      (1005) user      (1005)    16071 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/gcs_storage_client.py
--rw-r--r--   0 user      (1005) user      (1005)     2802 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/gzip_decoder.py
--rw-r--r--   0 user      (1005) user      (1005)     2919 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/local_storage_client.py
--rw-r--r--   0 user      (1005) user      (1005)    39670 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/network.py
--rw-r--r--   0 user      (1005) user      (1005)    18430 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/ocsp_asn1crypto.py
--rw-r--r--   0 user      (1005) user      (1005)    68441 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/ocsp_snowflake.py
--rw-r--r--   0 user      (1005) user      (1005)     4672 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/options.py
--rw-r--r--   0 user      (1005) user      (1005)    15817 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/pandas_tools.py
--rw-r--r--   0 user      (1005) user      (1005)     1582 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/proxy.py
--rw-r--r--   0 user      (1005) user      (1005)        0 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/py.typed
--rw-r--r--   0 user      (1005) user      (1005)    24990 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/result_batch.py
--rw-r--r--   0 user      (1005) user      (1005)     8797 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/result_set.py
--rw-r--r--   0 user      (1005) user      (1005)    21830 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/s3_storage_client.py
--rw-r--r--   0 user      (1005) user      (1005)     5343 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/secret_detector.py
--rw-r--r--   0 user      (1005) user      (1005)     1120 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/sfbinaryformat.py
--rw-r--r--   0 user      (1005) user      (1005)    12449 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/sfdatetime.py
--rw-r--r--   0 user      (1005) user      (1005)     4313 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/snow_logging.py
--rw-r--r--   0 user      (1005) user      (1005)      432 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/sqlstate.py
--rw-r--r--   0 user      (1005) user      (1005)      813 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/ssd_internal_keys.py
--rw-r--r--   0 user      (1005) user      (1005)     4559 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/ssl_wrap_socket.py
--rw-r--r--   0 user      (1005) user      (1005)    16995 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/storage_client.py
--rw-r--r--   0 user      (1005) user      (1005)     8861 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/telemetry.py
--rw-r--r--   0 user      (1005) user      (1005)    18837 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/telemetry_oob.py
--rw-r--r--   0 user      (1005) user      (1005)      982 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/test_util.py
--rw-r--r--   0 user      (1005) user      (1005)     2795 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/time_util.py
-drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-03-23 18:13:34.852110 snowflake-connector-python-3.0.2/src/snowflake/connector/tool/
--rw-r--r--   0 user      (1005) user      (1005)       76 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/tool/__init__.py
--rw-r--r--   0 user      (1005) user      (1005)     1485 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/tool/dump_certs.py
--rw-r--r--   0 user      (1005) user      (1005)     4575 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/tool/dump_ocsp_response.py
--rw-r--r--   0 user      (1005) user      (1005)     6601 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/tool/dump_ocsp_response_cache.py
--rw-r--r--   0 user      (1005) user      (1005)     2119 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/tool/probe_connection.py
--rw-r--r--   0 user      (1005) user      (1005)     1021 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/url_util.py
--rw-r--r--   0 user      (1005) user      (1005)    10405 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/util_text.py
-drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-03-23 18:13:34.852110 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/
--rw-r--r--   0 user      (1005) user      (1005)       76 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/__init__.py
-drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-03-23 18:13:34.860110 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/requests/
--rw-r--r--   0 user      (1005) user      (1005)    10142 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/requests/LICENSE
--rw-r--r--   0 user      (1005) user      (1005)     4751 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/requests/__init__.py
--rw-r--r--   0 user      (1005) user      (1005)      440 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/requests/__version__.py
--rw-r--r--   0 user      (1005) user      (1005)     1397 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/requests/_internal_utils.py
--rw-r--r--   0 user      (1005) user      (1005)    21313 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/requests/adapters.py
--rw-r--r--   0 user      (1005) user      (1005)     6377 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/requests/api.py
--rw-r--r--   0 user      (1005) user      (1005)    10187 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/requests/auth.py
--rw-r--r--   0 user      (1005) user      (1005)      429 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/requests/certs.py
--rw-r--r--   0 user      (1005) user      (1005)     1451 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/requests/compat.py
--rw-r--r--   0 user      (1005) user      (1005)    18560 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/requests/cookies.py
--rw-r--r--   0 user      (1005) user      (1005)     3813 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/requests/exceptions.py
--rw-r--r--   0 user      (1005) user      (1005)     3885 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/requests/help.py
--rw-r--r--   0 user      (1005) user      (1005)      733 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/requests/hooks.py
--rw-r--r--   0 user      (1005) user      (1005)    35230 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/requests/models.py
--rw-r--r--   0 user      (1005) user      (1005)    30180 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/requests/sessions.py
--rw-r--r--   0 user      (1005) user      (1005)     4235 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/requests/status_codes.py
--rw-r--r--   0 user      (1005) user      (1005)     2912 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/requests/structures.py
--rw-r--r--   0 user      (1005) user      (1005)    33230 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/requests/utils.py
-drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-03-23 18:13:34.860110 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/
--rw-r--r--   0 user      (1005) user      (1005)     1115 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/LICENSE.txt
--rw-r--r--   0 user      (1005) user      (1005)     2763 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/__init__.py
--rw-r--r--   0 user      (1005) user      (1005)    10811 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/_collections.py
--rw-r--r--   0 user      (1005) user      (1005)       64 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/_version.py
--rw-r--r--   0 user      (1005) user      (1005)    20070 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/connection.py
--rw-r--r--   0 user      (1005) user      (1005)    39093 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/connectionpool.py
-drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-03-23 18:13:34.864110 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/contrib/
--rw-r--r--   0 user      (1005) user      (1005)        0 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/contrib/__init__.py
--rw-r--r--   0 user      (1005) user      (1005)      957 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/contrib/_appengine_environ.py
-drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-03-23 18:13:34.864110 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/
--rw-r--r--   0 user      (1005) user      (1005)        0 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/__init__.py
--rw-r--r--   0 user      (1005) user      (1005)    17632 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/bindings.py
--rw-r--r--   0 user      (1005) user      (1005)    13922 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/low_level.py
--rw-r--r--   0 user      (1005) user      (1005)    11010 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/contrib/appengine.py
--rw-r--r--   0 user      (1005) user      (1005)     4538 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/contrib/ntlmpool.py
--rw-r--r--   0 user      (1005) user      (1005)    16385 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/contrib/pyopenssl.py
--rw-r--r--   0 user      (1005) user      (1005)    34416 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/contrib/securetransport.py
--rw-r--r--   0 user      (1005) user      (1005)     7097 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/contrib/socks.py
--rw-r--r--   0 user      (1005) user      (1005)     8217 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/exceptions.py
--rw-r--r--   0 user      (1005) user      (1005)     8579 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/fields.py
--rw-r--r--   0 user      (1005) user      (1005)     2440 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/filepost.py
-drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-03-23 18:13:34.864110 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/packages/
--rw-r--r--   0 user      (1005) user      (1005)        0 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/packages/__init__.py
-drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-03-23 18:13:34.864110 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/packages/backports/
--rw-r--r--   0 user      (1005) user      (1005)        0 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/packages/backports/__init__.py
--rw-r--r--   0 user      (1005) user      (1005)     1417 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/packages/backports/makefile.py
--rw-r--r--   0 user      (1005) user      (1005)    34665 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/packages/six.py
--rw-r--r--   0 user      (1005) user      (1005)    19786 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/poolmanager.py
--rw-r--r--   0 user      (1005) user      (1005)     5985 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/request.py
--rw-r--r--   0 user      (1005) user      (1005)    28276 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/response.py
-drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-03-23 18:13:34.868110 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/util/
--rw-r--r--   0 user      (1005) user      (1005)     1155 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/util/__init__.py
--rw-r--r--   0 user      (1005) user      (1005)     4901 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/util/connection.py
--rw-r--r--   0 user      (1005) user      (1005)     1605 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/util/proxy.py
--rw-r--r--   0 user      (1005) user      (1005)      498 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/util/queue.py
--rw-r--r--   0 user      (1005) user      (1005)     4225 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/util/request.py
--rw-r--r--   0 user      (1005) user      (1005)     3510 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/util/response.py
--rw-r--r--   0 user      (1005) user      (1005)    22001 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/util/retry.py
--rw-r--r--   0 user      (1005) user      (1005)    17165 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/util/ssl_.py
--rw-r--r--   0 user      (1005) user      (1005)     5758 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/util/ssl_match_hostname.py
--rw-r--r--   0 user      (1005) user      (1005)     6895 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/util/ssltransport.py
--rw-r--r--   0 user      (1005) user      (1005)    10003 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/util/timeout.py
--rw-r--r--   0 user      (1005) user      (1005)    14270 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/util/url.py
--rw-r--r--   0 user      (1005) user      (1005)     5403 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/util/wait.py
--rw-r--r--   0 user      (1005) user      (1005)      107 2023-03-23 18:06:38.000000 snowflake-connector-python-3.0.2/src/snowflake/connector/version.py
-drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-03-23 18:13:34.868110 snowflake-connector-python-3.0.2/src/snowflake_connector_python.egg-info/
--rw-r--r--   0 user      (1005) user      (1005)    47777 2023-03-23 18:13:34.000000 snowflake-connector-python-3.0.2/src/snowflake_connector_python.egg-info/PKG-INFO
--rw-r--r--   0 user      (1005) user      (1005)     8774 2023-03-23 18:13:34.000000 snowflake-connector-python-3.0.2/src/snowflake_connector_python.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1005) user      (1005)        1 2023-03-23 18:13:34.000000 snowflake-connector-python-3.0.2/src/snowflake_connector_python.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1005) user      (1005)      322 2023-03-23 18:13:34.000000 snowflake-connector-python-3.0.2/src/snowflake_connector_python.egg-info/entry_points.txt
--rw-r--r--   0 user      (1005) user      (1005)        1 2023-03-23 18:07:20.000000 snowflake-connector-python-3.0.2/src/snowflake_connector_python.egg-info/not-zip-safe
--rw-r--r--   0 user      (1005) user      (1005)      623 2023-03-23 18:13:34.000000 snowflake-connector-python-3.0.2/src/snowflake_connector_python.egg-info/requires.txt
--rw-r--r--   0 user      (1005) user      (1005)       10 2023-03-23 18:13:34.000000 snowflake-connector-python-3.0.2/src/snowflake_connector_python.egg-info/top_level.txt
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-04-20 20:32:57.279553 snowflake-connector-python-3.0.3/
+-rw-r--r--   0 user      (1005) user      (1005)     1479 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/CONTRIBUTING.md
+-rw-r--r--   0 user      (1005) user      (1005)    46505 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/DESCRIPTION.md
+-rw-r--r--   0 user      (1005) user      (1005)    11365 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/LICENSE.txt
+-rw-r--r--   0 user      (1005) user      (1005)      578 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/MANIFEST.in
+-rw-r--r--   0 user      (1005) user      (1005)      457 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/NOTICE
+-rw-r--r--   0 user      (1005) user      (1005)    48563 2023-04-20 20:32:57.279553 snowflake-connector-python-3.0.3/PKG-INFO
+-rw-r--r--   0 user      (1005) user      (1005)     3045 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/README.md
+-rw-r--r--   0 user      (1005) user      (1005)      308 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/SECURITY.md
+-rw-r--r--   0 user      (1005) user      (1005)      696 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/pyproject.toml
+-rw-r--r--   0 user      (1005) user      (1005)     2996 2023-04-20 20:32:57.279553 snowflake-connector-python-3.0.3/setup.cfg
+-rw-r--r--   0 user      (1005) user      (1005)     8264 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/setup.py
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-04-20 20:32:57.239553 snowflake-connector-python-3.0.3/src/
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-04-20 20:32:57.239553 snowflake-connector-python-3.0.3/src/snowflake/
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-04-20 20:32:57.255553 snowflake-connector-python-3.0.3/src/snowflake/connector/
+-rw-r--r--   0 user      (1005) user      (1005)     1693 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/__init__.py
+-rw-r--r--   0 user      (1005) user      (1005)     1521 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/_sql_util.py
+-rw-r--r--   0 user      (1005) user      (1005)     4888 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/arrow_context.py
+-rw-r--r--   0 user      (1005) user      (1005)     6959 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/arrow_iterator.pyx
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-04-20 20:32:57.255553 snowflake-connector-python-3.0.3/src/snowflake/connector/auth/
+-rw-r--r--   0 user      (1005) user      (1005)      991 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/auth/__init__.py
+-rw-r--r--   0 user      (1005) user      (1005)    27245 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/auth/_auth.py
+-rw-r--r--   0 user      (1005) user      (1005)     6999 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/auth/by_plugin.py
+-rw-r--r--   0 user      (1005) user      (1005)     1016 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/auth/default.py
+-rw-r--r--   0 user      (1005) user      (1005)     2006 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/auth/idtoken.py
+-rw-r--r--   0 user      (1005) user      (1005)     6369 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/auth/keypair.py
+-rw-r--r--   0 user      (1005) user      (1005)     1470 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/auth/oauth.py
+-rw-r--r--   0 user      (1005) user      (1005)    10609 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/auth/okta.py
+-rw-r--r--   0 user      (1005) user      (1005)     1955 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/auth/usrpwdmfa.py
+-rw-r--r--   0 user      (1005) user      (1005)    14011 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/auth/webbrowser.py
+-rw-r--r--   0 user      (1005) user      (1005)     9873 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/azure_storage_client.py
+-rw-r--r--   0 user      (1005) user      (1005)     2355 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/bind_upload_agent.py
+-rw-r--r--   0 user      (1005) user      (1005)    20410 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/cache.py
+-rw-r--r--   0 user      (1005) user      (1005)     2894 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/compat.py
+-rw-r--r--   0 user      (1005) user      (1005)    63767 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/connection.py
+-rw-r--r--   0 user      (1005) user      (1005)    30347 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/connection_diagnostic.py
+-rw-r--r--   0 user      (1005) user      (1005)     8703 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/constants.py
+-rw-r--r--   0 user      (1005) user      (1005)    25717 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/converter.py
+-rw-r--r--   0 user      (1005) user      (1005)     2822 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/converter_issue23517.py
+-rw-r--r--   0 user      (1005) user      (1005)      437 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/converter_null.py
+-rw-r--r--   0 user      (1005) user      (1005)     7633 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/converter_snowsql.py
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-04-20 20:32:57.239553 snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-04-20 20:32:57.263553 snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/
+-rw-r--r--   0 user      (1005) user      (1005)      651 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/BinaryConverter.cpp
+-rw-r--r--   0 user      (1005) user      (1005)      555 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/BinaryConverter.hpp
+-rw-r--r--   0 user      (1005) user      (1005)      565 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/BooleanConverter.cpp
+-rw-r--r--   0 user      (1005) user      (1005)      512 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/BooleanConverter.hpp
+-rw-r--r--   0 user      (1005) user      (1005)    14375 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/CArrowChunkIterator.cpp
+-rw-r--r--   0 user      (1005) user      (1005)     2308 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/CArrowChunkIterator.hpp
+-rw-r--r--   0 user      (1005) user      (1005)      443 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/CArrowIterator.cpp
+-rw-r--r--   0 user      (1005) user      (1005)     1793 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/CArrowIterator.hpp
+-rw-r--r--   0 user      (1005) user      (1005)    34612 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/CArrowTableIterator.cpp
+-rw-r--r--   0 user      (1005) user      (1005)     5606 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/CArrowTableIterator.hpp
+-rw-r--r--   0 user      (1005) user      (1005)     1601 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/DateConverter.cpp
+-rw-r--r--   0 user      (1005) user      (1005)     1036 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/DateConverter.hpp
+-rw-r--r--   0 user      (1005) user      (1005)     1625 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/DecimalConverter.cpp
+-rw-r--r--   0 user      (1005) user      (1005)     2769 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/DecimalConverter.hpp
+-rw-r--r--   0 user      (1005) user      (1005)     1032 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/FloatConverter.cpp
+-rw-r--r--   0 user      (1005) user      (1005)      800 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/FloatConverter.hpp
+-rw-r--r--   0 user      (1005) user      (1005)      472 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/IColumnConverter.hpp
+-rw-r--r--   0 user      (1005) user      (1005)      240 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/IntConverter.cpp
+-rw-r--r--   0 user      (1005) user      (1005)     1687 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/IntConverter.hpp
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-04-20 20:32:57.263553 snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/Python/
+-rw-r--r--   0 user      (1005) user      (1005)      218 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/Python/Common.cpp
+-rw-r--r--   0 user      (1005) user      (1005)     2335 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/Python/Common.hpp
+-rw-r--r--   0 user      (1005) user      (1005)     1457 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/Python/Helpers.cpp
+-rw-r--r--   0 user      (1005) user      (1005)      939 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/Python/Helpers.hpp
+-rw-r--r--   0 user      (1005) user      (1005)     1287 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/SnowflakeType.cpp
+-rw-r--r--   0 user      (1005) user      (1005)      884 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/SnowflakeType.hpp
+-rw-r--r--   0 user      (1005) user      (1005)      649 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/StringConverter.cpp
+-rw-r--r--   0 user      (1005) user      (1005)      555 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/StringConverter.hpp
+-rw-r--r--   0 user      (1005) user      (1005)      241 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/TimeConverter.cpp
+-rw-r--r--   0 user      (1005) user      (1005)     1838 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/TimeConverter.hpp
+-rw-r--r--   0 user      (1005) user      (1005)     9470 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/TimeStampConverter.cpp
+-rw-r--r--   0 user      (1005) user      (1005)     4063 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/TimeStampConverter.hpp
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-04-20 20:32:57.263553 snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/Util/
+-rw-r--r--   0 user      (1005) user      (1005)      470 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/Util/macros.hpp
+-rw-r--r--   0 user      (1005) user      (1005)     2013 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/Util/time.cpp
+-rw-r--r--   0 user      (1005) user      (1005)     2269 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/Util/time.hpp
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-04-20 20:32:57.263553 snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/Logging/
+-rw-r--r--   0 user      (1005) user      (1005)     3008 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/Logging/logging.cpp
+-rw-r--r--   0 user      (1005) user      (1005)     1280 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/Logging/logging.hpp
+-rw-r--r--   0 user      (1005) user      (1005)    56987 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/cursor.py
+-rw-r--r--   0 user      (1005) user      (1005)     1268 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/dbapi.py
+-rw-r--r--   0 user      (1005) user      (1005)      615 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/description.py
+-rw-r--r--   0 user      (1005) user      (1005)     9376 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/encryption_util.py
+-rw-r--r--   0 user      (1005) user      (1005)     2646 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/errorcode.py
+-rw-r--r--   0 user      (1005) user      (1005)    19004 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/errors.py
+-rw-r--r--   0 user      (1005) user      (1005)      184 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/feature.py
+-rw-r--r--   0 user      (1005) user      (1005)     3246 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/file_compression_type.py
+-rw-r--r--   0 user      (1005) user      (1005)    47199 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/file_transfer_agent.py
+-rw-r--r--   0 user      (1005) user      (1005)     5427 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/file_util.py
+-rw-r--r--   0 user      (1005) user      (1005)    16068 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/gcs_storage_client.py
+-rw-r--r--   0 user      (1005) user      (1005)     2802 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/gzip_decoder.py
+-rw-r--r--   0 user      (1005) user      (1005)     2919 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/local_storage_client.py
+-rw-r--r--   0 user      (1005) user      (1005)    39670 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/network.py
+-rw-r--r--   0 user      (1005) user      (1005)    18430 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/ocsp_asn1crypto.py
+-rw-r--r--   0 user      (1005) user      (1005)    68441 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/ocsp_snowflake.py
+-rw-r--r--   0 user      (1005) user      (1005)     4673 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/options.py
+-rw-r--r--   0 user      (1005) user      (1005)    17118 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/pandas_tools.py
+-rw-r--r--   0 user      (1005) user      (1005)     1582 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/proxy.py
+-rw-r--r--   0 user      (1005) user      (1005)        0 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/py.typed
+-rw-r--r--   0 user      (1005) user      (1005)    24990 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/result_batch.py
+-rw-r--r--   0 user      (1005) user      (1005)     8797 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/result_set.py
+-rw-r--r--   0 user      (1005) user      (1005)    21830 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/s3_storage_client.py
+-rw-r--r--   0 user      (1005) user      (1005)     5343 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/secret_detector.py
+-rw-r--r--   0 user      (1005) user      (1005)     1120 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/sfbinaryformat.py
+-rw-r--r--   0 user      (1005) user      (1005)    12449 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/sfdatetime.py
+-rw-r--r--   0 user      (1005) user      (1005)     4313 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/snow_logging.py
+-rw-r--r--   0 user      (1005) user      (1005)      432 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/sqlstate.py
+-rw-r--r--   0 user      (1005) user      (1005)      813 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/ssd_internal_keys.py
+-rw-r--r--   0 user      (1005) user      (1005)     4559 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/ssl_wrap_socket.py
+-rw-r--r--   0 user      (1005) user      (1005)    17320 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/storage_client.py
+-rw-r--r--   0 user      (1005) user      (1005)     8861 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/telemetry.py
+-rw-r--r--   0 user      (1005) user      (1005)    18837 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/telemetry_oob.py
+-rw-r--r--   0 user      (1005) user      (1005)      982 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/test_util.py
+-rw-r--r--   0 user      (1005) user      (1005)     2795 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/time_util.py
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-04-20 20:32:57.263553 snowflake-connector-python-3.0.3/src/snowflake/connector/tool/
+-rw-r--r--   0 user      (1005) user      (1005)       76 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/tool/__init__.py
+-rw-r--r--   0 user      (1005) user      (1005)     1485 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/tool/dump_certs.py
+-rw-r--r--   0 user      (1005) user      (1005)     4575 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/tool/dump_ocsp_response.py
+-rw-r--r--   0 user      (1005) user      (1005)     6601 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/tool/dump_ocsp_response_cache.py
+-rw-r--r--   0 user      (1005) user      (1005)     2119 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/tool/probe_connection.py
+-rw-r--r--   0 user      (1005) user      (1005)     1021 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/url_util.py
+-rw-r--r--   0 user      (1005) user      (1005)    10405 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/util_text.py
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-04-20 20:32:57.267553 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/
+-rw-r--r--   0 user      (1005) user      (1005)       76 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/__init__.py
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-04-20 20:32:57.267553 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/requests/
+-rw-r--r--   0 user      (1005) user      (1005)    10142 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/requests/LICENSE
+-rw-r--r--   0 user      (1005) user      (1005)     4751 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/requests/__init__.py
+-rw-r--r--   0 user      (1005) user      (1005)      440 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/requests/__version__.py
+-rw-r--r--   0 user      (1005) user      (1005)     1397 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/requests/_internal_utils.py
+-rw-r--r--   0 user      (1005) user      (1005)    21313 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/requests/adapters.py
+-rw-r--r--   0 user      (1005) user      (1005)     6377 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/requests/api.py
+-rw-r--r--   0 user      (1005) user      (1005)    10187 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/requests/auth.py
+-rw-r--r--   0 user      (1005) user      (1005)      429 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/requests/certs.py
+-rw-r--r--   0 user      (1005) user      (1005)     1451 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/requests/compat.py
+-rw-r--r--   0 user      (1005) user      (1005)    18560 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/requests/cookies.py
+-rw-r--r--   0 user      (1005) user      (1005)     3813 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/requests/exceptions.py
+-rw-r--r--   0 user      (1005) user      (1005)     3885 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/requests/help.py
+-rw-r--r--   0 user      (1005) user      (1005)      733 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/requests/hooks.py
+-rw-r--r--   0 user      (1005) user      (1005)    35230 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/requests/models.py
+-rw-r--r--   0 user      (1005) user      (1005)    30180 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/requests/sessions.py
+-rw-r--r--   0 user      (1005) user      (1005)     4235 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/requests/status_codes.py
+-rw-r--r--   0 user      (1005) user      (1005)     2912 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/requests/structures.py
+-rw-r--r--   0 user      (1005) user      (1005)    33230 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/requests/utils.py
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-04-20 20:32:57.271553 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/
+-rw-r--r--   0 user      (1005) user      (1005)     1115 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/LICENSE.txt
+-rw-r--r--   0 user      (1005) user      (1005)     2763 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/__init__.py
+-rw-r--r--   0 user      (1005) user      (1005)    10811 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/_collections.py
+-rw-r--r--   0 user      (1005) user      (1005)       64 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/_version.py
+-rw-r--r--   0 user      (1005) user      (1005)    20070 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/connection.py
+-rw-r--r--   0 user      (1005) user      (1005)    39093 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/connectionpool.py
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-04-20 20:32:57.275553 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/contrib/
+-rw-r--r--   0 user      (1005) user      (1005)        0 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/contrib/__init__.py
+-rw-r--r--   0 user      (1005) user      (1005)      957 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/contrib/_appengine_environ.py
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-04-20 20:32:57.275553 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/
+-rw-r--r--   0 user      (1005) user      (1005)        0 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/__init__.py
+-rw-r--r--   0 user      (1005) user      (1005)    17632 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/bindings.py
+-rw-r--r--   0 user      (1005) user      (1005)    13922 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/low_level.py
+-rw-r--r--   0 user      (1005) user      (1005)    11010 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/contrib/appengine.py
+-rw-r--r--   0 user      (1005) user      (1005)     4538 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/contrib/ntlmpool.py
+-rw-r--r--   0 user      (1005) user      (1005)    16385 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0 user      (1005) user      (1005)    34416 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/contrib/securetransport.py
+-rw-r--r--   0 user      (1005) user      (1005)     7097 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/contrib/socks.py
+-rw-r--r--   0 user      (1005) user      (1005)     8217 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/exceptions.py
+-rw-r--r--   0 user      (1005) user      (1005)     8579 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/fields.py
+-rw-r--r--   0 user      (1005) user      (1005)     2440 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/filepost.py
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-04-20 20:32:57.275553 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/packages/
+-rw-r--r--   0 user      (1005) user      (1005)        0 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/packages/__init__.py
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-04-20 20:32:57.275553 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/packages/backports/
+-rw-r--r--   0 user      (1005) user      (1005)        0 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/packages/backports/__init__.py
+-rw-r--r--   0 user      (1005) user      (1005)     1417 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/packages/backports/makefile.py
+-rw-r--r--   0 user      (1005) user      (1005)    34665 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/packages/six.py
+-rw-r--r--   0 user      (1005) user      (1005)    19786 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/poolmanager.py
+-rw-r--r--   0 user      (1005) user      (1005)     5985 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/request.py
+-rw-r--r--   0 user      (1005) user      (1005)    28276 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/response.py
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-04-20 20:32:57.279553 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/util/
+-rw-r--r--   0 user      (1005) user      (1005)     1155 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/util/__init__.py
+-rw-r--r--   0 user      (1005) user      (1005)     4901 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/util/connection.py
+-rw-r--r--   0 user      (1005) user      (1005)     1605 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/util/proxy.py
+-rw-r--r--   0 user      (1005) user      (1005)      498 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/util/queue.py
+-rw-r--r--   0 user      (1005) user      (1005)     4225 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/util/request.py
+-rw-r--r--   0 user      (1005) user      (1005)     3510 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/util/response.py
+-rw-r--r--   0 user      (1005) user      (1005)    22001 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/util/retry.py
+-rw-r--r--   0 user      (1005) user      (1005)    17165 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/util/ssl_.py
+-rw-r--r--   0 user      (1005) user      (1005)     5758 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/util/ssl_match_hostname.py
+-rw-r--r--   0 user      (1005) user      (1005)     6895 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/util/ssltransport.py
+-rw-r--r--   0 user      (1005) user      (1005)    10003 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/util/timeout.py
+-rw-r--r--   0 user      (1005) user      (1005)    14270 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/util/url.py
+-rw-r--r--   0 user      (1005) user      (1005)     5403 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/util/wait.py
+-rw-r--r--   0 user      (1005) user      (1005)      107 2023-04-20 20:25:52.000000 snowflake-connector-python-3.0.3/src/snowflake/connector/version.py
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-04-20 20:32:57.279553 snowflake-connector-python-3.0.3/src/snowflake_connector_python.egg-info/
+-rw-r--r--   0 user      (1005) user      (1005)    48563 2023-04-20 20:32:57.000000 snowflake-connector-python-3.0.3/src/snowflake_connector_python.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1005) user      (1005)     8774 2023-04-20 20:32:57.000000 snowflake-connector-python-3.0.3/src/snowflake_connector_python.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1005) user      (1005)        1 2023-04-20 20:32:57.000000 snowflake-connector-python-3.0.3/src/snowflake_connector_python.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1005) user      (1005)      322 2023-04-20 20:32:57.000000 snowflake-connector-python-3.0.3/src/snowflake_connector_python.egg-info/entry_points.txt
+-rw-r--r--   0 user      (1005) user      (1005)        1 2023-04-20 20:26:37.000000 snowflake-connector-python-3.0.3/src/snowflake_connector_python.egg-info/not-zip-safe
+-rw-r--r--   0 user      (1005) user      (1005)      623 2023-04-20 20:32:57.000000 snowflake-connector-python-3.0.3/src/snowflake_connector_python.egg-info/requires.txt
+-rw-r--r--   0 user      (1005) user      (1005)       10 2023-04-20 20:32:57.000000 snowflake-connector-python-3.0.3/src/snowflake_connector_python.egg-info/top_level.txt
```

### Comparing `snowflake-connector-python-3.0.2/CONTRIBUTING.md` & `snowflake-connector-python-3.0.3/CONTRIBUTING.md`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 ## I'd like to contribute the bug fix or feature myself
 
 We encourage everyone to first open an issue to discuss any feature work or bug fixes with one of the maintainers.
 This should help guide contributors through potential pitfalls.
 
 ### Setup a development environment
 
-What is a development environment? It's a [virtualenv](https://virtualenv.pypa.io) that has all of neccessary
+What is a development environment? It's a [virtualenv](https://virtualenv.pypa.io) that has all of necessary
 dependencies installed with `snowflake-connector-python` installed as an editable package.
 
 Setting up a development environment is super easy with this [one simple tox command](https://tox.wiki/en/latest/example/devenv.html).
 
 ```shell
 tox --devenv venv37 -e py37
 . venv37/bin/activate
```

### Comparing `snowflake-connector-python-3.0.2/DESCRIPTION.md` & `snowflake-connector-python-3.0.3/DESCRIPTION.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,24 @@
 Snowflake Documentation is available at:
 https://docs.snowflake.com/
 
 Source code is also available at: https://github.com/snowflakedb/snowflake-connector-python
 
 # Release Notes
 
+- v3.0.3(April 20, 2023)
+
+  - Fixed a bug that prints error in logs for GET command on GCS.
+  - Added a parameter that allows users to skip file uploads to stage if file exists on stage and contents of the file match.
+  - Fixed a bug that occurred when writing a Pandas DataFrame with non-default index in `snowflake.connector.pandas_tool.write_pandas`.
+  - Fixed a bug that occurred when writing a Pandas DataFrame with column names containing double quotes in `snowflake.connector.pandas_tool.write_pandas`.
+  - Fixed a bug that occurred when writing a Pandas DataFrame with binary data in `snowflake.connector.pandas_tool.write_pandas`.
+  - Improved type hint of `SnowflakeCursor.execute` method.
+  - Improved GET logging to warn when downloading multiple files with the same name.
+
 - v3.0.2(March 23, 2023)
 
   - Fixed a memory leak in the logging module of the Cython extension.
   - Fixed a bug where the `put` command on AWS raised `AttributeError` when uploading file composed of multiple parts.
   - Fixed a bug of incorrect type hints of `SnowflakeCursor.fetch_arrow_all` and `SnowflakeCursor.fetchall`.
   - Fixed a bug where `snowflake.connector.util_text.split_statements` swallows the final line break in the case when there are no space between lines.
   - Improved logging to mask tokens in case of errors.
```

### Comparing `snowflake-connector-python-3.0.2/LICENSE.txt` & `snowflake-connector-python-3.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/MANIFEST.in` & `snowflake-connector-python-3.0.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/PKG-INFO` & `snowflake-connector-python-3.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snowflake-connector-python
-Version: 3.0.2
+Version: 3.0.3
 Summary: Snowflake Connector for Python
 Home-page: https://www.snowflake.com/
 Author: Snowflake, Inc
 Author-email: snowflake-python-libraries-dl@snowflake.com
 License: Apache-2.0
 Project-URL: Documentation, https://docs.snowflake.com/en/user-guide/python-connector.html
 Project-URL: Source, https://github.com/snowflakedb/snowflake-connector-python
@@ -48,14 +48,24 @@
 Snowflake Documentation is available at:
 https://docs.snowflake.com/
 
 Source code is also available at: https://github.com/snowflakedb/snowflake-connector-python
 
 # Release Notes
 
+- v3.0.3(April 20, 2023)
+
+  - Fixed a bug that prints error in logs for GET command on GCS.
+  - Added a parameter that allows users to skip file uploads to stage if file exists on stage and contents of the file match.
+  - Fixed a bug that occurred when writing a Pandas DataFrame with non-default index in `snowflake.connector.pandas_tool.write_pandas`.
+  - Fixed a bug that occurred when writing a Pandas DataFrame with column names containing double quotes in `snowflake.connector.pandas_tool.write_pandas`.
+  - Fixed a bug that occurred when writing a Pandas DataFrame with binary data in `snowflake.connector.pandas_tool.write_pandas`.
+  - Improved type hint of `SnowflakeCursor.execute` method.
+  - Improved GET logging to warn when downloading multiple files with the same name.
+
 - v3.0.2(March 23, 2023)
 
   - Fixed a memory leak in the logging module of the Cython extension.
   - Fixed a bug where the `put` command on AWS raised `AttributeError` when uploading file composed of multiple parts.
   - Fixed a bug of incorrect type hints of `SnowflakeCursor.fetch_arrow_all` and `SnowflakeCursor.fetchall`.
   - Fixed a bug where `snowflake.connector.util_text.split_statements` swallows the final line break in the case when there are no space between lines.
   - Improved logging to mask tokens in case of errors.
```

### Comparing `snowflake-connector-python-3.0.2/README.md` & `snowflake-connector-python-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/pyproject.toml` & `snowflake-connector-python-3.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/setup.cfg` & `snowflake-connector-python-3.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/setup.py` & `snowflake-connector-python-3.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/__init__.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/_sql_util.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/_sql_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/arrow_context.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/arrow_context.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/arrow_iterator.pyx` & `snowflake-connector-python-3.0.3/src/snowflake/connector/arrow_iterator.pyx`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/auth/__init__.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/auth/_auth.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/auth/_auth.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/auth/by_plugin.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/auth/by_plugin.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/auth/default.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/auth/default.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/auth/idtoken.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/auth/idtoken.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/auth/keypair.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/auth/keypair.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/auth/oauth.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/auth/oauth.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/auth/okta.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/auth/okta.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/auth/usrpwdmfa.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/auth/usrpwdmfa.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/auth/webbrowser.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/auth/webbrowser.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/azure_storage_client.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/azure_storage_client.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/bind_upload_agent.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/bind_upload_agent.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/cache.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/cache.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/compat.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/compat.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/connection.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/connection.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/connection_diagnostic.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/connection_diagnostic.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/constants.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/constants.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/converter.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/converter.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/converter_issue23517.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/converter_issue23517.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/converter_snowsql.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/converter_snowsql.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/BinaryConverter.cpp` & `snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/BinaryConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/BinaryConverter.hpp` & `snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/BinaryConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/BooleanConverter.cpp` & `snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/BooleanConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/BooleanConverter.hpp` & `snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/BooleanConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/CArrowChunkIterator.cpp` & `snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/CArrowChunkIterator.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/CArrowChunkIterator.hpp` & `snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/CArrowChunkIterator.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/CArrowIterator.hpp` & `snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/CArrowIterator.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/CArrowTableIterator.cpp` & `snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/CArrowTableIterator.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/CArrowTableIterator.hpp` & `snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/CArrowTableIterator.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/DateConverter.cpp` & `snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/DateConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/DateConverter.hpp` & `snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/DateConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/DecimalConverter.cpp` & `snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/DecimalConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/DecimalConverter.hpp` & `snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/DecimalConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/FloatConverter.cpp` & `snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/FloatConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/FloatConverter.hpp` & `snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/FloatConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/IntConverter.hpp` & `snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/IntConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/Python/Common.hpp` & `snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/Python/Common.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/Python/Helpers.cpp` & `snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/Python/Helpers.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/Python/Helpers.hpp` & `snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/Python/Helpers.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/SnowflakeType.cpp` & `snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/SnowflakeType.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/SnowflakeType.hpp` & `snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/SnowflakeType.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/StringConverter.cpp` & `snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/StringConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/StringConverter.hpp` & `snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/StringConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/TimeConverter.hpp` & `snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/TimeConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/TimeStampConverter.cpp` & `snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/TimeStampConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/TimeStampConverter.hpp` & `snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/TimeStampConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/Util/time.cpp` & `snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/Util/time.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/ArrowIterator/Util/time.hpp` & `snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/ArrowIterator/Util/time.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/Logging/logging.cpp` & `snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/Logging/logging.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/cpp/Logging/logging.hpp` & `snowflake-connector-python-3.0.3/src/snowflake/connector/cpp/Logging/logging.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/cursor.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/cursor.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     NamedTuple,
     NoReturn,
     Sequence,
     TypeVar,
     overload,
 )
 
-from typing_extensions import Self
+from typing_extensions import Literal, Self
 
 from snowflake.connector.result_batch import create_batches_from_response
 from snowflake.connector.result_set import ResultSet
 
 from . import compat
 from ._sql_util import get_file_transfer_type
 from .bind_upload_agent import BindUploadAgent, BindUploadError
@@ -59,15 +59,14 @@
     DatabaseError,
     Error,
     IntegrityError,
     InterfaceError,
     NotSupportedError,
     ProgrammingError,
 )
-from .file_transfer_agent import SnowflakeFileTransferAgent
 from .options import installed_pandas
 from .sqlstate import SQLSTATE_FEATURE_NOT_SUPPORTED
 from .telemetry import TelemetryData, TelemetryField
 from .time_util import get_time_millis
 
 if TYPE_CHECKING:  # pragma: no cover
     from pandas import DataFrame
@@ -603,14 +602,74 @@
             and len(processed_params) > 0
         ):
             query = command % processed_params
         else:
             query = command
         return query
 
+    @overload
+    def execute(
+        self,
+        command: str,
+        params: Sequence[Any] | dict[Any, Any] | None = None,
+        _bind_stage: str | None = None,
+        timeout: int | None = None,
+        _exec_async: bool = False,
+        _no_retry: bool = False,
+        _do_reset: bool = True,
+        _put_callback: SnowflakeProgressPercentage = None,
+        _put_azure_callback: SnowflakeProgressPercentage = None,
+        _put_callback_output_stream: IO[str] = sys.stdout,
+        _get_callback: SnowflakeProgressPercentage = None,
+        _get_azure_callback: SnowflakeProgressPercentage = None,
+        _get_callback_output_stream: IO[str] = sys.stdout,
+        _show_progress_bar: bool = True,
+        _statement_params: dict[str, str] | None = None,
+        _is_internal: bool = False,
+        _describe_only: bool = False,
+        _no_results: Literal[False] = False,
+        _is_put_get: bool | None = None,
+        _raise_put_get_error: bool = True,
+        _force_put_overwrite: bool = False,
+        _skip_upload_on_content_match: bool = False,
+        file_stream: IO[bytes] | None = None,
+        num_statements: int | None = None,
+    ) -> Self | None:
+        ...
+
+    @overload
+    def execute(
+        self,
+        command: str,
+        params: Sequence[Any] | dict[Any, Any] | None = None,
+        _bind_stage: str | None = None,
+        timeout: int | None = None,
+        _exec_async: bool = False,
+        _no_retry: bool = False,
+        _do_reset: bool = True,
+        _put_callback: SnowflakeProgressPercentage = None,
+        _put_azure_callback: SnowflakeProgressPercentage = None,
+        _put_callback_output_stream: IO[str] = sys.stdout,
+        _get_callback: SnowflakeProgressPercentage = None,
+        _get_azure_callback: SnowflakeProgressPercentage = None,
+        _get_callback_output_stream: IO[str] = sys.stdout,
+        _show_progress_bar: bool = True,
+        _statement_params: dict[str, str] | None = None,
+        _is_internal: bool = False,
+        _describe_only: bool = False,
+        _no_results: Literal[True] = True,
+        _is_put_get: bool | None = None,
+        _raise_put_get_error: bool = True,
+        _force_put_overwrite: bool = False,
+        _skip_upload_on_content_match: bool = False,
+        file_stream: IO[bytes] | None = None,
+        num_statements: int | None = None,
+    ) -> dict[str, Any] | None:
+        ...
+
     def execute(
         self,
         command: str,
         params: Sequence[Any] | dict[Any, Any] | None = None,
         _bind_stage: str | None = None,
         timeout: int | None = None,
         _exec_async: bool = False,
@@ -626,14 +685,15 @@
         _statement_params: dict[str, str] | None = None,
         _is_internal: bool = False,
         _describe_only: bool = False,
         _no_results: bool = False,
         _is_put_get: bool | None = None,
         _raise_put_get_error: bool = True,
         _force_put_overwrite: bool = False,
+        _skip_upload_on_content_match: bool = False,
         file_stream: IO[bytes] | None = None,
         num_statements: int | None = None,
     ) -> Self | dict[str, Any] | None:
         """Executes a command/query.
 
         Args:
             command: The SQL command to be executed.
@@ -656,14 +716,16 @@
             _no_results: This flag tells the back-end to not return the result, just fire the query and return the
                 response returned by Snowflake's server.
             _use_ijson: This flag doesn't do anything as ijson support has ended.
             _is_put_get: Force decision of this SQL query being a PUT, or GET command. This is detected otherwise.
             _raise_put_get_error: Whether to raise PUT and GET errors.
             _force_put_overwrite: If the SQL query is a PUT, then this flag can force overwriting of an already
                 existing file on stage.
+            _skip_upload_on_content_match: If the SQL query is a PUT with overwrite enabled, then this flag will skip upload
+                if the file contents match to ease concurrent uploads.
             file_stream: File-like object to be uploaded with PUT
             num_statements: Query level parameter submitted in _statement_params constraining exact number of
             statements being submitted (or 0 if submitting an uncounted number) when using a multi-statement query.
 
         Returns:
             The cursor itself, or None if some error happened, or the response returned
             by Snowflake if the _no_results flag is on.
@@ -779,14 +841,16 @@
 
             self._is_file_transfer = "command" in data and data["command"] in (
                 "UPLOAD",
                 "DOWNLOAD",
             )
             logger.debug("PUT OR GET: %s", self.is_file_transfer)
             if self.is_file_transfer:
+                from .file_transfer_agent import SnowflakeFileTransferAgent
+
                 # Decide whether to use the old, or new code path
                 sf_file_transfer_agent = SnowflakeFileTransferAgent(
                     self,
                     query,
                     ret,
                     put_callback=_put_callback,
                     put_azure_callback=_put_azure_callback,
@@ -794,14 +858,15 @@
                     get_callback=_get_callback,
                     get_azure_callback=_get_azure_callback,
                     get_callback_output_stream=_get_callback_output_stream,
                     show_progress_bar=_show_progress_bar,
                     raise_put_get_error=_raise_put_get_error,
                     force_put_overwrite=_force_put_overwrite
                     or data.get("overwrite", False),
+                    skip_upload_on_content_match=_skip_upload_on_content_match,
                     source_from_stream=file_stream,
                     multipart_threshold=data.get("threshold"),
                     use_s3_regional_url=self._connection.enable_stage_s3_privatelink_for_us_east_1,
                 )
                 sf_file_transfer_agent.execute()
                 data = sf_file_transfer_agent.result()
                 self._total_rowcount = len(data["rowset"]) if "rowset" in data else -1
```

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/dbapi.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/dbapi.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/description.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/description.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/encryption_util.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/encryption_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/errorcode.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/errorcode.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/errors.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/errors.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/file_compression_type.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/file_compression_type.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/file_transfer_agent.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/file_transfer_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,14 +131,15 @@
     src_compression_type: CompressionType | None = None
     dst_compression_type: CompressionType = None
     require_compress: bool = False
     dst_file_name: str | None = None
     dst_file_size: int = -1
     intermediate_stream: IO[bytes] | None = None
     src_stream: IO[bytes] | None = None
+    skip_upload_on_content_match: bool = False
     # Specific to Downloads only
     local_location: str | None = None
 
 
 def _update_progress(
     file_name: str,
     start_time: float,
@@ -317,14 +318,15 @@
         put_callback_output_stream: IO[str] = sys.stdout,
         get_callback: type[SnowflakeProgressPercentage] | None = None,
         get_azure_callback: type[SnowflakeProgressPercentage] | None = None,
         get_callback_output_stream: IO[str] = sys.stdout,
         show_progress_bar: bool = True,
         raise_put_get_error: bool = True,
         force_put_overwrite: bool = True,
+        skip_upload_on_content_match: bool = False,
         multipart_threshold: int | None = None,
         source_from_stream: IO[bytes] | None = None,
         use_s3_regional_url: bool = False,
     ) -> None:
         self._cursor = cursor
         self._command = command
         self._ret = ret
@@ -341,14 +343,15 @@
         # when we have not checked whether we should use accelerate, this boolean is None
         # _use_accelerate_endpoint in SnowflakeFileTransferAgent could be passed to each SnowflakeS3RestClient
         # so we could avoid check accelerate configuration for each S3 client created for each file meta.
         self._use_accelerate_endpoint: bool | None = None
         self._raise_put_get_error = raise_put_get_error
         self._show_progress_bar = show_progress_bar
         self._force_put_overwrite = force_put_overwrite
+        self._skip_upload_on_content_match = skip_upload_on_content_match
         self._source_from_stream = source_from_stream
         # The list of self-sufficient file metas that are sent to
         # remote storage clients to get operated on.
         self._file_metadata: list[SnowflakeFileMeta] = []
         self._results: list[SnowflakeFileMeta] = []
         self._multipart_threshold = multipart_threshold or 67108864  # Historical value
         self._use_s3_regional_url = use_s3_regional_url
@@ -372,14 +375,15 @@
 
         if self._stage_location_type == LOCAL_FS:
             if not os.path.isdir(self._stage_info["location"]):
                 os.makedirs(self._stage_info["location"])
 
         for m in self._file_metadata:
             m.overwrite = self._overwrite
+            m.skip_upload_on_content_match = self._skip_upload_on_content_match
             m.sfagent = self
             if self._stage_location_type != LOCAL_FS:
                 m.put_callback = self._put_callback
                 m.put_azure_callback = self._put_azure_callback
                 m.put_callback_output_stream = self._put_callback_output_stream
                 m.get_callback = self._get_callback
                 m.get_azure_callback = self._get_azure_callback
@@ -1009,42 +1013,55 @@
                             stage_location_type=self._stage_location_type,
                             encryption_material=self._encryption_material[0]
                             if len(self._encryption_material) > 0
                             else None,
                         )
                     )
         elif self._command_type == CMD_TYPE_DOWNLOAD:
+            basename_counts = dict()
             for idx, file_name in enumerate(self._src_files):
                 if not file_name:
                     continue
                 first_path_sep = file_name.find("/")
                 dst_file_name = (
                     file_name[first_path_sep + 1 :]
                     if first_path_sep >= 0
                     else file_name
                 )
                 url = None
                 if self._presigned_urls and idx < len(self._presigned_urls):
                     url = self._presigned_urls[idx]
+
+                basename = os.path.basename(file_name)
+                basename_counts[basename] = basename_counts.get(basename, 0) + 1
+
                 self._file_metadata.append(
                     SnowflakeFileMeta(
-                        name=os.path.basename(file_name),
+                        name=basename,
                         src_file_name=file_name,
                         dst_file_name=dst_file_name,
                         stage_location_type=self._stage_location_type,
                         local_location=self._local_location,
                         presigned_url=url,
                         encryption_material=self._src_file_to_encryption_material[
                             file_name
                         ]
                         if file_name in self._src_file_to_encryption_material
                         else None,
                     )
                 )
 
+            # TODO: remove this warning once we support directory structure for GET
+            duplicate_basenames = [k for k, v in basename_counts.items() if v > 1]
+            if duplicate_basenames:
+                logger.warning(
+                    f"Downloading multiple files with the same name could cause failures. "
+                    f"File names with multiple entries: {duplicate_basenames}"
+                )
+
     def _process_file_compression_type(self) -> None:
         user_specified_source_compression = None
         if self._source_compression == "auto_detect":
             auto_detect = True
         elif self._source_compression == "none":
             auto_detect = False
         else:
```

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/file_util.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/file_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/gcs_storage_client.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/gcs_storage_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,15 +213,15 @@
         meta.gcs_file_header_encryption_metadata = encryption_metadata
 
     def finish_download(self) -> None:
         super().finish_download()
         # Sadly, we can only determine the src file size after we've
         # downloaded it, unlike the other cloud providers where the
         # metadata can be read beforehand.
-        self.meta.src_file_size = os.path.getsize(self.intermediate_dst_path)
+        self.meta.src_file_size = os.path.getsize(self.full_dst_file_name)
 
     def _update_presigned_url(self) -> None:
         """Updates the file metas with presigned urls if any.
 
         Currently only the file metas generated for PUT/GET on a GCP account need the presigned urls.
         """
         logger.debug("Updating presigned url")
```

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/gzip_decoder.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/gzip_decoder.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/local_storage_client.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/local_storage_client.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/network.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/network.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/ocsp_asn1crypto.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/ocsp_asn1crypto.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/ocsp_snowflake.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/ocsp_snowflake.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/options.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/options.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,14 +79,15 @@
     """
     try:
         pandas = importlib.import_module("pandas")
         # since we enable relative imports without dots this import gives us an issues when ran from test directory
         from pandas import DataFrame  # NOQA
 
         pyarrow = importlib.import_module("pyarrow")
+
         # Check whether we have the currently supported pyarrow installed
         installed_packages = {
             package.metadata["Name"]: package for package in distributions()
         }
         if {"pyarrow", "snowflake-connector-python"} <= installed_packages.keys():
             dependencies = installed_packages[
                 "snowflake-connector-python"
```

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/pandas_tools.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/pandas_tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,21 +28,23 @@
         sqlalchemy = None
 
 T = TypeVar("T", bound=collections.abc.Sequence)
 
 logger = getLogger(__name__)
 
 
-def chunk_helper(lst: T, n: int) -> Iterator[tuple[int, T]]:
+def chunk_helper(
+    lst: pandas.DataFrame, n: int
+) -> Iterator[tuple[int, pandas.DataFrame]]:
     """Helper generator to chunk a sequence efficiently with current index like if enumerate was called on sequence."""
     if len(lst) == 0:
         yield 0, lst
         return
     for i in range(0, len(lst), n):
-        yield int(i / n), lst[i : i + n]
+        yield int(i / n), lst.iloc[i : i + n]
 
 
 def build_location_helper(
     database: str | None, schema: str | None, name: str, quote_identifiers: bool
 ) -> str:
     """Helper to format table/stage/file format's location."""
     if quote_identifiers:
@@ -166,14 +168,27 @@
         raise ValueError(
             "Unsupported table type. Expected table types: temp/temporary, transient"
         )
 
     if chunk_size is None:
         chunk_size = len(df)
 
+    if not (
+        isinstance(df.index, pandas.RangeIndex)
+        and 1 == df.index.step
+        and 0 == df.index.start
+    ):
+        warnings.warn(
+            f"Pandas Dataframe has non-standard index of type {str(type(df.index))} which will not be written."
+            f" Consider changing the index to pd.RangeIndex(start=0,...,step=1) or "
+            f"call reset_index() to keep index as column(s)",
+            UserWarning,
+            stacklevel=2,
+        )
+
     cursor = conn.cursor()
     stage_location = build_location_helper(
         database=database,
         schema=schema,
         name=random_string(),
         quote_identifiers=quote_identifiers,
     )
@@ -200,20 +215,21 @@
             # Remove chunk file
             os.remove(chunk_path)
 
     # in Snowflake, all parquet data is stored in a single column, $1, so we must select columns explicitly
     # see (https://docs.snowflake.com/en/user-guide/script-data-load-transform-parquet.html)
     if quote_identifiers:
         quote = '"'
-        columns = '"' + '","'.join(list(df.columns)) + '"'
-        parquet_columns = "$1:" + ",$1:".join(f'"{c}"' for c in df.columns)
+        # if the column name contains a double quote, we need to escape it by replacing with two double quotes
+        # https://docs.snowflake.com/en/sql-reference/identifiers-syntax#double-quoted-identifiers
+        snowflake_column_names = [str(c).replace('"', '""') for c in df.columns]
     else:
         quote = ""
-        columns = ",".join(list(df.columns))
-        parquet_columns = "$1:" + ",$1:".join(df.columns)
+        snowflake_column_names = list(df.columns)
+    columns = quote + f"{quote},{quote}".join(snowflake_column_names) + quote
 
     def drop_object(name: str, object_type: str) -> None:
         drop_sql = f"DROP {object_type.upper()} IF EXISTS {name} /* Python:snowflake.connector.pandas_tools.write_pandas() */"
         logger.debug(f"dropping {object_type} with '{drop_sql}'")
         cursor.execute(drop_sql, _is_internal=True)
 
     if auto_create_table or overwrite:
@@ -236,15 +252,18 @@
         column_type_mapping = dict(
             cursor.execute(infer_schema_sql, _is_internal=True).fetchall()
         )
         # Infer schema can return the columns out of order depending on the chunking we do when uploading
         # so we have to iterate through the dataframe columns to make sure we create the table with its
         # columns in order
         create_table_columns = ", ".join(
-            [f"{quote}{c}{quote} {column_type_mapping[c]}" for c in df.columns]
+            [
+                f"{quote}{snowflake_col}{quote} {column_type_mapping[col]}"
+                for snowflake_col, col in zip(snowflake_column_names, df.columns)
+            ]
         )
 
         target_table_location = build_location_helper(
             database,
             schema,
             random_string() if overwrite else table_name,
             quote_identifiers,
@@ -253,28 +272,36 @@
         create_table_sql = (
             f"CREATE {table_type.upper()} TABLE IF NOT EXISTS {target_table_location} "
             f"({create_table_columns})"
             f" /* Python:snowflake.connector.pandas_tools.write_pandas() */ "
         )
         logger.debug(f"auto creating table with '{create_table_sql}'")
         cursor.execute(create_table_sql, _is_internal=True)
+        # need explicit casting when the underlying table schema is inferred
+        parquet_columns = "$1:" + ",$1:".join(
+            f"{quote}{snowflake_col}{quote}::{column_type_mapping[col]}"
+            for snowflake_col, col in zip(snowflake_column_names, df.columns)
+        )
     else:
         target_table_location = build_location_helper(
             database=database,
             schema=schema,
             name=table_name,
             quote_identifiers=quote_identifiers,
         )
+        parquet_columns = "$1:" + ",$1:".join(
+            f"{quote}{snowflake_col}{quote}" for snowflake_col in snowflake_column_names
+        )
 
     try:
         copy_into_sql = (
             f"COPY INTO {target_table_location} /* Python:snowflake.connector.pandas_tools.write_pandas() */ "
             f"({columns}) "
             f"FROM (SELECT {parquet_columns} FROM @{stage_location}) "
-            f"FILE_FORMAT=(TYPE=PARQUET COMPRESSION={compression_map[compression]}) "
+            f"FILE_FORMAT=(TYPE=PARQUET COMPRESSION={compression_map[compression]}{' BINARY_AS_TEXT=FALSE' if auto_create_table or overwrite else ''}) "
             f"PURGE=TRUE ON_ERROR={on_error}"
         )
         logger.debug(f"copying into with '{copy_into_sql}'")
         copy_results = cursor.execute(copy_into_sql, _is_internal=True).fetchall()
 
         if overwrite:
             original_table_location = build_location_helper(
```

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/proxy.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/proxy.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/result_batch.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/result_batch.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/result_set.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/result_set.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/s3_storage_client.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/s3_storage_client.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/secret_detector.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/secret_detector.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/sfbinaryformat.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/sfbinaryformat.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/sfdatetime.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/sfdatetime.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/snow_logging.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/snow_logging.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/ssd_internal_keys.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/ssd_internal_keys.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/ssl_wrap_socket.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/ssl_wrap_socket.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/storage_client.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/storage_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,31 +181,43 @@
             Updates meta.result_status.
         """
         pass
 
     def preprocess(self) -> None:
         meta = self.meta
         logger.debug(f"Preprocessing {meta.src_file_name}")
+
+        file_header = self.get_file_header(
+            meta.dst_file_name
+        )  # check if file exists on remote
         if not meta.overwrite:
             self.get_digest()  # self.get_file_header needs digest for multiparts upload when aws is used.
-            self.get_file_header(meta.dst_file_name)  # Check if file exists on remote
             if meta.result_status == ResultStatus.UPLOADED:
                 # Skipped
                 logger.debug(
                     f'file already exists location="{self.stage_info["location"]}", '
                     f'file_name="{meta.dst_file_name}"'
                 )
                 meta.dst_file_size = 0
                 meta.result_status = ResultStatus.SKIPPED
                 self.preprocessed = True
                 return
         # Uploading
         if meta.require_compress:
             self.compress()
         self.get_digest()
+
+        if (
+            meta.skip_upload_on_content_match
+            and file_header
+            and meta.sha256_digest == file_header.digest
+        ):
+            logger.debug(f"same file contents for {meta.name}, skipping upload")
+            meta.result_status = ResultStatus.SKIPPED
+
         self.preprocessed = True
 
     def prepare_upload(self) -> None:
         meta = self.meta
 
         if not self.preprocessed:
             self.preprocess()
```

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/telemetry.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/telemetry.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/telemetry_oob.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/telemetry_oob.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/test_util.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/test_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/time_util.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/time_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/tool/dump_certs.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/tool/dump_certs.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/tool/dump_ocsp_response.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/tool/dump_ocsp_response.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/tool/dump_ocsp_response_cache.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/tool/dump_ocsp_response_cache.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/tool/probe_connection.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/tool/probe_connection.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/url_util.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/url_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/util_text.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/util_text.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/requests/LICENSE` & `snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/requests/LICENSE`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/requests/__init__.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/requests/_internal_utils.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/requests/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/requests/adapters.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/requests/api.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/requests/api.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/requests/auth.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/requests/auth.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/requests/compat.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/requests/compat.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/requests/cookies.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/requests/exceptions.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/requests/help.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/requests/help.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/requests/hooks.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/requests/models.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/requests/models.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/requests/sessions.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/requests/status_codes.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/requests/structures.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/requests/structures.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/requests/utils.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/requests/utils.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/LICENSE.txt` & `snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/__init__.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/_collections.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/connection.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/connectionpool.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/contrib/_appengine_environ.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/contrib/_appengine_environ.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/bindings.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/low_level.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/contrib/appengine.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/contrib/appengine.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/contrib/ntlmpool.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/contrib/ntlmpool.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/contrib/pyopenssl.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/contrib/securetransport.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/contrib/securetransport.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/contrib/socks.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/exceptions.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/fields.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/filepost.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/packages/backports/makefile.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/packages/backports/makefile.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/packages/six.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/packages/six.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/poolmanager.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/request.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/request.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/response.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/util/__init__.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/util/connection.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/util/proxy.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/util/request.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/util/response.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/util/retry.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/util/ssl_.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/util/ssl_match_hostname.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/util/ssltransport.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/util/timeout.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/util/url.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake/connector/vendored/urllib3/util/wait.py` & `snowflake-connector-python-3.0.3/src/snowflake/connector/vendored/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake_connector_python.egg-info/PKG-INFO` & `snowflake-connector-python-3.0.3/src/snowflake_connector_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snowflake-connector-python
-Version: 3.0.2
+Version: 3.0.3
 Summary: Snowflake Connector for Python
 Home-page: https://www.snowflake.com/
 Author: Snowflake, Inc
 Author-email: snowflake-python-libraries-dl@snowflake.com
 License: Apache-2.0
 Project-URL: Documentation, https://docs.snowflake.com/en/user-guide/python-connector.html
 Project-URL: Source, https://github.com/snowflakedb/snowflake-connector-python
@@ -48,14 +48,24 @@
 Snowflake Documentation is available at:
 https://docs.snowflake.com/
 
 Source code is also available at: https://github.com/snowflakedb/snowflake-connector-python
 
 # Release Notes
 
+- v3.0.3(April 20, 2023)
+
+  - Fixed a bug that prints error in logs for GET command on GCS.
+  - Added a parameter that allows users to skip file uploads to stage if file exists on stage and contents of the file match.
+  - Fixed a bug that occurred when writing a Pandas DataFrame with non-default index in `snowflake.connector.pandas_tool.write_pandas`.
+  - Fixed a bug that occurred when writing a Pandas DataFrame with column names containing double quotes in `snowflake.connector.pandas_tool.write_pandas`.
+  - Fixed a bug that occurred when writing a Pandas DataFrame with binary data in `snowflake.connector.pandas_tool.write_pandas`.
+  - Improved type hint of `SnowflakeCursor.execute` method.
+  - Improved GET logging to warn when downloading multiple files with the same name.
+
 - v3.0.2(March 23, 2023)
 
   - Fixed a memory leak in the logging module of the Cython extension.
   - Fixed a bug where the `put` command on AWS raised `AttributeError` when uploading file composed of multiple parts.
   - Fixed a bug of incorrect type hints of `SnowflakeCursor.fetch_arrow_all` and `SnowflakeCursor.fetchall`.
   - Fixed a bug where `snowflake.connector.util_text.split_statements` swallows the final line break in the case when there are no space between lines.
   - Improved logging to mask tokens in case of errors.
```

### Comparing `snowflake-connector-python-3.0.2/src/snowflake_connector_python.egg-info/SOURCES.txt` & `snowflake-connector-python-3.0.3/src/snowflake_connector_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.0.2/src/snowflake_connector_python.egg-info/requires.txt` & `snowflake-connector-python-3.0.3/src/snowflake_connector_python.egg-info/requires.txt`

 * *Files identical despite different names*

