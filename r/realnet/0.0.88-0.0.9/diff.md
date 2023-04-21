# Comparing `tmp/realnet-0.0.88.tar.gz` & `tmp/realnet-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "realnet-0.0.88.tar", last modified: Fri Apr 21 01:44:14 2023, max compression
+gzip compressed data, was "dist/realnet-0.0.9.tar", last modified: Fri Sep 11 21:55:22 2020, max compression
```

## Comparing `realnet-0.0.88.tar` & `realnet-0.0.9.tar`

### file list

```diff
@@ -1,186 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:44:14.189601 realnet-0.0.88/
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-21 01:41:30.000000 realnet-0.0.88/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7492 2023-04-21 01:44:14.189601 realnet-0.0.88/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-04-21 01:41:30.000000 realnet-0.0.88/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:44:14.177601 realnet-0.0.88/realnet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:44:14.177601 realnet-0.0.88/realnet/cmd/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/cmd/create.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/cmd/get.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/cmd/info.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/cmd/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/cmd/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:44:14.177601 realnet-0.0.88/realnet/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/core/acl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/core/hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (123)    21596 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/core/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     9290 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/core/type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:44:14.177601 realnet-0.0.88/realnet/provider/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/provider/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:44:14.177601 realnet-0.0.88/realnet/provider/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/provider/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/provider/aws/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:44:14.177601 realnet-0.0.88/realnet/provider/generic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/provider/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/provider/generic/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/provider/generic/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/provider/generic/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:44:14.177601 realnet-0.0.88/realnet/provider/json/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/provider/json/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:44:14.177601 realnet-0.0.88/realnet/provider/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/provider/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/provider/sql/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/provider/sql/init.py
--rw-r--r--   0 runner    (1001) docker     (123)    17851 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/provider/sql/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    12486 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/provider/sql/org.py
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/provider/sql/orgs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:44:14.177601 realnet-0.0.88/realnet/provider/sql/postgres/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/provider/sql/postgres/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11838 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/provider/sql/postgres/item.py
--rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/provider/sql/roles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:44:14.177601 realnet-0.0.88/realnet/provider/sql/sqlite/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/provider/sql/sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/provider/sql/type.py
--rw-r--r--   0 runner    (1001) docker     (123)    15084 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/provider/sql/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:44:14.177601 realnet-0.0.88/realnet/provider/xml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/provider/xml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:44:14.177601 realnet-0.0.88/realnet/provider/yaml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/provider/yaml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/realnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:44:14.177601 realnet-0.0.88/realnet/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/resource/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:44:14.181601 realnet-0.0.88/realnet/resource/accounts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/resource/accounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/resource/accounts/accounts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:44:14.181601 realnet-0.0.88/realnet/resource/apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/resource/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/resource/apps/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:44:14.181601 realnet-0.0.88/realnet/resource/attributes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/resource/attributes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/resource/attributes/attributes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:44:14.181601 realnet-0.0.88/realnet/resource/auths/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/resource/auths/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/resource/auths/auths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:44:14.181601 realnet-0.0.88/realnet/resource/chatgpt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/resource/chatgpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/resource/chatgpt/chatgpt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:44:14.181601 realnet-0.0.88/realnet/resource/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/resource/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/resource/clients/clients.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:44:14.181601 realnet-0.0.88/realnet/resource/ctrls/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/resource/ctrls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/resource/ctrls/ctrls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:44:14.181601 realnet-0.0.88/realnet/resource/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/resource/endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/resource/endpoints/endpoints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:44:14.181601 realnet-0.0.88/realnet/resource/files/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/resource/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/resource/files/files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:44:14.181601 realnet-0.0.88/realnet/resource/forms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/resource/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/resource/forms/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:44:14.181601 realnet-0.0.88/realnet/resource/gltf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/resource/gltf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/resource/gltf/export.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/resource/gltf/gltf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:44:14.181601 realnet-0.0.88/realnet/resource/groups/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/resource/groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/resource/groups/groups.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:44:14.181601 realnet-0.0.88/realnet/resource/items/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/resource/items/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35333 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/resource/items/items.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:44:14.181601 realnet-0.0.88/realnet/resource/login/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/resource/login/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/resource/login/login.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:44:14.181601 realnet-0.0.88/realnet/resource/public/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/resource/public/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/resource/public/public.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:44:14.181601 realnet-0.0.88/realnet/resource/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/resource/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/resource/resources/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:44:14.181601 realnet-0.0.88/realnet/resource/roles/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/resource/roles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/resource/roles/roles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:44:14.181601 realnet-0.0.88/realnet/resource/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/resource/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21652 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/resource/types/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:44:14.181601 realnet-0.0.88/realnet/resource/views/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/resource/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/resource/views/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:44:14.181601 realnet-0.0.88/realnet/runner/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/runner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:44:14.181601 realnet-0.0.88/realnet/runner/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/runner/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/runner/http/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     7670 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/runner/http/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    21120 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/runner/http/router.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/runner/http/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:44:14.181601 realnet-0.0.88/realnet/runner/http/static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/runner/http/static/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:44:14.173601 realnet-0.0.88/realnet/runner/http/static/font-awesome/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:44:14.181601 realnet-0.0.88/realnet/runner/http/static/font-awesome/css/
--rw-r--r--   0 runner    (1001) docker     (123)    37414 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/runner/http/static/font-awesome/css/font-awesome.css
--rw-r--r--   0 runner    (1001) docker     (123)    31000 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/runner/http/static/font-awesome/css/font-awesome.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:44:14.185601 realnet-0.0.88/realnet/runner/http/static/font-awesome/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   134808 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/runner/http/static/font-awesome/fonts/FontAwesome.otf
--rw-r--r--   0 runner    (1001) docker     (123)   165742 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (123)   444379 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (123)   165548 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    98024 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (123)    77160 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:44:14.173601 realnet-0.0.88/realnet/runner/http/static/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:44:14.185601 realnet-0.0.88/realnet/runner/http/static/scripts/ace/
--rw-r--r--   0 runner    (1001) docker     (123)   373401 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/runner/http/static/scripts/ace/ace.js
--rw-r--r--   0 runner    (1001) docker     (123)    13008 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/runner/http/static/scripts/ace/ext-beautify.js
--rw-r--r--   0 runner    (1001) docker     (123)    39778 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/runner/http/static/scripts/ace/ext-language_tools.js
--rw-r--r--   0 runner    (1001) docker     (123)    31853 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/runner/http/static/scripts/ace/mode-css.js
--rw-r--r--   0 runner    (1001) docker     (123)   101769 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/runner/http/static/scripts/ace/mode-html.js
--rw-r--r--   0 runner    (1001) docker     (123)    18573 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/runner/http/static/scripts/ace/mode-javascript.js
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/runner/http/static/scripts/ace/mode-json.js
--rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/runner/http/static/scripts/ace/mode-python.js
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/runner/http/static/scripts/ace/theme-monokai.js
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/runner/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:44:14.185601 realnet-0.0.88/realnet/runner/sqs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/runner/sqs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/runner/sqs/sqs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:44:14.185601 realnet-0.0.88/realnet/shell/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/shell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/shell/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/shell/cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/shell/proto.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/shell/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:44:14.185601 realnet-0.0.88/realnet/static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/static/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:44:14.189601 realnet-0.0.88/realnet/static/initialization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/static/initialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/static/initialization/access.json
--rw-r--r--   0 runner    (1001) docker     (123)    24153 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/static/initialization/apps.json
--rw-r--r--   0 runner    (1001) docker     (123)    13136 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/static/initialization/controls.json
--rw-r--r--   0 runner    (1001) docker     (123)    38721 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/static/initialization/core.json
--rw-r--r--   0 runner    (1001) docker     (123)   115082 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/static/initialization/forms.json
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/static/initialization/geometry.json
--rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/static/initialization/views.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:44:14.189601 realnet-0.0.88/realnet/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10742 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/templates/control.html
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/templates/form.html
--rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/templates/item.html
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/templates/login.html
--rw-r--r--   0 runner    (1001) docker     (123)    16417 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/templates/main.html
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/templates/nav.html
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/templates/register.html
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/templates/register_org.html
--rw-r--r--   0 runner    (1001) docker     (123)    26169 2023-04-21 01:41:30.000000 realnet-0.0.88/realnet/templates/view.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:44:14.177601 realnet-0.0.88/realnet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7492 2023-04-21 01:44:14.000000 realnet-0.0.88/realnet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-04-21 01:44:14.000000 realnet-0.0.88/realnet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 01:44:14.000000 realnet-0.0.88/realnet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-21 01:44:14.000000 realnet-0.0.88/realnet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-21 01:44:14.000000 realnet-0.0.88/realnet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-21 01:44:14.000000 realnet-0.0.88/realnet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 01:44:14.189601 realnet-0.0.88/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-21 01:41:32.000000 realnet-0.0.88/setup.py
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2020-09-11 21:55:22.000000 realnet-0.0.9/
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2020-09-11 21:55:22.000000 realnet-0.0.9/realnet/
+-rw-rw-r--   0 marko     (1000) marko     (1000)      617 2020-09-11 21:54:38.000000 realnet-0.0.9/realnet/realnet.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)      103 2020-09-11 21:54:38.000000 realnet-0.0.9/realnet/type.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)      356 2020-09-11 21:54:38.000000 realnet-0.0.9/realnet/status.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1856 2020-09-11 21:54:38.000000 realnet-0.0.9/realnet/item.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)      717 2020-09-11 21:54:38.000000 realnet-0.0.9/realnet/create.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)      721 2020-09-11 21:54:38.000000 realnet-0.0.9/realnet/import_cmd.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)      121 2020-09-05 02:13:16.000000 realnet-0.0.9/realnet/__main__.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1578 2020-09-07 22:20:34.000000 realnet-0.0.9/realnet/output.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)      324 2020-09-06 22:08:26.000000 realnet-0.0.9/realnet/auth.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)      273 2020-09-06 22:08:26.000000 realnet-0.0.9/realnet/logout.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)      473 2020-09-11 21:54:38.000000 realnet-0.0.9/realnet/test.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1636 2020-09-11 21:54:38.000000 realnet-0.0.9/realnet/runner.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)      938 2020-09-11 21:54:38.000000 realnet-0.0.9/realnet/realnet_command.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)        0 2020-09-11 21:54:38.000000 realnet-0.0.9/realnet/bash.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)      475 2020-09-11 21:54:38.000000 realnet-0.0.9/realnet/input.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1513 2020-09-11 21:54:38.000000 realnet-0.0.9/realnet/get.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)      432 2020-09-11 21:54:38.000000 realnet-0.0.9/realnet/delete.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)        0 2020-09-11 21:54:38.000000 realnet-0.0.9/realnet/__init__.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1753 2020-09-11 21:54:38.000000 realnet-0.0.9/realnet/put.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)      270 2020-09-11 21:54:38.000000 realnet-0.0.9/realnet/login.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)      686 2020-09-11 21:54:38.000000 realnet-0.0.9/realnet/export.py
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2020-09-11 21:55:22.000000 realnet-0.0.9/realnet.egg-info/
+-rw-rw-r--   0 marko     (1000) marko     (1000)      584 2020-09-11 21:55:22.000000 realnet-0.0.9/realnet.egg-info/SOURCES.txt
+-rw-rw-r--   0 marko     (1000) marko     (1000)        1 2020-09-11 21:55:22.000000 realnet-0.0.9/realnet.egg-info/dependency_links.txt
+-rw-rw-r--   0 marko     (1000) marko     (1000)        8 2020-09-11 21:55:22.000000 realnet-0.0.9/realnet.egg-info/top_level.txt
+-rw-rw-r--   0 marko     (1000) marko     (1000)       51 2020-09-11 21:55:22.000000 realnet-0.0.9/realnet.egg-info/entry_points.txt
+-rw-rw-r--   0 marko     (1000) marko     (1000)       75 2020-09-11 21:55:22.000000 realnet-0.0.9/realnet.egg-info/requires.txt
+-rw-rw-r--   0 marko     (1000) marko     (1000)      448 2020-09-11 21:55:22.000000 realnet-0.0.9/realnet.egg-info/PKG-INFO
+-rw-rw-r--   0 marko     (1000) marko     (1000)        9 2020-09-04 11:15:07.000000 realnet-0.0.9/README.md
+-rw-rw-r--   0 marko     (1000) marko     (1000)       38 2020-09-11 21:55:22.000000 realnet-0.0.9/setup.cfg
+-rw-rw-r--   0 marko     (1000) marko     (1000)      448 2020-09-11 21:55:22.000000 realnet-0.0.9/PKG-INFO
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1138 2020-09-11 21:54:38.000000 realnet-0.0.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

