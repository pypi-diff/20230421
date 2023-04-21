# Comparing `tmp/kraken_std-0.8.5.tar.gz` & `tmp/kraken_std-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kraken_std-0.8.5.tar", max compression
+gzip compressed data, was "kraken_std-0.8.6.tar", max compression
```

## Comparing `kraken_std-0.8.5.tar` & `kraken_std-0.8.6.tar`

### file list

```diff
@@ -1,81 +1,81 @@
--rw-r--r--   0        0        0      988 2023-01-22 14:38:01.549959 kraken_std-0.8.5/LICENSE
--rw-r--r--   0        0        0     1745 2023-04-19 15:41:46.082711 kraken_std-0.8.5/pyproject.toml
--rw-r--r--   0        0        0     1498 2023-02-08 16:53:28.240291 kraken_std-0.8.5/readme.md
--rw-r--r--   0        0        0       22 2023-04-19 15:41:46.086711 kraken_std-0.8.5/src/kraken/std/__init__.py
--rw-r--r--   0        0        0    13390 2023-04-06 12:43:19.047013 kraken_std-0.8.5/src/kraken/std/cargo/__init__.py
--rw-r--r--   0        0        0     2403 2023-01-22 14:38:01.549959 kraken_std-0.8.5/src/kraken/std/cargo/config.py
--rw-r--r--   0        0        0     1753 2023-01-22 14:38:01.549959 kraken_std-0.8.5/src/kraken/std/cargo/data/certs/cert.pem
--rw-r--r--   0        0        0     3243 2023-01-22 14:38:01.549959 kraken_std-0.8.5/src/kraken/std/cargo/data/certs/key.pem
--rw-r--r--   0        0        0     7912 2023-04-05 21:42:55.754805 kraken_std-0.8.5/src/kraken/std/cargo/manifest.py
--rw-r--r--   0        0        0     2294 2023-01-22 14:38:01.549959 kraken_std-0.8.5/src/kraken/std/cargo/mitm.py
--rw-r--r--   0        0        0     1737 2023-01-22 14:38:01.549959 kraken_std-0.8.5/src/kraken/std/cargo/mitm_impl.py
--rw-r--r--   0        0        0        0 2023-03-06 13:53:50.490907 kraken_std-0.8.5/src/kraken/std/cargo/tasks/__init__.py
--rw-r--r--   0        0        0     5640 2023-03-20 14:35:25.194513 kraken_std-0.8.5/src/kraken/std/cargo/tasks/cargo_auth_proxy_task.py
--rw-r--r--   0        0        0     5959 2023-04-19 15:08:11.413164 kraken_std-0.8.5/src/kraken/std/cargo/tasks/cargo_build_task.py
--rw-r--r--   0        0        0     3163 2023-04-05 21:42:55.754805 kraken_std-0.8.5/src/kraken/std/cargo/tasks/cargo_bump_version_task.py
--rw-r--r--   0        0        0     2177 2023-03-20 14:35:25.194513 kraken_std-0.8.5/src/kraken/std/cargo/tasks/cargo_check_toolchain_version.py
--rw-r--r--   0        0        0      907 2023-01-22 14:38:01.549959 kraken_std-0.8.5/src/kraken/std/cargo/tasks/cargo_clippy_task.py
--rw-r--r--   0        0        0      732 2023-04-19 15:08:11.413164 kraken_std-0.8.5/src/kraken/std/cargo/tasks/cargo_deny_task.py
--rw-r--r--   0        0        0      730 2023-01-22 14:38:01.549959 kraken_std-0.8.5/src/kraken/std/cargo/tasks/cargo_fmt_task.py
--rw-r--r--   0        0        0     2074 2023-01-22 14:38:01.549959 kraken_std-0.8.5/src/kraken/std/cargo/tasks/cargo_publish_task.py
--rw-r--r--   0        0        0     2088 2023-01-22 14:38:01.549959 kraken_std-0.8.5/src/kraken/std/cargo/tasks/cargo_sync_config_task.py
--rw-r--r--   0        0        0      493 2023-01-22 14:38:01.549959 kraken_std-0.8.5/src/kraken/std/cargo/tasks/cargo_test_task.py
--rw-r--r--   0        0        0      391 2023-02-14 17:29:44.373684 kraken_std-0.8.5/src/kraken/std/cargo/tasks/cargo_update_task.py
--rw-r--r--   0        0        0      720 2023-03-06 13:53:50.490907 kraken_std-0.8.5/src/kraken/std/cargo/version.py
--rw-r--r--   0        0        0        0 2023-03-06 13:53:50.490907 kraken_std-0.8.5/src/kraken/std/descriptors/__init__.py
--rw-r--r--   0        0        0      874 2023-01-22 14:38:01.549959 kraken_std-0.8.5/src/kraken/std/descriptors/resource.py
--rw-r--r--   0        0        0    10002 2023-01-22 14:38:01.549959 kraken_std-0.8.5/src/kraken/std/dist.py
--rw-r--r--   0        0        0     3911 2023-01-22 14:38:01.549959 kraken_std-0.8.5/src/kraken/std/docker/__init__.py
--rw-r--r--   0        0        0     3254 2023-01-22 14:38:01.549959 kraken_std-0.8.5/src/kraken/std/docker/buildx.py
--rw-r--r--   0        0        0     1426 2023-01-22 14:38:01.549959 kraken_std-0.8.5/src/kraken/std/docker/dockerapi.py
--rw-r--r--   0        0        0     8949 2023-04-19 15:39:43.860433 kraken_std-0.8.5/src/kraken/std/docker/kaniko.py
--rw-r--r--   0        0        0     1938 2023-01-22 14:38:01.549959 kraken_std-0.8.5/src/kraken/std/docker/manifest_tool.py
--rw-r--r--   0        0        0     3650 2023-01-22 14:38:01.549959 kraken_std-0.8.5/src/kraken/std/docker/native.py
--rw-r--r--   0        0        0        0 2023-01-22 14:38:01.549959 kraken_std-0.8.5/src/kraken/std/docker/py.typed
--rw-r--r--   0        0        0     2264 2023-04-19 15:40:38.993462 kraken_std-0.8.5/src/kraken/std/docker/util.py
--rw-r--r--   0        0        0     1761 2023-04-05 21:42:55.754805 kraken_std-0.8.5/src/kraken/std/git/__init__.py
--rw-r--r--   0        0        0     1107 2023-01-22 14:38:01.549959 kraken_std-0.8.5/src/kraken/std/git/config.py
--rw-r--r--   0        0        0     9451 2023-04-19 15:08:11.413164 kraken_std-0.8.5/src/kraken/std/git/gitignore.py
--rw-r--r--   0        0        0        0 2023-03-06 13:53:50.490907 kraken_std-0.8.5/src/kraken/std/git/tasks/__init__.py
--rw-r--r--   0        0        0      448 2023-04-05 21:42:55.754805 kraken_std-0.8.5/src/kraken/std/git/tasks/const.py
--rw-r--r--   0        0        0     2919 2023-04-05 21:42:55.754805 kraken_std-0.8.5/src/kraken/std/git/tasks/gitignore_check_task.py
--rw-r--r--   0        0        0     2754 2023-04-05 21:42:55.754805 kraken_std-0.8.5/src/kraken/std/git/tasks/gitignore_sync_task.py
--rw-r--r--   0        0        0     2973 2023-03-06 13:53:50.490907 kraken_std-0.8.5/src/kraken/std/git/version.py
--rw-r--r--   0        0        0     6368 2023-04-19 15:08:11.413164 kraken_std-0.8.5/src/kraken/std/helm/__init__.py
--rw-r--r--   0        0        0     2132 2023-01-22 14:38:01.549959 kraken_std-0.8.5/src/kraken/std/helm/helmapi.py
--rw-r--r--   0        0        0     2310 2023-04-19 15:08:11.413164 kraken_std-0.8.5/src/kraken/std/http/__init__.py
--rw-r--r--   0        0        0     3431 2023-04-19 15:08:11.413164 kraken_std-0.8.5/src/kraken/std/http/lint_ban_bare_requests.py
--rw-r--r--   0        0        0        0 2023-01-22 14:38:01.549959 kraken_std-0.8.5/src/kraken/std/py.typed
--rw-r--r--   0        0        0     1670 2023-04-19 15:39:43.860433 kraken_std-0.8.5/src/kraken/std/python/__init__.py
--rw-r--r--   0        0        0     3586 2023-02-08 16:53:28.240291 kraken_std-0.8.5/src/kraken/std/python/buildsystem/__init__.py
--rw-r--r--   0        0        0     1332 2023-04-05 22:25:55.652556 kraken_std-0.8.5/src/kraken/std/python/buildsystem/helpers.py
--rw-r--r--   0        0        0     3120 2023-03-06 13:53:50.494907 kraken_std-0.8.5/src/kraken/std/python/buildsystem/maturin.py
--rw-r--r--   0        0        0     7926 2023-04-05 22:23:34.040338 kraken_std-0.8.5/src/kraken/std/python/buildsystem/poetry.py
--rw-r--r--   0        0        0     4415 2023-04-05 22:03:27.278276 kraken_std-0.8.5/src/kraken/std/python/buildsystem/slap.py
--rw-r--r--   0        0        0     4892 2023-04-05 22:23:34.040338 kraken_std-0.8.5/src/kraken/std/python/pyproject.py
--rw-r--r--   0        0        0     6401 2023-01-22 14:38:01.549959 kraken_std-0.8.5/src/kraken/std/python/settings.py
--rw-r--r--   0        0        0        0 2023-03-06 13:53:50.494907 kraken_std-0.8.5/src/kraken/std/python/tasks/__init__.py
--rw-r--r--   0        0        0     3249 2023-02-08 16:53:28.240291 kraken_std-0.8.5/src/kraken/std/python/tasks/base_task.py
--rw-r--r--   0        0        0     2076 2023-02-08 16:53:28.240291 kraken_std-0.8.5/src/kraken/std/python/tasks/black_task.py
--rw-r--r--   0        0        0     1922 2023-01-22 14:38:01.549959 kraken_std-0.8.5/src/kraken/std/python/tasks/build_task.py
--rw-r--r--   0        0        0     1046 2023-02-08 16:53:28.240291 kraken_std-0.8.5/src/kraken/std/python/tasks/flake8_task.py
--rw-r--r--   0        0        0     2377 2023-04-19 15:39:43.860433 kraken_std-0.8.5/src/kraken/std/python/tasks/info_task.py
--rw-r--r--   0        0        0     2834 2023-01-22 14:38:01.549959 kraken_std-0.8.5/src/kraken/std/python/tasks/install_task.py
--rw-r--r--   0        0        0     1844 2023-02-08 16:53:28.240291 kraken_std-0.8.5/src/kraken/std/python/tasks/isort_task.py
--rw-r--r--   0        0        0      946 2023-02-08 16:53:28.240291 kraken_std-0.8.5/src/kraken/std/python/tasks/login_task.py
--rw-r--r--   0        0        0     1463 2023-02-08 16:53:28.240291 kraken_std-0.8.5/src/kraken/std/python/tasks/mypy_subtest_task.py
--rw-r--r--   0        0        0     2352 2023-02-08 16:53:28.240291 kraken_std-0.8.5/src/kraken/std/python/tasks/mypy_task.py
--rw-r--r--   0        0        0     2598 2023-01-22 14:38:01.549959 kraken_std-0.8.5/src/kraken/std/python/tasks/publish_task.py
--rw-r--r--   0        0        0     2043 2023-02-08 16:53:28.240291 kraken_std-0.8.5/src/kraken/std/python/tasks/pycln_task.py
--rw-r--r--   0        0        0     1034 2023-02-08 16:53:28.240291 kraken_std-0.8.5/src/kraken/std/python/tasks/pylint_task.py
--rw-r--r--   0        0        0     2398 2023-03-06 13:53:50.494907 kraken_std-0.8.5/src/kraken/std/python/tasks/pytest_task.py
--rw-r--r--   0        0        0     4531 2023-03-06 13:53:50.494907 kraken_std-0.8.5/src/kraken/std/python/tasks/pyupgrade_task.py
--rw-r--r--   0        0        0     1778 2023-02-08 16:53:28.240291 kraken_std-0.8.5/src/kraken/std/python/tasks/update_lockfile_task.py
--rw-r--r--   0        0        0     1656 2023-01-22 14:38:01.549959 kraken_std-0.8.5/src/kraken/std/python/tasks/update_pyproject_task.py
--rw-r--r--   0        0        0     1127 2023-03-20 14:35:25.194513 kraken_std-0.8.5/src/kraken/std/python/version.py
--rw-r--r--   0        0        0     4042 2023-01-22 14:38:01.549959 kraken_std-0.8.5/src/kraken/std/sccache.py
--rw-r--r--   0        0        0      390 2023-03-20 14:35:25.194513 kraken_std-0.8.5/src/kraken/std/util/__init__.py
--rw-r--r--   0        0        0     1906 2023-03-20 14:35:25.194513 kraken_std-0.8.5/src/kraken/std/util/check_file_exists_and_is_committed_task.py
--rw-r--r--   0        0        0     6010 2023-03-20 14:35:25.194513 kraken_std-0.8.5/src/kraken/std/util/check_valid_readme_exists_task.py
--rw-r--r--   0        0        0     2645 2023-03-20 14:35:25.194513 kraken_std-0.8.5/src/kraken/std/util/copyright_task.py
--rw-r--r--   0        0        0     2516 1970-01-01 00:00:00.000000 kraken_std-0.8.5/PKG-INFO
+-rw-r--r--   0        0        0      988 2023-04-21 14:35:45.319872 kraken_std-0.8.6/LICENSE
+-rw-r--r--   0        0        0     1745 2023-04-21 14:36:34.194043 kraken_std-0.8.6/pyproject.toml
+-rw-r--r--   0        0        0     1498 2023-04-21 14:35:45.319872 kraken_std-0.8.6/readme.md
+-rw-r--r--   0        0        0       22 2023-04-21 14:36:34.198043 kraken_std-0.8.6/src/kraken/std/__init__.py
+-rw-r--r--   0        0        0    13390 2023-04-21 14:35:45.319872 kraken_std-0.8.6/src/kraken/std/cargo/__init__.py
+-rw-r--r--   0        0        0     2403 2023-04-21 14:35:45.319872 kraken_std-0.8.6/src/kraken/std/cargo/config.py
+-rw-r--r--   0        0        0     1753 2023-04-21 14:35:45.319872 kraken_std-0.8.6/src/kraken/std/cargo/data/certs/cert.pem
+-rw-r--r--   0        0        0     3243 2023-04-21 14:35:45.319872 kraken_std-0.8.6/src/kraken/std/cargo/data/certs/key.pem
+-rw-r--r--   0        0        0     7912 2023-04-21 14:35:45.319872 kraken_std-0.8.6/src/kraken/std/cargo/manifest.py
+-rw-r--r--   0        0        0     2294 2023-04-21 14:35:45.319872 kraken_std-0.8.6/src/kraken/std/cargo/mitm.py
+-rw-r--r--   0        0        0     1737 2023-04-21 14:35:45.319872 kraken_std-0.8.6/src/kraken/std/cargo/mitm_impl.py
+-rw-r--r--   0        0        0        0 2023-04-21 14:35:45.319872 kraken_std-0.8.6/src/kraken/std/cargo/tasks/__init__.py
+-rw-r--r--   0        0        0     5640 2023-04-21 14:35:45.319872 kraken_std-0.8.6/src/kraken/std/cargo/tasks/cargo_auth_proxy_task.py
+-rw-r--r--   0        0        0     5959 2023-04-21 14:35:45.319872 kraken_std-0.8.6/src/kraken/std/cargo/tasks/cargo_build_task.py
+-rw-r--r--   0        0        0     3163 2023-04-21 14:35:45.319872 kraken_std-0.8.6/src/kraken/std/cargo/tasks/cargo_bump_version_task.py
+-rw-r--r--   0        0        0     2177 2023-04-21 14:35:45.319872 kraken_std-0.8.6/src/kraken/std/cargo/tasks/cargo_check_toolchain_version.py
+-rw-r--r--   0        0        0      907 2023-04-21 14:35:45.319872 kraken_std-0.8.6/src/kraken/std/cargo/tasks/cargo_clippy_task.py
+-rw-r--r--   0        0        0      732 2023-04-21 14:35:45.319872 kraken_std-0.8.6/src/kraken/std/cargo/tasks/cargo_deny_task.py
+-rw-r--r--   0        0        0      730 2023-04-21 14:35:45.319872 kraken_std-0.8.6/src/kraken/std/cargo/tasks/cargo_fmt_task.py
+-rw-r--r--   0        0        0     2074 2023-04-21 14:35:45.319872 kraken_std-0.8.6/src/kraken/std/cargo/tasks/cargo_publish_task.py
+-rw-r--r--   0        0        0     2088 2023-04-21 14:35:45.319872 kraken_std-0.8.6/src/kraken/std/cargo/tasks/cargo_sync_config_task.py
+-rw-r--r--   0        0        0      493 2023-04-21 14:35:45.319872 kraken_std-0.8.6/src/kraken/std/cargo/tasks/cargo_test_task.py
+-rw-r--r--   0        0        0      391 2023-04-21 14:35:45.319872 kraken_std-0.8.6/src/kraken/std/cargo/tasks/cargo_update_task.py
+-rw-r--r--   0        0        0      720 2023-04-21 14:35:45.319872 kraken_std-0.8.6/src/kraken/std/cargo/version.py
+-rw-r--r--   0        0        0        0 2023-04-21 14:35:45.319872 kraken_std-0.8.6/src/kraken/std/descriptors/__init__.py
+-rw-r--r--   0        0        0      874 2023-04-21 14:35:45.319872 kraken_std-0.8.6/src/kraken/std/descriptors/resource.py
+-rw-r--r--   0        0        0    10002 2023-04-21 14:35:45.323872 kraken_std-0.8.6/src/kraken/std/dist.py
+-rw-r--r--   0        0        0     3911 2023-04-21 14:35:45.323872 kraken_std-0.8.6/src/kraken/std/docker/__init__.py
+-rw-r--r--   0        0        0     3254 2023-04-21 14:35:45.323872 kraken_std-0.8.6/src/kraken/std/docker/buildx.py
+-rw-r--r--   0        0        0     1426 2023-04-21 14:35:45.323872 kraken_std-0.8.6/src/kraken/std/docker/dockerapi.py
+-rw-r--r--   0        0        0     8949 2023-04-21 14:35:45.323872 kraken_std-0.8.6/src/kraken/std/docker/kaniko.py
+-rw-r--r--   0        0        0     1938 2023-04-21 14:35:45.323872 kraken_std-0.8.6/src/kraken/std/docker/manifest_tool.py
+-rw-r--r--   0        0        0     3650 2023-04-21 14:35:45.323872 kraken_std-0.8.6/src/kraken/std/docker/native.py
+-rw-r--r--   0        0        0        0 2023-04-21 14:35:45.323872 kraken_std-0.8.6/src/kraken/std/docker/py.typed
+-rw-r--r--   0        0        0     2264 2023-04-21 14:35:45.323872 kraken_std-0.8.6/src/kraken/std/docker/util.py
+-rw-r--r--   0        0        0     1761 2023-04-21 14:35:45.323872 kraken_std-0.8.6/src/kraken/std/git/__init__.py
+-rw-r--r--   0        0        0     1107 2023-04-21 14:35:45.323872 kraken_std-0.8.6/src/kraken/std/git/config.py
+-rw-r--r--   0        0        0     9451 2023-04-21 14:35:45.323872 kraken_std-0.8.6/src/kraken/std/git/gitignore.py
+-rw-r--r--   0        0        0        0 2023-04-21 14:35:45.323872 kraken_std-0.8.6/src/kraken/std/git/tasks/__init__.py
+-rw-r--r--   0        0        0      448 2023-04-21 14:35:45.323872 kraken_std-0.8.6/src/kraken/std/git/tasks/const.py
+-rw-r--r--   0        0        0     2919 2023-04-21 14:35:45.323872 kraken_std-0.8.6/src/kraken/std/git/tasks/gitignore_check_task.py
+-rw-r--r--   0        0        0     2754 2023-04-21 14:35:45.323872 kraken_std-0.8.6/src/kraken/std/git/tasks/gitignore_sync_task.py
+-rw-r--r--   0        0        0     2973 2023-04-21 14:35:45.323872 kraken_std-0.8.6/src/kraken/std/git/version.py
+-rw-r--r--   0        0        0     6368 2023-04-21 14:35:45.323872 kraken_std-0.8.6/src/kraken/std/helm/__init__.py
+-rw-r--r--   0        0        0     2132 2023-04-21 14:35:45.323872 kraken_std-0.8.6/src/kraken/std/helm/helmapi.py
+-rw-r--r--   0        0        0     2310 2023-04-21 14:35:45.323872 kraken_std-0.8.6/src/kraken/std/http/__init__.py
+-rw-r--r--   0        0        0     3431 2023-04-21 14:35:45.323872 kraken_std-0.8.6/src/kraken/std/http/lint_ban_bare_requests.py
+-rw-r--r--   0        0        0        0 2023-04-21 14:35:45.323872 kraken_std-0.8.6/src/kraken/std/py.typed
+-rw-r--r--   0        0        0     1670 2023-04-21 14:35:45.323872 kraken_std-0.8.6/src/kraken/std/python/__init__.py
+-rw-r--r--   0        0        0     3586 2023-04-21 14:35:45.323872 kraken_std-0.8.6/src/kraken/std/python/buildsystem/__init__.py
+-rw-r--r--   0        0        0     1332 2023-04-21 14:35:45.323872 kraken_std-0.8.6/src/kraken/std/python/buildsystem/helpers.py
+-rw-r--r--   0        0        0     3120 2023-04-21 14:35:45.323872 kraken_std-0.8.6/src/kraken/std/python/buildsystem/maturin.py
+-rw-r--r--   0        0        0     7985 2023-04-21 14:35:45.323872 kraken_std-0.8.6/src/kraken/std/python/buildsystem/poetry.py
+-rw-r--r--   0        0        0     4415 2023-04-21 14:35:45.323872 kraken_std-0.8.6/src/kraken/std/python/buildsystem/slap.py
+-rw-r--r--   0        0        0     6406 2023-04-21 14:35:45.323872 kraken_std-0.8.6/src/kraken/std/python/pyproject.py
+-rw-r--r--   0        0        0     6401 2023-04-21 14:35:45.323872 kraken_std-0.8.6/src/kraken/std/python/settings.py
+-rw-r--r--   0        0        0        0 2023-04-21 14:35:45.323872 kraken_std-0.8.6/src/kraken/std/python/tasks/__init__.py
+-rw-r--r--   0        0        0     3249 2023-04-21 14:35:45.323872 kraken_std-0.8.6/src/kraken/std/python/tasks/base_task.py
+-rw-r--r--   0        0        0     2076 2023-04-21 14:35:45.323872 kraken_std-0.8.6/src/kraken/std/python/tasks/black_task.py
+-rw-r--r--   0        0        0     1922 2023-04-21 14:35:45.323872 kraken_std-0.8.6/src/kraken/std/python/tasks/build_task.py
+-rw-r--r--   0        0        0     1046 2023-04-21 14:35:45.323872 kraken_std-0.8.6/src/kraken/std/python/tasks/flake8_task.py
+-rw-r--r--   0        0        0     2377 2023-04-21 14:35:45.323872 kraken_std-0.8.6/src/kraken/std/python/tasks/info_task.py
+-rw-r--r--   0        0        0     2834 2023-04-21 14:35:45.323872 kraken_std-0.8.6/src/kraken/std/python/tasks/install_task.py
+-rw-r--r--   0        0        0     1844 2023-04-21 14:35:45.323872 kraken_std-0.8.6/src/kraken/std/python/tasks/isort_task.py
+-rw-r--r--   0        0        0      946 2023-04-21 14:35:45.323872 kraken_std-0.8.6/src/kraken/std/python/tasks/login_task.py
+-rw-r--r--   0        0        0     1463 2023-04-21 14:35:45.323872 kraken_std-0.8.6/src/kraken/std/python/tasks/mypy_subtest_task.py
+-rw-r--r--   0        0        0     2352 2023-04-21 14:35:45.323872 kraken_std-0.8.6/src/kraken/std/python/tasks/mypy_task.py
+-rw-r--r--   0        0        0     2598 2023-04-21 14:35:45.323872 kraken_std-0.8.6/src/kraken/std/python/tasks/publish_task.py
+-rw-r--r--   0        0        0     2043 2023-04-21 14:35:45.323872 kraken_std-0.8.6/src/kraken/std/python/tasks/pycln_task.py
+-rw-r--r--   0        0        0     1034 2023-04-21 14:35:45.323872 kraken_std-0.8.6/src/kraken/std/python/tasks/pylint_task.py
+-rw-r--r--   0        0        0     2398 2023-04-21 14:35:45.323872 kraken_std-0.8.6/src/kraken/std/python/tasks/pytest_task.py
+-rw-r--r--   0        0        0     4531 2023-04-21 14:35:45.323872 kraken_std-0.8.6/src/kraken/std/python/tasks/pyupgrade_task.py
+-rw-r--r--   0        0        0     1778 2023-04-21 14:35:45.323872 kraken_std-0.8.6/src/kraken/std/python/tasks/update_lockfile_task.py
+-rw-r--r--   0        0        0     1656 2023-04-21 14:35:45.323872 kraken_std-0.8.6/src/kraken/std/python/tasks/update_pyproject_task.py
+-rw-r--r--   0        0        0     1127 2023-04-21 14:35:45.323872 kraken_std-0.8.6/src/kraken/std/python/version.py
+-rw-r--r--   0        0        0     4042 2023-04-21 14:35:45.323872 kraken_std-0.8.6/src/kraken/std/sccache.py
+-rw-r--r--   0        0        0      390 2023-04-21 14:35:45.323872 kraken_std-0.8.6/src/kraken/std/util/__init__.py
+-rw-r--r--   0        0        0     1906 2023-04-21 14:35:45.323872 kraken_std-0.8.6/src/kraken/std/util/check_file_exists_and_is_committed_task.py
+-rw-r--r--   0        0        0     6010 2023-04-21 14:35:45.323872 kraken_std-0.8.6/src/kraken/std/util/check_valid_readme_exists_task.py
+-rw-r--r--   0        0        0     2645 2023-04-21 14:35:45.323872 kraken_std-0.8.6/src/kraken/std/util/copyright_task.py
+-rw-r--r--   0        0        0     2516 1970-01-01 00:00:00.000000 kraken_std-0.8.6/PKG-INFO
```

### Comparing `kraken_std-0.8.5/LICENSE` & `kraken_std-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/pyproject.toml` & `kraken_std-0.8.6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "kraken-std"
-version = "0.8.5"
+version = "0.8.6"
 description = "The Kraken standard library."
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 packages = [{ include = "kraken/std", from = "src" }]
 classifiers = []
 keywords = []
```

### Comparing `kraken_std-0.8.5/readme.md` & `kraken_std-0.8.6/readme.md`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/cargo/__init__.py` & `kraken_std-0.8.6/src/kraken/std/cargo/__init__.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/cargo/config.py` & `kraken_std-0.8.6/src/kraken/std/cargo/config.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/cargo/data/certs/cert.pem` & `kraken_std-0.8.6/src/kraken/std/cargo/data/certs/cert.pem`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/cargo/data/certs/key.pem` & `kraken_std-0.8.6/src/kraken/std/cargo/data/certs/key.pem`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/cargo/manifest.py` & `kraken_std-0.8.6/src/kraken/std/cargo/manifest.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/cargo/mitm.py` & `kraken_std-0.8.6/src/kraken/std/cargo/mitm.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/cargo/mitm_impl.py` & `kraken_std-0.8.6/src/kraken/std/cargo/mitm_impl.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/cargo/tasks/cargo_auth_proxy_task.py` & `kraken_std-0.8.6/src/kraken/std/cargo/tasks/cargo_auth_proxy_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/cargo/tasks/cargo_build_task.py` & `kraken_std-0.8.6/src/kraken/std/cargo/tasks/cargo_build_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/cargo/tasks/cargo_bump_version_task.py` & `kraken_std-0.8.6/src/kraken/std/cargo/tasks/cargo_bump_version_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/cargo/tasks/cargo_check_toolchain_version.py` & `kraken_std-0.8.6/src/kraken/std/cargo/tasks/cargo_check_toolchain_version.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/cargo/tasks/cargo_clippy_task.py` & `kraken_std-0.8.6/src/kraken/std/cargo/tasks/cargo_clippy_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/cargo/tasks/cargo_deny_task.py` & `kraken_std-0.8.6/src/kraken/std/cargo/tasks/cargo_deny_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/cargo/tasks/cargo_fmt_task.py` & `kraken_std-0.8.6/src/kraken/std/cargo/tasks/cargo_fmt_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/cargo/tasks/cargo_publish_task.py` & `kraken_std-0.8.6/src/kraken/std/cargo/tasks/cargo_publish_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/cargo/tasks/cargo_sync_config_task.py` & `kraken_std-0.8.6/src/kraken/std/cargo/tasks/cargo_sync_config_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/cargo/version.py` & `kraken_std-0.8.6/src/kraken/std/cargo/version.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/descriptors/resource.py` & `kraken_std-0.8.6/src/kraken/std/descriptors/resource.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/dist.py` & `kraken_std-0.8.6/src/kraken/std/dist.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/docker/__init__.py` & `kraken_std-0.8.6/src/kraken/std/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/docker/buildx.py` & `kraken_std-0.8.6/src/kraken/std/docker/buildx.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/docker/dockerapi.py` & `kraken_std-0.8.6/src/kraken/std/docker/dockerapi.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/docker/kaniko.py` & `kraken_std-0.8.6/src/kraken/std/docker/kaniko.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/docker/manifest_tool.py` & `kraken_std-0.8.6/src/kraken/std/docker/manifest_tool.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/docker/native.py` & `kraken_std-0.8.6/src/kraken/std/docker/native.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/docker/util.py` & `kraken_std-0.8.6/src/kraken/std/docker/util.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/git/__init__.py` & `kraken_std-0.8.6/src/kraken/std/git/__init__.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/git/config.py` & `kraken_std-0.8.6/src/kraken/std/git/config.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/git/gitignore.py` & `kraken_std-0.8.6/src/kraken/std/git/gitignore.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/git/tasks/gitignore_check_task.py` & `kraken_std-0.8.6/src/kraken/std/git/tasks/gitignore_check_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/git/tasks/gitignore_sync_task.py` & `kraken_std-0.8.6/src/kraken/std/git/tasks/gitignore_sync_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/git/version.py` & `kraken_std-0.8.6/src/kraken/std/git/version.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/helm/__init__.py` & `kraken_std-0.8.6/src/kraken/std/helm/__init__.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/helm/helmapi.py` & `kraken_std-0.8.6/src/kraken/std/helm/helmapi.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/http/__init__.py` & `kraken_std-0.8.6/src/kraken/std/http/__init__.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/http/lint_ban_bare_requests.py` & `kraken_std-0.8.6/src/kraken/std/http/lint_ban_bare_requests.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/python/__init__.py` & `kraken_std-0.8.6/src/kraken/std/python/__init__.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/python/buildsystem/__init__.py` & `kraken_std-0.8.6/src/kraken/std/python/buildsystem/__init__.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/python/buildsystem/helpers.py` & `kraken_std-0.8.6/src/kraken/std/python/buildsystem/helpers.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/python/buildsystem/maturin.py` & `kraken_std-0.8.6/src/kraken/std/python/buildsystem/maturin.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/python/buildsystem/poetry.py` & `kraken_std-0.8.6/src/kraken/std/python/buildsystem/poetry.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,15 @@
 
     def build(self, output_directory: Path, as_version: str | None = None) -> list[Path]:
         previous_version: str | None = None
         revert_version_paths: list[Path] = []
         if as_version is not None:
             # Bump the in-source version number.
             pyproject = Pyproject.read(self.project_directory / "pyproject.toml")
+            pyproject.update_relative_packages(as_version)
             previous_version = pyproject.set_poetry_version(as_version)
             pyproject.save()
             for package in pyproject.get_poetry_packages(fallback=True):
                 package_dir = self.project_directory / (package.from_ or "") / package.include
                 n_replaced = update_python_version_str_in_source_files(as_version, package_dir)
                 if n_replaced > 0:
                     revert_version_paths.append(package_dir)
```

### Comparing `kraken_std-0.8.5/src/kraken/std/python/buildsystem/slap.py` & `kraken_std-0.8.6/src/kraken/std/python/buildsystem/slap.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/python/pyproject.py` & `kraken_std-0.8.6/src/kraken/std/python/pyproject.py`

 * *Files 21% similar despite different names*

```diff
@@ -50,14 +50,46 @@
         path = path or self._path
         with path.open("wb") as fp:
             tomli_w.dump(self.to_json(), fp)
 
     def get_poetry_sources(self) -> list[dict[str, Any]]:
         return list(self._poetry_section().setdefault("source", []))
 
+    def _find_dependencies_definitions(self, pyproject_section: Dict[str, Any], version: str) -> None:
+        """
+        Finds and updates the version of local dependencies listed in the
+        "dev-dependencies" and "dependencies" sections of the PyProject.toml file.
+        Args:
+            pyproject_section (Dict[str, Any]): A dictionary representing a section of the PyProject.toml file.
+            version (str): The version to update local dependencies with.
+        """
+
+        # TODO(@niklas.rosenstein): Support Poetry dependency groups
+        #       https://python-poetry.org/docs/master/managing-dependencies/#dependency-groups
+
+        for key, value in pyproject_section.items():
+            if key in ("dependencies", "dev-dependencies"):
+                if type(value) == dict:
+                    self._update_dependencies_version(value, version)
+                pass
+            else:
+                if type(value) is dict:
+                    self._find_dependencies_definitions(value, version)
+
+    def _update_dependencies_version(self, obj: Dict[str, Any], version: str) -> None:
+        for _key, value in obj.items():
+            if type(value) == dict:
+                if "path" in value and "develop" in value:
+                    del value["path"]
+                    del value["develop"]
+                    value["version"] = version
+
+    def update_relative_packages(self, version: str) -> None:
+        self._find_dependencies_definitions(self._poetry_section(), version)
+
     def delete_poetry_source(self, source_name: str) -> None:
         sources_conf = self._poetry_section().setdefault("source", [])
         index = next((i for i, v in enumerate(sources_conf) if v["name"] == source_name), None)
         if index is None:
             raise KeyError(source_name)
         del sources_conf[index]
```

### Comparing `kraken_std-0.8.5/src/kraken/std/python/settings.py` & `kraken_std-0.8.6/src/kraken/std/python/settings.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/python/tasks/base_task.py` & `kraken_std-0.8.6/src/kraken/std/python/tasks/base_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/python/tasks/black_task.py` & `kraken_std-0.8.6/src/kraken/std/python/tasks/black_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/python/tasks/build_task.py` & `kraken_std-0.8.6/src/kraken/std/python/tasks/build_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/python/tasks/flake8_task.py` & `kraken_std-0.8.6/src/kraken/std/python/tasks/flake8_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/python/tasks/info_task.py` & `kraken_std-0.8.6/src/kraken/std/python/tasks/info_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/python/tasks/install_task.py` & `kraken_std-0.8.6/src/kraken/std/python/tasks/install_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/python/tasks/isort_task.py` & `kraken_std-0.8.6/src/kraken/std/python/tasks/isort_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/python/tasks/login_task.py` & `kraken_std-0.8.6/src/kraken/std/python/tasks/login_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/python/tasks/mypy_subtest_task.py` & `kraken_std-0.8.6/src/kraken/std/python/tasks/mypy_subtest_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/python/tasks/mypy_task.py` & `kraken_std-0.8.6/src/kraken/std/python/tasks/mypy_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/python/tasks/publish_task.py` & `kraken_std-0.8.6/src/kraken/std/python/tasks/publish_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/python/tasks/pycln_task.py` & `kraken_std-0.8.6/src/kraken/std/python/tasks/pycln_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/python/tasks/pylint_task.py` & `kraken_std-0.8.6/src/kraken/std/python/tasks/pylint_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/python/tasks/pytest_task.py` & `kraken_std-0.8.6/src/kraken/std/python/tasks/pytest_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/python/tasks/pyupgrade_task.py` & `kraken_std-0.8.6/src/kraken/std/python/tasks/pyupgrade_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/python/tasks/update_lockfile_task.py` & `kraken_std-0.8.6/src/kraken/std/python/tasks/update_lockfile_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/python/tasks/update_pyproject_task.py` & `kraken_std-0.8.6/src/kraken/std/python/tasks/update_pyproject_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/python/version.py` & `kraken_std-0.8.6/src/kraken/std/python/version.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/sccache.py` & `kraken_std-0.8.6/src/kraken/std/sccache.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/util/check_file_exists_and_is_committed_task.py` & `kraken_std-0.8.6/src/kraken/std/util/check_file_exists_and_is_committed_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/util/check_valid_readme_exists_task.py` & `kraken_std-0.8.6/src/kraken/std/util/check_valid_readme_exists_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/src/kraken/std/util/copyright_task.py` & `kraken_std-0.8.6/src/kraken/std/util/copyright_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.5/PKG-INFO` & `kraken_std-0.8.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kraken-std
-Version: 0.8.5
+Version: 0.8.6
 Summary: The Kraken standard library.
 License: MIT
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

