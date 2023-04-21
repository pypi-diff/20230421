# Comparing `tmp/tuxmake-1.8.0.tar.gz` & `tmp/tuxmake-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuxmake-1.8.0.tar", last modified: Tue Oct 25 12:50:27 2022, max compression
+gzip compressed data, was "tuxmake-1.9.0.tar", last modified: Tue Jan 17 12:59:35 2023, max compression
```

## Comparing `tuxmake-1.8.0.tar` & `tuxmake-1.9.0.tar`

### file list

```diff
@@ -1,240 +1,240 @@
--rw-r--r--   0        0        0      207 2022-01-17 18:20:24.932316 tuxmake-1.8.0/.ackrc
--rw-r--r--   0        0        0       30 2020-07-21 21:47:43.351426 tuxmake-1.8.0/.flake8
--rw-r--r--   0        0        0      105 2021-02-24 19:11:31.330544 tuxmake-1.8.0/.gitignore
--rw-r--r--   0        0        0     6392 2022-05-25 17:56:05.985268 tuxmake-1.8.0/.gitlab-ci.yml
--rw-r--r--   0        0        0     1054 2020-07-21 21:47:43.351426 tuxmake-1.8.0/LICENSE
--rw-r--r--   0        0        0     3191 2022-10-17 11:45:50.138618 tuxmake-1.8.0/Makefile
--rw-r--r--   0        0        0     4941 2021-03-10 20:07:53.156597 tuxmake-1.8.0/README.md
--rw-r--r--   0        0        0      151 2022-10-25 12:50:21.851931 tuxmake-1.8.0/debian/changelog
--rw-r--r--   0        0        0      878 2022-05-04 19:27:44.019045 tuxmake-1.8.0/debian/control
--rw-r--r--   0        0        0      100 2021-02-24 19:11:31.334544 tuxmake-1.8.0/debian/gbp.conf
--rwxr-xr-x   0        0        0      539 2022-05-04 19:27:44.019045 tuxmake-1.8.0/debian/rules
--rw-r--r--   0        0        0       12 2021-02-19 19:03:40.336999 tuxmake-1.8.0/debian/source/format
--rw-r--r--   0        0        0       24 2021-02-24 19:11:31.334544 tuxmake-1.8.0/debian/tuxmake.bash-completion
--rw-r--r--   0        0        0       10 2021-02-19 19:03:40.336999 tuxmake-1.8.0/debian/tuxmake.manpages
--rw-r--r--   0        0        0      194 2021-02-19 19:03:40.336999 tuxmake-1.8.0/debian/watch
--rw-r--r--   0        0        0     1825 2022-05-05 19:32:50.521489 tuxmake-1.8.0/docs/architectures.md
--rw-r--r--   0        0        0      342 2021-06-11 19:19:48.364575 tuxmake-1.8.0/docs/chat.md
--rw-r--r--   0        0        0     3370 2021-02-24 19:11:31.334544 tuxmake-1.8.0/docs/code-of-conduct.md
--rw-r--r--   0        0        0      657 2021-03-01 19:50:07.790172 tuxmake-1.8.0/docs/container-about.md
--rw-r--r--   0        0        0      503 2021-03-01 19:50:07.790172 tuxmake-1.8.0/docs/container-usage.md
--rw-r--r--   0        0        0     1828 2021-03-10 21:40:08.629900 tuxmake-1.8.0/docs/contributing.md
--rw-r--r--   0        0        0     2352 2022-01-17 18:20:24.932316 tuxmake-1.8.0/docs/curated_containers.md
--rw-r--r--   0        0        0     5670 2021-05-27 12:38:47.396728 tuxmake-1.8.0/docs/custom_containers.md
--rw-r--r--   0        0        0      133 2021-02-19 19:03:40.336999 tuxmake-1.8.0/docs/extra.css
--rw-r--r--   0        0        0      828 2021-03-29 15:20:53.428834 tuxmake-1.8.0/docs/install-deb.md
--rw-r--r--   0        0        0      417 2022-01-17 18:20:24.932316 tuxmake-1.8.0/docs/install-pypi.md
--rw-r--r--   0        0        0      767 2021-06-24 17:17:19.210224 tuxmake-1.8.0/docs/install-rpm.md
--rw-r--r--   0        0        0     1738 2022-05-05 20:05:11.550147 tuxmake-1.8.0/docs/kconfig.md
-lrwxr-xr-x   0        0        0        0 2021-02-19 19:03:40.336999 tuxmake-1.8.0/docs/license.md -> ../LICENSE
--rw-r--r--   0        0        0     5648 2022-06-30 12:57:16.723455 tuxmake-1.8.0/docs/metadata.md
--rw-r--r--   0        0        0      236 2021-02-19 19:03:40.336999 tuxmake-1.8.0/docs/mkautodoc.css
--rw-r--r--   0        0        0     1530 2021-02-24 19:11:31.334544 tuxmake-1.8.0/docs/packaging.md
--rw-r--r--   0        0        0      411 2022-03-02 15:23:17.692529 tuxmake-1.8.0/docs/python.md
--rw-r--r--   0        0        0      872 2022-05-04 19:27:44.019045 tuxmake-1.8.0/docs/python_runtime.md
--rw-r--r--   0        0        0     3364 2021-05-27 18:01:05.522833 tuxmake-1.8.0/docs/reproducible_builds.md
--rw-r--r--   0        0        0      718 2022-05-04 19:27:44.019045 tuxmake-1.8.0/docs/resources.md
--rw-r--r--   0        0        0      564 2021-04-01 18:05:11.035171 tuxmake-1.8.0/docs/run-uninstalled.md
--rw-r--r--   0        0        0     2749 2021-07-12 19:20:00.087118 tuxmake-1.8.0/docs/runtimes.md
--rw-r--r--   0        0        0     5115 2022-05-04 19:27:44.019045 tuxmake-1.8.0/docs/targets.md
--rw-r--r--   0        0        0     1601 2021-07-19 17:52:53.967073 tuxmake-1.8.0/docs/toolchains.md
--rw-r--r--   0        0        0     2001 2021-02-19 19:03:40.336999 tuxmake-1.8.0/docs/tuxmake.svg
--rw-r--r--   0        0        0     3585 2021-02-24 19:11:31.334544 tuxmake-1.8.0/docs/tuxmake_full.svg
--rw-r--r--   0        0        0     5493 2021-02-19 19:03:40.336999 tuxmake-1.8.0/docs/tuxmake_icon.svg
--rw-r--r--   0        0        0      568 2021-02-24 19:11:31.334544 tuxmake-1.8.0/docs/wrappers.md
--rw-r--r--   0        0        0     1457 2022-05-04 19:27:44.019045 tuxmake-1.8.0/mkdocs.yml
--rw-r--r--   0        0        0      397 2021-02-19 19:03:40.336999 tuxmake-1.8.0/pyproject.toml
--rw-r--r--   0        0        0      323 2021-02-19 19:03:40.336999 tuxmake-1.8.0/requirements-dev.txt
--rwxr-xr-x   0        0        0      123 2020-10-01 18:26:08.493036 tuxmake-1.8.0/run
--rw-r--r--   0        0        0      489 2021-02-19 19:03:40.336999 tuxmake-1.8.0/scripts/cli2md.py
--rwxr-xr-x   0        0        0      493 2021-02-19 19:03:40.336999 tuxmake-1.8.0/scripts/cli2md.sh
--rwxr-xr-x   0        0        0      205 2021-02-19 19:03:40.336999 tuxmake-1.8.0/scripts/cli2rst.sh
--rwxr-xr-x   0        0        0      896 2021-03-29 15:20:53.428834 tuxmake-1.8.0/scripts/package-repos
--rwxr-xr-x   0        0        0      166 2021-02-19 19:03:40.336999 tuxmake-1.8.0/scripts/readme2index.sh
--rwxr-xr-x   0        0        0     1859 2022-05-27 12:36:03.982287 tuxmake-1.8.0/scripts/release
--rwxr-xr-x   0        0        0      473 2021-02-19 19:03:40.336999 tuxmake-1.8.0/scripts/run-tests
--rwxr-xr-x   0        0        0      260 2021-02-24 19:11:31.338544 tuxmake-1.8.0/scripts/target-deps
--rw-r--r--   0        0        0     1990 2022-05-05 15:08:17.541771 tuxmake-1.8.0/scripts/test_doc.py
--rw-r--r--   0        0        0       63 2022-05-04 19:27:44.019045 tuxmake-1.8.0/support/docker/.gitignore
--rw-r--r--   0        0        0      821 2021-07-12 19:20:00.087118 tuxmake-1.8.0/support/docker/Dockerfile.arc
--rw-r--r--   0        0        0     2302 2022-10-22 00:54:59.405410 tuxmake-1.8.0/support/docker/Dockerfile.base
--rw-r--r--   0        0        0     6708 2022-10-22 11:56:12.142648 tuxmake-1.8.0/support/docker/Dockerfile.build
--rw-r--r--   0        0        0     1323 2021-07-20 18:09:57.480336 tuxmake-1.8.0/support/docker/Dockerfile.ci
--rw-r--r--   0        0        0      578 2022-10-22 11:56:12.134649 tuxmake-1.8.0/support/docker/Dockerfile.clang-android
--rw-r--r--   0        0        0     3366 2022-05-25 17:56:12.829200 tuxmake-1.8.0/support/docker/Makefile
--rw-r--r--   0        0        0     4299 2022-05-04 19:27:44.023045 tuxmake-1.8.0/support/docker/README.md
--rw-r--r--   0        0        0      120 2021-07-12 19:20:00.091118 tuxmake-1.8.0/support/docker/arc-gcc-8.sha256sum
--rw-r--r--   0        0        0      123 2021-07-12 19:20:00.091118 tuxmake-1.8.0/support/docker/arc-gcc-9.sha256sum
--rw-r--r--   0        0        0      101 2022-05-04 19:27:44.023045 tuxmake-1.8.0/support/docker/conf/pinning-bullseye
--rwxr-xr-x   0        0        0     8585 2022-10-22 11:56:12.142648 tuxmake-1.8.0/support/docker/configure
--rwxr-xr-x   0        0        0     2911 2022-05-04 19:27:44.023045 tuxmake-1.8.0/support/docker/gen-gitlab-ci
--rwxr-xr-x   0        0        0      312 2021-07-12 19:20:00.091118 tuxmake-1.8.0/support/docker/get-arch-images
--rwxr-xr-x   0        0        0      137 2021-07-12 19:20:00.091118 tuxmake-1.8.0/support/docker/list-images
--rw-r--r--   0        0        0     3253 2022-05-04 19:27:44.023045 tuxmake-1.8.0/support/docker/test/test_configure.sh
--rwxr-xr-x   0        0        0      259 2022-05-04 19:27:44.023045 tuxmake-1.8.0/support/docker/test/test_gitlab_ci.sh
--rw-r--r--   0        0        0     2720 2022-05-04 19:27:44.023045 tuxmake-1.8.0/support/docker/tuxmake-ci-images.yml
--rw-r--r--   0        0        0    20585 2022-08-10 19:17:24.844678 tuxmake-1.8.0/support/docker/tuxmake-images.yml
--rw-r--r--   0        0        0        0 2020-07-21 21:47:43.355426 tuxmake-1.8.0/test/__init__.py
--rw-r--r--   0        0        0     2018 2022-05-04 19:27:44.023045 tuxmake-1.8.0/test/conftest.py
--rw-r--r--   0        0        0       15 2020-07-21 21:47:43.355426 tuxmake-1.8.0/test/fakelinux/Kbuild
--rw-r--r--   0        0        0       15 2020-07-21 21:47:43.355426 tuxmake-1.8.0/test/fakelinux/Kconfig
--rw-r--r--   0        0        0     6608 2022-05-25 17:15:42.157651 tuxmake-1.8.0/test/fakelinux/Makefile
-lrwxr-xr-x   0        0        0        0 2022-05-04 19:27:44.027045 tuxmake-1.8.0/test/fakelinux/arch/aarch64 -> arm64
--rw-r--r--   0        0        0       55 2022-05-04 19:27:44.027045 tuxmake-1.8.0/test/fakelinux/arch/arc/Makefile
--rw-r--r--   0        0        0       50 2022-05-04 19:27:44.027045 tuxmake-1.8.0/test/fakelinux/arch/arm/Makefile
--rw-r--r--   0        0        0        0 2022-10-17 11:45:50.138618 tuxmake-1.8.0/test/fakelinux/arch/arm/boot/dts/.gitkeep
--rw-r--r--   0        0        0       99 2022-05-04 19:27:44.027045 tuxmake-1.8.0/test/fakelinux/arch/arm64/Makefile
--rw-r--r--   0        0        0        0 2022-10-13 17:37:37.027379 tuxmake-1.8.0/test/fakelinux/arch/arm64/boot/dts/.gitkeep
-lrwxr-xr-x   0        0        0        0 2022-05-04 19:27:44.027045 tuxmake-1.8.0/test/fakelinux/arch/armv8l -> arm
--rw-r--r--   0        0        0       54 2022-05-04 19:27:44.027045 tuxmake-1.8.0/test/fakelinux/arch/hexagon/Makefile
--rw-r--r--   0        0        0       51 2022-05-04 19:27:44.027045 tuxmake-1.8.0/test/fakelinux/arch/i386/Makefile
-lrwxr-xr-x   0        0        0        0 2022-05-04 19:27:44.027045 tuxmake-1.8.0/test/fakelinux/arch/i686 -> i386
--rw-r--r--   0        0        0       56 2022-05-04 19:27:44.027045 tuxmake-1.8.0/test/fakelinux/arch/mips/Makefile
--rw-r--r--   0        0        0       54 2022-05-04 19:27:44.027045 tuxmake-1.8.0/test/fakelinux/arch/parisc/Makefile
--rw-r--r--   0        0        0       54 2022-05-04 19:27:44.027045 tuxmake-1.8.0/test/fakelinux/arch/powerpc/Makefile
--rw-r--r--   0        0        0       56 2022-05-04 19:27:44.027045 tuxmake-1.8.0/test/fakelinux/arch/riscv/Makefile
--rw-r--r--   0        0        0       33 2022-05-04 19:27:44.027045 tuxmake-1.8.0/test/fakelinux/arch/s390/Makefile
--rw-r--r--   0        0        0       49 2022-05-04 19:27:44.027045 tuxmake-1.8.0/test/fakelinux/arch/sh/Makefile
--rw-r--r--   0        0        0       52 2022-05-04 19:27:44.027045 tuxmake-1.8.0/test/fakelinux/arch/sparc/Makefile
--rw-r--r--   0        0        0       51 2022-05-04 19:27:44.027045 tuxmake-1.8.0/test/fakelinux/arch/x86_64/Makefile
--rw-r--r--   0        0        0       31 2022-05-05 20:05:11.550147 tuxmake-1.8.0/test/fakelinux/config/test.config
--rw-r--r--   0        0        0      100 2021-02-19 19:03:40.340999 tuxmake-1.8.0/test/fakelinux/scripts/kconfig/config.c
--rwxr-xr-x   0        0        0      696 2021-10-04 17:33:12.234846 tuxmake-1.8.0/test/fakelinux/scripts/kconfig/merge_config.sh
--rw-r--r--   0        0        0       30 2022-01-17 18:20:24.936317 tuxmake-1.8.0/test/fakelinux/tools/testing/selftests/bpf/config
--rw-r--r--   0        0        0      246 2022-01-12 11:59:55.925204 tuxmake-1.8.0/test/fakelinux/vmlinux.c
-lrwxr-xr-x   0        0        0        0 2021-02-19 19:03:40.340999 tuxmake-1.8.0/test/integration-slow/docker -> runtime
-lrwxr-xr-x   0        0        0        0 2021-02-19 19:03:40.340999 tuxmake-1.8.0/test/integration-slow/docker-local -> runtime
--rwxr-xr-x   0        0        0     3394 2021-02-19 19:03:40.340999 tuxmake-1.8.0/test/integration-slow/matrix
-lrwxr-xr-x   0        0        0        0 2021-02-19 19:03:40.340999 tuxmake-1.8.0/test/integration-slow/podman -> runtime
-lrwxr-xr-x   0        0        0        0 2021-02-19 19:03:40.340999 tuxmake-1.8.0/test/integration-slow/podman-local -> runtime
--rwxr-xr-x   0        0        0      137 2021-02-19 19:03:40.340999 tuxmake-1.8.0/test/integration-slow/runtime
--rwxr-xr-x   0        0        0       45 2021-05-27 18:01:05.522833 tuxmake-1.8.0/test/integration/auxbin/hostname
--rwxr-xr-x   0        0        0      159 2021-05-07 12:01:31.522844 tuxmake-1.8.0/test/integration/auxbin/which
--rwxr-xr-x   0        0        0       45 2021-05-27 18:01:05.522833 tuxmake-1.8.0/test/integration/auxbin/whoami
--rwxr-xr-x   0        0        0     1336 2022-05-04 19:27:44.027045 tuxmake-1.8.0/test/integration/bin/tuxcmd
-lrwxr-xr-x   0        0        0        0 2021-02-19 19:03:40.340999 tuxmake-1.8.0/test/integration/bin/tuxmake -> ../../../run
--rwxr-xr-x   0        0        0     8599 2022-10-17 11:45:50.142619 tuxmake-1.8.0/test/integration/fakelinux
--rwxr-xr-x   0        0        0      631 2022-05-25 17:56:05.985268 tuxmake-1.8.0/test/integration/runtimes-print-support-matrix
--rw-r--r--   0        0        0     2025 2022-05-04 19:27:44.031045 tuxmake-1.8.0/test/integration/test_helper.sh
--rw-r--r--   0        0        0      120 2021-02-19 19:03:40.340999 tuxmake-1.8.0/test/logs/case.log
--rw-r--r--   0        0        0      680 2021-02-19 19:03:40.340999 tuxmake-1.8.0/test/logs/compiler-lacks.log
--rw-r--r--   0        0        0      720 2021-02-19 19:03:40.340999 tuxmake-1.8.0/test/logs/compiler-not-found.log
--rw-r--r--   0        0        0      413 2021-02-19 19:03:40.340999 tuxmake-1.8.0/test/logs/garbage.log
--rw-r--r--   0        0        0      748 2021-02-19 19:03:40.340999 tuxmake-1.8.0/test/logs/invalid-config.log
--rw-r--r--   0        0        0    28772 2021-02-19 19:03:40.340999 tuxmake-1.8.0/test/logs/no-rule-to-make-target.log
--rw-r--r--   0        0        0     3289 2021-02-19 19:03:40.340999 tuxmake-1.8.0/test/logs/no-such-file-or-directory.log
--rw-r--r--   0        0        0       45 2021-02-19 19:03:40.340999 tuxmake-1.8.0/test/logs/non-utf8.log
--rw-r--r--   0        0        0       32 2022-06-30 12:57:16.727455 tuxmake-1.8.0/test/logs/simple.log
--rw-r--r--   0        0        0     2320 2022-10-17 11:45:50.146619 tuxmake-1.8.0/test/test_arch.py
--rw-r--r--   0        0        0    39591 2022-10-17 11:45:50.146619 tuxmake-1.8.0/test/test_build.py
--rw-r--r--   0        0        0      619 2021-05-17 18:48:25.275796 tuxmake-1.8.0/test/test_build_info.py
--rw-r--r--   0        0        0      351 2021-05-17 18:48:25.275796 tuxmake-1.8.0/test/test_cache.py
--rw-r--r--   0        0        0    15778 2021-11-18 18:24:55.045970 tuxmake-1.8.0/test/test_cli.py
--rw-r--r--   0        0        0     2779 2021-05-26 17:31:06.703699 tuxmake-1.8.0/test/test_cmdline.py
--rw-r--r--   0        0        0      851 2022-05-04 19:27:44.031045 tuxmake-1.8.0/test/test_configurable_object.py
--rw-r--r--   0        0        0      306 2021-06-24 17:17:19.214223 tuxmake-1.8.0/test/test_deprecated.py
--rw-r--r--   0        0        0      492 2021-05-17 18:48:25.275796 tuxmake-1.8.0/test/test_exceptions.py
--rw-r--r--   0        0        0      735 2022-06-30 12:57:16.727455 tuxmake-1.8.0/test/test_log_parser.py
--rw-r--r--   0        0        0      372 2021-05-17 18:48:25.275796 tuxmake-1.8.0/test/test_main.py
--rw-r--r--   0        0        0     5346 2021-07-12 17:35:10.502137 tuxmake-1.8.0/test/test_metadata.py
--rw-r--r--   0        0        0     1340 2021-05-17 18:48:25.275796 tuxmake-1.8.0/test/test_output.py
--rw-r--r--   0        0        0    14776 2022-09-09 02:34:13.381994 tuxmake-1.8.0/test/test_runtime.py
--rw-r--r--   0        0        0     3847 2022-05-04 19:27:44.031045 tuxmake-1.8.0/test/test_target.py
--rw-r--r--   0        0        0     1399 2021-05-17 18:48:25.275796 tuxmake-1.8.0/test/test_toolchain.py
--rw-r--r--   0        0        0     2412 2022-05-04 19:27:44.031045 tuxmake-1.8.0/test/test_utils.py
--rw-r--r--   0        0        0     1602 2022-05-04 19:27:44.031045 tuxmake-1.8.0/test/test_wrapper.py
--rw-r--r--   0        0        0     1050 2022-10-25 12:50:21.855931 tuxmake-1.8.0/tuxmake.PKGBUILD
--rw-r--r--   0        0        0     3982 2021-03-10 21:40:08.629900 tuxmake-1.8.0/tuxmake.rst
--rw-r--r--   0        0        0     1614 2022-10-25 12:50:21.843931 tuxmake-1.8.0/tuxmake.spec
--rw-r--r--   0        0        0       67 2022-10-25 12:50:21.831931 tuxmake-1.8.0/tuxmake/__init__.py
--rw-r--r--   0        0        0       96 2020-10-30 19:36:51.001129 tuxmake-1.8.0/tuxmake/__main__.py
--rw-r--r--   0        0        0     1540 2022-10-17 11:45:50.146619 tuxmake-1.8.0/tuxmake/arch.py
-lrwxr-xr-x   0        0        0        0 2021-01-21 21:38:43.327256 tuxmake-1.8.0/tuxmake/arch/aarch64.ini -> arm64.ini
-lrwxr-xr-x   0        0        0        0 2021-01-21 21:38:37.291321 tuxmake-1.8.0/tuxmake/arch/amd64.ini -> x86_64.ini
--rw-r--r--   0        0        0      124 2021-02-19 19:03:40.340999 tuxmake-1.8.0/tuxmake/arch/arc.ini
--rw-r--r--   0        0        0      131 2022-05-04 19:35:12.786595 tuxmake-1.8.0/tuxmake/arch/arm.ini
--rw-r--r--   0        0        0      329 2022-05-27 12:32:42.965088 tuxmake-1.8.0/tuxmake/arch/arm64.ini
-lrwxr-xr-x   0        0        0        0 2022-05-05 19:32:50.521489 tuxmake-1.8.0/tuxmake/arch/armel.ini -> armv5.ini
-lrwxr-xr-x   0        0        0        0 2022-05-05 19:32:50.521489 tuxmake-1.8.0/tuxmake/arch/armhf.ini -> arm.ini
--rw-r--r--   0        0        0      130 2022-05-05 19:32:50.521489 tuxmake-1.8.0/tuxmake/arch/armv5.ini
-lrwxr-xr-x   0        0        0        0 2021-07-19 17:52:53.971073 tuxmake-1.8.0/tuxmake/arch/armv8l.ini -> arm.ini
--rw-r--r--   0        0        0      200 2021-05-13 18:52:26.703789 tuxmake-1.8.0/tuxmake/arch/hexagon.ini
--rw-r--r--   0        0        0      143 2022-10-17 11:45:50.146619 tuxmake-1.8.0/tuxmake/arch/i386.ini
-lrwxr-xr-x   0        0        0        0 2021-07-19 20:15:14.466498 tuxmake-1.8.0/tuxmake/arch/i686.ini -> i386.ini
--rw-r--r--   0        0        0      131 2021-09-24 13:43:57.410569 tuxmake-1.8.0/tuxmake/arch/mips.ini
--rw-r--r--   0        0        0      137 2021-05-13 14:19:16.567361 tuxmake-1.8.0/tuxmake/arch/openrisc.ini
--rw-r--r--   0        0        0      133 2021-02-19 19:03:40.344999 tuxmake-1.8.0/tuxmake/arch/parisc.ini
--rw-r--r--   0        0        0      141 2021-05-27 12:38:47.400728 tuxmake-1.8.0/tuxmake/arch/powerpc.ini
--rw-r--r--   0        0        0      135 2021-05-27 12:38:47.400728 tuxmake-1.8.0/tuxmake/arch/riscv.ini
--rw-r--r--   0        0        0      130 2021-02-19 19:03:40.344999 tuxmake-1.8.0/tuxmake/arch/s390.ini
--rw-r--r--   0        0        0      123 2021-02-19 19:03:40.344999 tuxmake-1.8.0/tuxmake/arch/sh.ini
--rw-r--r--   0        0        0      133 2021-05-27 12:38:47.400728 tuxmake-1.8.0/tuxmake/arch/sparc.ini
--rw-r--r--   0        0        0      182 2021-05-13 14:19:16.567361 tuxmake-1.8.0/tuxmake/arch/um.ini
--rw-r--r--   0        0        0      146 2022-10-17 11:45:50.150619 tuxmake-1.8.0/tuxmake/arch/x86_64.ini
--rw-r--r--   0        0        0    24585 2022-10-17 11:45:50.150619 tuxmake-1.8.0/tuxmake/build.py
--rw-r--r--   0        0        0      967 2022-05-04 19:27:44.031045 tuxmake-1.8.0/tuxmake/build_utils.py
--rw-r--r--   0        0        0      406 2021-02-24 19:11:31.346543 tuxmake-1.8.0/tuxmake/cache.py
--rw-r--r--   0        0        0     5866 2022-05-04 19:27:44.031045 tuxmake-1.8.0/tuxmake/cli.py
--rw-r--r--   0        0        0    13684 2022-05-04 19:27:44.031045 tuxmake-1.8.0/tuxmake/cmdline.py
--rw-r--r--   0        0        0     2470 2022-05-04 19:27:44.035045 tuxmake-1.8.0/tuxmake/config.py
--rw-r--r--   0        0        0      263 2021-06-24 17:17:19.214223 tuxmake-1.8.0/tuxmake/deprecated.py
--rw-r--r--   0        0        0     2460 2022-05-04 19:27:44.035045 tuxmake-1.8.0/tuxmake/exceptions.py
--rw-r--r--   0        0        0      632 2022-06-30 12:57:16.727455 tuxmake-1.8.0/tuxmake/log.py
--rw-r--r--   0        0        0      580 2021-06-24 17:17:19.214223 tuxmake-1.8.0/tuxmake/logging.py
--rw-r--r--   0        0        0     1361 2022-05-04 19:27:44.035045 tuxmake-1.8.0/tuxmake/metadata.pl
--rw-r--r--   0        0        0     5281 2022-05-04 19:27:44.035045 tuxmake-1.8.0/tuxmake/metadata.py
--rw-r--r--   0        0        0      654 2021-03-01 19:50:07.794172 tuxmake-1.8.0/tuxmake/metadata/artifacts.ini
--rw-r--r--   0        0        0      504 2020-10-01 18:26:08.513036 tuxmake-1.8.0/tuxmake/metadata/ccache.ini
--rw-r--r--   0        0        0      134 2020-10-01 18:26:08.513036 tuxmake-1.8.0/tuxmake/metadata/compiler.ini
--rw-r--r--   0        0        0      257 2020-10-01 18:26:08.513036 tuxmake-1.8.0/tuxmake/metadata/git.ini
--rw-r--r--   0        0        0      237 2021-06-28 18:22:58.491678 tuxmake-1.8.0/tuxmake/metadata/hardware.ini
--rw-r--r--   0        0        0      317 2022-05-25 17:15:42.157651 tuxmake-1.8.0/tuxmake/metadata/os.ini
--rw-r--r--   0        0        0       89 2021-06-28 18:35:34.379417 tuxmake-1.8.0/tuxmake/metadata/resources.ini
--rw-r--r--   0        0        0      352 2020-10-01 18:26:08.513036 tuxmake-1.8.0/tuxmake/metadata/sccache.ini
--rw-r--r--   0        0        0      217 2022-01-17 18:20:24.940317 tuxmake-1.8.0/tuxmake/metadata/source.ini
--rw-r--r--   0        0        0       96 2021-02-19 19:03:40.344999 tuxmake-1.8.0/tuxmake/metadata/system_map.ini
--rw-r--r--   0        0        0     1614 2022-05-04 19:27:44.035045 tuxmake-1.8.0/tuxmake/metadata/tools.ini
--rw-r--r--   0        0        0      208 2020-10-01 18:26:08.513036 tuxmake-1.8.0/tuxmake/metadata/uname.ini
--rw-r--r--   0        0        0      339 2021-02-19 19:03:40.344999 tuxmake-1.8.0/tuxmake/metadata/vmlinux.ini
--rw-r--r--   0        0        0      524 2022-01-17 18:20:24.940317 tuxmake-1.8.0/tuxmake/output.py
--rw-r--r--   0        0        0    19424 2022-09-09 02:34:13.385994 tuxmake-1.8.0/tuxmake/runtime.py
--rwxr-xr-x   0        0        0     5810 2022-08-10 19:17:24.844678 tuxmake-1.8.0/tuxmake/runtime/bin/tuxmake-check-environment
--rwxr-xr-x   0        0        0      802 2022-05-04 19:27:44.035045 tuxmake-1.8.0/tuxmake/runtime/bin/tuxmake-logger
--rwxr-xr-x   0        0        0     2515 2022-05-04 19:27:44.035045 tuxmake-1.8.0/tuxmake/runtime/bin/tuxmake-run-offline
-lrwxr-xr-x   0        0        0        0 2021-02-19 19:03:40.344999 tuxmake-1.8.0/tuxmake/runtime/docker-local.ini -> docker.ini
--rw-r--r--   0        0        0     7493 2022-10-07 21:33:25.730135 tuxmake-1.8.0/tuxmake/runtime/docker.ini
--rw-r--r--   0        0        0        0 2020-10-01 18:26:08.513036 tuxmake-1.8.0/tuxmake/runtime/null.ini
-lrwxr-xr-x   0        0        0        0 2021-02-19 19:03:40.344999 tuxmake-1.8.0/tuxmake/runtime/podman-local.ini -> docker.ini
-lrwxr-xr-x   0        0        0        0 2021-02-19 19:03:40.344999 tuxmake-1.8.0/tuxmake/runtime/podman.ini -> docker.ini
--rw-r--r--   0        0        0     8710 2022-05-05 20:05:11.550147 tuxmake-1.8.0/tuxmake/target.py
--rw-r--r--   0        0        0       93 2022-05-04 19:27:44.035045 tuxmake-1.8.0/tuxmake/target/clang-analyzer.ini
--rw-r--r--   0        0        0      246 2021-05-07 12:01:31.522844 tuxmake-1.8.0/tuxmake/target/config.ini
--rw-r--r--   0        0        0      332 2022-05-04 19:27:44.035045 tuxmake-1.8.0/tuxmake/target/cpupower.ini
--rw-r--r--   0        0        0      171 2022-05-04 19:27:44.035045 tuxmake-1.8.0/tuxmake/target/debugkernel.ini
--rw-r--r--   0        0        0      109 2022-01-26 20:50:21.366112 tuxmake-1.8.0/tuxmake/target/default.ini
--rw-r--r--   0        0        0      651 2022-10-17 11:45:50.150619 tuxmake-1.8.0/tuxmake/target/dtbs-legacy.ini
--rw-r--r--   0        0        0      482 2022-10-17 11:45:50.150619 tuxmake-1.8.0/tuxmake/target/dtbs.ini
--rw-r--r--   0        0        0      320 2022-05-04 19:27:44.035045 tuxmake-1.8.0/tuxmake/target/headers.ini
--rw-r--r--   0        0        0      154 2021-02-24 19:11:31.354543 tuxmake-1.8.0/tuxmake/target/kernel.ini
--rw-r--r--   0        0        0     1307 2022-05-04 19:27:44.035045 tuxmake-1.8.0/tuxmake/target/kselftest-bpf.ini
--rw-r--r--   0        0        0      238 2022-05-04 19:27:44.035045 tuxmake-1.8.0/tuxmake/target/kselftest-merge.ini
--rw-r--r--   0        0        0      339 2022-05-04 19:27:44.035045 tuxmake-1.8.0/tuxmake/target/kselftest.ini
--rw-r--r--   0        0        0      399 2022-05-04 19:27:44.035045 tuxmake-1.8.0/tuxmake/target/modules.ini
--rw-r--r--   0        0        0      296 2022-05-04 19:27:44.035045 tuxmake-1.8.0/tuxmake/target/perf.ini
--rw-r--r--   0        0        0      165 2021-06-17 12:25:40.231629 tuxmake-1.8.0/tuxmake/target/targz-pkg.ini
--rw-r--r--   0        0        0      270 2021-02-24 19:11:31.354543 tuxmake-1.8.0/tuxmake/target/xipkernel.ini
--rw-r--r--   0        0        0     1367 2021-11-18 21:30:50.567869 tuxmake-1.8.0/tuxmake/toolchain.py
--rw-r--r--   0        0        0      111 2021-02-19 19:03:40.344999 tuxmake-1.8.0/tuxmake/toolchain/clang.ini
--rw-r--r--   0        0        0       98 2021-11-18 21:34:09.033790 tuxmake-1.8.0/tuxmake/toolchain/gcc.ini
--rw-r--r--   0        0        0      104 2021-11-18 21:34:09.033790 tuxmake-1.8.0/tuxmake/toolchain/llvm.ini
-lrwxr-xr-x   0        0        0        0 2021-07-19 17:52:53.975073 tuxmake-1.8.0/tuxmake/toolchain/rust.ini -> rustgcc.ini
--rw-r--r--   0        0        0      104 2021-07-19 17:52:53.975073 tuxmake-1.8.0/tuxmake/toolchain/rustclang.ini
--rw-r--r--   0        0        0       76 2021-07-19 17:52:53.975073 tuxmake-1.8.0/tuxmake/toolchain/rustgcc.ini
--rw-r--r--   0        0        0       87 2021-07-19 17:52:53.975073 tuxmake-1.8.0/tuxmake/toolchain/rustllvm.ini
--rw-r--r--   0        0        0     1340 2022-05-04 19:27:44.035045 tuxmake-1.8.0/tuxmake/utils.py
--rw-r--r--   0        0        0     1637 2022-05-04 19:27:44.035045 tuxmake-1.8.0/tuxmake/wrapper.py
--rw-r--r--   0        0        0      120 2022-01-14 14:57:37.795278 tuxmake-1.8.0/tuxmake/wrapper/ccache.ini
--rw-r--r--   0        0        0       26 2021-02-24 19:11:31.354543 tuxmake-1.8.0/tuxmake/wrapper/none.ini
--rw-r--r--   0        0        0      177 2021-05-07 12:01:31.522844 tuxmake-1.8.0/tuxmake/wrapper/sccache.ini
--rw-r--r--   0        0        0      338 2021-02-24 19:11:31.354543 tuxmake-1.8.0/tuxmake/xdg.py
--rw-r--r--   0        0        0     5252 1970-01-01 00:00:00.000000 tuxmake-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0      207 2022-01-17 18:20:24.932316 tuxmake-1.9.0/.ackrc
+-rw-r--r--   0        0        0       30 2020-07-21 21:47:43.351426 tuxmake-1.9.0/.flake8
+-rw-r--r--   0        0        0      105 2021-02-24 19:11:31.330544 tuxmake-1.9.0/.gitignore
+-rw-r--r--   0        0        0     6392 2023-01-09 22:04:50.532508 tuxmake-1.9.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0     1054 2020-07-21 21:47:43.351426 tuxmake-1.9.0/LICENSE
+-rw-r--r--   0        0        0     3191 2022-10-17 11:45:50.138618 tuxmake-1.9.0/Makefile
+-rw-r--r--   0        0        0     4941 2021-03-10 20:07:53.156597 tuxmake-1.9.0/README.md
+-rw-r--r--   0        0        0      151 2023-01-17 12:59:29.323319 tuxmake-1.9.0/debian/changelog
+-rw-r--r--   0        0        0      878 2022-05-04 19:27:44.019045 tuxmake-1.9.0/debian/control
+-rw-r--r--   0        0        0      100 2021-02-24 19:11:31.334544 tuxmake-1.9.0/debian/gbp.conf
+-rwxr-xr-x   0        0        0      539 2022-05-04 19:27:44.019045 tuxmake-1.9.0/debian/rules
+-rw-r--r--   0        0        0       12 2021-02-19 19:03:40.336999 tuxmake-1.9.0/debian/source/format
+-rw-r--r--   0        0        0       24 2021-02-24 19:11:31.334544 tuxmake-1.9.0/debian/tuxmake.bash-completion
+-rw-r--r--   0        0        0       10 2021-02-19 19:03:40.336999 tuxmake-1.9.0/debian/tuxmake.manpages
+-rw-r--r--   0        0        0      194 2021-02-19 19:03:40.336999 tuxmake-1.9.0/debian/watch
+-rw-r--r--   0        0        0     1825 2022-05-05 19:32:50.521489 tuxmake-1.9.0/docs/architectures.md
+-rw-r--r--   0        0        0      342 2021-06-11 19:19:48.364575 tuxmake-1.9.0/docs/chat.md
+-rw-r--r--   0        0        0     3370 2021-02-24 19:11:31.334544 tuxmake-1.9.0/docs/code-of-conduct.md
+-rw-r--r--   0        0        0      657 2021-03-01 19:50:07.790172 tuxmake-1.9.0/docs/container-about.md
+-rw-r--r--   0        0        0      503 2021-03-01 19:50:07.790172 tuxmake-1.9.0/docs/container-usage.md
+-rw-r--r--   0        0        0     1828 2021-03-10 21:40:08.629900 tuxmake-1.9.0/docs/contributing.md
+-rw-r--r--   0        0        0     2352 2022-01-17 18:20:24.932316 tuxmake-1.9.0/docs/curated_containers.md
+-rw-r--r--   0        0        0     5670 2021-05-27 12:38:47.396728 tuxmake-1.9.0/docs/custom_containers.md
+-rw-r--r--   0        0        0      133 2021-02-19 19:03:40.336999 tuxmake-1.9.0/docs/extra.css
+-rw-r--r--   0        0        0      828 2021-03-29 15:20:53.428834 tuxmake-1.9.0/docs/install-deb.md
+-rw-r--r--   0        0        0      417 2022-01-17 18:20:24.932316 tuxmake-1.9.0/docs/install-pypi.md
+-rw-r--r--   0        0        0      767 2021-06-24 17:17:19.210224 tuxmake-1.9.0/docs/install-rpm.md
+-rw-r--r--   0        0        0     1738 2022-05-05 20:05:11.550147 tuxmake-1.9.0/docs/kconfig.md
+lrwxr-xr-x   0        0        0        0 2021-02-19 19:03:40.336999 tuxmake-1.9.0/docs/license.md -> ../LICENSE
+-rw-r--r--   0        0        0     5648 2022-06-30 12:57:16.723455 tuxmake-1.9.0/docs/metadata.md
+-rw-r--r--   0        0        0      236 2021-02-19 19:03:40.336999 tuxmake-1.9.0/docs/mkautodoc.css
+-rw-r--r--   0        0        0     1530 2021-02-24 19:11:31.334544 tuxmake-1.9.0/docs/packaging.md
+-rw-r--r--   0        0        0      411 2022-03-02 15:23:17.692529 tuxmake-1.9.0/docs/python.md
+-rw-r--r--   0        0        0      872 2022-05-04 19:27:44.019045 tuxmake-1.9.0/docs/python_runtime.md
+-rw-r--r--   0        0        0     3364 2021-05-27 18:01:05.522833 tuxmake-1.9.0/docs/reproducible_builds.md
+-rw-r--r--   0        0        0      718 2022-05-04 19:27:44.019045 tuxmake-1.9.0/docs/resources.md
+-rw-r--r--   0        0        0      564 2021-04-01 18:05:11.035171 tuxmake-1.9.0/docs/run-uninstalled.md
+-rw-r--r--   0        0        0     2749 2021-07-12 19:20:00.087118 tuxmake-1.9.0/docs/runtimes.md
+-rw-r--r--   0        0        0     5115 2022-05-04 19:27:44.019045 tuxmake-1.9.0/docs/targets.md
+-rw-r--r--   0        0        0     1601 2021-07-19 17:52:53.967073 tuxmake-1.9.0/docs/toolchains.md
+-rw-r--r--   0        0        0     2001 2021-02-19 19:03:40.336999 tuxmake-1.9.0/docs/tuxmake.svg
+-rw-r--r--   0        0        0     3585 2021-02-24 19:11:31.334544 tuxmake-1.9.0/docs/tuxmake_full.svg
+-rw-r--r--   0        0        0     5493 2021-02-19 19:03:40.336999 tuxmake-1.9.0/docs/tuxmake_icon.svg
+-rw-r--r--   0        0        0      568 2021-02-24 19:11:31.334544 tuxmake-1.9.0/docs/wrappers.md
+-rw-r--r--   0        0        0     1471 2023-01-03 19:14:13.224618 tuxmake-1.9.0/mkdocs.yml
+-rw-r--r--   0        0        0      397 2021-02-19 19:03:40.336999 tuxmake-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0      323 2021-02-19 19:03:40.336999 tuxmake-1.9.0/requirements-dev.txt
+-rwxr-xr-x   0        0        0      123 2020-10-01 18:26:08.493036 tuxmake-1.9.0/run
+-rw-r--r--   0        0        0      489 2021-02-19 19:03:40.336999 tuxmake-1.9.0/scripts/cli2md.py
+-rwxr-xr-x   0        0        0      493 2021-02-19 19:03:40.336999 tuxmake-1.9.0/scripts/cli2md.sh
+-rwxr-xr-x   0        0        0      205 2021-02-19 19:03:40.336999 tuxmake-1.9.0/scripts/cli2rst.sh
+-rwxr-xr-x   0        0        0      896 2021-03-29 15:20:53.428834 tuxmake-1.9.0/scripts/package-repos
+-rwxr-xr-x   0        0        0      166 2021-02-19 19:03:40.336999 tuxmake-1.9.0/scripts/readme2index.sh
+-rwxr-xr-x   0        0        0     1859 2022-05-27 12:36:03.982287 tuxmake-1.9.0/scripts/release
+-rwxr-xr-x   0        0        0      473 2021-02-19 19:03:40.336999 tuxmake-1.9.0/scripts/run-tests
+-rwxr-xr-x   0        0        0      260 2021-02-24 19:11:31.338544 tuxmake-1.9.0/scripts/target-deps
+-rw-r--r--   0        0        0     1990 2022-05-05 15:08:17.541771 tuxmake-1.9.0/scripts/test_doc.py
+-rw-r--r--   0        0        0       63 2022-05-04 19:27:44.019045 tuxmake-1.9.0/support/docker/.gitignore
+-rw-r--r--   0        0        0      821 2021-07-12 19:20:00.087118 tuxmake-1.9.0/support/docker/Dockerfile.arc
+-rw-r--r--   0        0        0     2595 2023-01-16 16:52:22.589442 tuxmake-1.9.0/support/docker/Dockerfile.base
+-rw-r--r--   0        0        0     7509 2023-01-16 19:38:54.887142 tuxmake-1.9.0/support/docker/Dockerfile.build
+-rw-r--r--   0        0        0     1323 2021-07-20 18:09:57.480336 tuxmake-1.9.0/support/docker/Dockerfile.ci
+-rw-r--r--   0        0        0      579 2023-01-03 19:14:13.228618 tuxmake-1.9.0/support/docker/Dockerfile.clang-android
+-rw-r--r--   0        0        0     3366 2022-05-25 17:56:12.829200 tuxmake-1.9.0/support/docker/Makefile
+-rw-r--r--   0        0        0     4299 2022-05-04 19:27:44.023045 tuxmake-1.9.0/support/docker/README.md
+-rw-r--r--   0        0        0      120 2021-07-12 19:20:00.091118 tuxmake-1.9.0/support/docker/arc-gcc-8.sha256sum
+-rw-r--r--   0        0        0      123 2021-07-12 19:20:00.091118 tuxmake-1.9.0/support/docker/arc-gcc-9.sha256sum
+-rw-r--r--   0        0        0      160 2023-01-03 19:14:13.228618 tuxmake-1.9.0/support/docker/conf/pinning-bullseye
+-rwxr-xr-x   0        0        0     8585 2022-12-20 16:57:39.647730 tuxmake-1.9.0/support/docker/configure
+-rwxr-xr-x   0        0        0     2911 2022-05-04 19:27:44.023045 tuxmake-1.9.0/support/docker/gen-gitlab-ci
+-rwxr-xr-x   0        0        0      312 2021-07-12 19:20:00.091118 tuxmake-1.9.0/support/docker/get-arch-images
+-rwxr-xr-x   0        0        0      137 2021-07-12 19:20:00.091118 tuxmake-1.9.0/support/docker/list-images
+-rw-r--r--   0        0        0     3253 2022-05-04 19:27:44.023045 tuxmake-1.9.0/support/docker/test/test_configure.sh
+-rwxr-xr-x   0        0        0      259 2022-05-04 19:27:44.023045 tuxmake-1.9.0/support/docker/test/test_gitlab_ci.sh
+-rw-r--r--   0        0        0     2720 2022-05-04 19:27:44.023045 tuxmake-1.9.0/support/docker/tuxmake-ci-images.yml
+-rw-r--r--   0        0        0    20585 2023-01-16 19:55:35.837446 tuxmake-1.9.0/support/docker/tuxmake-images.yml
+-rw-r--r--   0        0        0        0 2020-07-21 21:47:43.355426 tuxmake-1.9.0/test/__init__.py
+-rw-r--r--   0        0        0     2018 2022-05-04 19:27:44.023045 tuxmake-1.9.0/test/conftest.py
+-rw-r--r--   0        0        0       15 2020-07-21 21:47:43.355426 tuxmake-1.9.0/test/fakelinux/Kbuild
+-rw-r--r--   0        0        0       15 2020-07-21 21:47:43.355426 tuxmake-1.9.0/test/fakelinux/Kconfig
+-rw-r--r--   0        0        0     6608 2022-05-25 17:15:42.157651 tuxmake-1.9.0/test/fakelinux/Makefile
+lrwxr-xr-x   0        0        0        0 2022-05-04 19:27:44.027045 tuxmake-1.9.0/test/fakelinux/arch/aarch64 -> arm64
+-rw-r--r--   0        0        0       55 2022-05-04 19:27:44.027045 tuxmake-1.9.0/test/fakelinux/arch/arc/Makefile
+-rw-r--r--   0        0        0       50 2022-05-04 19:27:44.027045 tuxmake-1.9.0/test/fakelinux/arch/arm/Makefile
+-rw-r--r--   0        0        0        0 2022-10-17 11:45:50.138618 tuxmake-1.9.0/test/fakelinux/arch/arm/boot/dts/.gitkeep
+-rw-r--r--   0        0        0       99 2022-05-04 19:27:44.027045 tuxmake-1.9.0/test/fakelinux/arch/arm64/Makefile
+-rw-r--r--   0        0        0        0 2022-10-13 17:37:37.027379 tuxmake-1.9.0/test/fakelinux/arch/arm64/boot/dts/.gitkeep
+lrwxr-xr-x   0        0        0        0 2022-05-04 19:27:44.027045 tuxmake-1.9.0/test/fakelinux/arch/armv8l -> arm
+-rw-r--r--   0        0        0       54 2022-05-04 19:27:44.027045 tuxmake-1.9.0/test/fakelinux/arch/hexagon/Makefile
+-rw-r--r--   0        0        0       51 2022-05-04 19:27:44.027045 tuxmake-1.9.0/test/fakelinux/arch/i386/Makefile
+lrwxr-xr-x   0        0        0        0 2022-05-04 19:27:44.027045 tuxmake-1.9.0/test/fakelinux/arch/i686 -> i386
+-rw-r--r--   0        0        0       56 2022-05-04 19:27:44.027045 tuxmake-1.9.0/test/fakelinux/arch/mips/Makefile
+-rw-r--r--   0        0        0       54 2022-05-04 19:27:44.027045 tuxmake-1.9.0/test/fakelinux/arch/parisc/Makefile
+-rw-r--r--   0        0        0       54 2022-05-04 19:27:44.027045 tuxmake-1.9.0/test/fakelinux/arch/powerpc/Makefile
+-rw-r--r--   0        0        0       56 2022-05-04 19:27:44.027045 tuxmake-1.9.0/test/fakelinux/arch/riscv/Makefile
+-rw-r--r--   0        0        0       33 2022-05-04 19:27:44.027045 tuxmake-1.9.0/test/fakelinux/arch/s390/Makefile
+-rw-r--r--   0        0        0       49 2022-05-04 19:27:44.027045 tuxmake-1.9.0/test/fakelinux/arch/sh/Makefile
+-rw-r--r--   0        0        0       52 2022-05-04 19:27:44.027045 tuxmake-1.9.0/test/fakelinux/arch/sparc/Makefile
+-rw-r--r--   0        0        0       51 2022-05-04 19:27:44.027045 tuxmake-1.9.0/test/fakelinux/arch/x86_64/Makefile
+-rw-r--r--   0        0        0       31 2022-05-05 20:05:11.550147 tuxmake-1.9.0/test/fakelinux/config/test.config
+-rw-r--r--   0        0        0      100 2021-02-19 19:03:40.340999 tuxmake-1.9.0/test/fakelinux/scripts/kconfig/config.c
+-rwxr-xr-x   0        0        0      696 2021-10-04 17:33:12.234846 tuxmake-1.9.0/test/fakelinux/scripts/kconfig/merge_config.sh
+-rw-r--r--   0        0        0       30 2022-01-17 18:20:24.936317 tuxmake-1.9.0/test/fakelinux/tools/testing/selftests/bpf/config
+-rw-r--r--   0        0        0      246 2022-01-12 11:59:55.925204 tuxmake-1.9.0/test/fakelinux/vmlinux.c
+lrwxr-xr-x   0        0        0        0 2021-02-19 19:03:40.340999 tuxmake-1.9.0/test/integration-slow/docker -> runtime
+lrwxr-xr-x   0        0        0        0 2021-02-19 19:03:40.340999 tuxmake-1.9.0/test/integration-slow/docker-local -> runtime
+-rwxr-xr-x   0        0        0     3394 2021-02-19 19:03:40.340999 tuxmake-1.9.0/test/integration-slow/matrix
+lrwxr-xr-x   0        0        0        0 2021-02-19 19:03:40.340999 tuxmake-1.9.0/test/integration-slow/podman -> runtime
+lrwxr-xr-x   0        0        0        0 2021-02-19 19:03:40.340999 tuxmake-1.9.0/test/integration-slow/podman-local -> runtime
+-rwxr-xr-x   0        0        0      137 2021-02-19 19:03:40.340999 tuxmake-1.9.0/test/integration-slow/runtime
+-rwxr-xr-x   0        0        0       45 2021-05-27 18:01:05.522833 tuxmake-1.9.0/test/integration/auxbin/hostname
+-rwxr-xr-x   0        0        0      159 2021-05-07 12:01:31.522844 tuxmake-1.9.0/test/integration/auxbin/which
+-rwxr-xr-x   0        0        0       45 2021-05-27 18:01:05.522833 tuxmake-1.9.0/test/integration/auxbin/whoami
+-rwxr-xr-x   0        0        0     1336 2022-05-04 19:27:44.027045 tuxmake-1.9.0/test/integration/bin/tuxcmd
+lrwxr-xr-x   0        0        0        0 2021-02-19 19:03:40.340999 tuxmake-1.9.0/test/integration/bin/tuxmake -> ../../../run
+-rwxr-xr-x   0        0        0     8599 2022-10-17 11:45:50.142619 tuxmake-1.9.0/test/integration/fakelinux
+-rwxr-xr-x   0        0        0      631 2022-05-25 17:56:05.985268 tuxmake-1.9.0/test/integration/runtimes-print-support-matrix
+-rw-r--r--   0        0        0     2025 2022-05-04 19:27:44.031045 tuxmake-1.9.0/test/integration/test_helper.sh
+-rw-r--r--   0        0        0      120 2021-02-19 19:03:40.340999 tuxmake-1.9.0/test/logs/case.log
+-rw-r--r--   0        0        0      680 2021-02-19 19:03:40.340999 tuxmake-1.9.0/test/logs/compiler-lacks.log
+-rw-r--r--   0        0        0      720 2021-02-19 19:03:40.340999 tuxmake-1.9.0/test/logs/compiler-not-found.log
+-rw-r--r--   0        0        0      413 2021-02-19 19:03:40.340999 tuxmake-1.9.0/test/logs/garbage.log
+-rw-r--r--   0        0        0      748 2021-02-19 19:03:40.340999 tuxmake-1.9.0/test/logs/invalid-config.log
+-rw-r--r--   0        0        0    28772 2021-02-19 19:03:40.340999 tuxmake-1.9.0/test/logs/no-rule-to-make-target.log
+-rw-r--r--   0        0        0     3289 2021-02-19 19:03:40.340999 tuxmake-1.9.0/test/logs/no-such-file-or-directory.log
+-rw-r--r--   0        0        0       45 2021-02-19 19:03:40.340999 tuxmake-1.9.0/test/logs/non-utf8.log
+-rw-r--r--   0        0        0       32 2022-06-30 12:57:16.727455 tuxmake-1.9.0/test/logs/simple.log
+-rw-r--r--   0        0        0     2320 2022-10-17 11:45:50.146619 tuxmake-1.9.0/test/test_arch.py
+-rw-r--r--   0        0        0    40357 2023-01-16 16:52:19.105475 tuxmake-1.9.0/test/test_build.py
+-rw-r--r--   0        0        0      619 2021-05-17 18:48:25.275796 tuxmake-1.9.0/test/test_build_info.py
+-rw-r--r--   0        0        0      351 2021-05-17 18:48:25.275796 tuxmake-1.9.0/test/test_cache.py
+-rw-r--r--   0        0        0    15778 2021-11-18 18:24:55.045970 tuxmake-1.9.0/test/test_cli.py
+-rw-r--r--   0        0        0     2779 2021-05-26 17:31:06.703699 tuxmake-1.9.0/test/test_cmdline.py
+-rw-r--r--   0        0        0      851 2022-05-04 19:27:44.031045 tuxmake-1.9.0/test/test_configurable_object.py
+-rw-r--r--   0        0        0      306 2021-06-24 17:17:19.214223 tuxmake-1.9.0/test/test_deprecated.py
+-rw-r--r--   0        0        0      492 2021-05-17 18:48:25.275796 tuxmake-1.9.0/test/test_exceptions.py
+-rw-r--r--   0        0        0      735 2022-06-30 12:57:16.727455 tuxmake-1.9.0/test/test_log_parser.py
+-rw-r--r--   0        0        0      372 2021-05-17 18:48:25.275796 tuxmake-1.9.0/test/test_main.py
+-rw-r--r--   0        0        0     5346 2021-07-12 17:35:10.502137 tuxmake-1.9.0/test/test_metadata.py
+-rw-r--r--   0        0        0     1340 2021-05-17 18:48:25.275796 tuxmake-1.9.0/test/test_output.py
+-rw-r--r--   0        0        0    15023 2023-01-03 19:14:13.228618 tuxmake-1.9.0/test/test_runtime.py
+-rw-r--r--   0        0        0     3847 2022-05-04 19:27:44.031045 tuxmake-1.9.0/test/test_target.py
+-rw-r--r--   0        0        0     1399 2021-05-17 18:48:25.275796 tuxmake-1.9.0/test/test_toolchain.py
+-rw-r--r--   0        0        0     2412 2022-05-04 19:27:44.031045 tuxmake-1.9.0/test/test_utils.py
+-rw-r--r--   0        0        0     1602 2022-05-04 19:27:44.031045 tuxmake-1.9.0/test/test_wrapper.py
+-rw-r--r--   0        0        0     1050 2023-01-17 12:59:29.331319 tuxmake-1.9.0/tuxmake.PKGBUILD
+-rw-r--r--   0        0        0     3982 2021-03-10 21:40:08.629900 tuxmake-1.9.0/tuxmake.rst
+-rw-r--r--   0        0        0     1614 2023-01-17 12:59:29.319319 tuxmake-1.9.0/tuxmake.spec
+-rw-r--r--   0        0        0       67 2023-01-17 12:59:29.311319 tuxmake-1.9.0/tuxmake/__init__.py
+-rw-r--r--   0        0        0       96 2020-10-30 19:36:51.001129 tuxmake-1.9.0/tuxmake/__main__.py
+-rw-r--r--   0        0        0     1540 2022-10-17 11:45:50.146619 tuxmake-1.9.0/tuxmake/arch.py
+lrwxr-xr-x   0        0        0        0 2021-01-21 21:38:43.327256 tuxmake-1.9.0/tuxmake/arch/aarch64.ini -> arm64.ini
+lrwxr-xr-x   0        0        0        0 2021-01-21 21:38:37.291321 tuxmake-1.9.0/tuxmake/arch/amd64.ini -> x86_64.ini
+-rw-r--r--   0        0        0      124 2021-02-19 19:03:40.340999 tuxmake-1.9.0/tuxmake/arch/arc.ini
+-rw-r--r--   0        0        0      131 2022-05-04 19:35:12.786595 tuxmake-1.9.0/tuxmake/arch/arm.ini
+-rw-r--r--   0        0        0      329 2022-05-27 12:32:42.965088 tuxmake-1.9.0/tuxmake/arch/arm64.ini
+lrwxr-xr-x   0        0        0        0 2022-05-05 19:32:50.521489 tuxmake-1.9.0/tuxmake/arch/armel.ini -> armv5.ini
+lrwxr-xr-x   0        0        0        0 2022-05-05 19:32:50.521489 tuxmake-1.9.0/tuxmake/arch/armhf.ini -> arm.ini
+-rw-r--r--   0        0        0      130 2022-05-05 19:32:50.521489 tuxmake-1.9.0/tuxmake/arch/armv5.ini
+lrwxr-xr-x   0        0        0        0 2021-07-19 17:52:53.971073 tuxmake-1.9.0/tuxmake/arch/armv8l.ini -> arm.ini
+-rw-r--r--   0        0        0      200 2021-05-13 18:52:26.703789 tuxmake-1.9.0/tuxmake/arch/hexagon.ini
+-rw-r--r--   0        0        0      143 2022-10-17 11:45:50.146619 tuxmake-1.9.0/tuxmake/arch/i386.ini
+lrwxr-xr-x   0        0        0        0 2021-07-19 20:15:14.466498 tuxmake-1.9.0/tuxmake/arch/i686.ini -> i386.ini
+-rw-r--r--   0        0        0      131 2021-09-24 13:43:57.410569 tuxmake-1.9.0/tuxmake/arch/mips.ini
+-rw-r--r--   0        0        0      137 2021-05-13 14:19:16.567361 tuxmake-1.9.0/tuxmake/arch/openrisc.ini
+-rw-r--r--   0        0        0      133 2021-02-19 19:03:40.344999 tuxmake-1.9.0/tuxmake/arch/parisc.ini
+-rw-r--r--   0        0        0      141 2021-05-27 12:38:47.400728 tuxmake-1.9.0/tuxmake/arch/powerpc.ini
+-rw-r--r--   0        0        0      135 2021-05-27 12:38:47.400728 tuxmake-1.9.0/tuxmake/arch/riscv.ini
+-rw-r--r--   0        0        0      130 2021-02-19 19:03:40.344999 tuxmake-1.9.0/tuxmake/arch/s390.ini
+-rw-r--r--   0        0        0      123 2021-02-19 19:03:40.344999 tuxmake-1.9.0/tuxmake/arch/sh.ini
+-rw-r--r--   0        0        0      133 2021-05-27 12:38:47.400728 tuxmake-1.9.0/tuxmake/arch/sparc.ini
+-rw-r--r--   0        0        0      182 2021-05-13 14:19:16.567361 tuxmake-1.9.0/tuxmake/arch/um.ini
+-rw-r--r--   0        0        0      146 2022-10-17 11:45:50.150619 tuxmake-1.9.0/tuxmake/arch/x86_64.ini
+-rw-r--r--   0        0        0    24639 2023-01-16 16:52:19.105475 tuxmake-1.9.0/tuxmake/build.py
+-rw-r--r--   0        0        0      967 2022-05-04 19:27:44.031045 tuxmake-1.9.0/tuxmake/build_utils.py
+-rw-r--r--   0        0        0      406 2021-02-24 19:11:31.346543 tuxmake-1.9.0/tuxmake/cache.py
+-rw-r--r--   0        0        0     5866 2022-05-04 19:27:44.031045 tuxmake-1.9.0/tuxmake/cli.py
+-rw-r--r--   0        0        0    13684 2022-05-04 19:27:44.031045 tuxmake-1.9.0/tuxmake/cmdline.py
+-rw-r--r--   0        0        0     2470 2022-05-04 19:27:44.035045 tuxmake-1.9.0/tuxmake/config.py
+-rw-r--r--   0        0        0      263 2021-06-24 17:17:19.214223 tuxmake-1.9.0/tuxmake/deprecated.py
+-rw-r--r--   0        0        0     2460 2022-05-04 19:27:44.035045 tuxmake-1.9.0/tuxmake/exceptions.py
+-rw-r--r--   0        0        0      632 2022-06-30 12:57:16.727455 tuxmake-1.9.0/tuxmake/log.py
+-rw-r--r--   0        0        0      580 2021-06-24 17:17:19.214223 tuxmake-1.9.0/tuxmake/logging.py
+-rw-r--r--   0        0        0     1361 2022-05-04 19:27:44.035045 tuxmake-1.9.0/tuxmake/metadata.pl
+-rw-r--r--   0        0        0     5346 2023-01-16 16:52:19.105475 tuxmake-1.9.0/tuxmake/metadata.py
+-rw-r--r--   0        0        0      654 2021-03-01 19:50:07.794172 tuxmake-1.9.0/tuxmake/metadata/artifacts.ini
+-rw-r--r--   0        0        0      504 2020-10-01 18:26:08.513036 tuxmake-1.9.0/tuxmake/metadata/ccache.ini
+-rw-r--r--   0        0        0      134 2020-10-01 18:26:08.513036 tuxmake-1.9.0/tuxmake/metadata/compiler.ini
+-rw-r--r--   0        0        0      257 2020-10-01 18:26:08.513036 tuxmake-1.9.0/tuxmake/metadata/git.ini
+-rw-r--r--   0        0        0      237 2021-06-28 18:22:58.491678 tuxmake-1.9.0/tuxmake/metadata/hardware.ini
+-rw-r--r--   0        0        0      317 2022-05-25 17:15:42.157651 tuxmake-1.9.0/tuxmake/metadata/os.ini
+-rw-r--r--   0        0        0       89 2021-06-28 18:35:34.379417 tuxmake-1.9.0/tuxmake/metadata/resources.ini
+-rw-r--r--   0        0        0      352 2020-10-01 18:26:08.513036 tuxmake-1.9.0/tuxmake/metadata/sccache.ini
+-rw-r--r--   0        0        0      217 2022-01-17 18:20:24.940317 tuxmake-1.9.0/tuxmake/metadata/source.ini
+-rw-r--r--   0        0        0       96 2021-02-19 19:03:40.344999 tuxmake-1.9.0/tuxmake/metadata/system_map.ini
+-rw-r--r--   0        0        0     1614 2022-05-04 19:27:44.035045 tuxmake-1.9.0/tuxmake/metadata/tools.ini
+-rw-r--r--   0        0        0      208 2020-10-01 18:26:08.513036 tuxmake-1.9.0/tuxmake/metadata/uname.ini
+-rw-r--r--   0        0        0      339 2021-02-19 19:03:40.344999 tuxmake-1.9.0/tuxmake/metadata/vmlinux.ini
+-rw-r--r--   0        0        0      524 2022-01-17 18:20:24.940317 tuxmake-1.9.0/tuxmake/output.py
+-rw-r--r--   0        0        0    19908 2023-01-16 19:33:30.071147 tuxmake-1.9.0/tuxmake/runtime.py
+-rwxr-xr-x   0        0        0     5810 2022-08-10 19:17:24.844678 tuxmake-1.9.0/tuxmake/runtime/bin/tuxmake-check-environment
+-rwxr-xr-x   0        0        0      802 2022-05-04 19:27:44.035045 tuxmake-1.9.0/tuxmake/runtime/bin/tuxmake-logger
+-rwxr-xr-x   0        0        0     2515 2022-05-04 19:27:44.035045 tuxmake-1.9.0/tuxmake/runtime/bin/tuxmake-run-offline
+lrwxr-xr-x   0        0        0        0 2021-02-19 19:03:40.344999 tuxmake-1.9.0/tuxmake/runtime/docker-local.ini -> docker.ini
+-rw-r--r--   0        0        0     7683 2023-01-16 20:46:02.578206 tuxmake-1.9.0/tuxmake/runtime/docker.ini
+-rw-r--r--   0        0        0        0 2020-10-01 18:26:08.513036 tuxmake-1.9.0/tuxmake/runtime/null.ini
+lrwxr-xr-x   0        0        0        0 2021-02-19 19:03:40.344999 tuxmake-1.9.0/tuxmake/runtime/podman-local.ini -> docker.ini
+lrwxr-xr-x   0        0        0        0 2021-02-19 19:03:40.344999 tuxmake-1.9.0/tuxmake/runtime/podman.ini -> docker.ini
+-rw-r--r--   0        0        0     8710 2022-05-05 20:05:11.550147 tuxmake-1.9.0/tuxmake/target.py
+-rw-r--r--   0        0        0       93 2022-05-04 19:27:44.035045 tuxmake-1.9.0/tuxmake/target/clang-analyzer.ini
+-rw-r--r--   0        0        0      246 2021-05-07 12:01:31.522844 tuxmake-1.9.0/tuxmake/target/config.ini
+-rw-r--r--   0        0        0      332 2022-05-04 19:27:44.035045 tuxmake-1.9.0/tuxmake/target/cpupower.ini
+-rw-r--r--   0        0        0      171 2022-05-04 19:27:44.035045 tuxmake-1.9.0/tuxmake/target/debugkernel.ini
+-rw-r--r--   0        0        0      109 2022-01-26 20:50:21.366112 tuxmake-1.9.0/tuxmake/target/default.ini
+-rw-r--r--   0        0        0      651 2022-10-17 11:45:50.150619 tuxmake-1.9.0/tuxmake/target/dtbs-legacy.ini
+-rw-r--r--   0        0        0      482 2022-10-17 11:45:50.150619 tuxmake-1.9.0/tuxmake/target/dtbs.ini
+-rw-r--r--   0        0        0      320 2022-05-04 19:27:44.035045 tuxmake-1.9.0/tuxmake/target/headers.ini
+-rw-r--r--   0        0        0      154 2021-02-24 19:11:31.354543 tuxmake-1.9.0/tuxmake/target/kernel.ini
+-rw-r--r--   0        0        0     1307 2022-05-04 19:27:44.035045 tuxmake-1.9.0/tuxmake/target/kselftest-bpf.ini
+-rw-r--r--   0        0        0      238 2022-05-04 19:27:44.035045 tuxmake-1.9.0/tuxmake/target/kselftest-merge.ini
+-rw-r--r--   0        0        0      339 2022-05-04 19:27:44.035045 tuxmake-1.9.0/tuxmake/target/kselftest.ini
+-rw-r--r--   0        0        0      399 2022-05-04 19:27:44.035045 tuxmake-1.9.0/tuxmake/target/modules.ini
+-rw-r--r--   0        0        0      296 2022-05-04 19:27:44.035045 tuxmake-1.9.0/tuxmake/target/perf.ini
+-rw-r--r--   0        0        0      165 2021-06-17 12:25:40.231629 tuxmake-1.9.0/tuxmake/target/targz-pkg.ini
+-rw-r--r--   0        0        0      270 2021-02-24 19:11:31.354543 tuxmake-1.9.0/tuxmake/target/xipkernel.ini
+-rw-r--r--   0        0        0     1460 2023-01-16 16:52:19.105475 tuxmake-1.9.0/tuxmake/toolchain.py
+-rw-r--r--   0        0        0      111 2021-02-19 19:03:40.344999 tuxmake-1.9.0/tuxmake/toolchain/clang.ini
+-rw-r--r--   0        0        0       98 2021-11-18 21:34:09.033790 tuxmake-1.9.0/tuxmake/toolchain/gcc.ini
+-rw-r--r--   0        0        0      104 2021-11-18 21:34:09.033790 tuxmake-1.9.0/tuxmake/toolchain/llvm.ini
+lrwxr-xr-x   0        0        0        0 2021-07-19 17:52:53.975073 tuxmake-1.9.0/tuxmake/toolchain/rust.ini -> rustgcc.ini
+-rw-r--r--   0        0        0      104 2021-07-19 17:52:53.975073 tuxmake-1.9.0/tuxmake/toolchain/rustclang.ini
+-rw-r--r--   0        0        0       76 2021-07-19 17:52:53.975073 tuxmake-1.9.0/tuxmake/toolchain/rustgcc.ini
+-rw-r--r--   0        0        0       87 2021-07-19 17:52:53.975073 tuxmake-1.9.0/tuxmake/toolchain/rustllvm.ini
+-rw-r--r--   0        0        0     1340 2022-05-04 19:27:44.035045 tuxmake-1.9.0/tuxmake/utils.py
+-rw-r--r--   0        0        0     1636 2023-01-16 16:52:19.109475 tuxmake-1.9.0/tuxmake/wrapper.py
+-rw-r--r--   0        0        0      120 2022-01-14 14:57:37.795278 tuxmake-1.9.0/tuxmake/wrapper/ccache.ini
+-rw-r--r--   0        0        0       26 2021-02-24 19:11:31.354543 tuxmake-1.9.0/tuxmake/wrapper/none.ini
+-rw-r--r--   0        0        0      177 2021-05-07 12:01:31.522844 tuxmake-1.9.0/tuxmake/wrapper/sccache.ini
+-rw-r--r--   0        0        0      338 2021-02-24 19:11:31.354543 tuxmake-1.9.0/tuxmake/xdg.py
+-rw-r--r--   0        0        0     5252 1970-01-01 00:00:00.000000 tuxmake-1.9.0/PKG-INFO
```

### Comparing `tuxmake-1.8.0/.gitlab-ci.yml` & `tuxmake-1.9.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/LICENSE` & `tuxmake-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/Makefile` & `tuxmake-1.9.0/Makefile`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/README.md` & `tuxmake-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/debian/control` & `tuxmake-1.9.0/debian/control`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/debian/rules` & `tuxmake-1.9.0/debian/rules`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/docs/architectures.md` & `tuxmake-1.9.0/docs/architectures.md`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/docs/code-of-conduct.md` & `tuxmake-1.9.0/docs/code-of-conduct.md`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/docs/container-about.md` & `tuxmake-1.9.0/docs/container-about.md`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/docs/contributing.md` & `tuxmake-1.9.0/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/docs/curated_containers.md` & `tuxmake-1.9.0/docs/curated_containers.md`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/docs/custom_containers.md` & `tuxmake-1.9.0/docs/custom_containers.md`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/docs/install-deb.md` & `tuxmake-1.9.0/docs/install-deb.md`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/docs/install-rpm.md` & `tuxmake-1.9.0/docs/install-rpm.md`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/docs/kconfig.md` & `tuxmake-1.9.0/docs/kconfig.md`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/docs/metadata.md` & `tuxmake-1.9.0/docs/metadata.md`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/docs/packaging.md` & `tuxmake-1.9.0/docs/packaging.md`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/docs/python_runtime.md` & `tuxmake-1.9.0/docs/python_runtime.md`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/docs/reproducible_builds.md` & `tuxmake-1.9.0/docs/reproducible_builds.md`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/docs/resources.md` & `tuxmake-1.9.0/docs/resources.md`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/docs/run-uninstalled.md` & `tuxmake-1.9.0/docs/run-uninstalled.md`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/docs/runtimes.md` & `tuxmake-1.9.0/docs/runtimes.md`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/docs/targets.md` & `tuxmake-1.9.0/docs/targets.md`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/docs/toolchains.md` & `tuxmake-1.9.0/docs/toolchains.md`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/docs/tuxmake.svg` & `tuxmake-1.9.0/docs/tuxmake.svg`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/docs/tuxmake_full.svg` & `tuxmake-1.9.0/docs/tuxmake_full.svg`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/docs/tuxmake_icon.svg` & `tuxmake-1.9.0/docs/tuxmake_icon.svg`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/docs/wrappers.md` & `tuxmake-1.9.0/docs/wrappers.md`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/mkdocs.yml` & `tuxmake-1.9.0/mkdocs.yml`

 * *Files 9% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 site_dir: public
 repo_url: https://gitlab.com/Linaro/tuxmake/
 site_url: "https://tuxmake.org/"
 theme:
   name: material
   logo: tuxmake.svg
   favicon: tuxmake_icon.svg
+  font: false
 markdown_extensions:
   - mkautodoc
 extra_css:
   - mkautodoc.css
   - extra.css
 
 nav:
```

### Comparing `tuxmake-1.8.0/scripts/package-repos` & `tuxmake-1.9.0/scripts/package-repos`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/scripts/release` & `tuxmake-1.9.0/scripts/release`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/scripts/test_doc.py` & `tuxmake-1.9.0/scripts/test_doc.py`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/support/docker/Dockerfile.arc` & `tuxmake-1.9.0/support/docker/Dockerfile.arc`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/support/docker/Dockerfile.base` & `tuxmake-1.9.0/support/docker/Dockerfile.base`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 ARG BASE
 FROM ${BASE}
 
 ENV DEBIAN_FRONTEND=noninteractive
 
 COPY conf/ /srv/tuxmake-conf
 
-RUN . /etc/os-release \
+RUN export VERSION_ID=0 && . /etc/os-release \
     && if [ "${VERSION_CODENAME}" = "" ]; then exit; fi \
     && echo "deb http://deb.debian.org/debian ${VERSION_CODENAME}-backports main" > /etc/apt/sources.list.d/backports.list \
+    && if [ "${VERSION_ID}" -eq 11 ]; then echo "deb http://snapshot.debian.org/archive/debian/20221013T214821Z/ bullseye-backports main" > /etc/apt/sources.list.d/backports-snapshot.list && echo "Acquire::Check-Valid-Until no;" > /etc/apt/apt.conf.d/99novalidity; fi \
     && if [ "${VERSION_ID}" -le 10 ]; then echo "deb http://deb.debian.org/debian ${VERSION_CODENAME}-proposed-updates main" > /etc/apt/sources.list.d/proposed-updates.list; fi \
     && pinning=/srv/tuxmake-conf/pinning-${VERSION_CODENAME} \
     && if [ -f "${pinning}" ]; then cp "${pinning}" /etc/apt/preferences.d/; fi
 
 # Heavyweight: package installation
 # This list of packages was seeded from kernelci's base image
 # https://github.com/kernelci/kernelci-core/blob/master/jenkins/dockerfiles/build-base/Dockerfile
```

### Comparing `tuxmake-1.8.0/support/docker/Dockerfile.build` & `tuxmake-1.9.0/support/docker/Dockerfile.build`

 * *Files 15% similar despite different names*

```diff
@@ -13,14 +13,19 @@
 
 RUN if [ -f /etc/apt/sources.list.d/extra.list ]; then exit; fi; \
     if [ -n "${EXTRA_APT_REPO_KEY}" ]; then \
         wget -O /etc/apt/trusted.gpg.d/extra.asc "${EXTRA_APT_REPO_KEY}"; \
     fi; \
     if [ -n "${EXTRA_APT_REPO}" ]; then \
         echo "${EXTRA_APT_REPO}" > /etc/apt/sources.list.d/extra.list; \
+    fi; \
+    if [ "${HOSTARCH}" = riscv64 ]; then \
+        apt-get update -q && apt-get install -qy debian-ports-archive-keyring; \
+        echo "deb http://deb.debian.org/debian-ports sid main" > /etc/apt/sources.list.d/foreign.list; \
+        echo "deb http://deb.debian.org/debian-ports unreleased main" >> /etc/apt/sources.list.d/foreign.list; \
     fi
 
 
 # Install basic toolchain packages. Which toolchain exactly is defined by the
 # $PACKAGES build argument
 RUN apt-get update -q && \
     apt-get install \
@@ -48,14 +53,20 @@
     else \
         arch=$(dpkg-architecture --host-type=${HOSTARCH}-linux-gnu --query=DEB_HOST_ARCH); \
     fi; \
     case "${arch}" in \
         amd64|arm64|armel|armhf|i386|mips64el|mipsel|ppc64el|s390x) \
             supported=yes; \
             ;; \
+        riscv64) \
+            supported=no; \
+            if grep -q unstable /etc/apt/sources.list.d/debian.sources; then \
+                supported=yes; \
+            fi; \
+            ;; \
         *) \
             supported=no; \
             ;; \
     esac; \
     if [ "$(uname -m)" != "${HOSTARCH}" -a -n "${HOSTARCH}" ]; then \
         dpkg --add-architecture ${arch}; \
     fi && \
@@ -108,14 +119,21 @@
         libssl-dev libssl-dev:${arch} \
         $(test "${arch}" != "s390x" && echo libunwind-dev libunwind-dev:${arch}) \
         libzstd-dev libzstd-dev:${arch} \
         linux-libc-dev \
         linux-libc-dev-${arch}-cross \
         systemtap-sdt-dev:${arch} \
         && \
+    if dpkg --compare-versions "${debianversion}" ge 12; then \
+        apt-get install  \
+            --assume-yes \
+            --no-install-recommends \
+            --option=debug::pkgProblemResolver=yes \
+            pkg-config:${arch}; \
+    fi && \
     : This is a horrible hack, but a foreign binutils-dev is not installable && \
     : See https://bugs.debian.org/983540 && \
     apt-get download ${INSTALL_OPTIONS} binutils-dev:${arch} && \
     dpkg -x binutils-dev*.deb /tmp/binutils-dev && \
     rsync -avp /tmp/binutils-dev/ / && \
     rm -rf binutils-dev*.deb /tmp/binutils-dev
```

### Comparing `tuxmake-1.8.0/support/docker/Dockerfile.ci` & `tuxmake-1.9.0/support/docker/Dockerfile.ci`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/support/docker/Dockerfile.clang-android` & `tuxmake-1.9.0/support/docker/Dockerfile.clang-android`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ARG BASE
 FROM ${BASE}
 
-ARG ANDROID_CLANG=r468909
+ARG ANDROID_CLANG=r475365b
 
 RUN wget --progress=dot:giga https://android.googlesource.com/platform/prebuilts/clang/host/linux-x86/+archive/refs/heads/master/clang-${ANDROID_CLANG}.tar.gz && \
     tar xaf clang-${ANDROID_CLANG}.tar.gz -C /usr/local && \
     rm -f clang-${ANDROID_CLANG}.tar.gz
 
 RUN apt-get update -q=2 && \
     gccversion=$(apt-cache policy gcc | sed -e '/Candidate:/!d; s/\s*Candidate:\s*.*://; s/\..*//') && \
```

### Comparing `tuxmake-1.8.0/support/docker/Makefile` & `tuxmake-1.9.0/support/docker/Makefile`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/support/docker/README.md` & `tuxmake-1.9.0/support/docker/README.md`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/support/docker/configure` & `tuxmake-1.9.0/support/docker/configure`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/support/docker/gen-gitlab-ci` & `tuxmake-1.9.0/support/docker/gen-gitlab-ci`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/support/docker/test/test_configure.sh` & `tuxmake-1.9.0/support/docker/test/test_configure.sh`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/support/docker/tuxmake-ci-images.yml` & `tuxmake-1.9.0/support/docker/tuxmake-ci-images.yml`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/support/docker/tuxmake-images.yml` & `tuxmake-1.9.0/support/docker/tuxmake-images.yml`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/test/conftest.py` & `tuxmake-1.9.0/test/conftest.py`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/test/fakelinux/Makefile` & `tuxmake-1.9.0/test/fakelinux/Makefile`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/test/fakelinux/scripts/kconfig/merge_config.sh` & `tuxmake-1.9.0/test/fakelinux/scripts/kconfig/merge_config.sh`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/test/integration-slow/matrix` & `tuxmake-1.9.0/test/integration-slow/matrix`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/test/integration/bin/tuxcmd` & `tuxmake-1.9.0/test/integration/bin/tuxcmd`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/test/integration/fakelinux` & `tuxmake-1.9.0/test/integration/fakelinux`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/test/integration/runtimes-print-support-matrix` & `tuxmake-1.9.0/test/integration/runtimes-print-support-matrix`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/test/integration/test_helper.sh` & `tuxmake-1.9.0/test/integration/test_helper.sh`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/test/logs/compiler-lacks.log` & `tuxmake-1.9.0/test/logs/compiler-lacks.log`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/test/logs/compiler-not-found.log` & `tuxmake-1.9.0/test/logs/compiler-not-found.log`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/test/logs/invalid-config.log` & `tuxmake-1.9.0/test/logs/invalid-config.log`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/test/logs/no-rule-to-make-target.log` & `tuxmake-1.9.0/test/logs/no-rule-to-make-target.log`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/test/logs/no-such-file-or-directory.log` & `tuxmake-1.9.0/test/logs/no-such-file-or-directory.log`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/test/test_arch.py` & `tuxmake-1.9.0/test/test_arch.py`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/test/test_build.py` & `tuxmake-1.9.0/test/test_build.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import subprocess
 import shutil
 import urllib
 from tuxmake.arch import Architecture, Native
 from tuxmake.toolchain import Toolchain
 from tuxmake.build import build
 from tuxmake.build import Build
+from tuxmake.build import BuildInfo
 from tuxmake.build import defaults
 from tuxmake.build import Terminated
 from tuxmake.build import get_image
 from tuxmake.build import DEFAULT_CONTAINER_REGISTRY
 from tuxmake.target import Command
 from tuxmake.target import default_compression
 import tuxmake.exceptions
@@ -1097,7 +1098,28 @@
         assert "modules.tar.xz" in artifacts
 
     def test_compression_none(self, linux):
         build = Build(tree=linux, compression_type="none")
         build.run()
         artifacts = [str(f.name) for f in build.output_dir.glob("*")]
         assert "modules.tar" in artifacts
+
+
+class TestCustomCrossCompile:
+    def test_CROSS_COMPILE(self, linux, Popen):
+        build = Build(
+            tree=linux, target_arch="arm64", make_variables={"CROSS_COMPILE": "foo-"}
+        )
+        build.status["config"] = BuildInfo("PASS")
+        build.build(build.targets[1])
+        assert "CROSS_COMPILE=foo-" in args(Popen)
+
+    def test_CROSS_COMPILE_COMPAT(self, linux, Popen):
+        build = Build(
+            tree=linux,
+            target_arch="arm64",
+            make_variables={"CROSS_COMPILE_COMPAT": "foo-"},
+        )
+        build.get_dynamic_makevars()
+        build.status["config"] = BuildInfo("PASS")
+        build.build(build.targets[1])
+        assert "CROSS_COMPILE_COMPAT=foo-" in args(Popen)
```

### Comparing `tuxmake-1.8.0/test/test_build_info.py` & `tuxmake-1.9.0/test/test_build_info.py`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/test/test_cli.py` & `tuxmake-1.9.0/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/test/test_cmdline.py` & `tuxmake-1.9.0/test/test_cmdline.py`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/test/test_configurable_object.py` & `tuxmake-1.9.0/test/test_configurable_object.py`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/test/test_log_parser.py` & `tuxmake-1.9.0/test/test_log_parser.py`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/test/test_metadata.py` & `tuxmake-1.9.0/test/test_metadata.py`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/test/test_output.py` & `tuxmake-1.9.0/test/test_output.py`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/test/test_runtime.py` & `tuxmake-1.9.0/test/test_runtime.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,14 +195,21 @@
     def test_environment(self, linux, spawn_container):
         runtime = DockerRuntime()
         runtime.environment["FOO"] = "BAR"
         runtime.start_container()
         cmd = spawn_container.call_args[0][0]
         assert "--env=FOO=BAR" in cmd
 
+    def test_caps(self, linux, spawn_container):
+        runtime = DockerRuntime()
+        runtime.caps = ["SYS_PTRACE"]
+        runtime.start_container()
+        cmd = spawn_container.call_args[0][0]
+        assert "--cap-add=SYS_PTRACE" in cmd
+
     def test_output_dir(self, linux, tmp_path, spawn_container):
         runtime = DockerRuntime()
         runtime.output_dir = tmp_path
         runtime.start_container()
         cmd = spawn_container.call_args[0][0]
         assert f"--volume={tmp_path}:{tmp_path}" in cmd
```

### Comparing `tuxmake-1.8.0/test/test_target.py` & `tuxmake-1.9.0/test/test_target.py`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/test/test_toolchain.py` & `tuxmake-1.9.0/test/test_toolchain.py`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/test/test_utils.py` & `tuxmake-1.9.0/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/test/test_wrapper.py` & `tuxmake-1.9.0/test/test_wrapper.py`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/tuxmake.PKGBUILD` & `tuxmake-1.9.0/tuxmake.PKGBUILD`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 pkgname=tuxmake
-pkgver=1.8.0
+pkgver=1.9.0
 pkgrel=1
 pkgdesc='Thin wrapper to build Linux kernels'
 url='https://tuxmake.org/'
 license=('MIT')
 arch=('any')
 depends=('perl' 'python')
 makedepends=('git' 'python-build' 'python-docutils' 'python-flit' 'python-installer' 'python-wheel')
```

### Comparing `tuxmake-1.8.0/tuxmake.rst` & `tuxmake-1.9.0/tuxmake.rst`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/tuxmake.spec` & `tuxmake-1.9.0/tuxmake.spec`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Name:      tuxmake
-Version:   1.8.0
+Version:   1.9.0
 Release:   0%{?dist}
 Summary:   Thin wrapper to build Linux kernels
 License:   Expat
 URL:       https://tuxmake.org
 Source0:   %{pypi_source}
```

### Comparing `tuxmake-1.8.0/tuxmake/arch.py` & `tuxmake-1.9.0/tuxmake/arch.py`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/tuxmake/build.py` & `tuxmake-1.9.0/tuxmake/build.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,16 +116,15 @@
     - **kconfig**: which configuration to build (`str`). Defaults to
       `defconfig`.
     - **kconfig_add**: additional kconfig fragments/options to use. List of
       `str`, defaulting to an empty list.
     - **make_variables**: KEY=VALUE arguments to pass to `make`. `dict` with
       strings as values and strings as keys. Some `KEY`s are now allowed, as
       they would interfere with the tuxmake normal operation(e.g. `ARCH`, `CC`,
-      `CROSS_COMPILE`, `HOSTCC`, INSTALL_MOD_PATH`, `INSTALL_DTBS_PATH`, `O`,
-      etc).
+      `HOSTCC`, INSTALL_MOD_PATH`, `INSTALL_DTBS_PATH`, `O`,  etc).
     - **targets**: targets to build, list of `str`. If `None` or an empty list
       is passed, the default list of targets will be built.
     - **compression_type**: compression type to use in compressed artifacts.
       `str`, must be one of "xz", "none".
     - **kernel_image**: which kernel image to build, overriding the default
       kernel image name defined for the target architecture.
     - **jobs**: number of concurrent jobs to run (as in `make -j N`). `int`,
@@ -141,33 +140,32 @@
       after the build finishes. Ignored if *build_dir* is passed, in which
       case the build directory *will not be removed*.
     """
 
     MAKE_VARIABLES_REJECTLIST = [
         "ARCH",
         "CC",
-        "CROSS_COMPILE",
         "HOSTCC",
         "INSTALL_DTBS_PATH",
         "INSTALL_MOD_PATH",
         "O",
     ]
 
     def __init__(
         self,
         tree=".",
         output_dir=None,
         build_dir=None,
         target_arch=None,
         toolchain=None,
         wrapper=None,
-        environment={},
+        environment=None,
         kconfig=defaults.kconfig,
-        kconfig_add=[],
-        make_variables={},
+        kconfig_add=None,
+        make_variables=None,
         targets=defaults.targets,
         compression_type=None,
         kernel_image=None,
         jobs=None,
         runtime=None,
         fail_fast=False,
         verbose=False,
@@ -189,23 +187,23 @@
 
         self.target_arch = target_arch and Architecture(target_arch) or native_arch
         self.toolchain = toolchain and Toolchain(toolchain) or NoExplicitToolchain()
         self.wrapper = wrapper and Wrapper(wrapper) or Wrapper("none")
 
         self.timestamp = get_directory_timestamp(self.source_tree)
         self.__environment__ = None
-        self.__environment_input__ = environment
+        self.__environment_input__ = environment or {}
 
         self.kconfig = kconfig
-        self.kconfig_add = kconfig_add
+        self.kconfig_add = kconfig_add or []
 
-        for k in make_variables.keys():
+        self.make_variables = make_variables or {}
+        for k in self.make_variables.keys():
             if k in self.MAKE_VARIABLES_REJECTLIST:
                 raise UnsupportedMakeVariable(k)
-        self.make_variables = make_variables
 
         self.dynamic_make_variables = dict(self.target_arch.dynamic_makevars)
 
         if not targets:
             targets = defaults.targets
 
         if kernel_image:
@@ -466,23 +464,24 @@
         expanded_makevars = {k: self.format_cmd_part(v) for k, v in makevars.items()}
         expanded_makevars.update(self.makevars)
         return [f"{k}={v}" for k, v in expanded_makevars.items() if v]
 
     @property
     def makevars(self):
         mvars = {}
-        mvars.update(self.make_variables)
         mvars.update(self.target_arch.makevars)
         mvars.update(self.toolchain.expand_makevars(self.target_arch))
+        mvars.update(self.make_variables)
         mvars.update(self.wrapper.wrap(mvars))
         return mvars
 
     def get_dynamic_makevars(self):
         for k, v in self.dynamic_make_variables.items():
-            self.make_variables[k] = self.get_command_output(v).strip()
+            if k not in self.make_variables:
+                self.make_variables[k] = self.get_command_output(v).strip()
 
     def get_command_output(self, cmd):
         with tempfile.TemporaryFile(mode="w+", encoding="utf-8") as f:
             self.run_cmd(["sh", "-c", cmd], stdout=f, echo=False)
             f.seek(0)
             return f.read().strip()
 
@@ -615,19 +614,20 @@
             shutil.rmtree(self.build_dir, ignore_errors=True)
 
     def check_environment(self):
         self.runtime.prepare()
         self.get_dynamic_makevars()
         cmd = [str(self.runtime.get_check_environment_command())]
         cmd.append(f"{self.target_arch.name}_{self.toolchain.name}")
-        cross = self.makevars.get("CROSS_COMPILE")
+        makevars = self.makevars
+        cross = makevars.get("CROSS_COMPILE")
         if cross:
             cmd.append(cross)
         if "CROSS_COMPILE_COMPAT" in self.dynamic_make_variables:
-            cross_compat = self.makevars.get("CROSS_COMPILE_COMPAT")
+            cross_compat = makevars.get("CROSS_COMPILE_COMPAT")
             if cross_compat:
                 cmd.append(cross_compat)
             else:
                 cmd.append("")
         result = self.run_cmd(cmd)
         self.cleanup()
         if not result:
```

### Comparing `tuxmake-1.8.0/tuxmake/build_utils.py` & `tuxmake-1.9.0/tuxmake/build_utils.py`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/tuxmake/cli.py` & `tuxmake-1.9.0/tuxmake/cli.py`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/tuxmake/cmdline.py` & `tuxmake-1.9.0/tuxmake/cmdline.py`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/tuxmake/config.py` & `tuxmake-1.9.0/tuxmake/config.py`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/tuxmake/exceptions.py` & `tuxmake-1.9.0/tuxmake/exceptions.py`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/tuxmake/log.py` & `tuxmake-1.9.0/tuxmake/log.py`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/tuxmake/logging.py` & `tuxmake-1.9.0/tuxmake/logging.py`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/tuxmake/metadata.pl` & `tuxmake-1.9.0/tuxmake/metadata.pl`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/tuxmake/metadata.py` & `tuxmake-1.9.0/tuxmake/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,17 @@
 
     def before_build(self):
         for _, _, extractor in self.each_extractor():
             extractor.before_build()
 
     def collect(self):
         build = self.build
-        compiler = build.toolchain.compiler(build.target_arch)
+        compiler = build.toolchain.compiler(
+            build.target_arch, build.makevars.get("CROSS_COMPILE", None)
+        )
         metadata_input_data = {
             handler.name: {
                 key: build.format_cmd_part(cmd.replace("{compiler}", compiler))
                 for key, cmd in handler.commands.items()
             }
             for handler in self.handlers
         }
```

### Comparing `tuxmake-1.8.0/tuxmake/metadata/artifacts.ini` & `tuxmake-1.9.0/tuxmake/metadata/artifacts.ini`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/tuxmake/metadata/tools.ini` & `tuxmake-1.9.0/tuxmake/metadata/tools.ini`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/tuxmake/output.py` & `tuxmake-1.9.0/tuxmake/output.py`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/tuxmake/runtime.py` & `tuxmake-1.9.0/tuxmake/runtime.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,16 @@
     * **output_dir**: directory where to save logs of the execution.
       For container runtimes, this directory is bind mounted inside the
       container under the same location.
       Type: `Optional[Path]`; defaults to `None` (meaning, no logs are saved).
     * **environment**: extra environment variables to be used for all commands
       ran by this runtime. Type: `dict` with `str` keys and values; defaults to
       an empty dict.
+    * **caps**: additional capabilities needed by the container ran by this runtime.
+      Type: `list` with `str`; defaults to an empty list.
     """
 
     basedir = "runtime"
     name = "runtime"
     exception = InvalidRuntimeError
     bindir = Path(__file__).parent / basedir / "bin"
 
@@ -107,14 +109,15 @@
         self.__logger__: Optional[subprocess.Popen] = None
 
         self.basename: str = "run"
         self.quiet: bool = False
         self.source_dir: Path = Path.cwd()
         self.output_dir: Optional[Path] = None
         self.environment = {}
+        self.caps: Optional[list] = []
 
     def __init_config__(self):
         self.toolchains = Toolchain.supported()
 
     def get_image(self):
         if not self.__image__:
             raise ImageRequired()
@@ -321,14 +324,15 @@
         targets="",
         skip_build=False,
         target_bases="",
         target_kinds="",
         target_hosts="",
         target_skip="",
         packages="",
+        rebuild_targets="",
         install_options="",
         extra_apt_repo=None,
         extra_apt_repo_key=None,
     ):
         self.name = name
         self.kind = kind
         self.base = base
@@ -339,14 +343,15 @@
         self.target_bases = splitmap(target_bases)
         self.target_kinds = splitmap(target_kinds)
         self.target_hosts = splitlistmap(target_hosts)
         self.target_skip = split(target_skip)
         self.packages = split(packages)
         self.install_options = install_options
         self.rebuild = rebuild
+        self.rebuild_targets = splitmap(rebuild_targets)
         self.extra_apt_repo = extra_apt_repo
         self.extra_apt_repo_key = extra_apt_repo_key
 
 
 class ContainerRuntime(Runtime):
     prepare_failed_msg = "failed to pull remote image {image}"
     bindir = Path("/tuxmake")
@@ -372,14 +377,17 @@
                 for target in image.targets:
                     cross_config = dict(self.config[entry])
                     cross_config["base"] = image.target_bases.get(target, image.name)
                     cross_config["kind"] = image.target_kinds.get(
                         target, "cross-" + image.kind
                     )
                     cross_config["hosts"] = image.target_hosts.get(target, image.hosts)
+                    cross_config["rebuild"] = image.rebuild_targets.get(
+                        target, image.rebuild
+                    )
                     cross_config["skip_build"] = target in image.target_skip
                     cross_image = Image(
                         name=f"{target}_{image.name}", group=group, **cross_config
                     )
                     image_list.append(cross_image)
         self.images = self.base_images + self.ci_images + self.toolchain_images
         self.toolchain_images_map = {
@@ -433,25 +441,27 @@
             subprocess.check_call(pull)
 
         do_pull()
         cache.set(pull, time.time())
 
     def start_container(self):
         env = (f"--env={k}={v}" for k, v in self.environment.items())
+        caps = (f"--cap-add={cap}" for cap in self.caps)
 
         user_opts = self.get_user_opts()
         extra_opts = self.__get_extra_opts__()
         cmd = [
             self.command,
             "run",
             "--rm",
             "--init",
             "--detach",
             "--env=KBUILD_BUILD_USER=tuxmake",
             *env,
+            *caps,
             *user_opts,
             *self.get_volume_opts(),
             f"--workdir={self.source_dir}",
             *self.get_logging_opts(),
             *extra_opts,
             self.get_image(),
             "sleep",
```

### Comparing `tuxmake-1.8.0/tuxmake/runtime/bin/tuxmake-check-environment` & `tuxmake-1.9.0/tuxmake/runtime/bin/tuxmake-check-environment`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/tuxmake/runtime/bin/tuxmake-logger` & `tuxmake-1.9.0/tuxmake/runtime/bin/tuxmake-logger`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/tuxmake/runtime/bin/tuxmake-run-offline` & `tuxmake-1.9.0/tuxmake/runtime/bin/tuxmake-run-offline`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/tuxmake/runtime/docker.ini` & `tuxmake-1.9.0/tuxmake/runtime/docker.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Lists of images to build. Each image needs to have a corresponding section
 # below.
 [runtime]
-bases = base-debian10, base-debian11, base-debiantesting
+bases = base-debian10, base-debian11, base-debiantesting, base-debianunstable
 toolchains =
     gcc,
     gcc-8,
     gcc-9,
     gcc-10,
     gcc-11,
     gcc-12,
@@ -80,14 +80,20 @@
 
 [base-debiantesting]
 kind    = base
 base    = docker.io/library/debian:testing-slim
 hosts   = amd64, arm64
 rebuild = monthly
 
+[base-debianunstable]
+kind    = base
+base    = docker.io/library/debian:unstable-slim
+hosts   = amd64, arm64
+rebuild = monthly
+
 [gcc]
 kind    = gcc-build
 base    = base-debian11
 hosts   = amd64, arm64
 rebuild = monthly
 targets = x86_64, arm64, i386, arm, armv5, mips, riscv, arc, parisc, powerpc, s390, sh, sparc
 target_bases = riscv:gcc-10, arc:gcc-9
@@ -135,17 +141,18 @@
 rebuild = monthly
 packages = gcc-11, g++-11
 
 [gcc-12]
 kind = gcc-build
 base = base-debiantesting
 hosts = amd64, arm64
-# targets: no riscv, parisc, sh, sparc for now
-targets = x86_64, arm64, i386, arm, armv5, mips, powerpc, s390
+# targets: no parisc, sh, sparc for now
+targets = x86_64, arm64, i386, arm, armv5, mips, powerpc, riscv, s390
 target_hosts = parisc:amd64, powerpc:amd64, sh:amd64, sparc:amd64
+target_bases = riscv:base-debianunstable
 rebuild = monthly
 packages = gcc-12, g++-12
 
 [clang]
 kind = clang-build
 base = base-debian11
 hosts = amd64, arm64
```

### Comparing `tuxmake-1.8.0/tuxmake/target.py` & `tuxmake-1.9.0/tuxmake/target.py`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/tuxmake/target/dtbs-legacy.ini` & `tuxmake-1.9.0/tuxmake/target/dtbs-legacy.ini`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/tuxmake/target/kselftest-bpf.ini` & `tuxmake-1.9.0/tuxmake/target/kselftest-bpf.ini`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/tuxmake/toolchain.py` & `tuxmake-1.9.0/tuxmake/toolchain.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,17 +30,19 @@
         }
 
     def get_image(self, arch):
         return self.image.format(
             toolchain=self.name, arch=arch.name, version_suffix=self.version_suffix
         )
 
-    def compiler(self, arch):
+    def compiler(self, arch, cross_compile=None):
+        if not cross_compile:
+            cross_compile = arch.makevars.get("CROSS_COMPILE", "")
         return self.__compiler__.format(
-            CROSS_COMPILE=arch.makevars.get("CROSS_COMPILE", "")
+            CROSS_COMPILE=cross_compile,
         )
 
 
 class NoExplicitToolchain(Toolchain):
     def __init__(self):
         super().__init__("gcc")
         self.makevars = {}
```

### Comparing `tuxmake-1.8.0/tuxmake/utils.py` & `tuxmake-1.9.0/tuxmake/utils.py`

 * *Files identical despite different names*

### Comparing `tuxmake-1.8.0/tuxmake/wrapper.py` & `tuxmake-1.9.0/tuxmake/wrapper.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,12 +41,12 @@
 
     def wrap(self, makevars):
         if not self.command:
             return makevars
         cross = makevars.get("CROSS_COMPILE", "")
         if makevars.get("LLVM") == "1":
             return {"CC": f"{self.command} clang", "HOSTCC": f"{self.command} clang"}
-        return {
-            k: f"{self.command} {v}"
-            for k, v in makevars.items()
-            if k in ("CC", "HOSTCC")
-        } or {"CC": f"{self.command} {cross}gcc", "HOSTCC": f"{self.command} gcc"}
+        compilers = {
+            "CC": makevars.get("CC") or f"{cross}gcc",
+            "HOSTCC": makevars.get("HOSTCC") or "gcc",
+        }
+        return {k: f"{self.command} {v}" for k, v in compilers.items()}
```

### Comparing `tuxmake-1.8.0/PKG-INFO` & `tuxmake-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuxmake
-Version: 1.8.0
+Version: 1.9.0
 Summary: Thin wrapper to build Linux kernels
 Home-page: https://tuxmake.org/
 Author: Antonio Terceiro
 Author-email: antonio.terceiro@linaro.org
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
```

