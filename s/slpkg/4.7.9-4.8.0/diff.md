# Comparing `tmp/slpkg-4.7.9.tar.gz` & `tmp/slpkg-4.8.0.tar.gz`

## Comparing `slpkg-4.7.9.tar` & `slpkg-4.8.0.tar`

### file list

```diff
@@ -1,97 +1,98 @@
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-19 14:43:01.000000 slpkg-4.7.9/
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-19 14:36:36.000000 slpkg-4.7.9/filelists/
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-19 14:36:36.000000 slpkg-4.7.9/filelists/multilib/
--rw-r--r--   0 dslackw   (1000) users      (100)    15477 2023-04-19 14:36:36.000000 slpkg-4.7.9/filelists/multilib/README.ERIC
--rw-r--r--   0 dslackw   (1000) users      (100)      250 2023-04-19 14:36:36.000000 slpkg-4.7.9/filelists/multilib/glibc_packages.pkgs
--rw-r--r--   0 dslackw   (1000) users      (100)      831 2023-04-19 14:36:36.000000 slpkg-4.7.9/filelists/multilib/README
--rw-r--r--   0 dslackw   (1000) users      (100)     4508 2023-04-19 14:36:36.000000 slpkg-4.7.9/filelists/multilib/compat32.pkgs
--rw-r--r--   0 dslackw   (1000) users      (100)       88 2023-04-19 14:36:36.000000 slpkg-4.7.9/filelists/README
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-19 14:36:36.000000 slpkg-4.7.9/slackbuild/
--rw-r--r--   0 dslackw   (1000) users      (100)      941 2023-04-19 14:36:36.000000 slpkg-4.7.9/slackbuild/slack-desc
--rw-r--r--   0 dslackw   (1000) users      (100)      432 2023-04-19 14:36:36.000000 slpkg-4.7.9/slackbuild/doinst.sh
--rw-r--r--   0 dslackw   (1000) users      (100)      304 2023-04-19 14:36:36.000000 slpkg-4.7.9/slackbuild/README
--rwxr-xr-x   0 dslackw   (1000) users      (100)     4280 2023-04-19 14:36:36.000000 slpkg-4.7.9/slackbuild/slpkg.SlackBuild
--rwxr-xr-x   0 dslackw   (1000) users      (100)       70 2023-04-19 14:36:36.000000 slpkg-4.7.9/setup.py
--rw-r--r--   0 dslackw   (1000) users      (100)       84 2023-04-19 14:36:36.000000 slpkg-4.7.9/requirements.txt
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-19 14:36:36.000000 slpkg-4.7.9/configs/
--rw-r--r--   0 dslackw   (1000) users      (100)     9164 2023-04-19 14:36:36.000000 slpkg-4.7.9/configs/repositories.toml
--rw-r--r--   0 dslackw   (1000) users      (100)      483 2023-04-19 14:36:36.000000 slpkg-4.7.9/configs/blacklist.toml
--rw-r--r--   0 dslackw   (1000) users      (100)     3634 2023-04-19 14:36:36.000000 slpkg-4.7.9/configs/slpkg.toml
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-19 14:36:36.000000 slpkg-4.7.9/tests/
--rw-r--r--   0 dslackw   (1000) users      (100)     2340 2023-04-19 14:36:36.000000 slpkg-4.7.9/tests/test_configs.py
--rw-r--r--   0 dslackw   (1000) users      (100)      770 2023-04-19 14:36:36.000000 slpkg-4.7.9/tests/test_checks.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1891 2023-04-19 14:36:36.000000 slpkg-4.7.9/tests/test_utilities.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1455 2023-04-19 14:36:36.000000 slpkg-4.7.9/tests/test_sbo_queries.py
--rw-r--r--   0 dslackw   (1000) users      (100)      255 2023-04-19 14:36:36.000000 slpkg-4.7.9/tests/test_blacklist.py
--rw-r--r--   0 dslackw   (1000) users      (100)      588 2023-04-19 14:36:36.000000 slpkg-4.7.9/tests/test_colors.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1567 2023-04-19 14:36:36.000000 slpkg-4.7.9/tests/test_upgrade.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1787 2023-04-19 14:36:36.000000 slpkg-4.7.9/tests/test_bin_queries.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1076 2023-04-19 14:36:36.000000 slpkg-4.7.9/LICENSE
--rwxr-xr-x   0 dslackw   (1000) users      (100)     1773 2023-04-19 14:36:36.000000 slpkg-4.7.9/install.sh
--rw-r--r--   0 dslackw   (1000) users      (100)    45099 2023-04-19 14:36:36.000000 slpkg-4.7.9/ChangeLog.txt
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-19 14:36:36.000000 slpkg-4.7.9/man/
--rw-r--r--   0 dslackw   (1000) users      (100)     8987 2023-04-19 14:36:36.000000 slpkg-4.7.9/man/slpkg.1
--rw-r--r--   0 dslackw   (1000) users      (100)     9918 2023-04-19 14:36:36.000000 slpkg-4.7.9/man/slpkg-fr.1
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-19 14:36:36.000000 slpkg-4.7.9/completion/
--rw-r--r--   0 dslackw   (1000) users      (100)      910 2023-04-19 14:36:36.000000 slpkg-4.7.9/completion/slpkg
--rw-r--r--   0 dslackw   (1000) users      (100)       93 2023-04-19 14:36:36.000000 slpkg-4.7.9/.gitignore
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/binaries/
--rw-r--r--   0 dslackw   (1000) users      (100)     1947 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/binaries/required.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2110 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/binaries/queries.py
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/binaries/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)     9605 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/binaries/install.py
--rw-r--r--   0 dslackw   (1000) users      (100)    63573 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/install_data.py
--rw-r--r--   0 dslackw   (1000) users      (100)    27456 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/repositories.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2463 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/repo_info.py
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/sbos/
--rw-r--r--   0 dslackw   (1000) users      (100)     1368 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/sbos/queries.py
--rw-r--r--   0 dslackw   (1000) users      (100)    14873 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/sbos/slackbuild.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1042 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/sbos/dependencies.py
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/sbos/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3983 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/form_configs.py
--rw-r--r--   0 dslackw   (1000) users      (100)    34184 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/update_repository.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1791 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/progress_bar.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2391 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/downloader.py
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/models/
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/models/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2630 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/models/models.py
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/views/
--rw-r--r--   0 dslackw   (1000) users      (100)     7070 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/views/view_package.py
--rw-r--r--   0 dslackw   (1000) users      (100)      629 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/views/version.py
--rw-r--r--   0 dslackw   (1000) users      (100)     6319 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/views/cli_menu.py
--rw-r--r--   0 dslackw   (1000) users      (100)     5523 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/views/ascii.py
--rw-r--r--   0 dslackw   (1000) users      (100)     4043 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/views/help_commands.py
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/views/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)     9821 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/views/views.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3029 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/checks.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1344 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/checksum.py
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2196 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/dialog_box.py
--rw-r--r--   0 dslackw   (1000) users      (100)     5193 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/configs.py
--rw-r--r--   0 dslackw   (1000) users      (100)      902 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/clean_logs.py
--rw-r--r--   0 dslackw   (1000) users      (100)     7000 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/utilities.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3970 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/dependees.py
--rw-r--r--   0 dslackw   (1000) users      (100)    11207 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/check_updates.py
--rw-r--r--   0 dslackw   (1000) users      (100)     5690 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/remove_packages.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1521 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/blacklist.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2603 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/download_only.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3136 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/tracking.py
--rw-r--r--   0 dslackw   (1000) users      (100)      245 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/logging_config.py
--rw-r--r--   0 dslackw   (1000) users      (100)    30063 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/main.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1470 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/find_installed.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3212 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/upgrade.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2872 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/search.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1363 2023-04-19 14:36:36.000000 slpkg-4.7.9/setup.cfg
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-19 14:42:55.000000 slpkg-4.7.9/slpkg.egg-info/
--rw-r--r--   0 dslackw   (1000) users      (100)        1 2023-04-19 14:42:55.000000 slpkg-4.7.9/slpkg.egg-info/dependency_links.txt
--rw-r--r--   0 dslackw   (1000) users      (100)     1105 2023-04-19 14:42:56.000000 slpkg-4.7.9/slpkg.egg-info/SOURCES.txt
--rw-r--r--   0 dslackw   (1000) users      (100)        6 2023-04-19 14:42:55.000000 slpkg-4.7.9/slpkg.egg-info/top_level.txt
--rw-r--r--   0 dslackw   (1000) users      (100)       77 2023-04-19 14:42:55.000000 slpkg-4.7.9/slpkg.egg-info/requires.txt
--rw-r--r--   0 dslackw   (1000) users      (100)     1271 2023-04-19 14:42:55.000000 slpkg-4.7.9/slpkg.egg-info/PKG-INFO
--rw-r--r--   0 dslackw   (1000) users      (100)     8341 2023-04-19 14:36:36.000000 slpkg-4.7.9/README.md
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-19 14:36:36.000000 slpkg-4.7.9/tools/
--rwxr-xr-x   0 dslackw   (1000) users      (100)      787 2023-04-19 14:36:36.000000 slpkg-4.7.9/tools/gen_sbo_txt.sh
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-19 14:36:36.000000 slpkg-4.7.9/bin/
--rwxr-xr-x   0 dslackw   (1000) users      (100)    11470 2023-04-19 14:36:36.000000 slpkg-4.7.9/bin/slpkg_new-configs
--rwxr-xr-x   0 dslackw   (1000) users      (100)      184 2023-04-19 14:36:36.000000 slpkg-4.7.9/bin/slpkg
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-21 14:30:41.000000 slpkg-4.8.0/
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-21 14:24:01.000000 slpkg-4.8.0/filelists/
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-21 14:24:01.000000 slpkg-4.8.0/filelists/multilib/
+-rw-r--r--   0 dslackw   (1000) users      (100)    15477 2023-04-21 14:24:01.000000 slpkg-4.8.0/filelists/multilib/README.ERIC
+-rw-r--r--   0 dslackw   (1000) users      (100)      250 2023-04-21 14:24:01.000000 slpkg-4.8.0/filelists/multilib/glibc_packages.pkgs
+-rw-r--r--   0 dslackw   (1000) users      (100)      831 2023-04-21 14:24:01.000000 slpkg-4.8.0/filelists/multilib/README
+-rw-r--r--   0 dslackw   (1000) users      (100)     4508 2023-04-21 14:24:01.000000 slpkg-4.8.0/filelists/multilib/compat32.pkgs
+-rw-r--r--   0 dslackw   (1000) users      (100)       88 2023-04-21 14:24:01.000000 slpkg-4.8.0/filelists/README
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-21 14:24:01.000000 slpkg-4.8.0/slackbuild/
+-rw-r--r--   0 dslackw   (1000) users      (100)      941 2023-04-21 14:24:01.000000 slpkg-4.8.0/slackbuild/slack-desc
+-rw-r--r--   0 dslackw   (1000) users      (100)      432 2023-04-21 14:24:01.000000 slpkg-4.8.0/slackbuild/doinst.sh
+-rw-r--r--   0 dslackw   (1000) users      (100)      304 2023-04-21 14:24:01.000000 slpkg-4.8.0/slackbuild/README
+-rwxr-xr-x   0 dslackw   (1000) users      (100)     4280 2023-04-21 14:24:01.000000 slpkg-4.8.0/slackbuild/slpkg.SlackBuild
+-rwxr-xr-x   0 dslackw   (1000) users      (100)       70 2023-04-21 14:24:01.000000 slpkg-4.8.0/setup.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     7920 2023-04-21 14:30:35.000000 slpkg-4.8.0/README.rst
+-rw-r--r--   0 dslackw   (1000) users      (100)       84 2023-04-21 14:24:01.000000 slpkg-4.8.0/requirements.txt
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-21 14:24:01.000000 slpkg-4.8.0/configs/
+-rw-r--r--   0 dslackw   (1000) users      (100)     9164 2023-04-21 14:24:01.000000 slpkg-4.8.0/configs/repositories.toml
+-rw-r--r--   0 dslackw   (1000) users      (100)      483 2023-04-21 14:24:01.000000 slpkg-4.8.0/configs/blacklist.toml
+-rw-r--r--   0 dslackw   (1000) users      (100)     3634 2023-04-21 14:24:01.000000 slpkg-4.8.0/configs/slpkg.toml
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-21 14:24:01.000000 slpkg-4.8.0/tests/
+-rw-r--r--   0 dslackw   (1000) users      (100)     2340 2023-04-21 14:24:01.000000 slpkg-4.8.0/tests/test_configs.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      770 2023-04-21 14:24:01.000000 slpkg-4.8.0/tests/test_checks.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1891 2023-04-21 14:24:01.000000 slpkg-4.8.0/tests/test_utilities.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1455 2023-04-21 14:24:01.000000 slpkg-4.8.0/tests/test_sbo_queries.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      255 2023-04-21 14:24:01.000000 slpkg-4.8.0/tests/test_blacklist.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      588 2023-04-21 14:24:01.000000 slpkg-4.8.0/tests/test_colors.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1567 2023-04-21 14:24:01.000000 slpkg-4.8.0/tests/test_upgrade.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1787 2023-04-21 14:24:01.000000 slpkg-4.8.0/tests/test_bin_queries.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1076 2023-04-21 14:24:01.000000 slpkg-4.8.0/LICENSE
+-rwxr-xr-x   0 dslackw   (1000) users      (100)     1773 2023-04-21 14:24:01.000000 slpkg-4.8.0/install.sh
+-rw-r--r--   0 dslackw   (1000) users      (100)    45268 2023-04-21 14:24:01.000000 slpkg-4.8.0/ChangeLog.txt
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-21 14:24:01.000000 slpkg-4.8.0/man/
+-rw-r--r--   0 dslackw   (1000) users      (100)     8987 2023-04-21 14:24:01.000000 slpkg-4.8.0/man/slpkg.1
+-rw-r--r--   0 dslackw   (1000) users      (100)     9918 2023-04-21 14:24:01.000000 slpkg-4.8.0/man/slpkg-fr.1
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-21 14:24:01.000000 slpkg-4.8.0/completion/
+-rw-r--r--   0 dslackw   (1000) users      (100)      910 2023-04-21 14:24:01.000000 slpkg-4.8.0/completion/slpkg
+-rw-r--r--   0 dslackw   (1000) users      (100)       93 2023-04-21 14:24:01.000000 slpkg-4.8.0/.gitignore
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/
+-rw-r--r--   0 dslackw   (1000) users      (100)     3983 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/dialog_configs.py
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/binaries/
+-rw-r--r--   0 dslackw   (1000) users      (100)     1574 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/binaries/required.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2110 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/binaries/queries.py
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/binaries/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     9605 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/binaries/install.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    63573 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/install_data.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    27456 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/repositories.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2463 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/repo_info.py
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/sbos/
+-rw-r--r--   0 dslackw   (1000) users      (100)     1368 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/sbos/queries.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    14873 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/sbos/slackbuild.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      924 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/sbos/dependencies.py
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/sbos/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    34184 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/update_repository.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1791 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/progress_bar.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2391 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/downloader.py
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/models/
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/models/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2630 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/models/models.py
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/views/
+-rw-r--r--   0 dslackw   (1000) users      (100)     7070 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/views/view_package.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      629 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/views/version.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     6319 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/views/cli_menu.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     5553 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/views/ascii.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     4043 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/views/help_commands.py
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/views/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     9827 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/views/views.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3029 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/checks.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1344 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/checksum.py
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2196 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/dialog_box.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     5193 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/configs.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      902 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/clean_logs.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     7000 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/utilities.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3970 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/dependees.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    11207 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/check_updates.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     5690 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/remove_packages.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1521 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/blacklist.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2603 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/download_only.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3043 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/tracking.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      245 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/logging_config.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    29938 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/main.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1423 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/find_installed.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3206 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/upgrade.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2872 2023-04-21 14:24:01.000000 slpkg-4.8.0/slpkg/search.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1354 2023-04-21 14:24:01.000000 slpkg-4.8.0/setup.cfg
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-21 14:29:47.000000 slpkg-4.8.0/slpkg.egg-info/
+-rw-r--r--   0 dslackw   (1000) users      (100)        1 2023-04-21 14:29:47.000000 slpkg-4.8.0/slpkg.egg-info/dependency_links.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)     1107 2023-04-21 14:29:47.000000 slpkg-4.8.0/slpkg.egg-info/SOURCES.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)        6 2023-04-21 14:29:47.000000 slpkg-4.8.0/slpkg.egg-info/top_level.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)       77 2023-04-21 14:29:47.000000 slpkg-4.8.0/slpkg.egg-info/requires.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)     1262 2023-04-21 14:29:47.000000 slpkg-4.8.0/slpkg.egg-info/PKG-INFO
+-rw-r--r--   0 dslackw   (1000) users      (100)     8453 2023-04-21 14:24:01.000000 slpkg-4.8.0/README.md
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-21 14:24:01.000000 slpkg-4.8.0/tools/
+-rwxr-xr-x   0 dslackw   (1000) users      (100)      787 2023-04-21 14:24:01.000000 slpkg-4.8.0/tools/gen_sbo_txt.sh
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-21 14:24:01.000000 slpkg-4.8.0/bin/
+-rwxr-xr-x   0 dslackw   (1000) users      (100)    11470 2023-04-21 14:24:01.000000 slpkg-4.8.0/bin/slpkg_new-configs
+-rwxr-xr-x   0 dslackw   (1000) users      (100)      184 2023-04-21 14:24:01.000000 slpkg-4.8.0/bin/slpkg
```

### Comparing `slpkg-4.7.9/filelists/multilib/README.ERIC` & `slpkg-4.8.0/filelists/multilib/README.ERIC`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.9/filelists/multilib/README` & `slpkg-4.8.0/filelists/multilib/README`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.9/filelists/multilib/compat32.pkgs` & `slpkg-4.8.0/filelists/multilib/compat32.pkgs`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.9/slackbuild/slack-desc` & `slpkg-4.8.0/slackbuild/slack-desc`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.9/slackbuild/slpkg.SlackBuild` & `slpkg-4.8.0/slackbuild/slpkg.SlackBuild`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.9/configs/repositories.toml` & `slpkg-4.8.0/configs/repositories.toml`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.9/configs/slpkg.toml` & `slpkg-4.8.0/configs/slpkg.toml`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.9/tests/test_configs.py` & `slpkg-4.8.0/tests/test_configs.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.9/tests/test_checks.py` & `slpkg-4.8.0/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.9/tests/test_utilities.py` & `slpkg-4.8.0/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.9/tests/test_sbo_queries.py` & `slpkg-4.8.0/tests/test_sbo_queries.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.9/tests/test_colors.py` & `slpkg-4.8.0/tests/test_colors.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.9/tests/test_upgrade.py` & `slpkg-4.8.0/tests/test_upgrade.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.9/tests/test_bin_queries.py` & `slpkg-4.8.0/tests/test_bin_queries.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.9/LICENSE` & `slpkg-4.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.9/install.sh` & `slpkg-4.8.0/install.sh`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.9/ChangeLog.txt` & `slpkg-4.8.0/ChangeLog.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,23 @@
-4.7.9 - 15/04/203
+4.8.0 - 19/04/2023
+Fixed:
+- Counting dependencies for tracking and blacklist packages
+- Resolving dependencies when are blacklisted or not included in the repository
+
+4.7.9 - 15/04/2023
 Updated:
 - For proxies configuration
 - For convert file sizes
 - For packages upgrade
 Fixed:
 - Clear screen when dialog is disabled
 Added:
 - Support to local repositories (Thanks to marav)
 
-4.7.8 - 12/04/203
+4.7.8 - 12/04/2023
 Added:
 - Module to support for Unix shell-style wildcards for blacklist (Thanks to marav)
 - Supports proxies (Thanks to tpiszcze) #160
 Updated:
 - Config file for --reinstall option (Thanks to rizitis)
 - Improve speed
```

### Comparing `slpkg-4.7.9/man/slpkg.1` & `slpkg-4.8.0/man/slpkg.1`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.9/man/slpkg-fr.1` & `slpkg-4.8.0/man/slpkg-fr.1`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.9/completion/slpkg` & `slpkg-4.8.0/completion/slpkg`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.9/slpkg/binaries/required.py` & `slpkg-4.8.0/slpkg/binaries/required.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,64 +1,50 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
-from slpkg.utilities import Utilities
 from slpkg.repositories import Repositories
 
 
 class Required:
     """ Creates a list of dependencies with
     the right order to install. """
 
     def __init__(self, data: dict, name: str):
         __slots__ = 'data', 'name,'
         self.data: dict = data
         self.name: str = name
         self.repos = Repositories()
-        self.utils = Utilities()
 
         self.special_repos: list = [
             self.repos.salixos_repo_name,
+            self.repos.salixos_patches_repo_name,
             self.repos.salixos_extra_repo_name,
             self.repos.slackel_repo_name,
             self.repos.slint_repo_name
         ]
 
         self.repo = self.data[name][11]
 
     def resolve(self) -> list:
         """ Resolve the dependencies. """
-        required: list[str] = self.data[self.name][6].split()
+        required: list[str] = list(self.remove_deps(self.data[self.name][6].split()))
 
         # Resolve dependencies for some special repos.
         if self.repo in self.special_repos:
-            requires: list = []
             for req in required:
-                if req in list(self.data.keys()):
-                    requires.append(req)
-            return requires
-
-        for req in required:
-
-            # Remove requirements that are included as dependencies,
-            # but are not included in the repository.
-            if req not in list(self.data.keys()) or self.utils.blacklist_pattern(req):
-                required.remove(req)
-                continue
-
-            if req:
-                try:
-                    sub_required: list[str] = self.data[req][6].split()
-                except KeyError:
-                    sub_required: list[str] = []
+                if req not in list(self.data.keys()):
+                    required.remove(req)
 
+        else:
+            for req in required:
+                sub_required: list[str] = list(self.remove_deps(self.data[req][6].split()))
                 for sub in sub_required:
                     required.append(sub)
 
-        # Clean for dependencies not in the repository.
-        for dep in required:
-            if dep not in list(self.data.keys()):
-                required.remove(dep)
-
         required.reverse()
-
         return list(dict.fromkeys(required))
+
+    def remove_deps(self, requires):
+        """ Remove requires that not in the repository or blacklisted. """
+        for dep in requires:
+            if dep in list(self.data.keys()):
+                yield dep
```

### Comparing `slpkg-4.7.9/slpkg/binaries/queries.py` & `slpkg-4.8.0/slpkg/binaries/queries.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.9/slpkg/binaries/install.py` & `slpkg-4.8.0/slpkg/binaries/install.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.9/slpkg/install_data.py` & `slpkg-4.8.0/slpkg/install_data.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.9/slpkg/repositories.py` & `slpkg-4.8.0/slpkg/repositories.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.9/slpkg/repo_info.py` & `slpkg-4.8.0/slpkg/repo_info.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.9/slpkg/sbos/queries.py` & `slpkg-4.8.0/slpkg/sbos/queries.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.9/slpkg/sbos/slackbuild.py` & `slpkg-4.8.0/slpkg/sbos/slackbuild.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.9/slpkg/form_configs.py` & `slpkg-4.8.0/slpkg/dialog_configs.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.9/slpkg/update_repository.py` & `slpkg-4.8.0/slpkg/update_repository.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.9/slpkg/progress_bar.py` & `slpkg-4.8.0/slpkg/progress_bar.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.9/slpkg/downloader.py` & `slpkg-4.8.0/slpkg/downloader.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.9/slpkg/models/models.py` & `slpkg-4.8.0/slpkg/models/models.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.9/slpkg/views/view_package.py` & `slpkg-4.8.0/slpkg/views/view_package.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.9/slpkg/views/version.py` & `slpkg-4.8.0/slpkg/views/version.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 class Version:
     """ Print the version. """
 
     def __init__(self):
-        self.version_info: tuple = (4, 7, 9)
+        self.version_info: tuple = (4, 8, 0)
         self.version: str = '{0}.{1}.{2}'.format(*self.version_info)
         self.license: str = 'MIT License'
         self.author: str = 'Dimitris Zlatanidis (dslackw)'
         self.homepage: str = 'https://dslackw.gitlab.io/slpkg'
 
     def view(self) -> None:
         """ Prints the version. """
```

### Comparing `slpkg-4.7.9/slpkg/views/cli_menu.py` & `slpkg-4.8.0/slpkg/views/cli_menu.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.9/slpkg/views/ascii.py` & `slpkg-4.8.0/slpkg/views/ascii.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,15 @@
         self.violet: str = self.color['violet']
         self.endc: str = self.color['endc']
         self.bgreen: str = f'{self.bold}{self.green}'
         self.bred: str = f'{self.bold}{self.red}'
 
     def draw_package_title_box(self, message: str, title: str) -> None:
         """ Drawing package title box. """
+        title = title.title()
         middle_title: int = int((self.columns / 2) - len(title) + 10)
 
         print(f'{self.bgreen}{self.upper_left_corner}' + f'{self.horizontal_line}' * (self.columns - 2) +
               f'{self.upper_right_corner}')
 
         print(f'{self.vertical_line}' + ' ' * middle_title + f'{title}' + ' ' *
               (self.columns - middle_title - len(title) - 2) + f'{self.vertical_line}')
```

### Comparing `slpkg-4.7.9/slpkg/views/help_commands.py` & `slpkg-4.8.0/slpkg/views/help_commands.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.9/slpkg/views/views.py` & `slpkg-4.8.0/slpkg/views/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 
     def view_skipping_packages(self, package: str, version: str) -> None:
         """ Print the skipping packages. """
         print(f'[{self.yellow}Skipping{self.endc}] {package}-{version} {self.red}(already installed){self.endc}')
 
     def build_packages(self, slackbuilds: list, dependencies: list) -> None:
         """ View packages for build only. """
-        self.ascii.draw_package_title_box('The following packages will be build:', 'Build Packages')
+        self.ascii.draw_package_title_box('The following packages will be build:', 'slpkg build packages')
 
         for sbo in slackbuilds:
             self.view_packages(sbo, mode='build')
 
         if dependencies:
             self.ascii.draw_middle_line()
             self.ascii.draw_dependency_line()
@@ -109,17 +109,17 @@
         self.summary(slackbuilds, dependencies, option='build')
 
     def install_packages(self, packages: list, dependencies: list, mode: str) -> None:
         """ View packages for install. """
         if dependencies is None:
             dependencies: list = []
 
-        title: str = 'Slpkg Install Packages'
+        title: str = 'slpkg install packages'
         if mode == 'upgrade':
-            title: str = 'Slpkg Upgrade Packages'
+            title: str = 'slpkg upgrade packages'
 
         self.ascii.draw_package_title_box('The following packages will be installed or upgraded:', title)
 
         for pkg in packages:
             self.view_packages(pkg, mode)
 
         if dependencies:
@@ -131,15 +131,15 @@
 
         self.summary(packages, dependencies, option=mode)
 
     def download_packages(self, slackbuilds: list, directory: Path) -> None:
         """ View downloaded packages. """
         mode = 'download'
 
-        self.ascii.draw_package_title_box('The following packages will be downloaded:', 'Slpkg Download Packages')
+        self.ascii.draw_package_title_box('The following packages will be downloaded:', 'slpkg download packages')
 
         if directory:
             self.download_only: Path = directory
 
         for sbo in slackbuilds:
             self.view_packages(sbo, mode)
 
@@ -158,15 +158,15 @@
 
             if requires:
                 dependencies += requires[0].split()
 
         if dependencies and not self.option_for_resolve_off:
             dependencies: list = self.choose_dependencies_for_remove(list(set(dependencies)))
 
-        self.ascii.draw_package_title_box('The following packages will be removed:', 'Slpkg Remove Packages')
+        self.ascii.draw_package_title_box('The following packages will be removed:', 'slpkg remove packages')
 
         for pkg in pkgs:
             if pkg not in dependencies:
                 self._view_removed(pkg)
 
         if dependencies and not self.option_for_resolve_off:
             self.ascii.draw_middle_line()
```

### Comparing `slpkg-4.7.9/slpkg/checks.py` & `slpkg-4.8.0/slpkg/checks.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.9/slpkg/checksum.py` & `slpkg-4.8.0/slpkg/checksum.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.9/slpkg/dialog_box.py` & `slpkg-4.8.0/slpkg/dialog_box.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.9/slpkg/configs.py` & `slpkg-4.8.0/slpkg/configs.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.9/slpkg/clean_logs.py` & `slpkg-4.8.0/slpkg/clean_logs.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.9/slpkg/utilities.py` & `slpkg-4.8.0/slpkg/utilities.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.9/slpkg/dependees.py` & `slpkg-4.8.0/slpkg/dependees.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.9/slpkg/check_updates.py` & `slpkg-4.8.0/slpkg/check_updates.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.9/slpkg/remove_packages.py` & `slpkg-4.8.0/slpkg/remove_packages.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.9/slpkg/blacklist.py` & `slpkg-4.8.0/slpkg/blacklist.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.9/slpkg/download_only.py` & `slpkg-4.8.0/slpkg/download_only.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.9/slpkg/tracking.py` & `slpkg-4.8.0/slpkg/tracking.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 
         packages: list = self.utils.apply_package_pattern(data, packages)
 
         char: str = f' {self.llc}{self.hl}'
         sp: str = ' ' * 4
 
         for package in packages:
+            how_many: int = 0
             pkg = f'{self.yellow}{package}{self.endc}'
 
             if self.option_for_pkg_version:
 
                 if self.option_for_binaries:
                     version: str = data[package][0]
                 else:
@@ -54,38 +55,36 @@
                 pkg = f'{self.yellow}{package} {version}{self.endc}'
 
             if self.option_for_binaries:
                 requires: list = data[package][6].split()
             else:
                 requires: list = data[package][7].split()
 
-            how_many: int = len(requires)
-
             print(pkg)
             print(char, end='')
 
             if not requires:
                 print(f' {self.cyan}No dependencies{self.endc}')
             else:
                 for i, req in enumerate(requires, start=1):
 
-                    if not self.utils.blacklist_pattern(req):
+                    how_many += 1
 
-                        require: str = f'{self.cyan}{req}{self.endc}'
+                    require: str = f'{self.cyan}{req}{self.endc}'
 
-                        if self.option_for_pkg_version:
+                    if self.option_for_pkg_version:
 
-                            if self.option_for_binaries:
-                                version: str = ' (not included)'
-                                if data.get(req):
-                                    version: str = f' {self.yellow}{data[req][0]}{self.endc}'
-                            else:
-                                version: str = f' {self.yellow}{data[req][2]}{self.endc}'
+                        if self.option_for_binaries:
+                            version: str = ' (not included)'
+                            if data.get(req):
+                                version: str = f' {self.yellow}{data[req][0]}{self.endc}'
+                        else:
+                            version: str = f' {self.yellow}{data[req][2]}{self.endc}'
 
-                            require: str = f'{self.cyan}{req}{self.endc}{version}'
+                        require: str = f'{self.cyan}{req}{self.endc}{version}'
 
-                        if i == 1:
-                            print(f' {require}')
-                        else:
-                            print(f'{sp}{require}')
+                    if i == 1:
+                        print(f' {require}')
+                    else:
+                        print(f'{sp}{require}')
 
             print(f'\n{self.grey}{how_many} dependencies for {package}{self.endc}\n')
```

### Comparing `slpkg-4.7.9/slpkg/main.py` & `slpkg-4.8.0/slpkg/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 from slpkg.search import SearchPackage
 from slpkg.views.cli_menu import Usage
 from slpkg.dialog_box import DialogBox
 from slpkg.views.version import Version
 from slpkg.download_only import Download
 from slpkg.views.views import ViewMessage
 from slpkg.sbos.queries import SBoQueries
-from slpkg.form_configs import FormConfigs
 from slpkg.views.help_commands import Help
 from slpkg.repositories import Repositories
 from slpkg.binaries.install import Packages
+from slpkg.dialog_configs import FormConfigs
 from slpkg.check_updates import CheckUpdates
 from slpkg.sbos.slackbuild import Slackbuilds
 from slpkg.binaries.queries import BinQueries
 from slpkg.logging_config import LoggingConfig
 from slpkg.find_installed import FindInstalled
 from slpkg.views.view_package import ViewPackage
 from slpkg.remove_packages import RemovePackages
@@ -468,24 +468,23 @@
 
                         choices += [(package, f'{split_inst_pkg[1]} -> {repo_ver}', True,
                                      f'Installed: {package}-{split_inst_pkg[1]} Build: {split_inst_pkg[3]} -> '
                                      f'Available: {repo_ver} Build: {repo_build_tag}')]
         else:
             for pkg in packages:
                 for package in repo_packages:
+
                     if pkg in package or pkg == '*':
                         if self.utils.is_option(self.flag_binaries, self.flags):
-                            try:
-                                repo_ver: str = self.data[pkg][0]
-                            except KeyError:
-                                repo_ver: str = ''
+                            repo_ver: str = self.data[package][0]
                             repo: str = self.binary_repo
                         else:
                             repo_ver: str = self.data[package][2]
                             repo: str = self.repos.sbo_enabled_repo_name
+
                         choices += [(package, repo_ver, False, f'Package: {package}-{repo_ver} '
                                                                f'> {repo}')]
 
         if not choices:
             return packages
 
         text: str = f'There are {len(choices)} packages:'
```

### Comparing `slpkg-4.7.9/slpkg/find_installed.py` & `slpkg-4.8.0/slpkg/find_installed.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,38 +10,35 @@
 
     def __init__(self):
         super(Configs, self).__init__()
 
         self.color = self.colour()
         self.utils = Utilities()
 
+        self.matching: list = []
         self.yellow: str = self.color['yellow']
         self.cyan: str = self.color['cyan']
         self.green: str = self.color['green']
         self.blue: str = self.color['blue']
         self.endc: str = self.color['endc']
         self.grey: str = self.color['grey']
 
-        self.installed: dict = self.utils.installed_packages
-
     def find(self, packages: list) -> None:
         """ Find the packages. """
-        matching: list = []
-
         print(f'The list below shows the installed packages '
               f'that contains \'{", ".join([p for p in packages])}\' files:\n')
 
         for pkg in packages:
-            for package in self.installed.values():
+            for package in self.utils.installed_packages.values():
                 if pkg in package or pkg == '*':
-                    matching.append(package)
+                    self.matching.append(package)
 
-        self.matched(matching)
+        self.matched()
 
-    def matched(self, matching: list) -> None:
+    def matched(self) -> None:
         """ Print the matched packages. """
-        if matching:
-            for package in matching:
+        if self.matching:
+            for package in self.matching:
                 print(f'{self.cyan}{package}{self.endc}')
-            print(f'\n{self.grey}Total found {len(matching)} packages.{self.endc}')
+            print(f'\n{self.grey}Total found {len(self.matching)} packages.{self.endc}')
         else:
             print('\nDoes not match any package.\n')
```

### Comparing `slpkg-4.7.9/slpkg/upgrade.py` & `slpkg-4.8.0/slpkg/upgrade.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
                             encoding='utf-8',
                             level=logging.INFO)
 
     def packages(self) -> Generator:
         """ Returns the upgradable packages. """
 
         # Returns the matched packages between two lists.
-        packages: list = list(set(self.utils.installed_packages.keys()) & set(list(self.data.keys())))
+        packages: list = list(set(self.utils.installed_packages.keys()) & set(self.data.keys()))
 
         for pkg in packages:
             if self.is_package_upgradeable(pkg):
                 yield pkg
 
     def is_package_upgradeable(self, name: str) -> bool:
         """ Compares version of packages and returns the maximum. """
```

### Comparing `slpkg-4.7.9/slpkg/search.py` & `slpkg-4.8.0/slpkg/search.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.9/setup.cfg` & `slpkg-4.8.0/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [metadata]
 name = slpkg
-version = 4.7.9
+version = 4.8.0
 license_file = LICENSE
 author = Dimitris Zlatanidis
 author_email = d.zlatanidis@gmail.com
-description = Packaging tool that interacts with the SBo repository
+description = Package manager utility for Slackware Linux.
 long_description = file:README.rst
 url = https://dslackw.gitlab.io/slpkg/
 project_urls = 
 	Source = https://dslackw.gitlab.io/slpkg/
 	Documentation = https://dslackw.gitlab.io/slpkg/
 classifiers = 
 	License :: OSI Approved :: MIT License
```

### Comparing `slpkg-4.7.9/slpkg.egg-info/SOURCES.txt` & `slpkg-4.8.0/slpkg.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 slpkg/check_updates.py
 slpkg/checks.py
 slpkg/checksum.py
 slpkg/clean_logs.py
 slpkg/configs.py
 slpkg/dependees.py
 slpkg/dialog_box.py
+slpkg/dialog_configs.py
 slpkg/download_only.py
 slpkg/downloader.py
 slpkg/find_installed.py
-slpkg/form_configs.py
 slpkg/install_data.py
 slpkg/logging_config.py
 slpkg/main.py
 slpkg/progress_bar.py
 slpkg/remove_packages.py
 slpkg/repo_info.py
 slpkg/repositories.py
```

### Comparing `slpkg-4.7.9/slpkg.egg-info/PKG-INFO` & `slpkg-4.8.0/slpkg.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: slpkg
-Version: 4.7.9
-Summary: Packaging tool that interacts with the SBo repository
+Version: 4.8.0
+Summary: Package manager utility for Slackware Linux.
 Home-page: https://dslackw.gitlab.io/slpkg/
 Author: Dimitris Zlatanidis
 Author-email: d.zlatanidis@gmail.com
 License: UNKNOWN
 Project-URL: Source, https://dslackw.gitlab.io/slpkg/
 Project-URL: Documentation, https://dslackw.gitlab.io/slpkg/
 Platform: UNKNOWN
```

### Comparing `slpkg-4.7.9/README.md` & `slpkg-4.8.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -26,27 +26,46 @@
 It automatically calculates dependencies and figures out what things need to happen to install packages.
 Slpkg makes it easier to manage groups of machines without the need for manual updates.
 Slpkg works in accordance with the standards of the [slackbuilds.org](https://www.slackbuilds.org) organization to build packages.
 It also uses the Slackware Linux instructions for installing, upgrading or removing packages.
 
 ### Screenshots
 
+```
+$ slpkg repo-info
+```
 <img src="https://gitlab.com/dslackw/images/raw/master/slpkg/slpkg_repo_info.png" width="700">
+
+```
+$ slpkg install audacity --bin-repo=alien
+```
 <img src="https://gitlab.com/dslackw/images/raw/master/slpkg/slpkg_install.png" width="700">
 <img src="https://gitlab.com/dslackw/images/raw/master/slpkg/slpkg_install_done.png" width="700">
+
+```
+$ slpkg remove audacity
+```
 <img src="https://gitlab.com/dslackw/images/raw/master/slpkg/slpkg_remove.png" width="700">
 <img src="https://gitlab.com/dslackw/images/raw/master/slpkg/slpkg_remove_done.png" width="700">
+
+```
+$ slpkg dependees --pkg-version --full-reverse greenlet
+```
 <img src="https://gitlab.com/dslackw/images/raw/master/slpkg/slpkg_dependees.png" width="700">
+
+```
+$ slpkg tracking --pkg-version slpkg Flask awscli
+```
 <img src="https://gitlab.com/dslackw/images/raw/master/slpkg/slpkg_tracking.png" width="700">
 
 ### Installation
 
 ```
-$ tar xvf slpkg-4.7.9.tar.gz
-$ cd slpkg-4.7.9
+$ tar xvf slpkg-4.8.0.tar.gz
+$ cd slpkg-4.8.0
 $ ./install.sh
 ```
 
 ### Requirements
 
 ```
 SQLAlchemy >= 1.4.46
@@ -142,16 +161,14 @@
 
 You can install a whole repository with the command:
 
 ```
     $ slpkg install '*' --bin-repo=<repository_name> --resolve-off
 ```
 
-Note: Apply the option '--resolve-off' to speed up the process, if the repository has no references to the dependencies.
-
 To remove a package with the dependencies:
 
 ```
     $ slpkg remove <package_name>
 ```
 
 If you want to search a package from all binaries repositories, run:
```

### Comparing `slpkg-4.7.9/tools/gen_sbo_txt.sh` & `slpkg-4.8.0/tools/gen_sbo_txt.sh`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.9/bin/slpkg_new-configs` & `slpkg-4.8.0/bin/slpkg_new-configs`

 * *Files identical despite different names*

