# Comparing `tmp/dockertown-0.2.0.tar.gz` & `tmp/dockertown-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dockertown-0.2.0.tar", last modified: Thu Apr 20 14:39:31 2023, max compression
+gzip compressed data, was "dockertown-0.2.1.tar", last modified: Thu Apr 20 15:13:04 2023, max compression
```

## Comparing `dockertown-0.2.0.tar` & `dockertown-0.2.1.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:39:31.985714 dockertown-0.2.0/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2475 2023-04-19 19:49:15.000000 dockertown-0.2.0/CONTRIBUTING.md
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1087 2023-04-19 19:49:15.000000 dockertown-0.2.0/LICENSE
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       67 2023-04-19 19:49:15.000000 dockertown-0.2.0/MANIFEST.in
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    14716 2023-04-20 14:39:31.985714 dockertown-0.2.0/PKG-INFO
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    14262 2023-04-19 19:49:15.000000 dockertown-0.2.0/README.md
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:39:31.977713 dockertown-0.2.0/docs/
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:39:31.977713 dockertown-0.2.0/docs/template/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4929 2023-04-19 19:49:15.000000 dockertown-0.2.0/docs/template/docker_client.md
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:39:31.977713 dockertown-0.2.0/docs/template/docker_objects/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      692 2023-04-19 19:49:15.000000 dockertown-0.2.0/docs/template/docker_objects/builders.md
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1078 2023-04-19 19:49:15.000000 dockertown-0.2.0/docs/template/docker_objects/configs.md
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1042 2023-04-19 19:49:15.000000 dockertown-0.2.0/docs/template/docker_objects/containers.md
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1249 2023-04-19 19:49:15.000000 dockertown-0.2.0/docs/template/docker_objects/images.md
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1180 2023-04-19 19:49:15.000000 dockertown-0.2.0/docs/template/docker_objects/networks.md
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      966 2023-04-19 19:49:15.000000 dockertown-0.2.0/docs/template/docker_objects/nodes.md
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1037 2023-04-19 19:49:15.000000 dockertown-0.2.0/docs/template/docker_objects/plugins.md
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1108 2023-04-19 19:49:15.000000 dockertown-0.2.0/docs/template/docker_objects/services.md
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      689 2023-04-19 19:49:15.000000 dockertown-0.2.0/docs/template/docker_objects/tasks.md
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1103 2023-04-19 19:49:15.000000 dockertown-0.2.0/docs/template/docker_objects/volumes.md
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:39:31.981713 dockertown-0.2.0/docs/template/sub-commands/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1279 2023-04-19 19:49:15.000000 dockertown-0.2.0/docs/template/sub-commands/buildx.md
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2097 2023-04-19 19:49:15.000000 dockertown-0.2.0/docs/template/sub-commands/compose.md
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1559 2023-04-19 19:49:15.000000 dockertown-0.2.0/docs/template/sub-commands/context.md
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:39:31.981713 dockertown-0.2.0/docs/template/user_guide/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3711 2023-04-19 19:49:15.000000 dockertown-0.2.0/docs/template/user_guide/docker_run.md
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      961 2023-04-19 19:49:15.000000 dockertown-0.2.0/docs/template/user_guide/exceptions.md
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     6442 2023-04-19 19:49:15.000000 dockertown-0.2.0/docs/template/user_guide/generic_resources.md
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3364 2023-04-19 19:49:15.000000 dockertown-0.2.0/docs/template/user_guide/running_inside_a_container.md
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       42 2023-04-19 19:49:15.000000 dockertown-0.2.0/lint-requirements.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       59 2023-04-19 19:49:15.000000 dockertown-0.2.0/requirements.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       38 2023-04-20 14:39:31.985714 dockertown-0.2.0/setup.cfg
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1022 2023-04-20 14:39:24.000000 dockertown-0.2.0/setup.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:39:31.977713 dockertown-0.2.0/src/
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:39:31.981713 dockertown-0.2.0/src/dockertown/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1332 2023-04-20 14:39:24.000000 dockertown-0.2.0/src/dockertown/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     9429 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/client_config.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1452 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/command_line_entrypoint.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:39:31.981713 dockertown-0.2.0/src/dockertown/components/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/__init__.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:39:31.981713 dockertown-0.2.0/src/dockertown/components/buildx/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/buildx/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    23517 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/buildx/cli_wrapper.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:39:31.981713 dockertown-0.2.0/src/dockertown/components/buildx/imagetools/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/buildx/imagetools/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2892 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/buildx/imagetools/cli_wrapper.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1364 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/buildx/imagetools/models.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1016 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/buildx/models.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:39:31.981713 dockertown-0.2.0/src/dockertown/components/compose/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/compose/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    31127 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/compose/cli_wrapper.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2918 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/compose/models.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:39:31.981713 dockertown-0.2.0/src/dockertown/components/config/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/config/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4775 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/config/cli_wrapper.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      601 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/config/models.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:39:31.981713 dockertown-0.2.0/src/dockertown/components/container/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/container/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    73220 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/container/cli_wrapper.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     7450 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/container/models.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:39:31.981713 dockertown-0.2.0/src/dockertown/components/context/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/context/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     7724 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/context/cli_wrapper.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      542 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/context/models.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:39:31.981713 dockertown-0.2.0/src/dockertown/components/image/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/image/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    23635 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/image/cli_wrapper.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1043 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/image/models.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:39:31.981713 dockertown-0.2.0/src/dockertown/components/manifest/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/manifest/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     5089 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/manifest/cli_wrapper.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      346 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/manifest/models.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:39:31.981713 dockertown-0.2.0/src/dockertown/components/network/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/network/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     7548 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/network/cli_wrapper.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      820 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/network/models.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:39:31.981713 dockertown-0.2.0/src/dockertown/components/node/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/node/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     7452 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/node/cli_wrapper.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2176 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/node/models.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:39:31.981713 dockertown-0.2.0/src/dockertown/components/plugin/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/plugin/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     9428 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/plugin/cli_wrapper.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      879 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/plugin/models.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:39:31.981713 dockertown-0.2.0/src/dockertown/components/secret/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/secret/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3307 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/secret/cli_wrapper.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      253 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/secret/models.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:39:31.981713 dockertown-0.2.0/src/dockertown/components/service/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/service/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    16688 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/service/cli_wrapper.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2193 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/service/models.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:39:31.981713 dockertown-0.2.0/src/dockertown/components/stack/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/stack/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     5523 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/stack/cli_wrapper.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:39:31.981713 dockertown-0.2.0/src/dockertown/components/swarm/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/swarm/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     9219 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/swarm/cli_wrapper.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:39:31.981713 dockertown-0.2.0/src/dockertown/components/system/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/system/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     6413 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/system/cli_wrapper.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     5429 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/system/models.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:39:31.985714 dockertown-0.2.0/src/dockertown/components/task/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/task/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3195 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/task/cli_wrapper.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3811 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/task/models.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:39:31.985714 dockertown-0.2.0/src/dockertown/components/trust/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/trust/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      486 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/trust/cli_wrapper.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:39:31.985714 dockertown-0.2.0/src/dockertown/components/volume/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/volume/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    10346 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/volume/cli_wrapper.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      385 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/volume/models.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    12100 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/docker_client.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4364 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/download_binaries.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1807 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/exceptions.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       69 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/py.typed
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      710 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/test_utils.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    11071 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/utils.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:39:31.981713 dockertown-0.2.0/src/dockertown.egg-info/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    14716 2023-04-20 14:39:31.000000 dockertown-0.2.0/src/dockertown.egg-info/PKG-INFO
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3882 2023-04-20 14:39:31.000000 dockertown-0.2.0/src/dockertown.egg-info/SOURCES.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2023-04-20 14:39:31.000000 dockertown-0.2.0/src/dockertown.egg-info/dependency_links.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       72 2023-04-20 14:39:31.000000 dockertown-0.2.0/src/dockertown.egg-info/entry_points.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       59 2023-04-20 14:39:31.000000 dockertown-0.2.0/src/dockertown.egg-info/requires.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       11 2023-04-20 14:39:31.000000 dockertown-0.2.0/src/dockertown.egg-info/top_level.txt
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:39:31.985714 dockertown-0.2.0/tests/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       29 2023-04-19 19:49:15.000000 dockertown-0.2.0/tests/test-requirements.txt
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 15:13:04.302507 dockertown-0.2.1/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2475 2023-04-19 19:49:15.000000 dockertown-0.2.1/CONTRIBUTING.md
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1087 2023-04-19 19:49:15.000000 dockertown-0.2.1/LICENSE
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       67 2023-04-19 19:49:15.000000 dockertown-0.2.1/MANIFEST.in
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    14716 2023-04-20 15:13:04.298507 dockertown-0.2.1/PKG-INFO
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    14262 2023-04-19 19:49:15.000000 dockertown-0.2.1/README.md
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 15:13:04.294507 dockertown-0.2.1/docs/
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 15:13:04.294507 dockertown-0.2.1/docs/template/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4929 2023-04-19 19:49:15.000000 dockertown-0.2.1/docs/template/docker_client.md
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 15:13:04.294507 dockertown-0.2.1/docs/template/docker_objects/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      692 2023-04-19 19:49:15.000000 dockertown-0.2.1/docs/template/docker_objects/builders.md
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1078 2023-04-19 19:49:15.000000 dockertown-0.2.1/docs/template/docker_objects/configs.md
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1042 2023-04-19 19:49:15.000000 dockertown-0.2.1/docs/template/docker_objects/containers.md
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1249 2023-04-19 19:49:15.000000 dockertown-0.2.1/docs/template/docker_objects/images.md
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1180 2023-04-19 19:49:15.000000 dockertown-0.2.1/docs/template/docker_objects/networks.md
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      966 2023-04-19 19:49:15.000000 dockertown-0.2.1/docs/template/docker_objects/nodes.md
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1037 2023-04-19 19:49:15.000000 dockertown-0.2.1/docs/template/docker_objects/plugins.md
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1108 2023-04-19 19:49:15.000000 dockertown-0.2.1/docs/template/docker_objects/services.md
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      689 2023-04-19 19:49:15.000000 dockertown-0.2.1/docs/template/docker_objects/tasks.md
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1103 2023-04-19 19:49:15.000000 dockertown-0.2.1/docs/template/docker_objects/volumes.md
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 15:13:04.294507 dockertown-0.2.1/docs/template/sub-commands/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1279 2023-04-19 19:49:15.000000 dockertown-0.2.1/docs/template/sub-commands/buildx.md
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2097 2023-04-19 19:49:15.000000 dockertown-0.2.1/docs/template/sub-commands/compose.md
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1559 2023-04-19 19:49:15.000000 dockertown-0.2.1/docs/template/sub-commands/context.md
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 15:13:04.298507 dockertown-0.2.1/docs/template/user_guide/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3711 2023-04-19 19:49:15.000000 dockertown-0.2.1/docs/template/user_guide/docker_run.md
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      961 2023-04-19 19:49:15.000000 dockertown-0.2.1/docs/template/user_guide/exceptions.md
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     6442 2023-04-19 19:49:15.000000 dockertown-0.2.1/docs/template/user_guide/generic_resources.md
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3364 2023-04-19 19:49:15.000000 dockertown-0.2.1/docs/template/user_guide/running_inside_a_container.md
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       42 2023-04-19 19:49:15.000000 dockertown-0.2.1/lint-requirements.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       73 2023-04-20 15:09:42.000000 dockertown-0.2.1/requirements.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       38 2023-04-20 15:13:04.302507 dockertown-0.2.1/setup.cfg
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1022 2023-04-20 15:13:02.000000 dockertown-0.2.1/setup.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 15:13:04.294507 dockertown-0.2.1/src/
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 15:13:04.298507 dockertown-0.2.1/src/dockertown/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1332 2023-04-20 15:13:02.000000 dockertown-0.2.1/src/dockertown/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     9429 2023-04-19 19:49:15.000000 dockertown-0.2.1/src/dockertown/client_config.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1452 2023-04-19 19:49:15.000000 dockertown-0.2.1/src/dockertown/command_line_entrypoint.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 15:13:04.298507 dockertown-0.2.1/src/dockertown/components/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.1/src/dockertown/components/__init__.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 15:13:04.298507 dockertown-0.2.1/src/dockertown/components/buildx/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.1/src/dockertown/components/buildx/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    23517 2023-04-19 19:49:15.000000 dockertown-0.2.1/src/dockertown/components/buildx/cli_wrapper.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 15:13:04.298507 dockertown-0.2.1/src/dockertown/components/buildx/imagetools/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.1/src/dockertown/components/buildx/imagetools/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2892 2023-04-19 19:49:15.000000 dockertown-0.2.1/src/dockertown/components/buildx/imagetools/cli_wrapper.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1364 2023-04-19 19:49:15.000000 dockertown-0.2.1/src/dockertown/components/buildx/imagetools/models.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1016 2023-04-19 19:49:15.000000 dockertown-0.2.1/src/dockertown/components/buildx/models.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 15:13:04.298507 dockertown-0.2.1/src/dockertown/components/compose/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.1/src/dockertown/components/compose/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    31127 2023-04-19 19:49:15.000000 dockertown-0.2.1/src/dockertown/components/compose/cli_wrapper.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2918 2023-04-19 19:49:15.000000 dockertown-0.2.1/src/dockertown/components/compose/models.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 15:13:04.298507 dockertown-0.2.1/src/dockertown/components/config/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.1/src/dockertown/components/config/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4775 2023-04-19 19:49:15.000000 dockertown-0.2.1/src/dockertown/components/config/cli_wrapper.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      601 2023-04-19 19:49:15.000000 dockertown-0.2.1/src/dockertown/components/config/models.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 15:13:04.298507 dockertown-0.2.1/src/dockertown/components/container/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.1/src/dockertown/components/container/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    73220 2023-04-19 19:49:15.000000 dockertown-0.2.1/src/dockertown/components/container/cli_wrapper.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     7450 2023-04-19 19:49:15.000000 dockertown-0.2.1/src/dockertown/components/container/models.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 15:13:04.298507 dockertown-0.2.1/src/dockertown/components/context/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.1/src/dockertown/components/context/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     7724 2023-04-19 19:49:15.000000 dockertown-0.2.1/src/dockertown/components/context/cli_wrapper.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      542 2023-04-19 19:49:15.000000 dockertown-0.2.1/src/dockertown/components/context/models.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 15:13:04.298507 dockertown-0.2.1/src/dockertown/components/image/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.1/src/dockertown/components/image/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    23925 2023-04-20 15:12:46.000000 dockertown-0.2.1/src/dockertown/components/image/cli_wrapper.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1651 2023-04-20 15:10:29.000000 dockertown-0.2.1/src/dockertown/components/image/models.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 15:13:04.298507 dockertown-0.2.1/src/dockertown/components/manifest/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.1/src/dockertown/components/manifest/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     5089 2023-04-19 19:49:15.000000 dockertown-0.2.1/src/dockertown/components/manifest/cli_wrapper.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      346 2023-04-19 19:49:15.000000 dockertown-0.2.1/src/dockertown/components/manifest/models.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 15:13:04.298507 dockertown-0.2.1/src/dockertown/components/network/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.1/src/dockertown/components/network/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     7548 2023-04-19 19:49:15.000000 dockertown-0.2.1/src/dockertown/components/network/cli_wrapper.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      820 2023-04-19 19:49:15.000000 dockertown-0.2.1/src/dockertown/components/network/models.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 15:13:04.298507 dockertown-0.2.1/src/dockertown/components/node/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.1/src/dockertown/components/node/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     7452 2023-04-19 19:49:15.000000 dockertown-0.2.1/src/dockertown/components/node/cli_wrapper.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2176 2023-04-19 19:49:15.000000 dockertown-0.2.1/src/dockertown/components/node/models.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 15:13:04.298507 dockertown-0.2.1/src/dockertown/components/plugin/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.1/src/dockertown/components/plugin/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     9428 2023-04-19 19:49:15.000000 dockertown-0.2.1/src/dockertown/components/plugin/cli_wrapper.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      879 2023-04-19 19:49:15.000000 dockertown-0.2.1/src/dockertown/components/plugin/models.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 15:13:04.298507 dockertown-0.2.1/src/dockertown/components/secret/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.1/src/dockertown/components/secret/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3307 2023-04-19 19:49:15.000000 dockertown-0.2.1/src/dockertown/components/secret/cli_wrapper.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      253 2023-04-19 19:49:15.000000 dockertown-0.2.1/src/dockertown/components/secret/models.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 15:13:04.298507 dockertown-0.2.1/src/dockertown/components/service/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.1/src/dockertown/components/service/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    16688 2023-04-19 19:49:15.000000 dockertown-0.2.1/src/dockertown/components/service/cli_wrapper.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2193 2023-04-19 19:49:15.000000 dockertown-0.2.1/src/dockertown/components/service/models.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 15:13:04.298507 dockertown-0.2.1/src/dockertown/components/stack/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.1/src/dockertown/components/stack/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     5523 2023-04-19 19:49:15.000000 dockertown-0.2.1/src/dockertown/components/stack/cli_wrapper.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 15:13:04.298507 dockertown-0.2.1/src/dockertown/components/swarm/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.1/src/dockertown/components/swarm/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     9219 2023-04-19 19:49:15.000000 dockertown-0.2.1/src/dockertown/components/swarm/cli_wrapper.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 15:13:04.298507 dockertown-0.2.1/src/dockertown/components/system/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.1/src/dockertown/components/system/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     6413 2023-04-19 19:49:15.000000 dockertown-0.2.1/src/dockertown/components/system/cli_wrapper.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     5429 2023-04-19 19:49:15.000000 dockertown-0.2.1/src/dockertown/components/system/models.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 15:13:04.298507 dockertown-0.2.1/src/dockertown/components/task/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.1/src/dockertown/components/task/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3195 2023-04-19 19:49:15.000000 dockertown-0.2.1/src/dockertown/components/task/cli_wrapper.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3811 2023-04-19 19:49:15.000000 dockertown-0.2.1/src/dockertown/components/task/models.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 15:13:04.298507 dockertown-0.2.1/src/dockertown/components/trust/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.1/src/dockertown/components/trust/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      486 2023-04-19 19:49:15.000000 dockertown-0.2.1/src/dockertown/components/trust/cli_wrapper.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 15:13:04.298507 dockertown-0.2.1/src/dockertown/components/volume/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.1/src/dockertown/components/volume/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    10346 2023-04-19 19:49:15.000000 dockertown-0.2.1/src/dockertown/components/volume/cli_wrapper.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      385 2023-04-19 19:49:15.000000 dockertown-0.2.1/src/dockertown/components/volume/models.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    12100 2023-04-19 19:49:15.000000 dockertown-0.2.1/src/dockertown/docker_client.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4364 2023-04-19 19:49:15.000000 dockertown-0.2.1/src/dockertown/download_binaries.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1807 2023-04-19 19:49:15.000000 dockertown-0.2.1/src/dockertown/exceptions.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       69 2023-04-19 19:49:15.000000 dockertown-0.2.1/src/dockertown/py.typed
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      710 2023-04-19 19:49:15.000000 dockertown-0.2.1/src/dockertown/test_utils.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    11071 2023-04-19 19:49:15.000000 dockertown-0.2.1/src/dockertown/utils.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 15:13:04.298507 dockertown-0.2.1/src/dockertown.egg-info/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    14716 2023-04-20 15:13:04.000000 dockertown-0.2.1/src/dockertown.egg-info/PKG-INFO
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3882 2023-04-20 15:13:04.000000 dockertown-0.2.1/src/dockertown.egg-info/SOURCES.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2023-04-20 15:13:04.000000 dockertown-0.2.1/src/dockertown.egg-info/dependency_links.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       72 2023-04-20 15:13:04.000000 dockertown-0.2.1/src/dockertown.egg-info/entry_points.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       73 2023-04-20 15:13:04.000000 dockertown-0.2.1/src/dockertown.egg-info/requires.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       11 2023-04-20 15:13:04.000000 dockertown-0.2.1/src/dockertown.egg-info/top_level.txt
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 15:13:04.298507 dockertown-0.2.1/tests/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       29 2023-04-19 19:49:15.000000 dockertown-0.2.1/tests/test-requirements.txt
```

### Comparing `dockertown-0.2.0/CONTRIBUTING.md` & `dockertown-0.2.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.0/LICENSE` & `dockertown-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.0/PKG-INFO` & `dockertown-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dockertown
-Version: 0.2.0
+Version: 0.2.1
 Summary: A decent Python wrapper for Docker CLI
 Home-page: UNKNOWN
 License: MIT
 Project-URL: Documentation, https://duckietown.github.io/dockertown/
 Project-URL: Source Code, https://github.com/duckietown/dockertown
 Project-URL: Bug Tracker, https://github.com/duckietown/dockertown/issues
 Platform: UNKNOWN
```

### Comparing `dockertown-0.2.0/README.md` & `dockertown-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.0/docs/template/docker_client.md` & `dockertown-0.2.1/docs/template/docker_client.md`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.0/docs/template/docker_objects/builders.md` & `dockertown-0.2.1/docs/template/docker_objects/builders.md`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.0/docs/template/docker_objects/configs.md` & `dockertown-0.2.1/docs/template/docker_objects/configs.md`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.0/docs/template/docker_objects/containers.md` & `dockertown-0.2.1/docs/template/docker_objects/containers.md`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.0/docs/template/docker_objects/images.md` & `dockertown-0.2.1/docs/template/docker_objects/images.md`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.0/docs/template/docker_objects/networks.md` & `dockertown-0.2.1/docs/template/docker_objects/networks.md`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.0/docs/template/docker_objects/nodes.md` & `dockertown-0.2.1/docs/template/docker_objects/nodes.md`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.0/docs/template/docker_objects/plugins.md` & `dockertown-0.2.1/docs/template/docker_objects/plugins.md`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.0/docs/template/docker_objects/services.md` & `dockertown-0.2.1/docs/template/docker_objects/services.md`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.0/docs/template/docker_objects/tasks.md` & `dockertown-0.2.1/docs/template/docker_objects/tasks.md`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.0/docs/template/docker_objects/volumes.md` & `dockertown-0.2.1/docs/template/docker_objects/volumes.md`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.0/docs/template/sub-commands/buildx.md` & `dockertown-0.2.1/docs/template/sub-commands/buildx.md`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.0/docs/template/sub-commands/compose.md` & `dockertown-0.2.1/docs/template/sub-commands/compose.md`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.0/docs/template/sub-commands/context.md` & `dockertown-0.2.1/docs/template/sub-commands/context.md`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.0/docs/template/user_guide/docker_run.md` & `dockertown-0.2.1/docs/template/user_guide/docker_run.md`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.0/docs/template/user_guide/exceptions.md` & `dockertown-0.2.1/docs/template/user_guide/exceptions.md`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.0/docs/template/user_guide/generic_resources.md` & `dockertown-0.2.1/docs/template/user_guide/generic_resources.md`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.0/docs/template/user_guide/running_inside_a_container.md` & `dockertown-0.2.1/docs/template/user_guide/running_inside_a_container.md`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.0/setup.py` & `dockertown-0.2.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 def get_long_description() -> str:
     return (CURRENT_DIR / "README.md").read_text(encoding="utf8")
 
 
 setup(
     name="dockertown",
-    version="0.2.0",
+    version="0.2.1",
     description="A decent Python wrapper for Docker CLI",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     install_requires=(CURRENT_DIR / "requirements.txt").read_text().splitlines(),
     packages=find_packages("src"),
     package_dir={"": "src"},
     include_package_data=True,  # will read the MANIFEST.in
```

### Comparing `dockertown-0.2.0/src/dockertown/__init__.py` & `dockertown-0.2.1/src/dockertown/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 
 from .client_config import ClientNotFoundError
 from .components.buildx.cli_wrapper import Builder
 from .components.config.cli_wrapper import Config
 from .components.container.cli_wrapper import Container, ContainerStats
 from .components.context.cli_wrapper import (
     Context,
```

### Comparing `dockertown-0.2.0/src/dockertown/client_config.py` & `dockertown-0.2.1/src/dockertown/client_config.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.0/src/dockertown/command_line_entrypoint.py` & `dockertown-0.2.1/src/dockertown/command_line_entrypoint.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.0/src/dockertown/components/buildx/cli_wrapper.py` & `dockertown-0.2.1/src/dockertown/components/buildx/cli_wrapper.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.0/src/dockertown/components/buildx/imagetools/cli_wrapper.py` & `dockertown-0.2.1/src/dockertown/components/buildx/imagetools/cli_wrapper.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.0/src/dockertown/components/buildx/imagetools/models.py` & `dockertown-0.2.1/src/dockertown/components/buildx/imagetools/models.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.0/src/dockertown/components/buildx/models.py` & `dockertown-0.2.1/src/dockertown/components/buildx/models.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.0/src/dockertown/components/compose/cli_wrapper.py` & `dockertown-0.2.1/src/dockertown/components/compose/cli_wrapper.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.0/src/dockertown/components/compose/models.py` & `dockertown-0.2.1/src/dockertown/components/compose/models.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.0/src/dockertown/components/config/cli_wrapper.py` & `dockertown-0.2.1/src/dockertown/components/config/cli_wrapper.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.0/src/dockertown/components/config/models.py` & `dockertown-0.2.1/src/dockertown/components/config/models.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.0/src/dockertown/components/container/cli_wrapper.py` & `dockertown-0.2.1/src/dockertown/components/container/cli_wrapper.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.0/src/dockertown/components/container/models.py` & `dockertown-0.2.1/src/dockertown/components/container/models.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.0/src/dockertown/components/context/cli_wrapper.py` & `dockertown-0.2.1/src/dockertown/components/context/cli_wrapper.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.0/src/dockertown/components/context/models.py` & `dockertown-0.2.1/src/dockertown/components/context/models.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.0/src/dockertown/components/image/cli_wrapper.py` & `dockertown-0.2.1/src/dockertown/components/image/cli_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from ...utils import (
     ValidPath,
     format_dict_for_cli,
     run,
     stream_stdout_and_stderr,
     to_list,
 )
-from .models import ImageGraphDriver, ImageInspectResult, ImageRootFS
+from .models import ImageGraphDriver, ImageInspectResult, ImageRootFS, ImageHistoryLayer
 
 
 class Image(ReloadableObjectFromJson):
     def __init__(
         self, client_config: ClientConfig, reference: str, is_immutable_id=False
     ):
         super().__init__(client_config, "id", reference, is_immutable_id)
@@ -262,17 +262,22 @@
         full_cmd.add_args_list("--tag", tags)
 
         docker_image = ImageCLI(self.client_config)
         full_cmd.append(context_path)
         image_id = run(full_cmd).splitlines()[-1].strip()
         return docker_image.inspect(image_id)
 
-    def history(self):
+    def history(self, x: str) -> List[ImageHistoryLayer]:
         """Not yet implemented"""
-        raise NotImplementedError
+        full_cmd = self.docker_cmd + ["history", "--no-trunc", "--format", "{{json .}}", x]
+        history: List[ImageHistoryLayer] = [
+            ImageHistoryLayer.parse_json(layer)
+            for layer in run(full_cmd).splitlines()
+        ]
+        return history
 
     def import_(
         self,
         source: ValidPath,
         tag: Optional[str] = None,
         changes: List[str] = [],
         message: Optional[str] = None,
```

### Comparing `dockertown-0.2.0/src/dockertown/components/manifest/cli_wrapper.py` & `dockertown-0.2.1/src/dockertown/components/manifest/cli_wrapper.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.0/src/dockertown/components/network/cli_wrapper.py` & `dockertown-0.2.1/src/dockertown/components/network/cli_wrapper.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.0/src/dockertown/components/network/models.py` & `dockertown-0.2.1/src/dockertown/components/network/models.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.0/src/dockertown/components/node/cli_wrapper.py` & `dockertown-0.2.1/src/dockertown/components/node/cli_wrapper.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.0/src/dockertown/components/node/models.py` & `dockertown-0.2.1/src/dockertown/components/node/models.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.0/src/dockertown/components/plugin/cli_wrapper.py` & `dockertown-0.2.1/src/dockertown/components/plugin/cli_wrapper.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.0/src/dockertown/components/plugin/models.py` & `dockertown-0.2.1/src/dockertown/components/plugin/models.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.0/src/dockertown/components/secret/cli_wrapper.py` & `dockertown-0.2.1/src/dockertown/components/secret/cli_wrapper.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.0/src/dockertown/components/service/cli_wrapper.py` & `dockertown-0.2.1/src/dockertown/components/service/cli_wrapper.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.0/src/dockertown/components/service/models.py` & `dockertown-0.2.1/src/dockertown/components/service/models.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.0/src/dockertown/components/stack/cli_wrapper.py` & `dockertown-0.2.1/src/dockertown/components/stack/cli_wrapper.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.0/src/dockertown/components/swarm/cli_wrapper.py` & `dockertown-0.2.1/src/dockertown/components/swarm/cli_wrapper.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.0/src/dockertown/components/system/cli_wrapper.py` & `dockertown-0.2.1/src/dockertown/components/system/cli_wrapper.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.0/src/dockertown/components/system/models.py` & `dockertown-0.2.1/src/dockertown/components/system/models.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.0/src/dockertown/components/task/cli_wrapper.py` & `dockertown-0.2.1/src/dockertown/components/task/cli_wrapper.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.0/src/dockertown/components/task/models.py` & `dockertown-0.2.1/src/dockertown/components/task/models.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.0/src/dockertown/components/volume/cli_wrapper.py` & `dockertown-0.2.1/src/dockertown/components/volume/cli_wrapper.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.0/src/dockertown/docker_client.py` & `dockertown-0.2.1/src/dockertown/docker_client.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.0/src/dockertown/download_binaries.py` & `dockertown-0.2.1/src/dockertown/download_binaries.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.0/src/dockertown/exceptions.py` & `dockertown-0.2.1/src/dockertown/exceptions.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.0/src/dockertown/test_utils.py` & `dockertown-0.2.1/src/dockertown/test_utils.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.0/src/dockertown/utils.py` & `dockertown-0.2.1/src/dockertown/utils.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.0/src/dockertown.egg-info/PKG-INFO` & `dockertown-0.2.1/src/dockertown.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dockertown
-Version: 0.2.0
+Version: 0.2.1
 Summary: A decent Python wrapper for Docker CLI
 Home-page: UNKNOWN
 License: MIT
 Project-URL: Documentation, https://duckietown.github.io/dockertown/
 Project-URL: Source Code, https://github.com/duckietown/dockertown
 Project-URL: Bug Tracker, https://github.com/duckietown/dockertown/issues
 Platform: UNKNOWN
```

### Comparing `dockertown-0.2.0/src/dockertown.egg-info/SOURCES.txt` & `dockertown-0.2.1/src/dockertown.egg-info/SOURCES.txt`

 * *Files identical despite different names*

