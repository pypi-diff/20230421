# Comparing `tmp/openapiart-0.2.8.tar.gz` & `tmp/openapiart-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openapiart-0.2.8.tar", last modified: Tue Feb 14 21:24:01 2023, max compression
+gzip compressed data, was "openapiart-0.2.9.tar", last modified: Thu Feb 16 21:19:27 2023, max compression
```

## Comparing `openapiart-0.2.8.tar` & `openapiart-0.2.9.tar`

### file list

```diff
@@ -1,96 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 21:24:01.292466 openapiart-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-02-14 21:23:20.000000 openapiart-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-02-14 21:23:20.000000 openapiart-0.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-02-14 21:24:01.292466 openapiart-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-02-14 21:23:20.000000 openapiart-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 21:24:01.284465 openapiart-0.2.8/openapiart/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39451 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/bundler.py
--rw-r--r--   0 runner    (1001) docker     (123)    10719 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/common.go
--rw-r--r--   0 runner    (1001) docker     (123)    35983 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    69619 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 21:24:01.288465 openapiart-0.2.8/openapiart/goserver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/goserver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 21:24:01.288465 openapiart-0.2.8/openapiart/goserver/api/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/goserver/api/api.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/goserver/api/common.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/goserver/api/service_a.api.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/goserver/api/service_a.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/goserver/api/service_b.api.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/goserver/api/service_b.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6228 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/goserver/generator_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    12535 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/goserver/go_controller_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/goserver/go_interface_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/goserver/goserver.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/goserver/http_setup.go
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/goserver/response.go
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/goserver/string_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/goserver/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/gotidy.py
--rw-r--r--   0 runner    (1001) docker     (123)    12748 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/openapiart.py
--rw-r--r--   0 runner    (1001) docker     (123)   111696 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/openapiartgo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/openapiartplugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    17145 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/openapiartprotobuf.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/openapiartpython.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/requirements.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 21:24:01.292466 openapiart-0.2.8/openapiart/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 21:24:01.292466 openapiart-0.2.8/openapiart/tests/api/
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/tests/api/api.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/tests/api/info.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 21:24:01.292466 openapiart-0.2.8/openapiart/tests/common/
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/tests/common/common.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 21:24:01.292466 openapiart-0.2.8/openapiart/tests/config/
--rw-r--r--   0 runner    (1001) docker     (123)    13618 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/tests/config/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/tests/config/negative_nested_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 21:24:01.292466 openapiart-0.2.8/openapiart/tests/field_uid/
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/tests/field_uid/fielduid.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/tests/field_uid/property_name_camel_case.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/tests/field_uid/property_name_pascal_case.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/tests/field_uid/property_name_upper_case.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/tests/field_uid/xenum.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/tests/field_uid/xinclude.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/tests/grpcserver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 21:24:01.292466 openapiart-0.2.8/openapiart/tests/multilevel/
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/tests/multilevel/multi.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 21:24:01.292466 openapiart-0.2.8/openapiart/tests/pattern/
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/tests/pattern/pattern.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/tests/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/tests/test_add.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/tests/test_auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/tests/test_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/tests/test_bundler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/tests/test_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/tests/test_fielduid.py
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/tests/test_formats.py
--rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/tests/test_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/tests/test_grpc_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/tests/test_int64.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/tests/test_license.py
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/tests/test_perf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/tests/test_protobuf.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/tests/test_py_go_diff.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/tests/test_remove.py
--rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/tests/test_unique.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/tests/test_validate_property_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/tests/test_validate_xenum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/tests/test_validate_xinclude.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/tests/test_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/tests/test_warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 21:24:01.292466 openapiart-0.2.8/openapiart/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/tests/utils/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 21:24:01.292466 openapiart-0.2.8/openapiart/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-02-14 21:23:20.000000 openapiart-0.2.8/openapiart/utils/autofielduid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 21:24:01.284465 openapiart-0.2.8/openapiart.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-02-14 21:24:01.000000 openapiart-0.2.8/openapiart.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-02-14 21:24:01.000000 openapiart-0.2.8/openapiart.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-14 21:24:01.000000 openapiart-0.2.8/openapiart.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-02-14 21:24:01.000000 openapiart-0.2.8/openapiart.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-14 21:24:01.000000 openapiart-0.2.8/openapiart.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-14 21:23:20.000000 openapiart-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-14 21:24:01.292466 openapiart-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-02-14 21:23:20.000000 openapiart-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 21:19:27.748009 openapiart-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-02-16 21:18:59.000000 openapiart-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-02-16 21:18:59.000000 openapiart-0.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-02-16 21:19:27.748009 openapiart-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-02-16 21:18:59.000000 openapiart-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 21:19:27.728009 openapiart-0.2.9/openapiart/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43622 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/bundler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11623 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/common.go
+-rw-r--r--   0 runner    (1001) docker     (123)    36032 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/common_test.go
+-rw-r--r--   0 runner    (1001) docker     (123)    74276 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 21:19:27.732009 openapiart-0.2.9/openapiart/goserver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/goserver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 21:19:27.732009 openapiart-0.2.9/openapiart/goserver/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/goserver/api/api.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/goserver/api/common.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/goserver/api/service_a.api.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/goserver/api/service_a.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/goserver/api/service_b.api.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/goserver/api/service_b.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6228 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/goserver/generator_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12535 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/goserver/go_controller_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/goserver/go_interface_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/goserver/goserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/goserver/http_setup.go
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/goserver/response.go
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/goserver/string_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/goserver/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/gotidy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13444 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/openapiart.py
+-rw-r--r--   0 runner    (1001) docker     (123)   117112 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/openapiartgo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/openapiartplugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17145 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/openapiartprotobuf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/openapiartpython.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 21:19:27.744009 openapiart-0.2.9/openapiart/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 21:19:27.744009 openapiart-0.2.9/openapiart/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/tests/api/api.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/tests/api/info.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 21:19:27.744009 openapiart-0.2.9/openapiart/tests/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/tests/common/common.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 21:19:27.744009 openapiart-0.2.9/openapiart/tests/config/
+-rw-r--r--   0 runner    (1001) docker     (123)    13618 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/tests/config/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/tests/config/negative_nested_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 21:19:27.748009 openapiart-0.2.9/openapiart/tests/field_uid/
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/tests/field_uid/fielduid.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/tests/field_uid/property_name_camel_case.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/tests/field_uid/property_name_pascal_case.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/tests/field_uid/property_name_upper_case.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/tests/field_uid/xenum.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/tests/field_uid/xinclude.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/tests/grpcserver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 21:19:27.748009 openapiart-0.2.9/openapiart/tests/multilevel/
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/tests/multilevel/multi.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 21:19:27.748009 openapiart-0.2.9/openapiart/tests/pattern/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/tests/pattern/pattern.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/tests/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/tests/test_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/tests/test_auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/tests/test_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/tests/test_bundler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/tests/test_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/tests/test_fielduid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/tests/test_formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/tests/test_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/tests/test_grpc_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/tests/test_http_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/tests/test_int64.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/tests/test_license.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/tests/test_perf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/tests/test_protobuf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/tests/test_py_go_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/tests/test_remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/tests/test_unique.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/tests/test_validate_property_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/tests/test_validate_xenum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/tests/test_validate_xinclude.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/tests/test_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/tests/test_warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 21:19:27.748009 openapiart-0.2.9/openapiart/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/tests/utils/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 21:19:27.748009 openapiart-0.2.9/openapiart/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-02-16 21:18:59.000000 openapiart-0.2.9/openapiart/utils/autofielduid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 21:19:27.728009 openapiart-0.2.9/openapiart.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-02-16 21:19:27.000000 openapiart-0.2.9/openapiart.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-02-16 21:19:27.000000 openapiart-0.2.9/openapiart.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-16 21:19:27.000000 openapiart-0.2.9/openapiart.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-02-16 21:19:27.000000 openapiart-0.2.9/openapiart.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-16 21:19:27.000000 openapiart-0.2.9/openapiart.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-16 21:18:59.000000 openapiart-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-16 21:19:27.748009 openapiart-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-02-16 21:18:59.000000 openapiart-0.2.9/setup.py
```

### Comparing `openapiart-0.2.8/LICENSE` & `openapiart-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `openapiart-0.2.8/PKG-INFO` & `openapiart-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openapiart
-Version: 0.2.8
+Version: 0.2.9
 Summary: The OpenAPI Artifact Generator Python Package
 Home-page: https://github.com/open-traffic-generator/openapiart
 Author: https://github.com/open-traffic-generator/openapiart
 Author-email: andy.balogh@keysight.com
 License: MIT
 Keywords: testing openapi artifact generator
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `openapiart-0.2.8/README.md` & `openapiart-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `openapiart-0.2.8/openapiart/bundler.py` & `openapiart-0.2.9/openapiart/bundler.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,18 +47,19 @@
 
     @staticmethod
     def literal_representer(dumper, data):
         return dumper.represent_scalar(
             "tag:yaml.org,2002:str", data, style="|"
         )
 
-    def __init__(self, api_files, output_dir="./"):
+    def __init__(self, api_files, output_dir="./", generate_version_api=False):
         self._parsers = {}
         self._api_files = api_files
         self._output_dir = os.path.abspath(output_dir)
+        self._generate_version_api = generate_version_api
         if os.path.exists(self._output_dir) is False:
             os.makedirs(self._output_dir)
         self.__python = os.path.normpath(sys.executable)
         self._content = {}
         self._includes = {}
         self._include_objects = {}
         self._resolved = []
@@ -86,57 +87,63 @@
         self._include_objects = {}
         self._resolved = []
         for api_filename in self._api_files:
             api_filename = os.path.normpath(os.path.abspath(api_filename))
             self._base_dir = os.path.dirname(api_filename)
             self._api_filename = os.path.basename(api_filename)
             self._read_file(self._base_dir, self._api_filename)
+
         self._resolve_x_include()
         self._resolve_x_pattern("x-field-pattern")
         self._resolve_x_constraint()
         self._resolve_x_status()
         self._remove_x_include()
         # TODO: restore behavior
         # self._resolve_x_unique()
         self._resolve_license()
-        self._resolve_x_enmu(self._content)
+        self._resolve_x_enum(self._content)
+        self._generate_version_api_spec(self._content)
         self._validate_field_uid()
         self._validate_response_uid()
         self._validate_errors()
         self._validate_required_responses()
         self._resolve_strings(self._content)
         self._resolve_keys(self._content)
+        self._api_version = self._content["info"]["version"]
         with open(self._output_filename, "w") as fp:
             yaml.dump(
                 self._content,
                 fp,
                 indent=2,
                 allow_unicode=True,
                 line_break="\n",
                 sort_keys=False,
             )
         with open(self._json_filename, "w") as fp:
             fp.write(json.dumps(self._content, indent=4))
         self._validate_file()
 
+    def get_api_version(self):
+        return self._api_version
+
     def _validate_errors(self):
         if len(self._errors) > 0:
             raise TypeError("\n".join(self._errors))
 
     def _inject_enum(self, property_name, property_object, schema_name):
         # if "enum" in property_object.keys():
         #     self._errors.append(
         #         "Please modify enum with x-enum within %s:%s"
         #         % (schema_name, property_name)
         #     )
         #     return
         if "x-enum" in property_object.keys():
             property_object["enum"] = list(property_object["x-enum"].keys())
 
-    def _resolve_x_enmu(self, content):
+    def _resolve_x_enum(self, content):
         for schema_name, schema_object in content["components"][
             "schemas"
         ].items():
             if "properties" not in schema_object:
                 continue
             for property_name, property_object in schema_object[
                 "properties"
@@ -151,14 +158,111 @@
                     property_object["type"] == "array"
                     and "items" in property_object
                 ):
                     self._inject_enum(
                         property_name, property_object["items"], schema_name
                     )
 
+    def _generate_version_api_spec(self, content):
+        if not self._generate_version_api:
+            return
+
+        print("Generating version API ...")
+        schema_name = "Version"
+        schema_ref = "#/components/schemas/{}".format(schema_name)
+        api_path = "/capabilities/version"
+
+        if schema_name in content["components"]["schemas"]:
+            schema = content["components"]["schemas"][schema_name]
+            for prop in ["api_spec_version", "sdk_version", "app_version"]:
+                if prop not in schema["properties"]:
+                    raise AssertionError(
+                        "Could not generate version schema: Version is missing property {}".format(
+                            prop
+                        )
+                    )
+                if schema["properties"][prop]["type"] != "string":
+                    raise AssertionError(
+                        "Could not generate version schema: Version property {} MUST be of type string".format(
+                            prop
+                        )
+                    )
+        else:
+            content["components"]["schemas"][schema_name] = {
+                "description": "Version details",
+                "type": "object",
+                "properties": {
+                    "api_spec_version": {
+                        "description": "Version of API specification",
+                        "type": "string",
+                        "default": "",
+                        "x-field-uid": 1,
+                    },
+                    "sdk_version": {
+                        "description": "Version of SDK generated from API specification",
+                        "type": "string",
+                        "default": "",
+                        "x-field-uid": 2,
+                    },
+                    "app_version": {
+                        "description": "Version of application consuming or serving the API",
+                        "type": "string",
+                        "default": "",
+                        "x-field-uid": 3,
+                    },
+                },
+            }
+
+        if api_path in content["paths"]:
+            assert (
+                content["paths"][api_path]["get"]["responses"]["200"][
+                    "content"
+                ]["application/json"]["schema"]["$ref"]
+                == schema_ref
+            ), "{} MUST have a 200 GET response {}".format(
+                api_path, schema_ref
+            )
+        else:
+            err_responses = {}
+            first_path = list(content["paths"].keys())[0]
+            first_method = list(content["paths"][first_path].keys())[0]
+            for code, res in content["paths"][first_path][first_method][
+                "responses"
+            ].items():
+                code_str = str(code)
+                if (
+                    not code_str.startswith("2")
+                    and not code_str.startswith("2")
+                    and not code_str.startswith("3")
+                ):
+                    err_responses[code] = res
+
+            content["paths"][api_path] = {
+                "get": {
+                    "tags": ["Capabilities"],
+                    "operationId": "get_version",
+                    "responses": {
+                        "200": {
+                            "description": "Version details from API server",
+                            "content": {
+                                "application/json": {
+                                    "schema": {"$ref": schema_ref}
+                                }
+                            },
+                            "x-field-uid": 1,
+                        },
+                    },
+                },
+            }
+
+            for code, res in err_responses.items():
+                content["paths"][api_path]["get"]["responses"][
+                    code
+                ] = copy.deepcopy(res)
+
     def _check_duplicate_uid(self, fields_uid, name):
         dup_values = set([x for x in fields_uid if fields_uid.count(x) > 1])
         if len(dup_values) > 0:
             self._errors.append(
                 "%s contain duplicate %s x-field-uid. x-field-uid should be unique."
                 % (name, list(dup_values))
             )
```

### Comparing `openapiart-0.2.8/openapiart/common.go` & `openapiart-0.2.9/openapiart/common.go`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 	"net/http"
 	"strconv"
 	"strings"
 	"time"
 	"net"
 	"regexp"
 	"google.golang.org/grpc"
+	"golang.org/x/mod/semver"
 )
 
 type grpcTransport struct {
 	clientConnection *grpc.ClientConn
 	location         string
 	requestTimeout   time.Duration
 	dialTimeout      time.Duration
@@ -414,7 +415,39 @@
 // 		}
 // 		if found {
 // 			break
 // 		}
 // 	}
 // 	return found
 // }
+
+func checkClientServerVersionCompatibility(clientVer string, serverVer string, componentName string) error {
+	c := clientVer
+	s := serverVer
+	if !strings.HasPrefix(clientVer, "v") {
+		c = "v" + clientVer
+	}
+	if !strings.HasPrefix(serverVer, "v") {
+		s = "v" + serverVer
+	}
+
+	if !semver.IsValid(c) {
+		return fmt.Errorf("client %s version '%s' is not a valid semver", componentName, clientVer)
+	}
+	if !semver.IsValid(s) {
+		return fmt.Errorf("server %s version '%s' is not a valid semver", componentName, serverVer)
+	}
+
+	err := fmt.Errorf("client %s version '%s' is not semver compatible with server %s version '%s'", componentName, clientVer, componentName, serverVer)
+
+	if v := semver.Compare(c, s); v > 0 {
+		if semver.MajorMinor(c) != semver.MajorMinor(s) {
+			return err
+		}
+	} else if v < 0 {
+		if semver.Major(c) != semver.Major(s) {
+			return err
+		}
+	}
+
+	return nil
+}
```

### Comparing `openapiart-0.2.8/openapiart/common.py` & `openapiart-0.2.9/openapiart/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import yaml
 import requests
 import urllib3
 import io
 import sys
 import time
 import grpc
+import semantic_version
 import types
 import platform
 from google.protobuf import json_format
 import sanity_pb2_grpc as pb2_grpc
 import sanity_pb2 as pb2
 
 try:
@@ -36,14 +37,15 @@
 def api(
     location=None,
     transport=None,
     verify=True,
     logger=None,
     loglevel=logging.INFO,
     ext=None,
+    version_check=False,
 ):
     """Create an instance of an Api class
 
     generator.Generator outputs a base Api class with the following:
     - an abstract method for each OpenAPI path item object
     - a concrete properties for each unique OpenAPI path item parameter.
```

### Comparing `openapiart-0.2.8/openapiart/generator.py` & `openapiart-0.2.9/openapiart/generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,14 +45,17 @@
     def __init__(
         self,
         openapi_filename,
         package_name,
         protobuf_package_name,
         output_dir=None,
         extension_prefix=None,
+        generate_version_api=None,
+        api_version=None,
+        sdk_version=None,
     ):
         self._parsers = {}
         self._base_url = ""
         self._generated_methods = []
         self._generated_classes = []
         self._generated_top_level_factories = []
         self._openapi_filename = openapi_filename
@@ -64,14 +67,23 @@
         if os.path.exists(self._output_dir) is False:
             os.mkdir(self._output_dir)
         self._package_name = package_name
         self._protobuf_package_name = protobuf_package_name
         self._output_file = package_name
         self._docs_dir = os.path.join(self._src_dir, "..", "docs")
         self._deprecated_properties = {}
+        self._generate_version_api = generate_version_api
+        if self._generate_version_api is None:
+            self._generate_version_api = False
+        self._api_version = api_version
+        if self._api_version is None:
+            self._api_version = ""
+        self._sdk_version = sdk_version
+        if self._sdk_version is None:
+            self._sdk_version = ""
         self._get_openapi_file()
         # self._plugins = self._load_plugins()
 
     def _get_parser(self, pattern):
         if pattern not in self._parsers:
             parser = parse(pattern)
             self._parsers[pattern] = parser
@@ -465,14 +477,19 @@
                     self._write(
                         1, "def %s(self, payload):" % rpc_method.method
                     )
                     self._write(2, "pb_obj = json_format.Parse(")
                     self._write(3, "self._serialize_payload(payload),")
                     self._write(3, "pb2.%s()" % rpc_method.request_class)
                     self._write(2, ")")
+                    if (
+                        self._generate_version_api
+                        and rpc_method.method != "get_version"
+                    ):
+                        self._write(2, "self._do_version_check_once()")
                     "%s=pb_obj" % rpc_method.request_property
                     self._write(
                         2,
                         "req_obj = pb2.{operation_name}Request({request_property}=pb_obj)".format(
                             operation_name=rpc_method.operation_name,
                             request_property=rpc_method.request_property,
                         ),
@@ -609,14 +626,20 @@
                 )
                 self._write(0)
                 self._write(2, "%s" % method["description"])
                 self._write(0)
                 self._write(2, "Return: %s" % method["response_type"])
                 self._write(2, '"""')
 
+                if (
+                    self._generate_version_api
+                    and method["name"] != "get_version"
+                ):
+                    self._write(2, "self._do_version_check_once()")
+
                 self._write(2, "return self._transport.send_recv(")
                 self._write(3, '"%s",' % method["http_method"])
                 self._write(3, '"%s",' % method["url"])
                 self._write(
                     3,
                     "payload=%s,"
                     % (
@@ -644,15 +667,36 @@
             self._write()
             self._write(0, "class %s(object):" % factory_class_name)
             self._write(1, '"""%s' % "OpenApi Abstract API")
             self._write(1, '"""')
             self._write()
             self._write(1, "__warnings__ = []")
             self._write(1, "def __init__(self, **kwargs):")
-            self._write(2, "pass")
+            if self._generate_version_api:
+                self._write(2, "self._version_meta = self.version()")
+                self._write(
+                    2,
+                    'self._version_meta.api_spec_version = "{}"'.format(
+                        self._api_version
+                    ),
+                )
+                self._write(
+                    2,
+                    'self._version_meta.sdk_version = "{}"'.format(
+                        self._sdk_version
+                    ),
+                )
+                self._write(
+                    2, 'self._version_check = kwargs.get("version_check")'
+                )
+                self._write(2, "if self._version_check is None:")
+                self._write(3, "self._version_check = False")
+                self._write(2, "self._version_check_err = None")
+            else:
+                self._write(2, "pass")
             for method in methods:
                 print("generating method %s" % method["name"])
                 self._write()
                 # TODO: restore behavior
                 # if method["x_status"] is not None:
                 #     self._write(
                 #         1,
@@ -709,14 +753,103 @@
             # self._write(1, "def clear_api_warnings(self):")
             # self._write(
             #     2, 'if "2.7" in platform.python_version().rsplit(".", 1)[0]:'
             # )
             # self._write(3, "del openapi_warnings[:]")
             # self._write(2, "else:")
             # self._write(3, "openapi_warnings.clear()")
+            self._generate_version_api_methods()
+
+    def _generate_version_api_methods(self):
+        if not self._generate_version_api:
+            return
+
+        self._write(
+            indent=1,
+            line="""def _check_client_server_version_compatibility(
+        self, client_ver, server_ver, component_name
+    ):
+        if not semantic_version.validate(client_ver):
+            raise AssertionError(
+                "Client {} version '{}' is not a valid semver".format(
+                    component_name, client_ver
+                )
+            )
+
+        if not semantic_version.validate(server_ver):
+            raise AssertionError(
+                "Server {} version '{}' is not a valid semver".format(
+                    component_name, server_ver
+                )
+            )
+
+        err = "Client {} version '{}' is not semver compatible with Server {} version '{}'".format(
+            component_name, client_ver, component_name, server_ver
+        )
+
+        c = semantic_version.Version(client_ver)
+        s = semantic_version.Version(server_ver)
+        v = semantic_version.compare(client_ver, server_ver)
+        if v > 0:
+            if c.major != s.major or c.minor != s.minor:
+                raise Exception(err)
+        elif v < 0:
+            if c.major != s.major:
+                raise Exception(err)
+
+    def get_local_version(self):
+        return self._version_meta
+
+    def get_remote_version(self):
+        return self.get_version()
+
+    def check_version_compatibility(self):
+        comp_err, api_err = self._do_version_check()
+        if comp_err is not None:
+            raise comp_err
+        if api_err is not None:
+            raise api_err
+
+    def _do_version_check(self):
+        local = self.get_local_version()
+        try:
+            remote = self.get_remote_version()
+        except Exception as e:
+            return None, e
+
+        try:
+            self._check_client_server_version_compatibility(
+                local.api_spec_version, remote.api_spec_version, "API spec"
+            )
+        except Exception as e:
+            msg = "client SDK version '{}' is not compatible with server SDK version '{}'".format(
+                local.sdk_version, remote.sdk_version
+            )
+            return Exception("{}: {}".format(msg, str(e))), None
+
+        return None, None
+
+    def _do_version_check_once(self):
+        if not self._version_check:
+            return
+
+        if self._version_check_err is not None:
+            raise self._version_check_err
+
+        comp_err, api_err = self._do_version_check()
+        if comp_err is not None:
+            self._version_check_err = comp_err
+            raise comp_err
+        if api_err is not None:
+            self._version_check_err = None
+            raise api_err
+
+        self._version_check = False
+        self._version_check_err = None""",
+        )
 
     def _get_object_property_class_names(self, ref):
         """Returns: `Tuple(object_name, property_name, class_name, ref_name)`"""
         object_name = None
         property_name = None
         class_name = None
         ref_name = None
```

### Comparing `openapiart-0.2.8/openapiart/goserver/api/service_a.api.yaml` & `openapiart-0.2.9/openapiart/goserver/api/service_a.api.yaml`

 * *Files identical despite different names*

### Comparing `openapiart-0.2.8/openapiart/goserver/api/service_b.api.yaml` & `openapiart-0.2.9/openapiart/goserver/api/service_b.api.yaml`

 * *Files identical despite different names*

### Comparing `openapiart-0.2.8/openapiart/goserver/api/service_b.yaml` & `openapiart-0.2.9/openapiart/goserver/api/service_b.yaml`

 * *Files identical despite different names*

### Comparing `openapiart-0.2.8/openapiart/goserver/generator_context.py` & `openapiart-0.2.9/openapiart/goserver/generator_context.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.2.8/openapiart/goserver/go_controller_generator.py` & `openapiart-0.2.9/openapiart/goserver/go_controller_generator.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.2.8/openapiart/goserver/go_interface_generator.py` & `openapiart-0.2.9/openapiart/goserver/go_interface_generator.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.2.8/openapiart/goserver/goserver.py` & `openapiart-0.2.9/openapiart/goserver/goserver.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.2.8/openapiart/goserver/http_setup.go` & `openapiart-0.2.9/openapiart/goserver/http_setup.go`

 * *Files identical despite different names*

### Comparing `openapiart-0.2.8/openapiart/goserver/response.go` & `openapiart-0.2.9/openapiart/goserver/response.go`

 * *Files identical despite different names*

### Comparing `openapiart-0.2.8/openapiart/goserver/writer.py` & `openapiart-0.2.9/openapiart/goserver/writer.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.2.8/openapiart/gotidy.py` & `openapiart-0.2.9/openapiart/gotidy.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.2.8/openapiart/openapiart.py` & `openapiart-0.2.9/openapiart/openapiart.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     def __init__(
         self,
         api_files,
         protobuf_name=None,
         artifact_dir=None,
         extension_prefix=None,
         proto_service=None,
+        generate_version_api=False,
     ):
         self._output_dir = os.path.abspath(
             artifact_dir if artifact_dir is not None else "art"
         )
         self._doc_dir = os.path.abspath(
             # doc dir name is not getting ignored by git
             os.path.join(artifact_dir, "..", "proto_doc")
@@ -53,14 +54,15 @@
         print(
             "Artifact output directory: {output_dir}".format(
                 output_dir=self._output_dir
             )
         )
         shutil.rmtree(self._output_dir, ignore_errors=True)
         self._api_files = api_files
+        self._generate_version_api = generate_version_api
         self._bundle()
         self._get_info()
         self._get_license()
         self._document()
 
     def _get_license(self):
         license_name = self._bundler._content["info"]["license"]["name"]
@@ -84,17 +86,20 @@
             raise ex
 
     def _bundle(self):
         # bundle the yaml files
         module = importlib.import_module("openapiart.bundler")
         bundler_class = getattr(module, "Bundler")
         self._bundler = bundler_class(
-            api_files=self._api_files, output_dir=self._output_dir
+            api_files=self._api_files,
+            output_dir=self._output_dir,
+            generate_version_api=self._generate_version_api,
         )
         self._bundler.bundle()
+        self._api_version = self._bundler.get_api_version()
         # read the entire openapi file
         with open(self._bundler.openapi_filepath) as fp:
             self._openapi = yaml.safe_load(fp.read())
 
     def _document(self):
         """Try documenting the openapi using redoc-cli
 
@@ -118,15 +123,15 @@
         except Exception as e:
             print("Bypassed creation of static documentation: {}".format(e))
 
     def GenerateProtoDef(self, package_name):
         self._protobuf_package_name = package_name
         self._generate_proto_file()
 
-    def GeneratePythonSdk(self, package_name):
+    def GeneratePythonSdk(self, package_name, sdk_version=""):
         """Generates a Python UX Sdk
         Args
         ----
         - package_name (str): the name of the python module
 
         Example
         -------
@@ -142,24 +147,28 @@
                 |_ __init__.py
                 |_ sanity.py
                 |_ sanity_pb.py
                 |_ sanity_grpc_pb.py
         ```
         """
         self._python_module_name = package_name
-        if not self.proto_file_exsists():
+        self._python_sdk_version = sdk_version
+        if not self.proto_file_exists():
             self._generate_proto_file()
         if self._python_module_name is not None:
             module = importlib.import_module("openapiart.generator")
             python_ux = getattr(module, "Generator")(
                 self._bundler.openapi_filepath,
                 self._python_module_name,
                 self._protobuf_package_name,
                 output_dir=self._output_dir,
                 extension_prefix=self._extension_prefix,
+                generate_version_api=self._generate_version_api,
+                api_version=self._api_version,
+                sdk_version=self._python_sdk_version,
             )
             python_ux.generate()
         try:
             python_sdk_dir = os.path.normpath(
                 os.path.join(self._output_dir, self._python_module_name)
             )
             process_args = [
@@ -207,15 +216,15 @@
             print("Formatting Generated Python SDK: {}".format(cmd))
             subprocess.check_call(cmd, shell=True)
             generate_requirements(
                 path=os.path.normpath(os.path.join(python_sdk_dir, ".."))
             )
         return self
 
-    def GenerateGoSdk(self, package_dir, package_name):
+    def GenerateGoSdk(self, package_dir, package_name, sdk_version=""):
         """Generates a Go UX Sdk
 
         Args
         ----
         - package_dir: Go mod package dir published under go.mod
         - package_name: Name of the Go package to generate
 
@@ -240,15 +249,16 @@
                             |_ sanitypb.pb.go
                             |_ sanitypb_grpc.go
         ```
         """
 
         self._go_sdk_package_dir = package_dir
         self._go_sdk_package_name = package_name
-        if not self.proto_file_exsists():
+        self._go_sdk_version = sdk_version
+        if not self.proto_file_exists():
             self._generate_proto_file()
         if self._go_sdk_package_dir and self._protobuf_package_name:
             go_sdk_output_dir = os.path.normpath(
                 os.path.join(
                     self._output_dir,
                     "..",
                     os.path.split(self._go_sdk_package_dir)[-1],
@@ -281,14 +291,17 @@
                     "info": self._info,
                     "license": self._license,
                     "protobuf_package_name": self._protobuf_package_name,
                     "go_sdk_package_dir": self._go_sdk_package_dir,
                     "go_sdk_package_name": self._go_sdk_package_name,
                     "output_dir": self._output_dir,
                     "proto_service": self._proto_service,
+                    "generate_version_api": self._generate_version_api,
+                    "api_version": self._api_version,
+                    "sdk_version": self._go_sdk_version,
                 }
             )
             print("Generating go ux sdk: {}".format(" ".join(process_args)))
             go_ux.generate(self._openapi)
         return self
 
     def GenerateGoServer(self, module_path, models_prefix="", models_path=""):
@@ -335,15 +348,15 @@
                 "output_dir": self._output_dir,
                 "proto_service": self._proto_service,
                 "doc_dir": self._doc_dir,
             }
         )
         protobuf.generate(self._openapi)
 
-    def proto_file_exsists(self):
+    def proto_file_exists(self):
         proto_file_path = os.path.normpath(
             os.path.join(
                 self._output_dir,
                 "{}.proto".format(self._protobuf_package_name),
             )
         )
         return os.path.exists(proto_file_path)
```

### Comparing `openapiart-0.2.8/openapiart/openapiartgo.py` & `openapiart-0.2.9/openapiart/openapiartgo.py`

 * *Files 3% similar despite different names*

```diff
@@ -272,14 +272,26 @@
             os.path.join(self._ux_path, "common.go")
         )
         self._init_fp(self._filename)
         self._write_package()
         with open(os.path.join(os.path.dirname(__file__), "common.go")) as fp:
             self._write(fp.read().strip().strip("\n"))
         self._write()
+
+        self._filename = os.path.normpath(
+            os.path.join(self._ux_path, "common_test.go")
+        )
+        self._init_fp(self._filename)
+        self._write_package()
+        with open(
+            os.path.join(os.path.dirname(__file__), "common_test.go")
+        ) as fp:
+            self._write(fp.read().strip().strip("\n"))
+        self._write()
+
         self._fp = go_pkg_fp
         self._filename = go_pkg_filename
 
     def _write_types(self):
         for _, go_type in self._oapi_go_types.items():
             if go_type.startswith("String"):
                 self._write("type {go_type} string".format(go_type=go_type))
@@ -588,18 +600,26 @@
                         rpc.responses.append(response)
                         http.responses.append(response)
 
         self._build_response_interfaces()
 
         # write the go code
         self._write(
-            """type {internal_struct_name} struct {{
+            """
+            type versionMeta struct {{
+                checkVersion  bool
+                localVersion  Version
+                remoteVersion Version
+                checkError    error
+            }}
+            type {internal_struct_name} struct {{
                 api
                 grpcClient {pb_pkg_name}.{proto_service}Client
                 httpClient httpClient
+                versionMeta *versionMeta
             }}
 
             // grpcConnect builds up a grpc connection
             func (api *{internal_struct_name}) grpcConnect() error {{
                 if api.grpcClient == nil {{
                     if api.grpc.clientConnection == nil {{
                         ctx, cancelFunc := context.WithTimeout(context.Background(), api.grpc.dialTimeout)
@@ -646,14 +666,15 @@
                 }}
                 return nil
             }}
 
             //  NewApi returns a new instance of the top level interface hierarchy
             func NewApi() {interface} {{
                 api := {internal_struct_name}{{}}
+                api.versionMeta = &versionMeta{{checkVersion: false}}
                 return &api
             }}
 
             // httpConnect builds up a http connection
             func (api *{internal_struct_name}) httpConnect() error {{
                 if api.httpClient.client == nil {{
                     tr := http.Transport{{
@@ -719,14 +740,16 @@
         for new in self._api.external_new_methods:
             methods.append(new.method_description)
             methods.append(new.method)
         for rpc in self._api.external_rpc_methods:
             methods.append(rpc.description)
             methods.append(rpc.method)
             # descriptions.append("(*{}).{}".format(self._api.external_interface_name, rpc.method_description))
+        if self._generate_version_api:
+            methods.extend(self._get_version_api_interface_method_signatures())
         method_signatures = "\n".join(methods)
         self._write(
             """
             {description}
             type {external_interface_name} interface {{
                 Api
                 {method_signatures}
@@ -749,14 +772,20 @@
                 }}
                 """.format(
                     internal_struct_name=self._api.internal_struct_name,
                     method=new.method,
                     interface=new.interface,
                 )
             )
+        if self._generate_version_api:
+            self._write(
+                self._get_version_api_interface_method_impl(
+                    self._api.internal_struct_name
+                )
+            )
         for rpc in self._api.external_rpc_methods:
             error_handling = ""
             for response in rpc.responses:
                 if response.status_code.startswith("2"):
                     continue
                 error_handling += """if resp.GetStatusCode_{status_code}() != nil {{
                         data, _ := yaml.Marshal(resp.GetStatusCode_{status_code}())
@@ -786,21 +815,28 @@
             # TODO: restore behavior
             # info = rpc.status.get("additional_information")
             # func = rpc.status.get("status")
             # status_str = "{func}{msg}".format(
             #     func="" if func is None else "api.{}".format(func),
             #     msg="(`%s`)" % info if info is not None else "",
             # )
+            if self._generate_version_api:
+                version_check = """
+                    if err := api.checkLocalRemoteVersionCompatibilityOnce(); err != nil {
+                        return nil, err
+                    }"""
+            else:
+                version_check = ""
             self._write(
                 """func (api *{internal_struct_name}) {method} {{
                     {validate}
+                    {version_check}
                     if api.hasHttpTransport() {{
                             {http_call}
                     }}
-
                     if err := api.grpcConnect(); err != nil {{
                         return nil, err
                     }}
                     request := {request}
                     ctx, cancelFunc := context.WithTimeout(context.Background(), api.grpc.requestTimeout)
                     defer cancelFunc()
                     resp, err := api.grpcClient.{operation_name}(ctx, &request)
@@ -815,14 +851,17 @@
                     method=rpc.method,
                     request=rpc.request,
                     operation_name=rpc.operation_name,
                     error_handling=error_handling,
                     return_value=return_value,
                     http_call=rpc.http_call,
                     validate=getattr(rpc, "validate", ""),
+                    version_check=""
+                    if rpc.method == "GetVersion() (Version, error)"
+                    else version_check,
                 )
             )
 
         for http in self._api.internal_http_methods:
             error_handling = ""
             success_method = None
             for response in http.responses:
@@ -879,14 +918,111 @@
                 )
             )
 
     def _build_request_interfaces(self):
         for new in self._api.external_new_methods:
             self._write_interface(new)
 
+    def _get_version_api_interface_method_signatures(self):
+        return [
+            "// GetLocalVersion provides version details of local client",
+            "GetLocalVersion() Version",
+            "// GetRemoteVersion provides version details received from remote server",
+            "GetRemoteVersion() (Version, error)",
+            "// SetVersionCompatibilityCheck allows enabling or disabling automatic version",
+            "// compatibility check between client and server API spec version upon API call",
+            "SetVersionCompatibilityCheck(bool)",
+            "// CheckVersionCompatibility compares API spec version for local client and remote server,",
+            "// and returns an error if they are not compatible according to Semantic Versioning 2.0.0",
+            "CheckVersionCompatibility() error",
+        ]
+
+    def _get_version_api_interface_method_impl(self, struct_name):
+        return """
+            func (api *{0}) GetLocalVersion() Version {{
+                if api.versionMeta.localVersion == nil {{
+                    api.versionMeta.localVersion = NewVersion().SetApiSpecVersion("{1}").SetSdkVersion("{2}")
+                }}
+
+                return api.versionMeta.localVersion
+            }}
+
+            func (api *{0}) GetRemoteVersion() (Version, error) {{
+                if api.versionMeta.remoteVersion == nil {{
+                    v, err := api.GetVersion()
+                    if err != nil {{
+                        return nil, fmt.Errorf("could not fetch remote version: %v", err)
+                    }}
+
+                    api.versionMeta.remoteVersion = v
+                }}
+
+                return api.versionMeta.remoteVersion, nil
+            }}
+
+            func (api *{0}) SetVersionCompatibilityCheck(v bool) {{
+                api.versionMeta.checkVersion = v
+            }}
+
+            func (api *{0}) checkLocalRemoteVersionCompatibility() (error, error) {{
+                localVer := api.GetLocalVersion()
+                remoteVer, err := api.GetRemoteVersion()
+                if err != nil {{
+                    return nil, err
+                }}
+                err = checkClientServerVersionCompatibility(localVer.ApiSpecVersion(), remoteVer.ApiSpecVersion(), "API spec")
+                if err != nil {{
+                    return fmt.Errorf(
+                        "client SDK version '%s' is not compatible with server SDK version '%s': %v",
+                        localVer.SdkVersion(), remoteVer.SdkVersion(), err,
+                    ), nil
+                }}
+
+                return nil, nil
+            }}
+
+            func (api *{0}) checkLocalRemoteVersionCompatibilityOnce() error {{
+                if !api.versionMeta.checkVersion {{
+                    return nil
+                }}
+
+                if api.versionMeta.checkError != nil {{
+                    return api.versionMeta.checkError
+                }}
+
+                compatErr, apiErr := api.checkLocalRemoteVersionCompatibility()
+                if compatErr != nil {{
+                    api.versionMeta.checkError = compatErr
+                    return compatErr
+                }}
+                if apiErr != nil {{
+                    api.versionMeta.checkError = nil
+                    return apiErr
+                }}
+
+                api.versionMeta.checkVersion = false
+                api.versionMeta.checkError = nil
+                return nil
+            }}
+
+            func (api *{0}) CheckVersionCompatibility() error {{
+                compatErr, apiErr := api.checkLocalRemoteVersionCompatibility()
+                if compatErr != nil {{
+                    return fmt.Errorf("version error: %v", compatErr)
+                }}
+                if apiErr != nil {{
+                    return apiErr
+                }}
+
+                return nil
+            }}
+        """.format(
+            struct_name, self._api_version, self._sdk_version
+        )
+
     def _write_component_interfaces(self):
         while True:
             components = [
                 component
                 for _, component in self._api.components.items()
                 if component.generated is False
             ]
```

### Comparing `openapiart-0.2.8/openapiart/openapiartplugin.py` & `openapiart-0.2.9/openapiart/openapiartplugin.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,14 +15,23 @@
             None
             if "python_module_name" not in kwargs
             else kwargs["python_module_name"]
         )
         self._protobuf_package_name = kwargs["protobuf_package_name"]
         self._protobuf_file_name = kwargs["protobuf_package_name"]
         self._go_sdk_package_dir = kwargs["go_sdk_package_dir"]
+        self._generate_version_api = kwargs.get("generate_version_api")
+        if self._generate_version_api is None:
+            self._generate_version_api = False
+        self._api_version = kwargs.get("api_version")
+        if self._api_version is None:
+            self._api_version = ""
+        self._sdk_version = kwargs.get("sdk_version")
+        if self._sdk_version is None:
+            self._sdk_version = ""
         self._go_sdk_package_name = (
             None
             if "go_sdk_package_name" not in kwargs
             else kwargs["go_sdk_package_name"]
         )
         self.default_indent = "    "
         self._parsers = {}
```

### Comparing `openapiart-0.2.8/openapiart/openapiartprotobuf.py` & `openapiart-0.2.9/openapiart/openapiartprotobuf.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.2.8/openapiart/requirements.py` & `openapiart-0.2.9/openapiart/requirements.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.2.8/openapiart/requirements.txt` & `openapiart-0.2.9/openapiart/requirements.txt`

 * *Files 18% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 typing
 setuptools
 wheel
 PyYAML
 openapi_spec_validator==0.3.0
 jsonpath_ng
 urllib3
+semantic_version
 typing_extensions ; python_version > '2.7'
 click==8.0.4; python_version > '2.7' # this is added because of the black failure in CI
 black==22.1.0 ; python_version > '2.7'
 grpcio==1.44.0 ; python_version > '2.7'
 grpcio==1.35.0 ; python_version == '2.7'
 grpcio-tools==1.44.0 ; python_version > '2.7'
 grpcio-tools==1.35.0 ; python_version == '2.7'
 pipreqs; python_version > '2.7'
 protobuf==3.15.0 ;  python_version <= '3.6'
-protobuf==3.20.1 ;  python_version > '3.6'
+protobuf==3.20.1 ;  python_version > '3.6'
```

### Comparing `openapiart-0.2.8/openapiart/tests/api/api.yaml` & `openapiart-0.2.9/openapiart/tests/api/api.yaml`

 * *Files identical despite different names*

### Comparing `openapiart-0.2.8/openapiart/tests/api/info.yaml` & `openapiart-0.2.9/openapiart/tests/api/info.yaml`

 * *Files identical despite different names*

### Comparing `openapiart-0.2.8/openapiart/tests/common/common.yaml` & `openapiart-0.2.9/openapiart/tests/common/common.yaml`

 * *Files identical despite different names*

### Comparing `openapiart-0.2.8/openapiart/tests/config/config.yaml` & `openapiart-0.2.9/openapiart/tests/config/config.yaml`

 * *Files identical despite different names*

### Comparing `openapiart-0.2.8/openapiart/tests/config/negative_nested_config.yaml` & `openapiart-0.2.9/openapiart/tests/config/negative_nested_config.yaml`

 * *Files identical despite different names*

### Comparing `openapiart-0.2.8/openapiart/tests/conftest.py` & `openapiart-0.2.9/openapiart/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.2.8/openapiart/tests/field_uid/fielduid.yaml` & `openapiart-0.2.9/openapiart/tests/field_uid/fielduid.yaml`

 * *Files identical despite different names*

### Comparing `openapiart-0.2.8/openapiart/tests/field_uid/property_name_camel_case.yaml` & `openapiart-0.2.9/openapiart/tests/field_uid/property_name_camel_case.yaml`

 * *Files identical despite different names*

### Comparing `openapiart-0.2.8/openapiart/tests/field_uid/property_name_pascal_case.yaml` & `openapiart-0.2.9/openapiart/tests/field_uid/property_name_pascal_case.yaml`

 * *Files identical despite different names*

### Comparing `openapiart-0.2.8/openapiart/tests/field_uid/property_name_upper_case.yaml` & `openapiart-0.2.9/openapiart/tests/field_uid/property_name_upper_case.yaml`

 * *Files identical despite different names*

### Comparing `openapiart-0.2.8/openapiart/tests/field_uid/xenum.yaml` & `openapiart-0.2.9/openapiart/tests/field_uid/xenum.yaml`

 * *Files identical despite different names*

### Comparing `openapiart-0.2.8/openapiart/tests/field_uid/xinclude.yaml` & `openapiart-0.2.9/openapiart/tests/field_uid/xinclude.yaml`

 * *Files identical despite different names*

### Comparing `openapiart-0.2.8/openapiart/tests/grpcserver.py` & `openapiart-0.2.9/openapiart/tests/grpcserver.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,16 +10,17 @@
 
 sys.path.append(os.path.join(os.path.dirname(__file__), "..", "..", "art"))
 sys.path.append(
     os.path.join(os.path.dirname(__file__), "..", "..", "art", "sanity")
 )
 pb2_grpc = importlib.import_module("sanity_pb2_grpc")
 pb2 = importlib.import_module("sanity_pb2")
+op = importlib.import_module("sanity")
 
-GRPC_PORT = 50051
+GRPC_PORT = 40052
 
 
 class OpenapiServicer(pb2_grpc.OpenapiServicer):
     def __init__(self):
         self._prefix_config = None
         super(OpenapiServicer, self).__init__()
 
@@ -61,14 +62,23 @@
         self._log("Executing GetConfig")
         response_200 = {"status_code_200": self._prefix_config}
         res_obj = json_format.Parse(
             json.dumps(response_200), pb2.GetConfigResponse()
         )
         return res_obj
 
+    def GetVersion(self, request, context):
+        self._log("Executing GetVersion")
+        v = op.api().get_local_version()
+        response_200 = {"status_code_200": v.serialize(v.DICT)}
+        res_obj = json_format.Parse(
+            json.dumps(response_200), pb2.GetVersionResponse()
+        )
+        return res_obj
+
 
 def gRpcServer():
     server = grpc.server(futures.ThreadPoolExecutor(max_workers=10))
     pb2_grpc.add_OpenapiServicer_to_server(OpenapiServicer(), server)
     print("gRPC Server: Starting server. Listening on port %s." % GRPC_PORT)
     server.add_insecure_port("[::]:{}".format(GRPC_PORT))
     server.start()
```

### Comparing `openapiart-0.2.8/openapiart/tests/multilevel/multi.yaml` & `openapiart-0.2.9/openapiart/tests/multilevel/multi.yaml`

 * *Files identical despite different names*

### Comparing `openapiart-0.2.8/openapiart/tests/pattern/pattern.yaml` & `openapiart-0.2.9/openapiart/tests/pattern/pattern.yaml`

 * *Files identical despite different names*

### Comparing `openapiart-0.2.8/openapiart/tests/server.py` & `openapiart-0.2.9/openapiart/tests/server.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import sys
 
 
 app = Flask(__name__)
 app.CONFIG = None
 app.PACKAGE = None
 app.UPDATE_CONFIG = None
-app.PORT = 18080
+app.PORT = 8444
 app.HOST = "0.0.0.0"
 
 
 @app.route("/api/config", methods=["POST"])
 def set_config():
     config = app.PACKAGE.Api().prefix_config()
     config.deserialize(request.data.decode("utf-8"))
@@ -45,14 +45,23 @@
     app.CONFIG.c = 1
     app.CONFIG.required_object.e_a = 1.1
     app.CONFIG.required_object.e_b = 1.2
     serialized_config = app.CONFIG.serialize()
     return Response(serialized_config, mimetype="application/json", status=200)
 
 
+@app.route("/api/capabilities/version", methods=["GET"])
+def get_version():
+    return Response(
+        app.PACKAGE.Api().get_local_version().serialize(),
+        mimetype="application/json",
+        status=200,
+    )
+
+
 @app.after_request
 def after_request(resp):
     print(request.method, request.url, " -> ", resp.status)
     return resp
 
 
 class OpenApiServer(object):
```

### Comparing `openapiart-0.2.8/openapiart/tests/test_add.py` & `openapiart-0.2.9/openapiart/tests/test_add.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.2.8/openapiart/tests/test_auto.py` & `openapiart-0.2.9/openapiart/tests/test_auto.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.2.8/openapiart/tests/test_bundle.py` & `openapiart-0.2.9/openapiart/tests/test_bundle.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.2.8/openapiart/tests/test_bundler.py` & `openapiart-0.2.9/openapiart/tests/test_bundler.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.2.8/openapiart/tests/test_constraints.py` & `openapiart-0.2.9/openapiart/tests/test_constraints.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.2.8/openapiart/tests/test_fielduid.py` & `openapiart-0.2.9/openapiart/tests/test_fielduid.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.2.8/openapiart/tests/test_formats.py` & `openapiart-0.2.9/openapiart/tests/test_formats.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.2.8/openapiart/tests/test_func.py` & `openapiart-0.2.9/openapiart/tests/test_func.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.2.8/openapiart/tests/test_grpc_response.py` & `openapiart-0.2.9/openapiart/tests/test_grpc_response.py`

 * *Files 24% similar despite different names*

```diff
@@ -34,9 +34,35 @@
         )
     assert (
         execinfo.value.args[0]
         == """ext and transport are not mutually exclusive. Please configure one of them."""
     )
 
 
+def test_grpc_valid_version_check(utils, grpc_api):
+    with open(utils.get_test_config_path("config.json")) as f:
+        payload = json.load(f)
+    try:
+        grpc_api._version_check = True
+        result = grpc_api.set_config(payload)
+        assert result.read() == b"success"
+    finally:
+        grpc_api._version_check = False
+
+
+def test_grpc_valid_inversion_check(utils, grpc_api):
+    with open(utils.get_test_config_path("config.json")) as f:
+        payload = json.load(f)
+    try:
+        grpc_api.get_local_version().api_spec_version = "0.2.1"
+        grpc_api._version_check = True
+        grpc_api.set_config(payload)
+        raise Exception("expected version error")
+    except Exception:
+        pass
+    finally:
+        grpc_api.get_local_version().api_spec_version = "0.1.0"
+        grpc_api._version_check = False
+
+
 if __name__ == "__main__":
     pytest.main(["-v", "-s", __file__])
```

### Comparing `openapiart-0.2.8/openapiart/tests/test_int64.py` & `openapiart-0.2.9/openapiart/tests/test_int64.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.2.8/openapiart/tests/test_perf.py` & `openapiart-0.2.9/openapiart/tests/test_perf.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.2.8/openapiart/tests/test_protobuf.py` & `openapiart-0.2.9/openapiart/tests/test_protobuf.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.2.8/openapiart/tests/test_py_go_diff.py` & `openapiart-0.2.9/openapiart/tests/test_py_go_diff.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.2.8/openapiart/tests/test_remove.py` & `openapiart-0.2.9/openapiart/tests/test_remove.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.2.8/openapiart/tests/test_unique.py` & `openapiart-0.2.9/openapiart/tests/test_unique.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.2.8/openapiart/tests/test_validate_property_name.py` & `openapiart-0.2.9/openapiart/tests/test_validate_property_name.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.2.8/openapiart/tests/test_validate_xenum.py` & `openapiart-0.2.9/openapiart/tests/test_validate_xenum.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.2.8/openapiart/tests/test_validate_xinclude.py` & `openapiart-0.2.9/openapiart/tests/test_validate_xinclude.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.2.8/openapiart/tests/test_validation.py` & `openapiart-0.2.9/openapiart/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.2.8/openapiart/tests/test_warnings.py` & `openapiart-0.2.9/openapiart/tests/test_warnings.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.2.8/openapiart/tests/utils/common.py` & `openapiart-0.2.9/openapiart/tests/utils/common.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.2.8/openapiart/utils/autofielduid.py` & `openapiart-0.2.9/openapiart/utils/autofielduid.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.2.8/openapiart.egg-info/PKG-INFO` & `openapiart-0.2.9/openapiart.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openapiart
-Version: 0.2.8
+Version: 0.2.9
 Summary: The OpenAPI Artifact Generator Python Package
 Home-page: https://github.com/open-traffic-generator/openapiart
 Author: https://github.com/open-traffic-generator/openapiart
 Author-email: andy.balogh@keysight.com
 License: MIT
 Keywords: testing openapi artifact generator
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `openapiart-0.2.8/openapiart.egg-info/SOURCES.txt` & `openapiart-0.2.9/openapiart.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 README.md
 pyproject.toml
 setup.py
 openapiart/__init__.py
 openapiart/bundler.py
 openapiart/common.go
 openapiart/common.py
+openapiart/common_test.go
 openapiart/generator.py
 openapiart/gotidy.py
 openapiart/openapiart.py
 openapiart/openapiartgo.py
 openapiart/openapiartplugin.py
 openapiart/openapiartprotobuf.py
 openapiart/openapiartpython.py
@@ -45,14 +46,15 @@
 openapiart/tests/test_bundle.py
 openapiart/tests/test_bundler.py
 openapiart/tests/test_constraints.py
 openapiart/tests/test_fielduid.py
 openapiart/tests/test_formats.py
 openapiart/tests/test_func.py
 openapiart/tests/test_grpc_response.py
+openapiart/tests/test_http_response.py
 openapiart/tests/test_int64.py
 openapiart/tests/test_license.py
 openapiart/tests/test_perf.py
 openapiart/tests/test_protobuf.py
 openapiart/tests/test_py_go_diff.py
 openapiart/tests/test_remove.py
 openapiart/tests/test_unique.py
```

### Comparing `openapiart-0.2.8/setup.py` & `openapiart-0.2.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 To build distribution: python setup.py sdist --formats=gztar bdist_wheel --universal
 """
 import os
 import setuptools
 
 pkg_name = "openapiart"
-version = "0.2.8"
+version = "0.2.9"
 
 base_dir = os.path.dirname(os.path.abspath(__file__))
 with open(os.path.join(base_dir, "README.md")) as fid:
     long_description = fid.read()
 
 requirements_path = os.path.join(base_dir, "openapiart", "requirements.txt")
 test_req_path = os.path.join(base_dir, "test_requirements.txt")
```

