# Comparing `tmp/gateway_provisioners-0.1.0.tar.gz` & `tmp/gateway_provisioners-0.2.0.tar.gz`

## Comparing `gateway_provisioners-0.1.0.tar` & `gateway_provisioners-0.2.0.tar`

### file list

```diff
@@ -1,144 +1,196 @@
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/.git-blame-ignore-revs
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/.readthedocs.yaml
--rw-r--r--   0        0        0     7578 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/Makefile
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/RELEASING.md
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/.github/dependabot.yml
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/.github/release.yml
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/.github/codeql/codeql-config.yml
--rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/.github/workflows/build.yml
--rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/.github/workflows/enforce-label.yml
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/.github/workflows/prep-release.yml
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/.github/workflows/publish-release.yml
--rw-r--r--   0        0        0     7083 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/docs/Makefile
--rw-r--r--   0        0        0     7267 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/docs/make.bat
--rw-r--r--   0        0        0    13367 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/docs/source/conf.py
--rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/docs/source/index.rst
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/docs/source/_static/custom.css
--rw-r--r--   0        0        0    16301 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/docs/source/_static/jupyter-logo.png
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/docs/source/api/gateway_provisioners.cli.rst
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/docs/source/api/gateway_provisioners.rst
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/docs/source/api/modules.rst
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/docs/source/contributors/contrib.md
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/docs/source/contributors/debug.md
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/docs/source/contributors/devinstall.md
--rw-r--r--   0        0        0     5156 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/docs/source/contributors/docker.md
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/docs/source/contributors/index.rst
--rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/docs/source/contributors/sequence-diagrams.md
--rw-r--r--   0        0        0    20440 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/docs/source/contributors/system-architecture.md
--rw-r--r--   0        0        0    10013 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/docs/source/developers/custom-images.md
--rw-r--r--   0        0        0     4540 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/docs/source/developers/dev-remote-provisioner.md
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/docs/source/developers/index.rst
--rw-r--r--   0        0        0     7672 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/docs/source/developers/kernel-launcher.md
--rw-r--r--   0        0        0     5102 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/docs/source/developers/kernel-specification.md
--rw-r--r--   0        0        0   292130 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/docs/source/images/debug_configuration.png
--rw-r--r--   0        0        0    69485 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/docs/source/images/deployment.png
--rw-r--r--   0        0        0    35101 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/docs/source/images/process_proxy_hierarchy.png
--rw-r--r--   0        0        0    57033 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/docs/source/images/yarnui.jpg
--rw-r--r--   0        0        0     6549 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/docs/source/operators/config-add-env.md
--rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/docs/source/operators/config-env-debug.md
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/docs/source/operators/config-file.md
--rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/docs/source/operators/config-kernel-override.md
--rw-r--r--   0        0        0     7963 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/docs/source/operators/config-security.md
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/docs/source/operators/config-sys-env.md
--rw-r--r--   0        0        0     9375 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/docs/source/operators/deploy-distributed.md
--rw-r--r--   0        0        0    10071 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/docs/source/operators/deploy-docker.md
--rw-r--r--   0        0        0    33757 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/docs/source/operators/deploy-kubernetes.md
--rw-r--r--   0        0        0     6014 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/docs/source/operators/deploy-yarn-cluster.md
--rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/docs/source/operators/index.rst
--rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/docs/source/operators/installing-gp.md
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/docs/source/operators/installing-kernels.md
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/docs/source/other/index.rst
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/docs/source/other/related-resources.md
--rw-r--r--   0        0        0    15860 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/docs/source/other/troubleshooting.md
--rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/docs/source/users/connecting-to-eg.md
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/docs/source/users/index.rst
--rw-r--r--   0        0        0     8580 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/docs/source/users/kernel-envs.md
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/__init__.py
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/_version.py
--rw-r--r--   0        0        0     4480 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/config_mixin.py
--rw-r--r--   0        0        0     8879 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/container.py
--rw-r--r--   0        0        0    15154 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/distributed.py
--rw-r--r--   0        0        0    11160 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/docker_swarm.py
--rw-r--r--   0        0        0    16693 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/k8s.py
--rw-r--r--   0        0        0    37844 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/remote_provisioner.py
--rw-r--r--   0        0        0    15155 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/response_manager.py
--rw-r--r--   0        0        0    26815 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/yarn.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/cli/__init__.py
--rw-r--r--   0        0        0    20861 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/cli/base_app.py
--rw-r--r--   0        0        0     5467 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/cli/docker_specapp.py
--rw-r--r--   0        0        0     6323 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/cli/image_bootstrapapp.py
--rw-r--r--   0        0        0     7229 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/cli/k8s_specapp.py
--rw-r--r--   0        0        0     5622 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/cli/ssh_specapp.py
--rw-r--r--   0        0        0    10390 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/cli/yarn_specapp.py
--rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/docker/gp-spark-base/Dockerfile
--rw-r--r--   0        0        0     3722 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/docker/kernel-image/Dockerfile
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/docker/server-image/Dockerfile
--rw-r--r--   0        0        0     9274 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/kernel-launchers/R/scripts/launch_IRkernel.R
--rwxr-xr-x   0        0        0     3942 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/kernel-launchers/bootstrap/bootstrap-kernel.sh
--rw-r--r--   0        0        0     5891 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/kernel-launchers/docker/scripts/launch_docker.py
--rw-r--r--   0        0        0     4213 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/kernel-launchers/kubernetes/scripts/kernel-pod.yaml.j2
--rw-r--r--   0        0        0    10340 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/kernel-launchers/kubernetes/scripts/launch_kubernetes.py
--rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/kernel-launchers/operators/scripts/launch_custom_resource.py
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/kernel-launchers/operators/scripts/sparkoperator.k8s.io-v1beta2.yaml.j2
--rw-r--r--   0        0        0    12940 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/kernel-launchers/python/scripts/launch_ipykernel.py
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/kernel-launchers/python/scripts/server_listener.py
--rw-r--r--   0        0        0    31960 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/kernel-launchers/scala/lib/toree-launcher_2.12-0.1.0.jar
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/kernel-launchers/scala/toree-launcher/build.sbt
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/kernel-launchers/scala/toree-launcher/project/build.properties
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/kernel-launchers/scala/toree-launcher/project/plugins.sbt
--rw-r--r--   0        0        0     9778 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/kernel-launchers/scala/toree-launcher/project/scalastyle-config.xml
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/kernel-launchers/scala/toree-launcher/src/main/main.iml
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/kernel-launchers/scala/toree-launcher/src/main/scala/launcher/KernelProfile.scala
--rw-r--r--   0        0        0    10694 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/kernel-launchers/scala/toree-launcher/src/main/scala/launcher/ToreeLauncher.scala
--rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/kernel-launchers/scala/toree-launcher/src/main/scala/launcher/utils/SecurityUtils.scala
--rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/kernel-launchers/scala/toree-launcher/src/main/scala/launcher/utils/SocketUtils.scala
--rw-r--r--   0        0        0    10974 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/kernel-launchers/shared/scripts/server_listener.py
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/kernel-resources/python/logo-64x64.png
--rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/kernel-resources/r/kernel.js
--rw-r--r--   0        0        0     8492 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/kernel-resources/r/logo-64x64.png
--rw-r--r--   0        0        0    31734 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/kernel-resources/scala/logo-64x64.png
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/kernel-specs/container_python/kernel.json
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/kernel-specs/container_r/kernel.json
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/kernel-specs/container_scala/kernel.json
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/kernel-specs/k8s_python_spark/kernel.json
--rwxr-xr-x   0        0        0      942 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/kernel-specs/k8s_python_spark/bin/run.sh
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/kernel-specs/k8s_r_spark/kernel.json
--rwxr-xr-x   0        0        0      929 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/kernel-specs/k8s_r_spark/bin/run.sh
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/kernel-specs/k8s_scala_spark/kernel.json
--rwxr-xr-x   0        0        0     2036 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/kernel-specs/k8s_scala_spark/bin/run.sh
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/kernel-specs/ssh_python/kernel.json
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/kernel-specs/ssh_python_spark/kernel.json
--rwxr-xr-x   0        0        0      780 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/kernel-specs/ssh_python_spark/bin/run.sh
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/kernel-specs/ssh_r/kernel.json
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/kernel-specs/ssh_r_spark/kernel.json
--rwxr-xr-x   0        0        0      772 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/kernel-specs/ssh_r_spark/bin/run.sh
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/kernel-specs/ssh_scala/kernel.json
--rwxr-xr-x   0        0        0     1843 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/kernel-specs/ssh_scala/bin/run.sh
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/kernel-specs/ssh_scala_spark/kernel.json
--rwxr-xr-x   0        0        0     1843 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/kernel-specs/ssh_scala_spark/bin/run.sh
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/kernel-specs/yarn_dask_python/kernel.json
--rwxr-xr-x   0        0        0      604 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/kernel-specs/yarn_dask_python/bin/run.sh
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/kernel-specs/yarn_spark_python/kernel.json
--rwxr-xr-x   0        0        0      774 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/kernel-specs/yarn_spark_python/bin/run.sh
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/kernel-specs/yarn_spark_r/kernel.json
--rwxr-xr-x   0        0        0      912 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/kernel-specs/yarn_spark_r/bin/run.sh
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/kernel-specs/yarn_spark_scala/kernel.json
--rwxr-xr-x   0        0        0     1837 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/gateway_provisioners/kernel-specs/yarn_spark_scala/bin/run.sh
--rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/tests/conftest.py
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/tests/test_docker_provisioners.py
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/tests/test_k8s_provisioners.py
--rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/tests/test_yarn_provisioners.py
--rw-r--r--   0        0        0     4416 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/tests/validators.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/tests/mocks/__init__.py
--rw-r--r--   0        0        0     4335 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/tests/mocks/docker_client.py
--rw-r--r--   0        0        0     4058 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/tests/mocks/k8s_client.py
--rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/tests/mocks/popen.py
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/tests/mocks/response_manager.py
--rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/tests/mocks/yarn_client.py
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/.gitignore
--rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/LICENSE.md
--rw-r--r--   0        0        0     4402 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/README.md
--rw-r--r--   0        0        0     6021 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    10966 2020-02-02 00:00:00.000000 gateway_provisioners-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/.git-blame-ignore-revs
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     6492 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0    10455 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/Makefile
+-rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/RELEASING.md
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/.github/release.yml
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/.github/codeql/codeql-config.yml
+-rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/.github/workflows/enforce-label.yml
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/.github/workflows/prep-release.yml
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/.github/workflows/publish-release.yml
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/.ruff_cache/content/1422657ec3f42481
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/.ruff_cache/content/1953ff89295be810
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/.ruff_cache/content/2d3abe5f0121a7e7
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/.ruff_cache/content/2d689b5551fff571
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/.ruff_cache/content/42b8301ef927422
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/.ruff_cache/content/4318684e830895f8
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/.ruff_cache/content/561e5686ab9b4abd
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/.ruff_cache/content/5a4f4526a7fc3bd5
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/.ruff_cache/content/632d54c78ba87657
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/.ruff_cache/content/73f4c92641076219
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/.ruff_cache/content/79e36d632bd3db39
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/.ruff_cache/content/7a10ba862b19053d
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/.ruff_cache/content/803dc844c4aa29b7
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/.ruff_cache/content/80a6c95c672401c3
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/.ruff_cache/content/81b90ef99fee2d9e
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/.ruff_cache/content/830f6cb0b52855b
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/.ruff_cache/content/8f94da9dacab542c
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/.ruff_cache/content/92aa6294043a54cb
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/.ruff_cache/content/95b1efb5f583416a
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/.ruff_cache/content/9fefc97ec4ad45a2
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/.ruff_cache/content/a15b4fbf9ea0397
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/.ruff_cache/content/acbd0490fbb27346
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/.ruff_cache/content/ba15dd97720c662
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/.ruff_cache/content/bea9dd0152046487
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/.ruff_cache/content/bfdb04f26c54bbf7
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/.ruff_cache/content/c1bfcb0eb9c4f4fa
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/.ruff_cache/content/c7d8b1fa81560781
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/.ruff_cache/content/c868d58ec599f544
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/.ruff_cache/content/cebeae8604007bfd
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/.ruff_cache/content/d834a4b58c720333
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/.ruff_cache/content/d8f07a4e63e6cdfd
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/.ruff_cache/content/dac37f547e2c4ebe
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/.ruff_cache/content/de6f7c621e212321
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/.ruff_cache/content/df7ea59a1b8304e1
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/.ruff_cache/content/ea30fe73d63ba8a1
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/.ruff_cache/content/ea787f628f6c56d8
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/.ruff_cache/content/f37352c294e55fac
+-rw-r--r--   0        0        0     7043 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/docs/Makefile
+-rw-r--r--   0        0        0     7267 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/docs/make.bat
+-rw-r--r--   0        0        0    11661 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/docs/source/conf.py
+-rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/docs/source/index.rst
+-rw-r--r--   0        0        0    16301 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/docs/source/_static/jupyter-logo.png
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/docs/source/api/gateway_provisioners.cli.rst
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/docs/source/api/gateway_provisioners.rst
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/docs/source/api/modules.rst
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/docs/source/contributors/contrib.md
+-rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/docs/source/contributors/devinstall.md
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/docs/source/contributors/index.rst
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/docs/source/contributors/related-resources.md
+-rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/docs/source/contributors/sequence-diagrams.md
+-rw-r--r--   0        0        0    23501 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/docs/source/contributors/system-architecture.md
+-rw-r--r--   0        0        0     7216 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/docs/source/developers/custom-images.md
+-rw-r--r--   0        0        0     4591 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/docs/source/developers/dev-remote-provisioner.md
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/docs/source/developers/index.rst
+-rw-r--r--   0        0        0     8778 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/docs/source/developers/kernel-launcher.md
+-rw-r--r--   0        0        0     4932 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/docs/source/developers/kernel-specification.md
+-rw-r--r--   0        0        0     6541 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/docs/source/operators/config-add-env.md
+-rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/docs/source/operators/config-env-debug.md
+-rw-r--r--   0        0        0     8926 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/docs/source/operators/config-file.md
+-rw-r--r--   0        0        0     3162 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/docs/source/operators/config-kernel-override.md
+-rw-r--r--   0        0        0     7958 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/docs/source/operators/config-security.md
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/docs/source/operators/config-sys-env.md
+-rw-r--r--   0        0        0    18467 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/docs/source/operators/deploy-distributed.md
+-rw-r--r--   0        0        0    10835 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/docs/source/operators/deploy-docker.md
+-rw-r--r--   0        0        0    24351 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/docs/source/operators/deploy-kubernetes.md
+-rw-r--r--   0        0        0    14962 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/docs/source/operators/deploy-yarn-cluster.md
+-rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/docs/source/operators/index.rst
+-rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/docs/source/operators/installing-gp-container.md
+-rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/docs/source/operators/installing-gp.md
+-rw-r--r--   0        0        0     6865 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/docs/source/operators/installing-kernels-container.md
+-rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/docs/source/operators/installing-kernels.md
+-rw-r--r--   0        0        0     4965 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/docs/source/users/connecting-to-a-gateway.md
+-rw-r--r--   0        0        0     2254 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/docs/source/users/index.rst
+-rw-r--r--   0        0        0     8723 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/docs/source/users/kernel-envs.md
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/__init__.py
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/_version.py
+-rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/config_mixin.py
+-rw-r--r--   0        0        0     9321 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/container.py
+-rw-r--r--   0        0        0     5610 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/crd.py
+-rw-r--r--   0        0        0    15128 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/distributed.py
+-rw-r--r--   0        0        0    11409 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/docker_swarm.py
+-rw-r--r--   0        0        0    17893 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/k8s.py
+-rw-r--r--   0        0        0    37841 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/remote_provisioner.py
+-rw-r--r--   0        0        0    15155 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/response_manager.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/spark_operator.py
+-rw-r--r--   0        0        0    26556 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/yarn.py
+-rw-r--r--   0        0        0     5998 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/app-support/README.md
+-rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/app-support/docker/Dockerfile
+-rwxr-xr-x   0        0        0     2264 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/app-support/docker/start-application.sh
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/app-support/kubernetes/helm/gateway-provisioners/Chart.yaml
+-rw-r--r--   0        0        0     6493 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/app-support/kubernetes/helm/gateway-provisioners/values.yaml
+-rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/app-support/kubernetes/helm/gateway-provisioners/templates/daemonset.yaml
+-rw-r--r--   0        0        0     5173 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/app-support/kubernetes/helm/gateway-provisioners/templates/deployment.yaml
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/app-support/kubernetes/helm/gateway-provisioners/templates/gp-clusterrole.yaml
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/app-support/kubernetes/helm/gateway-provisioners/templates/gp-clusterrolebinding.yaml
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/app-support/kubernetes/helm/gateway-provisioners/templates/gp-serviceaccount.yaml
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/app-support/kubernetes/helm/gateway-provisioners/templates/imagepullSecret.yaml
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/app-support/kubernetes/helm/gateway-provisioners/templates/ingress.yaml
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/app-support/kubernetes/helm/gateway-provisioners/templates/kip-clusterrole.yaml
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/app-support/kubernetes/helm/gateway-provisioners/templates/kip-clusterrolebinding.yaml
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/app-support/kubernetes/helm/gateway-provisioners/templates/kip-serviceaccount.yaml
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/app-support/kubernetes/helm/gateway-provisioners/templates/psp.yaml
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/app-support/kubernetes/helm/gateway-provisioners/templates/service.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/cli/__init__.py
+-rw-r--r--   0        0        0    23726 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/cli/base_app.py
+-rw-r--r--   0        0        0     5428 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/cli/docker_specapp.py
+-rw-r--r--   0        0        0     6322 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/cli/image_bootstrapapp.py
+-rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/cli/k8s_specapp.py
+-rw-r--r--   0        0        0     5631 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/cli/ssh_specapp.py
+-rw-r--r--   0        0        0    10297 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/cli/yarn_specapp.py
+-rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/docker/gp-spark-base/Dockerfile
+-rw-r--r--   0        0        0     3679 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/docker/kernel-image/Dockerfile
+-rw-r--r--   0        0        0     9274 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/kernel-launchers/R/scripts/launch_IRkernel.R
+-rwxr-xr-x   0        0        0     3938 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/kernel-launchers/bootstrap/bootstrap-kernel.sh
+-rw-r--r--   0        0        0     5893 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/kernel-launchers/docker/scripts/launch_docker.py
+-rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/kernel-launchers/kubernetes/scripts/kernel-pod.yaml.j2
+-rw-r--r--   0        0        0    13409 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/kernel-launchers/kubernetes/scripts/launch_kubernetes.py
+-rw-r--r--   0        0        0     5571 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/kernel-launchers/operators/scripts/launch_custom_resource.py
+-rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/kernel-launchers/operators/scripts/sparkoperator.k8s.io-v1beta2.yaml.j2
+-rw-r--r--   0        0        0    12940 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/kernel-launchers/python/scripts/launch_ipykernel.py
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/kernel-launchers/python/scripts/server_listener.py
+-rw-r--r--   0        0        0    31961 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/kernel-launchers/scala/lib/toree-launcher_2.12-0.2.0.jar
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/kernel-launchers/scala/toree-launcher/build.sbt
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/kernel-launchers/scala/toree-launcher/project/build.properties
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/kernel-launchers/scala/toree-launcher/project/plugins.sbt
+-rw-r--r--   0        0        0     9778 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/kernel-launchers/scala/toree-launcher/project/scalastyle-config.xml
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/kernel-launchers/scala/toree-launcher/src/main/main.iml
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/kernel-launchers/scala/toree-launcher/src/main/scala/launcher/KernelProfile.scala
+-rw-r--r--   0        0        0    10694 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/kernel-launchers/scala/toree-launcher/src/main/scala/launcher/ToreeLauncher.scala
+-rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/kernel-launchers/scala/toree-launcher/src/main/scala/launcher/utils/SecurityUtils.scala
+-rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/kernel-launchers/scala/toree-launcher/src/main/scala/launcher/utils/SocketUtils.scala
+-rw-r--r--   0        0        0    10973 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/kernel-launchers/shared/scripts/server_listener.py
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/kernel-resources/python/logo-64x64.png
+-rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/kernel-resources/r/kernel.js
+-rw-r--r--   0        0        0     8492 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/kernel-resources/r/logo-64x64.png
+-rw-r--r--   0        0        0    31734 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/kernel-resources/scala/logo-64x64.png
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/kernel-specs/container_python/kernel.json
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/kernel-specs/container_r/kernel.json
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/kernel-specs/container_scala/kernel.json
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/kernel-specs/k8s_python_spark/kernel.json
+-rwxr-xr-x   0        0        0      942 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/kernel-specs/k8s_python_spark/bin/run.sh
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/kernel-specs/k8s_python_spark_operator/kernel.json
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/kernel-specs/k8s_r_spark/kernel.json
+-rwxr-xr-x   0        0        0      929 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/kernel-specs/k8s_r_spark/bin/run.sh
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/kernel-specs/k8s_scala_spark/kernel.json
+-rwxr-xr-x   0        0        0     2036 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/kernel-specs/k8s_scala_spark/bin/run.sh
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/kernel-specs/ssh_python/kernel.json
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/kernel-specs/ssh_python_spark/kernel.json
+-rwxr-xr-x   0        0        0      780 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/kernel-specs/ssh_python_spark/bin/run.sh
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/kernel-specs/ssh_r/kernel.json
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/kernel-specs/ssh_r_spark/kernel.json
+-rwxr-xr-x   0        0        0      772 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/kernel-specs/ssh_r_spark/bin/run.sh
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/kernel-specs/ssh_scala/kernel.json
+-rwxr-xr-x   0        0        0     1843 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/kernel-specs/ssh_scala/bin/run.sh
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/kernel-specs/ssh_scala_spark/kernel.json
+-rwxr-xr-x   0        0        0     1843 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/kernel-specs/ssh_scala_spark/bin/run.sh
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/kernel-specs/yarn_dask_python/kernel.json
+-rwxr-xr-x   0        0        0      604 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/kernel-specs/yarn_dask_python/bin/run.sh
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/kernel-specs/yarn_spark_python/kernel.json
+-rwxr-xr-x   0        0        0      774 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/kernel-specs/yarn_spark_python/bin/run.sh
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/kernel-specs/yarn_spark_r/kernel.json
+-rwxr-xr-x   0        0        0      912 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/kernel-specs/yarn_spark_r/bin/run.sh
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/kernel-specs/yarn_spark_scala/kernel.json
+-rwxr-xr-x   0        0        0     1837 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/gateway_provisioners/kernel-specs/yarn_spark_scala/bin/run.sh
+-rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/tests/conftest.py
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/tests/test_docker_provisioners.py
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/tests/test_k8s_provisioners.py
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/tests/test_yarn_provisioners.py
+-rw-r--r--   0        0        0     4416 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/tests/validators.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/tests/mocks/__init__.py
+-rw-r--r--   0        0        0     4335 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/tests/mocks/docker_client.py
+-rw-r--r--   0        0        0     4058 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/tests/mocks/k8s_client.py
+-rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/tests/mocks/popen.py
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/tests/mocks/response_manager.py
+-rw-r--r--   0        0        0     4388 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/tests/mocks/yarn_client.py
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/.gitignore
+-rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/LICENSE.md
+-rw-r--r--   0        0        0     4384 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/README.md
+-rw-r--r--   0        0        0     6998 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    11097 2020-02-02 00:00:00.000000 gateway_provisioners-0.2.0/PKG-INFO
```

### Comparing `gateway_provisioners-0.1.0/.pre-commit-config.yaml` & `gateway_provisioners-0.2.0/.pre-commit-config.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -11,31 +11,32 @@
       - id: check-executables-have-shebangs
       - id: check-added-large-files
       - id: check-case-conflict
       - id: check-merge-conflict
       - id: check-json
       - id: check-toml
       - id: check-yaml
+        exclude: gateway_provisioners/app-support/kubernetes/.*.yaml
       - id: debug-statements
       - id: end-of-file-fixer
       - id: trailing-whitespace
 
   - repo: https://github.com/python-jsonschema/check-jsonschema
-    rev: 0.19.2
+    rev: 0.22.0
     hooks:
       - id: check-github-workflows
 
   - repo: https://github.com/executablebooks/mdformat
     rev: 0.7.16
     hooks:
       - id: mdformat
 
   - repo: https://github.com/psf/black
-    rev: 22.12.0
+    rev: 23.3.0
     hooks:
       - id: black
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.225
+    rev: v0.0.261
     hooks:
       - id: ruff
         args: ["--fix"]
```

### Comparing `gateway_provisioners-0.1.0/RELEASING.md` & `gateway_provisioners-0.2.0/RELEASING.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 # Making a Gateway Provisioners Release
 
 ## Using `jupyter_releaser`
 
 The recommended way to make a release is to use [`jupyter_releaser`](https://jupyter-releaser.readthedocs.io/en/latest/get_started/making_release_from_repo.html).
 
-Note that we must use manual versions since Jupyter Releaser does not
-yet support "next" or "patch" when dev versions are used.
-
 ## Manual Release
 
 To create a manual release, perform the following steps:
 
 ### Set up
 
 ```bash
@@ -21,31 +18,51 @@
 
 ### Update the version and apply the tag
 
 ```bash
 echo "Enter new version"
 read new_version
 hatch version ${new_version}
+git commit -a -m "Release ${new_version}"
 git tag -a ${new_version} -m "Release ${new_version}"
 ```
 
-### Build the artifacts
+If building the changelog notes via the releases page (prior to jupyter-releaser) you'll want to push
+the tags so the changelog generator can know what to reference, otherwise this can be skipped.
+
+```bash
+git push origin
+git push --tags origin
+```
 
 ```bash
 make clean dist
 ```
 
+### Run tests
+
+```bash
+make test
+```
+
 ### Update the version back to dev
 
 ```bash
 echo "Enter dev version"
 read dev_version
 hatch version ${dev_version}
+git commit -a -m "Back to dev"
 git push origin $(git branch --show-current)
 ```
 
+If tags were not pushed previously (to build changelog) push now.
+
+```bash
+git push --tags origin
+```
+
 ### Publish the artifacts to pypi
 
 ```bash
 twine check dist/*
 twine upload dist/*
 ```
```

### Comparing `gateway_provisioners-0.1.0/.github/workflows/build.yml` & `gateway_provisioners-0.2.0/.github/workflows/build.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 name: Builds
 on:
   push:
+    branches: ["main"]
   pull_request:
 
 jobs:
   build:
     name: Build and test
     runs-on: ${{ matrix.os }}
     strategy:
@@ -32,15 +33,15 @@
           conda --version
       - name: Add SBT launcher
         run: |
           mkdir -p $HOME/.sbt/launchers/1.3.12
           curl -L -o $HOME/.sbt/launchers/1.3.12/sbt-launch.jar https://repo1.maven.org/maven2/org/scala-sbt/sbt-launch/1.3.12/sbt-launch.jar
       - name: Install Python dependencies
         run: |
-          pip install ".[test]"
+          pip install ".[dev]"
       - name: Log Python dependencies
         run: |
           pip freeze
       - name: Build and install Gateway Provisioners
         uses: nick-invision/retry@v2.8.3
         with:
           timeout_minutes: 10
@@ -50,30 +51,26 @@
         uses: nick-invision/retry@v2.8.3
         with:
           timeout_minutes: 3
           max_attempts: 1
           command: |
             make test
 
-# Disabled for now, tokens are not in place
-#  check_release:
-#    name: Check Release
-#    runs-on: ubuntu-latest
-#    steps:
-#      - name: Checkout
-#        uses: actions/checkout@v3
-#      - name: Base Setup
-#        uses: jupyterlab/maintainer-tools/.github/actions/base-setup@v1
-#      - name: Install Dependencies
-#        run: |
-#          pip install -e .
-#      - name: Check Release
-#        uses: jupyter-server/jupyter_releaser/.github/actions/check-release@v2
-#        with:
-#          token: ${{ secrets.GITHUB_TOKEN }}
+  check_release:
+   name: Check Release
+   runs-on: ubuntu-latest
+   steps:
+     - name: Checkout
+       uses: actions/checkout@v3
+     - name: Base Setup
+       uses: jupyterlab/maintainer-tools/.github/actions/base-setup@v1
+     - name: Check Release
+       uses: jupyter-server/jupyter_releaser/.github/actions/check-release@v2
+       with:
+         token: ${{ secrets.GITHUB_TOKEN }}
 
   link_check:
     name: Check Links
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - uses: jupyterlab/maintainer-tools/.github/actions/base-setup@v1
@@ -127,15 +124,15 @@
 
   python_tests_check: # This job does nothing and is only used for the branch protection
     name: Check Jobs
     if: always()
     needs:
       - build
       - link_check
-      # - check_release
+      - check_release
       # - test_minimum_versions
       - build_docs
       - test_sdist
     runs-on: ubuntu-latest
     steps:
       - name: Decide whether the needed jobs succeeded or failed
         uses: re-actors/alls-green@release/v1
```

### Comparing `gateway_provisioners-0.1.0/.github/workflows/codeql-analysis.yml` & `gateway_provisioners-0.2.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `gateway_provisioners-0.1.0/.github/workflows/prep-release.yml` & `gateway_provisioners-0.2.0/.github/workflows/prep-release.yml`

 * *Files identical despite different names*

### Comparing `gateway_provisioners-0.1.0/.github/workflows/publish-release.yml` & `gateway_provisioners-0.2.0/.github/workflows/publish-release.yml`

 * *Files identical despite different names*

### Comparing `gateway_provisioners-0.1.0/docs/Makefile` & `gateway_provisioners-0.2.0/docs/Makefile`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 # Internal variables.
 PAPEROPT_a4     = -D latex_paper_size=a4
 PAPEROPT_letter = -D latex_paper_size=letter
 ALLSPHINXOPTS   = -d $(BUILDDIR)/doctrees $(PAPEROPT_$(PAPER)) $(SPHINXOPTS) source
 # the i18n builder cannot share the environment and doctrees with the others
 I18NSPHINXOPTS  = $(PAPEROPT_$(PAPER)) $(SPHINXOPTS) source
 
-DOC_REQUIREMENTS = doc-requirements.txt
 
 .PHONY: help clean html dirhtml singlehtml pickle json htmlhelp qthelp devhelp epub latex latexpdf text man changes linkcheck doctest coverage gettext requirements
 
 help:
 	@echo "Please use \`make <target>' where <target> is one of"
 	@echo "  html         to make standalone HTML files"
 	@echo "  dirhtml      to make HTML files named index.html in directories"
```

### Comparing `gateway_provisioners-0.1.0/docs/make.bat` & `gateway_provisioners-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `gateway_provisioners-0.1.0/docs/source/conf.py` & `gateway_provisioners-0.2.0/docs/source/conf.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,55 +18,64 @@
 # -- General configuration ------------------------------------------------
 
 # Set indicator that a Sphinx build is occurring so that code
 # can react accordingly.
 os.environ["SPHINX_BUILD_IN_PROGRESS"] = "1"
 
 # If your documentation needs a minimal Sphinx version, state it here.
-needs_sphinx = "3.0"
+# needs_sphinx = "3.0"
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     "myst_parser",
+    "sphinx.ext.autodoc",
     "sphinx.ext.doctest",
     "sphinx.ext.intersphinx",
+    "sphinx.ext.autosummary",
     "sphinx.ext.mathjax",
+    "sphinx.ext.napoleon",
     "sphinxcontrib_github_alt",
-    "sphinxcontrib.mermaid",
+    "sphinxcontrib.blockdiag",
+    "sphinxcontrib.seqdiag",
     "sphinxcontrib.openapi",
     "sphinxemoji.sphinxemoji",
-    "sphinx_copybutton",
-    "sphinx.ext.autodoc",
-    "sphinx.ext.autosummary",
     "sphinx_autodoc_typehints",
+    "sphinx_copybutton",
 ]
 
+try:
+    import enchant  # type:ignore  # noqa
+
+    extensions += ["sphinxcontrib.spelling"]
+except ImportError:
+    pass
+
 myst_enable_extensions = ["html_image"]
 myst_heading_anchors = 4  # Needs to be 4 or higher
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # The suffix(es) of source filenames.
 source_suffix = {
     ".rst": "restructuredtext",
-    ".txt": "markdown",
+    ".txt": "text",
     ".md": "markdown",
 }
 
 # The encoding of source files.
 # source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
-project = "Jupyter Enterprise Gateway"
+project = "Gateway Provisioners"
 copyright = "2022, Project Jupyter"
 author = "Jupyter Server Team"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
@@ -96,15 +105,15 @@
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
 # The reST default role (used for this markup: `text`) to use for all
 # documents.
-# default_role = None
+default_role = "literal"
 
 # If true, '()' will be appended to :func: etc. cross-reference text.
 # add_function_parentheses = True
 
 # If true, the current module name will be prepended to all description
 # unit titles (such as .. function::).
 # add_module_names = True
@@ -127,15 +136,14 @@
 
 
 # -- Options for HTML output ----------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 html_theme = "pydata_sphinx_theme"
-# html_theme = "sphinx_book_theme"
 html_logo = "_static/jupyter-logo.png"
 
 # Add any paths that contain custom themes here, relative to this directory.
 # html_theme_path = []
 
 # The name for this set of Sphinx documents.  If None, it defaults to
 # "<project> v<release> documentation".
@@ -156,17 +164,22 @@
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ["_static"]
 
 # These paths are either relative to html_static_path
 # or fully qualified paths (eg. https://...)
-html_css_files = [
-    "custom.css",
-]
+# html_css_files = [
+#     "custom.css",
+# ]
+
+html_context = {
+    # ...
+    "default_mode": "dark"
+}
 
 # Add any extra paths that contain custom files (such as robots.txt or
 # .htaccess) here, relative to this directory. These files are copied
 # directly to the root of the documentation.
 # html_extra_path = []
 
 # If not '', a 'Last updated on:' timestamp is inserted at every page bottom,
@@ -221,37 +234,37 @@
 # html_search_options = {'type': 'default'}
 
 # The name of a javascript file (relative to the configuration directory) that
 # implements a search results scorer. If empty, the default will be used.
 # html_search_scorer = 'scorer.js'
 
 # Output file base name for HTML help builder.
-htmlhelp_basename = "EnterpriseGatewaydoc"
+htmlhelp_basename = "GatewayProvisionersdoc"
 
 # -- Options for LaTeX output ---------------------------------------------
 
-latex_elements = {
-    # The paper size ('letterpaper' or 'a4paper').
-    # 'papersize': 'letterpaper',
-    # The font size ('10pt', '11pt' or '12pt').
-    # 'pointsize': '10pt',
-    # Additional stuff for the LaTeX preamble.
-    # 'preamble': '',
-    # Latex figure (float) alignment
-    # 'figure_align': 'htbp',
-}
+# latex_elements = {
+# The paper size ('letterpaper' or 'a4paper').
+# 'papersize': 'letterpaper',
+# The font size ('10pt', '11pt' or '12pt').
+# 'pointsize': '10pt',
+# Additional stuff for the LaTeX preamble.
+# 'preamble': '',
+# Latex figure (float) alignment
+# 'figure_align': 'htbp',
+# }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title,
 #  author, documentclass [howto, manual, or own class]).
 latex_documents = [
     (
         master_doc,
-        "EnterpriseGateway.tex",
-        "Enterprise Gateway Documentation",
+        "GatewayProvisioners.tex",
+        "Gateway Provisioners Documentation",
         "https://jupyter.org",
         "manual",
     ),
 ]
 
 # The name of an image file (relative to this directory) to place at the top of
 # the title page.
@@ -296,19 +309,20 @@
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
     (
         master_doc,
-        "remmote_provisioners",
-        "Remote Provisioners Documentation",
+        "gateway_provisioners",
+        "Gateway Provisioners Documentation",
         author,
-        "RemoteProvisioners",
-        "One line description of project.",
+        "GatewayProvisioners",
+        "Gateway Provisioners provides kernel provisioners that interact with kernels launched into resource-managed "
+        "clusters or otherwise run remotely from the launching server.",
         "Miscellaneous",
     ),
 ]
 
 # Documents to append as an appendix to all manuals.
 # texinfo_appendices = []
 
@@ -318,84 +332,14 @@
 # How to display URL addresses: 'footnote', 'no', or 'inline'.
 # texinfo_show_urls = 'footnote'
 
 # If true, do not generate a @detailmenu in the "Top" node's menu.
 # texinfo_no_detailmenu = False
 
 
-# -- Options for Epub output ----------------------------------------------
-
-# Bibliographic Dublin Core info.
-epub_title = project
-epub_author = author
-epub_publisher = author
-epub_copyright = copyright
-
-# The basename for the epub file. It defaults to the project name.
-# epub_basename = project
-
-# The HTML theme for the epub output. Since the default themes are not optimized
-# for small screen space, using the same theme for HTML and epub output is
-# usually not wise. This defaults to 'epub', a theme designed to save visual
-# space.
-# epub_theme = 'epub'
-
-# The language of the text. It defaults to the language option
-# or 'en' if the language is not set.
-# epub_language = ''
-
-# The scheme of the identifier. Typical schemes are ISBN or URL.
-# epub_scheme = ''
-
-# The unique identifier of the text. This can be a ISBN number
-# or the project homepage.
-# epub_identifier = ''
-
-# A unique identification for the text.
-# epub_uid = ''
-
-# A tuple containing the cover image and cover page html template filenames.
-# epub_cover = ()
-
-# A sequence of (type, uri, title) tuples for the guide element of content.opf.
-# epub_guide = ()
-
-# HTML files that should be inserted before the pages created by sphinx.
-# The format is a list of tuples containing the path and title.
-# epub_pre_files = []
-
-# HTML files shat should be inserted after the pages created by sphinx.
-# The format is a list of tuples containing the path and title.
-# epub_post_files = []
-
-# A list of files that should not be packed into the epub file.
-epub_exclude_files = ["search.html"]
-
-# The depth of the table of contents in toc.ncx.
-# epub_tocdepth = 3
-
-# Allow duplicate toc entries.
-# epub_tocdup = True
-
-# Choose between 'default' and 'includehidden'.
-# epub_tocscope = 'default'
-
-# Fix unsupported image types using the Pillow.
-# epub_fix_images = False
-
-# Scale large images.
-# epub_max_image_width = 0
-
-# How to display URL addresses: 'footnote', 'no', or 'inline'.
-# epub_show_urls = 'inline'
-
-# If false, no index is generated.
-# epub_use_index = True
-
-
 # Example configuration for intersphinx: refer to the Python standard library.
 intersphinx_mapping = {
     "python": ("https://docs.python.org/", None),
     "ipython": ("https://ipython.readthedocs.io/en/stable/", None),
     "jupyter": ("https://docs.jupyter.org/en/latest/", None),
     "jupyter_core": ("https://jupyter-core.readthedocs.io/en/stable/", None),
     "jupyter_client": ("https://jupyter-client.readthedocs.io/en/stable/", None),
```

### Comparing `gateway_provisioners-0.1.0/docs/source/index.rst` & `gateway_provisioners-0.2.0/docs/source/index.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Welcome to Gateway Provisioners!
 ================================
-Gateway Provisioners provides a pluggable framework for remote kernels leveraging
+`Gateway Provisioners <https://github.com/jupyter-server/gateway_provisioners>`_ provides a pluggable framework for remote kernels leveraging
 `Kernel Provisioners <https://jupyter-client.readthedocs.io/en/latest/provisioning.html>`_ introduced
 in recent versions of Jupyter Client (7.0+).  Many of the Kernel Provisioners provided by
 Gateway Provisioners are
 based on the same functionality introduced in `Enterprise Gateway's process proxy architecture
 <https://jupyter-enterprise-gateway.readthedocs.io/en/latest/contributors/system-architecture.html#process-proxy>`_,
 the difference being that Kernel Provisioners do not require the override of the ``KernelManager``
 class hierarchy, allowing *any* application that uses the ``jupyter_client`` package for its kernel
@@ -24,27 +24,20 @@
 
 1. `Users <users/index.html>`_: people using Jupyter web applications that wish to use Gateway Provisioners.
 2. `Operators <operators/index.html>`_: people deploying or serving Jupyter applications that wish to leverage Gateway Provisioners.
 3. `Developers <developers/index.html>`_: people writing applications or deploying kernels for other resource managers.
 4. `Contributors <contributors/index.html>`_: people contributing directly to the Gateway Provisioners project.
 
 If you find gaps in our documentation, please open an issue (or better yet, a pull request) on the
-Gateway Provisioners `Github repo <https://github.com/gateway-experiments/gateway_provisioners>`_.
-
-.. note::
-   The following pages are still in transition from the `Jupyter Enterprise Gateway repository
-   <https://github.com/jupyter-server/enterprise_gateway>`_.  As a result, you will find information that pertains
-   to Enterprise Gateway, but really has no application relative to Gateway Provisioners.
-   Please bear with us in these busy (and exciting) times!
+`Gateway Provisioners GitHub repo <https://github.com/jupyter-server/gateway_provisioners>`_.
 
 
 Table of Contents
 -----------------
 
 .. toctree::
    :maxdepth: 2
 
    Users <users/index>
    Operators <operators/index>
    Developers <developers/index>
    Contributors <contributors/index>
-   Other <other/index>
```

### Comparing `gateway_provisioners-0.1.0/docs/source/_static/jupyter-logo.png` & `gateway_provisioners-0.2.0/docs/source/_static/jupyter-logo.png`

 * *Files identical despite different names*

### Comparing `gateway_provisioners-0.1.0/docs/source/api/gateway_provisioners.cli.rst` & `gateway_provisioners-0.2.0/docs/source/api/gateway_provisioners.cli.rst`

 * *Files identical despite different names*

### Comparing `gateway_provisioners-0.1.0/docs/source/api/gateway_provisioners.rst` & `gateway_provisioners-0.2.0/docs/source/api/gateway_provisioners.rst`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,20 @@
 
 .. automodule:: gateway_provisioners.container
    :members:
    :undoc-members:
    :show-inheritance:
 
 
+.. automodule:: gateway_provisioners.crd
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+
 .. automodule:: gateway_provisioners.distributed
    :members:
    :undoc-members:
    :show-inheritance:
 
 
 .. automodule:: gateway_provisioners.docker_swarm
@@ -51,14 +57,20 @@
 
 .. automodule:: gateway_provisioners.response_manager
    :members:
    :undoc-members:
    :show-inheritance:
 
 
+.. automodule:: gateway_provisioners.spark_operator
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+
 .. automodule:: gateway_provisioners.yarn
    :members:
    :undoc-members:
    :show-inheritance:
 
 Module contents
 ---------------
```

### Comparing `gateway_provisioners-0.1.0/docs/source/contributors/contrib.md` & `gateway_provisioners-0.2.0/docs/source/contributors/contrib.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # Contributing to Gateway Provisioners
 
 Thank you for your interest in Gateway Provisioners! If you would like to contribute to the
 project please first take a look at the
 [Project Jupyter Contributor Documentation](https://jupyter.readthedocs.io/en/latest/contributing/content-contributor.html).
 
-Although not officially in the organization Gateway Provisioners is affiliated with the
-[Jupyter Server organization](https://github.com/jupyter-server) as it is maintained by
-several team members.
-Please check out our [team compass page](https://github.com/jupyter-server/team-compass#jupyter-server-team-compass)
-and try to attend our weekly dev meeting as we have a common goal of making all Jupyter server-side
-applications better!
+Gateway Provisioners is affiliated with the [Jupyter Server organization](https://github.com/jupyter-server) as
+it is maintained by several team members. Please check out our
+[team compass page](https://github.com/jupyter-server/team-compass#jupyter-server-team-compass) and try to attend
+our weekly dev meeting as we have a common goal of making all Jupyter server-side applications better!
 
 Prior to your contribution, we strongly recommend getting acquainted with Gateway Provisioners by checking
 out the [System Architecture](system-architecture.md) and [Development Workflow](devinstall.md) pages.
```

### Comparing `gateway_provisioners-0.1.0/docs/source/contributors/devinstall.md` & `gateway_provisioners-0.2.0/docs/source/contributors/devinstall.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,73 +1,111 @@
 # Development Workflow
 
-Here are instructions for setting up a development environment for the \[Gateway Provisioners\]https://github.com/gateway-experiments/gateway_provisioners)
+Here are instructions for setting up a development environment for the
+[Gateway Provisioners](https://github.com/jupyter-server/gateway_provisioners)
 project. It also includes common steps in the developer workflow such as building Gateway Provisioners,
-running tests, building docs, packaging kernel specifications, etc.
+running tests, building docs, etc.
 
 ## Prerequisites
 
+There are a couple of globally-scoped commands that are necessary to build Gateway Provisioners: `make` and `sbt`.
+
 ### `make`
 
 Our build framework is based on `make` so please ensure that [GNU make](https://www.gnu.org/software/make/) is
-installed on your system.  Note: if you use the typical `python -m build --wheel` command, it will bypass
-the build of the Scala launcher (see next item).
+installed on your system.
+
+```{admonition} Important!
+:class: warning
+If you use the typical `python -m build --wheel` or `hatch run build` commands, the Scala Launcher build (see next item)
+will not occur!  Always use `make dist` to build the distribution.
+```
 
 ### `sbt`
 
 Our Scala launcher is built using `sbt`
 ([Scala Build Tool](https://www.scala-sbt.org/index.html)).  Please check
 [here](https://www.scala-sbt.org/1.x/docs/Setup.html) for installation instructions for your platform.
-Our `make build-dependencies` target will check that `sbt` is in your path and issue a warning
-if it can't find such a file, but continues with the build.
 
 ## Clone the repo
 
 Clone this repository into a local directory.
 
 ```bash
 # make a directory under your HOME directory to put the source code
 mkdir -p ~/projects
-cd !$
+cd ~/projects
 
 # clone this repo
-git clone https://github.com/gateway-experiments/gateway_provisioners.git
+git clone https://github.com/jupyter-server/gateway_provisioners.git
 ```
 
 ## Make
 
 Gateway Provisioner's build environment is centered around `make` and the
-corresponding [`Makefile`](https://github.com/gateway-experiments/gateway_provisioners/blob/main/Makefile).
+corresponding [`Makefile`](https://github.com/jupyter-server/gateway_provisioners/blob/main/Makefile).
 
 Entering `make` with no parameters yields the following:
 
 ```text
-build-dependencies             Install packages necessary to complete the build
-clean-images                   Remove all docker images.  Targets clean-base-images and clean-kernel-images can also be used.
-clean                          Remove all build, test, coverage, and Python artifacts
-dist                           Build wheel and source distributions
-docs                           Generate Sphinx HTML documentation, including API docs
-images                         Build all docker images.  Targets base-images and kernel-images can also be used.
-install                        Install the package to the active Python's site-packages
-lint                           Check style and linting using pre-commit
-push-images                    Push all docker images.  Targets push-base-images and push-kernel-images can also be used.
-release                        Package and upload a release using twine
-test                           Run tests with the currently active Python version
+clean-images         Remove all docker images.  Targets clean-base-images, clean-kernel-images, and clean-app-images can also be used.
+clean                Remove all build, test, coverage, and Python artifacts
+dist                 Build wheel and source distributions
+docs                 Generate Sphinx HTML documentation, including API docs
+helm-chart           Make helm chart distribution
+images               Build all docker images.  Targets base-images, kernel-images, and app-images can also be used.
+install              Install the built package to the active Python's site-packages
+lint-fix             Run lint with updates enabled
+lint                 Check style and linting
+push-images          Push all docker images.  Targets push-base-images, push-kernel-images, push-app-images can also be used.
+release              Package and upload a release using twine
+test                 Run tests with the currently active Python version
 ```
 
 A typical sequence of commands might include the following:
 
-```bash
-# clean the environment
-make clean
+- Clean the current build environment
+
+  ```text
+  make clean
+  ```
+
+- Apply changes and ensure updates pass lint
+
+  ```text
+  make lint
+  ```
+
+- If lint-related errors are present, they can usually be fixed using `lint-fix`
+
+  ```text
+  make lint-fix
+  ```
+
+- Build the distribution
+
+  ```text
+  make dist
+  ```
+
+- Run tests via Makefile (`pytest -v`)
+
+  ```text
+  make test
+  ```
+
+- Build the docs
 
-# apply changes and ensure updates pass lint
-make lint
+  ```text
+  make docs
+  ```
 
-# build and install changes
-make install
+- Build the images
 
-# run tests via Makefile (and manually)
-make test
+  ```text
+  make images
+  ```
 
-# checkin and push commits as necessary
+```{seealso}
+See [Kernel-image Dockerfiles](../operators/installing-kernels-container.md#kernel-image-dockerfiles) in our
+Operators Guide for additional information regarding image Dockerfiles, build arguments, etc.
 ```
```

### Comparing `gateway_provisioners-0.1.0/docs/source/contributors/system-architecture.md` & `gateway_provisioners-0.2.0/docs/source/contributors/system-architecture.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,192 +1,262 @@
 # System Architecture
 
-Below are sections presenting details of the Gateway Provisioners internals and other related items. While we will attempt to maintain its consistency, the ultimate answers are in the code itself.
+Below are sections presenting details of the Gateway Provisioners internals and other related items. While
+we will attempt to maintain its consistency, the ultimate answers are in the code itself.
 
 ## Gateway Provisioners
 
-Process proxy classes derive from the abstract base class `BaseProvisionerABC` - which defines the four basic
-process methods. There are two immediate subclasses of `BaseProvisionerABC` - `LocalProvisioner`
-and `RemoteProvisionerBase`.
+Gateway provisioner classes derive from the abstract base class
+[`KernelProvisionerBase`](https://github.com/jupyter/jupyter_client/blob/adff6b1d4389c885ee7ff4764fc5ffad6fcbe53f/jupyter_client/provisioning/provisioner_base.py#L17) -
+which defines abstract methods for managing the kernel process's lifecycle. There are two immediate subclasses of
+`KernelProvisionerBase` - [`LocalProvisioner`](https://github.com/jupyter/jupyter_client/blob/adff6b1d4389c885ee7ff4764fc5ffad6fcbe53f/jupyter_client/provisioning/local_provisioner.py#L16)
+(provided by `jupyter_client`) and [`RemoteProvisionerBase`](https://github.com/jupyter-server/gateway_provisioners/blob/d400f6f48de61823c596e4f774a42b01b17e6887/gateway_provisioners/remote_provisioner.py#L75) -
+the base class of all Gateway Provisioners' provisioners.
 
 `LocalProvisioner` is essentially a pass-through to the current implementation. Kernel specifications that do not contain
 a `process_proxy` stanza will use `LocalProvisioner`.
 
-`RemoteProvisionerBase` is an abstract base class representing remote kernel processes. Currently, there are seven
-built-in subclasses of `RemoteProvisionerBase` ...
+`RemoteProvisionerBase` is an abstract base class representing remote kernel processes. Currently, there are five
+built-in subclasses of `RemoteProvisionerBase`:
 
-- `DistributedProvisioner` - largely a proof of concept class, `DistributedProvisioner` is responsible for the launch
+- [`DistributedProvisioner`](https://github.com/jupyter-server/gateway_provisioners/blob/d400f6f48de61823c596e4f774a42b01b17e6887/gateway_provisioners/distributed.py#L65) -
+  largely a proof of concept class, `DistributedProvisioner` is responsible for the launch
   and management of kernels distributed across an explicitly defined set of hosts using ssh. Hosts are determined
   via a round-robin algorithm (that we should make pluggable someday).
-- `YarnProvisioner` - is responsible for the discovery and management of kernels hosted as Hadoop YARN applications
-  within a managed cluster.
-- `KubernetesProvisioner` - is responsible for the discovery and management of kernels hosted
-  within a Kubernetes cluster.
-- `DockerSwarmProvisioner` - is responsible for the discovery and management of kernels hosted
-  within a Docker Swarm cluster.
-- `DockerProvisioner` - is responsible for the discovery and management of kernels hosted
-  within Docker configuration. Note: because these kernels will always run local to the corresponding Enterprise Gateway instance, these process proxies are of limited use.
-- `ConductorClusterProvisioner` - is responsible for the discovery and management of kernels hosted
-  within an IBM Spectrum Conductor cluster.
-- `SparkOperatorProvisioner` - is responsible for the discovery and management of kernels hosted
-  within a Kubernetes cluster but created as a `SparkApplication` instead of a Pod. The `SparkApplication` is a Kubernetes custom resource
-  defined inside the project [spark-on-k8s-operator](https://github.com/GoogleCloudPlatform/spark-on-k8s-operator), which
-  makes all kinds of spark on k8s components better organized and easy to configure.
-
-```{note}
-Before you run a kernel associated with `SparkOperatorProvisioner`, ensure that the [Kubernetes Operator for Apache Spark is installed](https://github.com/GoogleCloudPlatform/spark-on-k8s-operator#installation) in your Kubernetes cluster.
-```
-
-You might notice that the last six process proxies do not necessarily control the _launch_ of the kernel. This is
-because the native jupyter framework is utilized such that the script that is invoked by the framework is what
-launches the kernel against that particular resource manager. As a result, the _startup time_ actions of these process
-proxies is more about discovering where the kernel _landed_ within the cluster in order to establish a mechanism for
-determining lifetime. _Discovery_ typically consists of using the resource manager's API to locate the kernel whose name includes its kernel ID
-in some fashion.
-
-On the other hand, the `DistributedProvisioner` essentially wraps the kernel specification's argument vector (i.e., invocation
-string) in a remote shell since the host is determined by Enterprise Gateway, eliminating the discovery step from
-its implementation.
-
-These class definitions can be found in the
-[processproxies package](https://github.com/jupyter-server/enterprise_gateway/blob/main/enterprise_gateway/services/processproxies). However,
-Enterprise Gateway is architected such that additional process proxy implementations can be provided and are not
-required to be located within the Enterprise Gateway hierarchy - i.e., we embrace a _bring your own process proxy_ model.
-
-![Process Class Hierarchy](../images/process_proxy_hierarchy.png)
-
-### RemoteProvisionerBase
-
-As noted above, `RemoteProvisionerBase` is an abstract base class that derives from `BaseProvisionerABC`. Subclasses
-of `RemoteProvisionerBase` must implement two methods - `confirm_remote_startup()` and `handle_timeout()`:
-
-```python
-@abstractmethod
-def confirm_remote_startup(self, kernel_cmd, **kw):
+- [`YarnProvisioner`](https://github.com/jupyter-server/gateway_provisioners/blob/d400f6f48de61823c596e4f774a42b01b17e6887/gateway_provisioners/yarn.py#L42) -
+  is responsible for the discovery and management of kernels hosted as Hadoop YARN applications within a managed cluster.
+- [`KubernetesProvisioner`](https://github.com/jupyter-server/gateway_provisioners/blob/d400f6f48de61823c596e4f774a42b01b17e6887/gateway_provisioners/k8s.py#L56) -
+  is responsible for the discovery and management of kernels hosted within a Kubernetes cluster.
+- [`SparkOperatorProvisioner`](https://github.com/jupyter-server/gateway_provisioners/blob/4c82a803614e8b26803d4a25c18683e3e5f4ec06/gateway_provisioners/spark_operator.py#L8) -
+  is responsible for the discovery and management of kernels hosted within a Kubernetes cluster that are provisioned via
+  the Custom Resource Definition (CRD) `SparkApplication`.
+- [`DockerSwarmProvisioner`](https://github.com/jupyter-server/gateway_provisioners/blob/d400f6f48de61823c596e4f774a42b01b17e6887/gateway_provisioners/docker_swarm.py#L33) -
+  is responsible for the discovery and management of kernels hosted within a Docker Swarm cluster.
+- [`DockerProvisioner`](https://github.com/jupyter-server/gateway_provisioners/blob/d400f6f48de61823c596e4f774a42b01b17e6887/gateway_provisioners/docker_swarm.py#L159) -
+  is responsible for the discovery and management of kernels hosted within Docker configuration.
+
+```{attention}
+  Because `DockerProvisioner` kernels will always run local to the corresponding host application instance, these
+  provisioners are of limited use from a resource optimization standpoint.
+```
+
+You might notice that the last four provisioners do not necessarily control the _launch_ of the kernel. This is
+because the native Jupyter framework is utilized such that the script that is invoked by the framework is what
+launches the kernel against that particular resource manager. As a result, the _startup time_ actions of these remote
+provisioners is dedicated to discovering where the kernel _landed_ within the cluster. _Discovery_ typically consists
+of using the resource manager's API to locate the kernel whose "identifier" includes its kernel ID in some fashion.
+
+On the other hand, the `DistributedProvisioner` essentially wraps the kernel specification's argument vector (i.e.,
+invocation string) in a remote shell since the host is determined by Gateway Provisioners, eliminating the discovery
+step from its implementation.
+
+### Gateway Provisioner Class Hierarchy
+
+The following block diagram depicts the current class hierarchy for the Gateway Provisioners.  The blocks with an
+`ABC` badge and dashed border indicate abstract base classes.  Those light blue blocks come from `jupyter_client`,
+while the others reside in Gateway Provisioners.
+
+```{blockdiag}
+blockdiag {
+  node_width = 200;
+  node_height = 50;
+  orientation = portrait;
+  edge_layout = normal;
+  default_node_color = pink;
+
+  KernelProvisionerBase <- RemoteProvisionerBase <- ContainerProvisionerBase <- KubernetesProvisioner
+  KernelProvisionerBase <- RemoteProvisionerBase <- ContainerProvisionerBase <- KubernetesProvisioner <- CustomResourceProvisioner <- SparkOperatorProvisioner
+  KernelProvisionerBase <- RemoteProvisionerBase <- ContainerProvisionerBase <- DockerSwarmProvisioner
+  KernelProvisionerBase <- RemoteProvisionerBase <- ContainerProvisionerBase <- DockerProvisioner
+  KernelProvisionerBase <- RemoteProvisionerBase <- DistributedProvisioner
+  KernelProvisionerBase <- RemoteProvisionerBase <- YarnProvisioner
+  KernelProvisionerBase <- LocalProvisioner
+
+  KernelProvisionerBase, LocalProvisioner [color = lightblue];
+  RemoteProvisionerBase, ContainerProvisionerBase, DistributedProvisioner, YarnProvisioner, KubernetesProvisioner, CustomResourceProvisioner, SparkOperatorProvisioner, DockerSwarmProvisioner, DockerProvisioner  [color = lightyellow];
+  KernelProvisionerBase, RemoteProvisionerBase, ContainerProvisionerBase, CustomResourceProvisioner [style = dashed, numbered = ABC];
+}
 ```
 
-where
+### `RemoteProvisionerBase`
 
-- `kernel_cmd` is a list (argument vector) that should be invoked to launch the kernel. This parameter is an
-  artifact of the kernel manager `_launch_kernel()` method.
-- `**kw` is a set key-word arguments.
-
-`confirm_remote_startup()` is responsible for detecting that the remote kernel has been appropriately launched and is ready to receive requests. This can include gathering application status from the remote resource manager but is really a function of having received the connection information from the remote kernel launcher. (See [Kernel Launchers](#kernel-launchers))
+As noted above, `RemoteProvisionerBase` is an abstract base class that derives from `KernelProvisionerBase`. Subclasses
+of `RemoteProvisionerBase` must also implement `confirm_remote_startup()` and `log_kernel_launch()`, and are
+encouraged to override `handle_launch_timeout()`:
 
 ```python
-@abstractmethod
-def handle_timeout(self):
-```
-
-`handle_timeout()` is responsible for detecting that the remote kernel has failed to startup in an acceptable time. It
-should be called from `confirm_remote_startup()`. If the timeout expires, `handle_timeout()` should throw HTTP
-Error 500 (`Internal Server Error`).
-
-Kernel launch timeout expiration is expressed via the environment variable `KERNEL_LAUNCH_TIMEOUT`. If this
-value does not exist, it defaults to the Enterprise Gateway process environment variable `EG_KERNEL_LAUNCH_TIMEOUT` - which
-defaults to 30 seconds if unspecified. Since all `KERNEL_` environment variables "flow" from the Notebook server, the launch
-timeout can be specified as a client attribute of the Notebook session.
-
-#### YarnProvisioner
-
-As part of its base offering, Enterprise Gateway provides an implementation of a process proxy that communicates with the Hadoop YARN resource manager that has been instructed to launch a kernel on one of its worker nodes. The node on which the kernel is launched is up to the resource manager - which enables an optimized distribution of kernel resources.
-
-Derived from `RemoteProvisionerBase`, `YarnProvisioner` uses the `yarn-api-client` library to locate the kernel and monitor its lifecycle. However, once the kernel has returned its connection information, the primary kernel operations naturally take place over the ZeroMQ ports.
-
-This process proxy is reliant on the `--EnterpriseGatewayApp.yarn_endpoint` command line option or the `EG_YARN_ENDPOINT` environment variable to determine where the YARN resource manager is located. To accommodate increased flexibility, the endpoint definition can be defined within the process proxy stanza of the kernel specification, enabling the ability to direct specific kernels to different YARN clusters.
-
-In cases where the YARN cluster is configured for high availability, then the `--EnterpriseGatewayApp.alt_yarn_endpoint` command line option or the `EG_ALT_YARN_ENDPOINT` environment variable should also be defined. When set, the underlying `yarn-api-client` library will choose the active Resource Manager between the two.
+    @abstractmethod
+    async def confirm_remote_startup(self):
+        """Confirms the remote process has started and returned necessary connection information."""
+
+    @abstractmethod
+    def log_kernel_launch(self, cmd: List[str]) -> None:
+        """Logs the kernel launch from the respective remote provisioner"""
+
+    async def handle_launch_timeout(self):
+        """
+        Checks to see if the kernel launch timeout has been exceeded while awaiting connection info.
+        """
+```
+
+#### `YarnProvisioner`
+
+As part of its base offering, Gateway Provisioners provides an implementation of a kernel provisioner that communicates
+with the Hadoop YARN resource manager that has been instructed to launch a kernel on one of its worker nodes. The node
+on which the kernel is launched is up to the resource manager - which enables an optimized distribution of kernel
+resources.
+
+Derived from `RemoteProvisionerBase`, `YarnProvisioner` uses the [`yarn-api-client`](https://github.com/CODAIT/hadoop-yarn-api-python-client)
+library to locate the kernel and monitor its lifecycle. However, once the kernel has returned its connection
+information, the primary kernel operations naturally take place over the ZeroMQ ports.
+
+This provisioner is reliant on the `c.YarnProvisioner.yarn_endpoint` configurable option or the `GP_YARN_ENDPOINT`
+environment variable to determine where the YARN resource manager is located. To accommodate increased flexibility,
+the endpoint definition can be defined within the process proxy stanza of the kernel specification, enabling the
+ability to direct specific kernels to different YARN clusters.
+
+In cases where the YARN cluster is configured for high availability, then the `c.YarnProvisioner.alt_yarn_endpoint`
+command line option or the `GP_ALT_YARN_ENDPOINT` environment variable should also be defined. When set, the
+underlying `yarn-api-client` library will choose the active Resource Manager between the two.
 
 ```{note}
-If Enterprise Gateway is running on an edge node of the cluster and has a valid `yarn-site.xml` file in HADOOP_CONF_DIR, neither of these values are required (default = None).  In such cases, the `yarn-api-client` library will choose the active Resource Manager from the configuration files.
+If the host application is running on an edge node of the cluster and has a valid `yarn-site.xml` file in
+`HADOOP_CONF_DIR`, neither of these values are required (default = None).  In such cases, the `yarn-api-client`
+library will choose the active Resource Manager from the configuration files.
 ```
 
 ```{seealso}
-[Hadoop YARN deployments](../operators/deploy-yarn-cluster.md) in the Operators Guide for details.
+- [Hadoop YARN deployments](../operators/deploy-yarn-cluster.md) for deployment details.
+- [`YarnProvisioner` configuration options](../operators/config-file.md#yarnprovisioner) for other options.
 ```
 
-#### DistributedProvisioner
+#### `DistributedProvisioner`
 
 Like `YarnProvisioner`, Gateway Provisioners also provides an implementation of a basic
-round-robin remoting mechanism that is part of the `DistributedProvisioner` class. This class
+remoting mechanism that is part of the `DistributedProvisioner` class. This class
 uses the `c.DistributedProvisioner.remote_hosts` configuration option (or `GP_REMOTE_HOSTS`
-environment variable) to determine on which hosts a given kernel should be launched. It uses
-a basic round-robin algorithm to index into the list of remote hosts for selecting the target
-host. It then uses ssh to launch the kernel on the target host. As a result, all kernel specification
-files must reside on the remote hosts in the same directory structure as on the Enterprise
-Gateway server.
+environment variable) to determine on which hosts a given kernel should be launched. By default,
+`DistributedProvisioner` uses a basic round-robin algorithm to determine the target
+host of those configured in `remote_hosts`. (See [Specifying a load-balancing algorithm](../operators/deploy-distributed.md#specifying-a-load-balancing-algorithm)
+for other options.) It then uses ssh to launch the kernel on
+the selected target host. As a result, **all kernel specification files must reside on the remote
+hosts in the same directory structure as on the host application server**.
 
-It should be noted that kernels launched with this process proxy run in YARN _client_ mode - so their
-resources (within the kernel process itself) are not managed by the Hadoop YARN resource manager.
+It should be noted that spark-based kernels launched with `DistributedProvisioner` run in YARN _client_ mode -
+so their resources (within the kernel process itself) are not managed by the Hadoop YARN resource manager.
 
 Like the yarn endpoint parameter the `remote_hosts` parameter can be specified within the
-process proxy configuration to override the global value - enabling finer-grained kernel distributions.
+kernel provisioner configuration to override the global value, enabling finer-grained kernel distributions.
 
 ```{seealso}
 [Distributed deployments](../operators/deploy-distributed.md) in the Operators Guide for details.
 ```
 
-#### KubernetesProvisioner
+#### `ContainerProvisionerBase`
 
-With the popularity of Kubernetes within the enterprise, Gateway Provisioners provides an implementation
-of a process proxy that communicates with the Kubernetes resource manager via the Kubernetes API. Unlike
-the other offerings, in the case of Kubernetes, Enterprise Gateway is itself deployed within the Kubernetes
-cluster as a _Service_ and _Deployment_. The primary vehicle by which this is accomplished is via [Helm](https://helm.sh/) and Enterprise Gateway provides a set of [helm chart](https://github.com/jupyter-server/enterprise_gateway/tree/main/etc/kubernetes/helm/enterprise-gateway) files to simplify deployment.
+`ContainerProvisionerBase` is an abstract base class that derives from `RemoteProvisionerBase`. It implements all
+the methods inherited from `RemoteProvsionerBase` interacting with the container API and requiring method implementations
+to perform the platform's integration.  Subclasses
+of `ContainerProvisionerBase` must also implement `get_initial_states()`,  `get_error_states()`, `get_container_status()`,
+and `terminate_container_resources()`:
 
-```{seealso}
-[Kubernetes deployments](../operators/deploy-kubernetes.md) in the Operators Guide for details.
-```
+```python
+    @abstractmethod
+    def get_initial_states(self) -> Set[str]:
+        """Return list of states (in lowercase) indicating container is starting (includes running)."""
 
-#### DockerSwarmProvisioner
+    @abstractmethod
+    def get_error_states(self) -> Set[str]:
+        """Returns the list of error states (in lowercase)."""
 
-Gateway Provisioners provides an implementation of a process proxy that communicates with the Docker Swarm resource manager via the Docker API. When used, the kernels are launched as swarm services and can reside anywhere in the managed cluster. To leverage kernels configured in this manner, Enterprise Gateway can be deployed
-either as a Docker Swarm _service_ or a traditional Docker container.
+    @abstractmethod
+    def get_container_status(self, iteration: Optional[str]) -> str:
+        """Return current container state."""
 
-A similar `DockerProvisioner` implementation has also been provided. When used, the corresponding kernel will be launched as a traditional docker container that runs local to the launching Enterprise Gateway instance. As a result, its use has limited value.
+    @abstractmethod
+    def terminate_container_resources(self, restart: bool = False) -> Optional[bool]:
+        """Terminate any artifacts created on behalf of the container's lifetime."""
+```
+
+#### `KubernetesProvisioner`
+
+With the popularity of Kubernetes within the enterprise, Gateway Provisioners provides an implementation
+of a kernel provisioner that communicates with the Kubernetes resource manager via the Kubernetes API. Because
+kernels managed by `KubernetesProvisioner` are Kubernetes Pods and have _container_ behaviors, `KubernetesProvisioner`
+derives from `ContainerProvisionerBase`. Unlike the other offerings, in the case of Kubernetes, the host application
+is itself deployed within the Kubernetes cluster as a _Service_ and _Deployment_.
 
 ```{seealso}
-[Docker and Docker Swarm deployments](../operators/deploy-docker.md) in the Operators Guide for details.
+[Kubernetes deployments](../operators/deploy-kubernetes.md) in the Operators Guide for details.
 ```
 
-#### CustomResourceProvisioner
+#### `CustomResourceProvisioner`
 
-Gateway Provisioners also provides a implementation of a process proxy derived from `KubernetesProvisioner`
+Gateway Provisioners also provides an implementation of a kernel provisioner derived from `KubernetesProvisioner`
 called `CustomResourceProvisioner`.
 
 Instead of creating kernels based on a Kubernetes pod, `CustomResourceProvisioner`
 manages kernels via a custom resource definition (CRD). For example, `SparkApplication` is a CRD that includes
 many components of a Spark-on-Kubernetes application.
 
-If you are going to extend `CustomResourceProvisioner`, just follow steps below:
+`CustomResourceProvisioner` could be considered a _virtual abstract base class_ that provides the necessary method overrides of
+`KubernetesProvisioner` to manage the lifecycle of CRDs.  If you are going to extend `CustomResourceProvisioner`,
+all that should be necessary is to override these custom resource related attributes (i.e. `group`, `version`, `plural` and
+`object_kind`) that define the CRD attributes and its implementation should cover the rest.  Note that `object_kind` is
+an internal attribute that Gateway Provisioners uses, while the other attributes are associated with the Kubernetes CRD
+object definition.
+
+```{admonition} Note
+`CustomResourceProvisioner` is considered a _virtual_ ABC in that an instance of `CustomResourceProvisioner` _could_
+be instantiated, but it wouldn't be usable because it doesn't define the necessary attribute values
+to function.  In addition, the class itself doesn't define any abstract methods (today).
+```
+
+#### `SparkOperatorProvisioner`
+
+A great example of a `CustomResourceProvisioner` is `SparkOperatorProvisioner`.  As described in the previous section,
+it's implementation consists of overrides of attributes `group` (e.g, `"sparkoperator.k8s.io"`), `version`
+(i.e., `"v1beta2"`), `plural` (i.e., `"sparkapplications"`) and `object_kind` (i.e., `"SparkApplication"`).
+
+```{seealso}
+[Deploying Custom Resource Definitions](../operators/deploy-kubernetes.md#deploying-custom-resource-definitions) in the
+Operators Guide for details.
+```
 
-- override custom resource related variables(i.e. `group`, `version` and `plural`
-  and `get_container_status` method, wrt [launch_kubernetes.py](https://github.com/jupyter-server/enterprise_gateway/blob/main/etc/kernel-launchers/kubernetes/scripts/launch_kubernetes.py).
+#### `DockerSwarmProvisioner`
 
-- define a jinja template like
-  [kernel-pod.yaml.j2](https://github.com/jupyter-server/enterprise_gateway/blob/main/etc/kernel-launchers/kubernetes/scripts/kernel-pod.yaml.j2).
-  As a generic design, the template file should be named as {crd_group}-{crd_version} so that you can reuse
-  [launch_kubernetes.py](https://github.com/jupyter-server/enterprise_gateway/blob/main/etc/kernel-launchers/kubernetes/scripts/launch_kubernetes.py) in the kernelspec.
+Gateway Provisioners provides an implementation of a kernel provisioner that communicates with the Docker Swarm resource
+manager via the Docker API. When used, the kernels are launched as swarm services and can reside anywhere in the
+managed cluster.  The core of a Docker Swarm service is a container, so `DockerSwarmProvisioner` derives from
+`ContainerProvisionerBase`. To leverage kernels configured in this manner, the host application can be deployed either
+as a Docker Swarm _service_ or a traditional Docker container.
 
-- define a kernel specification like [spark_python_operator/kernel.json](https://github.com/jupyter-server/enterprise_gateway/blob/main/etc/kernelspecs/spark_python_operator/kernel.json).
+A similar `DockerProvisioner` implementation has also been provided. When used, the corresponding kernel will be
+launched as a traditional docker container that runs local to the launching host application. As a result,
+its use has limited value to address resource optimization.
+
+```{seealso}
+[Docker and Docker Swarm deployments](../operators/deploy-docker.md) in the Operators Guide for details.
+```
 
 ### Gateway Provisioners Configuration
 
 Each `kernel.json`'s `kernel_provisioner` stanza can specify an optional `config` stanza that is converted
 into a dictionary of name/value pairs and passed as an argument to each kernel provisioner's constructor
 relative to the provisioner identified by the `provisioner_name` entry.
 
 How each dictionary entry is interpreted is completely a function of the constructor relative to that provisioner
 class or its superclass. For example, an alternate list of remote hosts has meaning to the `DistributedProvisioner` but
 not to its superclasses. As a result, the superclass constructors will not attempt to interpret that value.
 
-In addition, certain dictionary entries can override or amend system-level configuration values set on the command-line, thereby
-allowing administrators to tune behaviors down to the kernel level. For example, an administrator might want to
-constrain Python kernels configured to use specific resources to an entirely different set of hosts (and ports) that other
-remote kernels might be targeting in order to isolate valuable resources. Similarly, an administrator might want to
-only authorize specific users to a given kernel.
+In addition, certain dictionary entries can override or amend system-level configuration values set in the
+application's configuration file, thereby allowing administrators to tune behaviors down to the kernel level.
+For example, an administrator might want to constrain Python kernels configured to use specific resources to an
+entirely different set of hosts (and ports) that other remote kernels might be targeting in order to isolate
+valuable resources. Similarly, an administrator might want to only authorize specific users to a given kernel.
 
 In such situations, one might find the following `kernel_provisioner` stanza:
 
 ```json
 {
   "metadata": {
     "kernel_provisioner": {
@@ -197,117 +267,145 @@
         "authorized_users": "bob,alice"
       }
     }
   }
 }
 ```
 
-In this example, the kernel associated with this `kernel.json` file is relegated to the hosts `priv_host1` and `priv_host2`
+In this example, the kernel associated with this `kernel.json` file is relegated to hosts `priv_host1` and `priv_host2`
 where kernel ports will be restricted to a range between `40000` and `41000` and only users `bob` and `alice` can
 launch such kernels (provided neither appear in the global set of `unauthorized_users` since denial takes precedence).
 
 For a current enumeration of which system-level configuration values can be overridden or amended on a per-kernel basis
 see [Per-kernel overrides](../operators/config-kernel-override.md).
 
+```{seealso}
+[Configuration Options](../operators/config-file.md#configuration-options) in our Operators Guide for an overview of all options.
+```
+
 ## Kernel Launchers
 
 As noted above, a kernel is considered started once the `launch_process()` method has conveyed its connection
 information back to the Gateway Provisioner's server process. Conveyance of connection information
 from a remote kernel is the responsibility of the remote kernel _launcher_.
 
 Kernel launchers provide a means of normalizing behaviors across kernels while avoiding kernel
 modifications. Besides providing a location where connection file creation can occur, they also
 provide a 'hook' for other kinds of behaviors - like establishing virtual environments or
 sandboxes, providing collaboration behavior, adhering to port range restrictions, etc.
 
 There are four primary tasks of a kernel launcher:
 
 1. Creation of the connection file and ZMQ ports on the remote (target) system along with a _server listener_ socket
-1. Conveyance of the connection (and listener socket) information back to the Gateway Provisioner's server process
+1. Conveyance of the connection (and listener socket) information back to the Gateway Provisioner's host application
 1. Invocation of the target kernel
 1. Listen for interrupt and shutdown requests from the Gateway Provisioner's server and carry out the action when appropriate
 
-Kernel launchers are minimally invoked with three parameters (all of which are conveyed by the `argv` stanza of the corresponding `kernel.json` file) - the kernel's ID as created by the server and conveyed via the placeholder `{kernel_id}`, a response address consisting of the Gateway Provisioner's server's IP and port on which to return the connection information similarly represented by the placeholder `{response_address}`, and a public-key used by the launcher to encrypt an AES key that encrypts the kernel's connection information back to the server and represented by the placeholder `{public_key}`.
-
-The kernel's ID is identified by the parameter `--kernel-id`. Its value (`{kernel_id}`) is essentially used to build a connection file to pass to the to-be-launched kernel, along with any other things - like log files, etc.
-
-The response address is identified by the parameter `--response-address`. Its value (`{response_address}`) consists of a string of the form `<IPV4:port>` where the IPV4 address points back to the Gateway Provisioner's server - which is listening for a response on the provided port. The port's default value is `8877`, but can be specified via the environment variable `GP_RESPONSE_PORT`.
-
-The public key is identified by the parameter `--public-key`. Its value (`{public_key}`) is used to encrypt an AES key created by the launcher to encrypt the kernel's connection information. The server, upon receipt of the response, uses the corresponding private key to decrypt the AES key, which it then uses to decrypt the connection information. Both the public and private keys are ephemeral; created upon Enterprise Gateway's startup. They can be ephemeral because they are only needed during a kernel's startup and never again.
+Kernel launchers are minimally invoked with three parameters (all of which are conveyed by the `argv` stanza of the
+corresponding `kernel.json` file): the kernel's ID as created by the server and conveyed via the
+placeholder `{kernel_id}`, a response address consisting of the Gateway Provisioner's server's IP and port on
+which to return the connection information similarly represented by the placeholder `{response_address}`, and a
+public-key used by the launcher to encrypt an AES key that, in turn, encrypts the kernel's connection information back to the
+server and represented by the placeholder `{public_key}`.
+
+The kernel's ID is identified by the parameter `--kernel-id`. Its value (`{kernel_id}`) is essentially used to build
+a connection file to pass to the to-be-launched kernel, along with any other things - like log files, etc.
+
+The response address is identified by the parameter `--response-address`. Its value (`{response_address}`) consists of
+a string of the form `<IPV4:port>` where the IPV4 address points back to the Gateway Provisioner's server - which is
+listening for a response on the provided port. The port's default value is `8877`, but can be specified via the
+environment variable `GP_RESPONSE_PORT`.
+
+The public key is identified by the parameter `--public-key`. Its value (`{public_key}`) is used to encrypt an
+AES key created by the launcher to encrypt the kernel's connection information. The server, upon receipt of the
+response, uses the corresponding private key to decrypt the AES key, which it then uses to decrypt the connection
+information. Both the public and private keys are ephemeral; created upon the initial load of Gateway Provisioners.
+They can be ephemeral because they are only needed during a kernel's startup and never again.
 
-Here's a [kernel.json](https://github.com/jupyter-server/enterprise_gateway/blob/main/etc/kernelspecs/spark_python_yarn_cluster/kernel.json) file illustrating these parameters...
-
-FIXME - the example is process-proxy
+Here's a `kernel.json` file illustrating these parameters...
 
 ```json
 {
-  "language": "python",
-  "display_name": "Spark - Python (YARN Cluster Mode)",
-  "metadata": {
-    "process_proxy": {
-      "class_name": "enterprise_gateway.services.processproxies.yarn.YarnProvisioner"
-    }
-  },
-  "env": {
-    "SPARK_HOME": "/usr/hdp/current/spark2-client",
-    "SPARK_OPTS": "--master yarn --deploy-mode cluster --name ${KERNEL_ID:-ERROR__NO__KERNEL_ID} --conf spark.yarn.submit.waitAppCompletion=false",
-    "LAUNCH_OPTS": ""
-  },
   "argv": [
-    "/usr/local/share/jupyter/kernels/spark_python_yarn_cluster/bin/run.sh",
+    "python",
+    "/usr/local/share/jupyter/kernels/k8s_python/scripts/launch_kubernetes.py",
     "--kernel-id",
     "{kernel_id}",
+    "--port-range",
+    "{port_range}",
     "--response-address",
     "{response_address}",
     "--public-key",
-    "{public_key}"
-  ]
+    "{public_key}",
+    "--kernel-class-name",
+    "ipykernel.ipkernel.IPythonKernel"
+  ],
+  "env": {},
+  "display_name": "Kubernetes Python",
+  "language": "python",
+  "interrupt_mode": "signal",
+  "metadata": {
+    "debugger": true,
+    "kernel_provisioner": {
+      "provisioner_name": "kubernetes-provisioner",
+      "config": {
+        "image_name": "elyra/kernel-py:dev",
+        "launch_timeout": 30
+      }
+    }
+  }
 }
+
 ```
 
 Other options supported by launchers include:
 
 - `--port-range {port_range}` - passes configured port-range to launcher where launcher applies that range to kernel ports. The port-range may be configured globally or on a per-kernel specification basis, as previously described.
 
 - `--spark-context-initialization-mode [lazy|eager|none]` - indicates the _timeframe_ in which the spark context will be created.
 
   - `lazy` (default) attempts to defer initialization as late as possible - although this can vary depending on the
     underlying kernel and launcher implementation.
   - `eager` attempts to create the spark context as soon as possible.
   - `none` skips spark context creation altogether.
 
   Note that some launchers may not be able to support all modes. For example, the scala launcher uses the Apache Toree
-  kernel - which currently assumes a spark context will exist. As a result, a mode of `none` doesn't apply.
+  kernel, which currently assumes a spark context will exist. As a result, a mode of `none` doesn't apply.
   Similarly, the `lazy` and `eager` modes in the Python launcher are essentially the same, with the spark context
   creation occurring immediately, but in the background thereby minimizing the kernel's startup time.
 
-Kernel.json files also include a `LAUNCH_OPTS:` section in the `env` stanza to allow for custom
+The `kernel.json` files also include a `LAUNCH_OPTS` section in the `env` stanza to allow for custom
 parameters to be conveyed in the launcher's environment. `LAUNCH_OPTS` are then referenced in
-the [run.sh](https://github.com/jupyter-server/enterprise_gateway/blob/main/etc/kernelspecs/spark_python_yarn_cluster/bin/run.sh)
-script as the initial arguments to the launcher
-(see [launch_ipykernel.py](https://github.com/jupyter-server/enterprise_gateway/blob/main/etc/kernel-launchers/python/scripts/launch_ipykernel.py)) ...
+the `run.sh` script (for spark-based kernels) as the initial arguments to the launcher:
 
 ```bash
 eval exec \
      "${SPARK_HOME}/bin/spark-submit" \
      "${SPARK_OPTS}" \
      "${PROG_HOME}/scripts/launch_ipykernel.py" \
      "${LAUNCH_OPTS}" \
      "$@"
 ```
 
+```{seealso}
+See [Implementing a Kernel Launcher](../developers/kernel-launcher.md) in the Developers Guide for additional
+information.
+```
+
 ## Extending Gateway Provisioners
 
 Theoretically speaking, enabling a kernel for use in other frameworks amounts to the following:
 
 1. Build a kernel specification file that identifies the provisioner class to be used.
 1. Implement the provisioner class such that it supports the four primitive functions of
    `poll()`, `wait()`, `send_signal(signum)` and `kill()` along with `launch_process()`. If this
    provisioner derives from another, these method implementations can be inherited.
 1. If the provisioner corresponds to a remote process, derive the provisioner class from
-   `RemoteProvisionerBase` and implement `confirm_remote_startup()` and `handle_timeout()`.
+   `RemoteProvisionerBase` and implement `confirm_remote_startup()` and `handle_launch_timeout()`.
 1. Insert invocation of a launcher (if necessary) which builds the connection file and
-   returns its contents on the `{response_address}` socket and following the encryption protocol set forth in the other launchers.
+   returns its contents on the `{response_address}` socket and following the encryption protocol set forth in the
+   other launchers.
 
 ```{seealso}
-This topic is covered in the [Developers Guide](../developers/index.rst).
+See [Implementing a Gateway Provisioner](../developers/dev-remote-provisioner.md) in the Developers Guide for
+additional information.
 ```
```

### Comparing `gateway_provisioners-0.1.0/docs/source/developers/dev-remote-provisioner.md` & `gateway_provisioners-0.2.0/docs/source/developers/dev-remote-provisioner.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,57 @@
-# Implementing a remote provisioner
+# Implementing a Gateway Provisioner
 
-A remote provisioner implementation is necessary if you want to interact with a resource manager that is not currently supported or extend some existing behaviors. Examples of resource managers in which there's been some interest include [Slurm Workload Manager](https://slurm.schedmd.com/documentation.html) and [Apache Mesos](https://mesos.apache.org/), for example. In the end, it's really a matter of having access to an API and the ability to apply "tags" or "labels" in order to _discover_ where the kernel is running within the managed cluster. Once you have that information, then it becomes of matter of implementing the appropriate methods to control the kernel's lifecycle.
-
-## General approach
-
-Please refer to the [Remote Provisioners section](../contributors/system-architecture.md#gateway-provisioners) in the System Architecture pages for descriptions and structure of existing remote provisioners. Here is the general guideline for the process of implementing a remote provisioner.
-
-1. Identify and understand how to _decorate_ your "job" within the resource manager. In Hadoop YARN, this is done by using the kernel's ID as the _application name_ by setting the [`--name` parameter to `${KERNEL_ID}`](https://github.com/jupyter-server/enterprise_gateway/blob/54c8e31d9b17418f35454b49db691d2ce5643c22/etc/kernelspecs/spark_python_yarn_cluster/kernel.json#L14). In Kubernetes, we apply the kernel's ID to the [`kernel-id` label on the POD](https://github.com/jupyter-server/enterprise_gateway/blob/54c8e31d9b17418f35454b49db691d2ce5643c22/etc/kernel-launchers/kubernetes/scripts/kernel-pod.yaml.j2#L16).
-1. Today, all invocations of kernels into resource managers use a shell or python script mechanism configured into the `argv` stanza of the kernelspec. If you take this approach, you need to apply the necessary changes to integrate with your resource manager.
-1. Determine how to interact with the resource manager's API to _discover_ the kernel and determine on which host it's running. This interaction should occur immediately following receipt of the kernel's connection information in its response from the kernel launcher. This extra step, performed within `confirm_remote_startup()`, is necessary to get the appropriate host name as reflected in the resource manager's API.
-1. Determine how to monitor the "job" using the resource manager API. This will become part of the `poll()` implementation to determine if the kernel is still running. This should be as quick as possible since it occurs every 3 seconds. If this is an expensive call, you may need to make some adjustments like skip the call every so often.
-1. Determine how to terminate "jobs" using the resource manager API. This will become part of the termination sequence, but probably only necessary if the message-based shutdown does not work (i.e., a last resort).
+A gateway provisioner implementation is necessary if you want to interact with a resource manager that is not
+currently supported or extend some existing behaviors. Examples of resource managers in which there's been interest
+include [Slurm Workload Manager](https://slurm.schedmd.com/documentation.html) and
+[Apache Mesos](https://mesos.apache.org/), for example. In the end, it's really a matter of having access to
+an API and the ability to apply "tags" or "labels" in order to _discover_ where the kernel is running within
+the managed cluster. Once you have that information, then it becomes a matter of implementing the appropriate
+methods to control the kernel's lifecycle.
+
+## General Approach
+
+Please refer to the [Gateway Provisioners section](../contributors/system-architecture.md#gateway-provisioners) in the
+System Architecture pages for descriptions and structure of existing gateway provisioners. Here is the general
+guideline for the process of implementing a gateway provisioner.
+
+1. Identify and understand how to _decorate_ your "job" within the resource manager. For example,
+   1. In Hadoop YARN, this is done by
+      using the kernel's ID as the _application name_ by setting the
+      [`--name` parameter to `${KERNEL_ID}`](https://github.com/jupyter-server/enterprise_gateway/blob/54c8e31d9b17418f35454b49db691d2ce5643c22/etc/kernelspecs/spark_python_yarn_cluster/kernel.json#L14).
+   1. In Kubernetes, we apply the kernel's ID to the [`kernel-id` label on the POD](https://github.com/jupyter-server/enterprise_gateway/blob/54c8e31d9b17418f35454b49db691d2ce5643c22/etc/kernel-launchers/kubernetes/scripts/kernel-pod.yaml.j2#L16).
+1. Today, all invocations of kernels into resource managers use a shell or python script mechanism configured into the
+   `argv` stanza of the kernelspec. If you take this approach, you need to apply the necessary changes to integrate
+   with your resource manager.
+1. Determine how to interact with the resource manager's API to _discover_ the kernel and determine on which
+   host it's running. This interaction should occur immediately following receipt of the kernel's connection
+   information in its response from the kernel launcher. This extra step, performed within `confirm_remote_startup()`,
+   is necessary to get the appropriate host name as reflected in the resource manager's API.
+1. Determine how to monitor the "job" using the resource manager API. This will become part of the `poll()`
+   implementation to determine if the kernel is still running. This should be as quick as possible since it occurs
+   every 3 seconds. If this is an expensive call, you may need to make some adjustments like skip the call every so often.
+1. Determine how to terminate "jobs" using the resource manager API. This will become part of the kernel's termination
+   sequence, but probably only necessary if the message-based shutdown does not work (i.e., a last resort).
 
 ```{tip}
-Because kernel IDs are globally unique, they serve as ideal identifiers for discovering where in the cluster the kernel is running and are recommended "keys".
+Because kernel IDs are globally unique, they serve as ideal identifiers for discovering where in the cluster the kernel
+is running and are recommended "keys".
 ```
 
-You will likely need to provide implementations for `launch_process()`, `poll()`, `wait()`, `send_signal()`, and `kill()`, although, depending on where your provisioner resides in the class hierarchy, some implementations may be reused.
-
-For example, if your provisioner is going to service remote kernels, you should consider deriving your implementation from the [`RemoteProvisioner` class](https://github.com/jupyter-server/enterprise_gateway/blob/54c8e31d9b17418f35454b49db691d2ce5643c22/enterprise_gateway/services/processproxies/processproxy.py#L981). If this is the case, then you'll need to implement `confirm_remote_startup()`.
-
-Likewise, if your process proxy is based on containers, you should consider deriving your implementation from the [`ContainerProvisioner`](https://github.com/jupyter-server/enterprise_gateway/blob/54c8e31d9b17418f35454b49db691d2ce5643c22/enterprise_gateway/services/processproxies/container.py#L34). If this is the case, then you'll need to implement `get_container_status()` and `terminate_container_resources()` rather than `confirm_remote_startup()`, etc.
+You will likely need to provide implementations for `launch_process()`, `poll()`, `wait()`, `send_signal()`, and
+`kill()`, although, depending on where your provisioner resides in the class hierarchy, some implementations may be
+reused.
+
+For example, if your provisioner is going to service remote kernels, you should consider deriving your implementation
+from the [`RemoteProvisionerBase` class](https://github.com/jupyter-server/gateway_provisioners/blob/9de8af8a361aa779f8eb4d10585c0d917bb3731f/gateway_provisioners/remote_provisioner.py#L75).
+If this is the case, then you'll need to implement `confirm_remote_startup()`.
+
+Likewise, if your process proxy is based on containers, you should consider deriving your implementation from
+the [`ContainerProvisionerBase` class](https://github.com/jupyter-server/gateway_provisioners/blob/9de8af8a361aa779f8eb4d10585c0d917bb3731f/gateway_provisioners/container.py#L32).
+If this is the case, then you'll need to implement `get_container_status()` and `terminate_container_resources()`
+rather than `confirm_remote_startup()`, etc.
 
-Once the remote provisioner has been implemented, construct an appropriate kernel specification that references your remote provisioner and iterate until you are satisfied with how your remote kernels behave.
+Once the gateway provisioner has been implemented, construct an appropriate kernel specification that references your
+gateway provisioner and iterate until you are satisfied with how your remote kernels behave.
 
-If you intend to contribute your remote provisioner into this package, you can extend the CLI tooling to create applicable kernel specifications and launch scripts.
+If you intend to contribute your gateway provisioner into this package, you can extend the CLI tooling to create
+applicable kernel specifications and launch scripts.
```

### Comparing `gateway_provisioners-0.1.0/docs/source/developers/index.rst` & `gateway_provisioners-0.2.0/docs/source/developers/index.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Developers Guide
 ================
 
-These pages target *developers* authoring remote provisioners for other resource managers, or integrating applications with remote kernel functionality.
+These pages target *developers* authoring gateway provisioners for other resource managers, or integrating
+applications with remote kernel functionality.
 
 .. admonition:: Use cases
 
-    - *As a developer, I want to explore supporting a different resource manager with Enterprise Gateway, by implementing a new `RemoteProvsioner` class such that I can easily take advantage of specific functionality provided by the resource manager.*
+    - *As a developer, I want to explore supporting a different resource manager by implementing a new Gateway Provisioner such that I can easily take advantage of specific functionality provided by the resource manager.*
     - *As a developer, I want to easily integrate the ability to launch remote kernels with existing platforms, so I can leverage my compute cluster in a customizable way.*
     - *As a developer, I am currently using Golang and need to implement a kernel launcher to allow the Go kernel I use to run remotely in my Kubernetes cluster.*
     - *As a developer, I'd like to extend some of the kernel container images and, eventually, create my own to better enable the data scientists I support.*
 
 .. toctree::
    :maxdepth: 1
    :name: developers
```

### Comparing `gateway_provisioners-0.1.0/docs/source/developers/kernel-launcher.md` & `gateway_provisioners-0.2.0/docs/source/developers/kernel-launcher.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,84 +1,154 @@
-# Implementing a kernel launcher
+# Implementing a Kernel Launcher
 
-A new implementation for a [_kernel launcher_](../contributors/system-architecture.md#kernel-launchers) becomes necessary when you want to introduce another kind of kernel to an existing configuration. Out of the box, Remote Provisioners provides [kernel launchers](https://github.com/jupyter-server/enterprise_gateway/tree/main/etc/kernel-launchers) that support the IPython kernel, the Apache Toree scala kernel, and the R kernel - IRKernel. There are other "language-agnostic kernel launchers" provided by Remote Provisioners, but those are used in container environments to start the container or pod where the "kernel image" uses on the three _language-based_ launchers to start the kernel within the container.
+A new implementation for a [_kernel launcher_](../contributors/system-architecture.md#kernel-launchers) becomes
+necessary when you want to introduce another kind of kernel to an existing configuration. Out of the box, Gateway
+Provisioners provides [kernel launchers](https://github.com/jupyter-server/gateway_provisioners/tree/main/gateway_provisioners/kernel-launchers)
+that support the IPython kernel ([and subclasses thereof](#invoking-subclasses-of-ipykernelkernelbasekernel)), the
+Apache Toree scala kernel, and the R kernel - IRKernel. There are other "language-agnostic kernel launchers"
+provided by Remote Provisioners, but those are used in container environments to start the container or pod where
+the "kernel image" uses one of the three _language-based_ launchers to start the kernel within the container.
+
+Its generally recommended that the launcher be written in the language of the kernel, but that is not a requirement
+so long as the launcher can start and manage the kernel's lifecycle and issue interrupts (if the kernel does not
+support message-based interrupts itself).
+
+The four tasks of a kernel launcher are:
+
+1. Create the necessary connection information based on the five zero-mq ports, a signature key and algorithm
+   specifier, along with a _server listener_ socket.
+1. Conveyance of the connection (and listener socket) information back to the host application (Gateway Provisioners)
+   process after properly encrypting the information.
+1. Invocation of the target kernel.
+1. Listen for interrupt and shutdown requests from the host application on the communication socket and carry out
+   the action when appropriate.
 
-Its generally recommended that the launcher be written in the language of the kernel, but that is not a requirement so long as the launcher can start and manage the kernel's lifecycle and issue interrupts (if the kernel does not support message-based interrupts itself).
+## Creating the Connection Information
 
-To reiterate, the four tasks of a kernel launcher are:
+If your target kernel exists, then there is probably support for creating ZeroMQ ports. If this proves difficult,
+you may be able to take a _hybrid approach_ where the connection information, encryption and listener portion of
+things is implemented in Python, while invocation takes place in the native language. This is how the
+[R kernel-launcher](https://github.com/jupyter-server/gateway_provisioners/tree/main/gateway_provisioners/kernel-launchers/R/scripts)
+support is implemented.
 
-1. Create the necessary connection information based on the 5 zero-mq ports, a signature key and algorithm specifier, along with a _server listener_ socket.
-1. Conveyance of the connection (and listener socket) information back to the hosting server (Remote Provisioners) process after encrypting the information using AES, then encrypting the AES key using the provided public key.
-1. Invocation of the target kernel.
-1. Listen for interrupt and shutdown requests from the host server on the communication socket and carry out the action when appropriate.
+When creating the connection information, your kernel launcher should handle the possibility that the `--port-range`
+option has been specified such that each port should reside within the specified range.
 
-## Creating the connection information
+The port used between the host application and the kernel launcher, known as the _communication port_, should also
+adhere to the port range. It is not required that this port be ZeroMQ (and is not a ZMQ port in existing
+implementations).
 
-If your target kernel exists, then there is probably support for creating ZeroMQ ports. If this proves difficult, you may be able to take a _hybrid approach_ where the connection information, encryption and listener portion of things is implemented in Python, while invocation takes place in the native language. This is how the [R kernel-launcher](https://github.com/jupyter-server/enterprise_gateway/tree/main/etc/kernel-launchers/R/scripts) support is implemented.
+Here's where the Python (and R) [ports are selected](https://github.com/jupyter-server/gateway_provisioners/blob/main/gateway_provisioners/kernel-launchers/shared/scripts/server_listener.py#L163-L180),
+adhering to any port range restrictions.
 
-When creating the connection information, your kernel launcher should handle the possibility that the `--port-range` option has been specified such that each port should reside within the specified range.
+## Encrypting the Connection Information
 
-The port used between host server and the kernel launcher, known as the _communication port_ should also adhere to the port range. It is not required that this port be ZeroMQ (and is not a ZMQ port in existing implementations).
+The next task of the kernel launcher is sending the connection information back to the host server. Prior to doing
+this, the connection information, including the communication port, is encrypted using AES encryption and a
+16-byte key. The AES key is then encrypted using the public key specified in the `public_key` parameter. These
+two fields (the AES-encrypted payload and the public-key-encrypted AES key) are then included into a JSON
+structure that also include the launcher's version information and base64-encoded. Here's such an example
+from the [Python (and R) kernel launchers](https://github.com/jupyter-server/gateway_provisioners/blob/main/gateway_provisioners/kernel-launchers/shared/scripts/server_listener.py#L77-L100).
 
-## Encrypting the connection information
+The payload is then [sent back on a socket](https://github.com/jupyter-server/gateway_provisioners/blob/9de8af8a361aa779f8eb4d10585c0d917bb3731f/gateway_provisioners/kernel-launchers/shared/scripts/server_listener.py#L102-L139)
+identified by the `--response-address` option.
 
-The next task of the kernel launcher is sending the connection information back to the host server. Prior to doing this, the connection information, including the communication port, is encrypted using AES encryption and a 16-byte key. The AES key is then encrypted using the public key specified in the `public_key` parameter. These two fields (the AES-encrypted payload and the publice-key-encrypted AES key) are then included into a JSON structure that also include the launcher's version information and base64 encoded. Here's such an example from the [Python kernel launcher](https://github.com/jupyter-server/enterprise_gateway/blob/54c8e31d9b17418f35454b49db691d2ce5643c22/etc/kernel-launchers/python/scripts/launch_ipykernel.py#L188-L209).
+## Invoking the Target Kernel
 
-The payload is then [sent back on a socket](https://github.com/jupyter-server/enterprise_gateway/blob/54c8e31d9b17418f35454b49db691d2ce5643c22/etc/kernel-launchers/python/scripts/launch_ipykernel.py#L212-L256) identified by the `--response-address` option.
+For the R kernel launcher, the kernel is started using [`IRKernel::main()`](https://github.com/jupyter-server/gateway_provisioners/blob/9de8af8a361aa779f8eb4d10585c0d917bb3731f/gateway_provisioners/kernel-launchers/R/scripts/launch_IRkernel.R#L232)
+after the `SparkContext` is initialized based on the `spark-context-initialization-mode` parameter.
 
-## Invoking the target kernel
+The scala kernel launcher works similarly in that the Apache Toree kernel provides an
+["entrypoint" to start the kernel](https://github.com/jupyter-server/gateway_provisioners/blob/9de8af8a361aa779f8eb4d10585c0d917bb3731f/gateway_provisioners/kernel-launchers/scala/toree-launcher/src/main/scala/launcher/ToreeLauncher.scala#L312),
+however, because the Toree kernel initializes a `SparkContext` itself, the need to do so is conveyed directly to the kernel.
 
-For the R kernel launcher, the kernel is started using [`IRKernel::main()`](https://github.com/jupyter-server/enterprise_gateway/blob/54c8e31d9b17418f35454b49db691d2ce5643c22/etc/kernel-launchers/R/scripts/launch_IRkernel.R#L252) after the `SparkContext` is initialized based on the `spark-context-initialization-mode` parameter.
+For the Python kernel launcher, it creates a namespace instance that contains the `SparkContext` information, if
+requested to do so via the `spark-context-initialization-mode` parameter, instantiates an `IPKernelApp` instance
+using the configured namespace, then calls the
+[`start()`](https://github.com/ipython/ipykernel/blob/6f448d280dadbff7245f4b28b5e210c899d79342/ipykernel/kernelapp.py#L694) method.
 
-The scala kernel launcher works similarly in that the Apache Toree kernel provides an ["entrypoint" to start the kernel](https://github.com/jupyter-server/enterprise_gateway/blob/00d7376b932eacd347b3c32c863691bfbad53b86/etc/kernel-launchers/scala/toree-launcher/src/main/scala/launcher/ToreeLauncher.scala#L332), however, because the Toree kernel initializes a `SparkContext` itself, the need to do so is conveyed directly to the kernel.
+### Invoking Subclasses of `ipykernel.kernelbase.Kernel`
 
-For the Python kernel launcher, it creates a namespace instance that contains the `SparkContext` information, if requested to do so via the `spark-context-initialization-mode` parameter, instantiates an `IPKernelApp` instance using the configured namespace, then calls the [`start()`](https://github.com/ipython/ipykernel/blob/6f448d280dadbff7245f4b28b5e210c899d79342/ipykernel/kernelapp.py#L694) method.
+Because the python kernel launcher uses `IPKernelApp`, support for any subclass of `ipykernel.kernelbase.Kernel`
+can be launched by Gateway Provisioner's Python kernel launcher.
 
-### Invoking subclasses of `ipykernel.kernelbase.Kernel`
+To specify an alternate subclass, add `--kernel-class-name` (along with the specified dotted class string) to
+the `kernel.json` file's `argv` stanza. Gateway Provisioner's Python launcher will import that class and pass it as
+a parameter to `IPKernelApp.initialize()`.
 
-Because the python kernel launcher uses `IPKernelApp`, support for any subclass of `ipykernel.kernelbase.Kernel` can be launched by Remote Provisioner's Python kernel launcher.
+````{tip}
+When generating kernel specfiications via the CLI tooling, this option is available via the
+`--ipykernel-subclass-name` parameter.
 
-To specify an alternate subclass, add `--kernel-class-name` (along with the specified dotted class string) to the `kernel.json` file's `argv` stanza. Remote Provisioner's Python launcher will import that class and pass it as a parameter to `IPKernelApp.initialize()`.
+For example, to generate the equivalent of the JSON below, enter:
+```bash
+jupyter ssh-spec install --ipykernel-subclass-name echo_kernel.kernel.EchoKernel --kernel-name echo --display-name Echo
+```
+````
 
 Here's an example `kernel.json` file that launches the "echo" kernel using the `DistributedProvisioner`:
 
 ```JSON
 {
-  "display_name": "Echo",
-  "language": "text",
-  "metadata": {
-    "kernel_provisioner": {
-      "class_name": "remote_provisioners.distributed.DistributedProvisioner"
-    }
-  },
   "argv": [
     "python",
     "/usr/local/share/jupyter/kernels/echo/scripts/launch_ipykernel.py",
-    "--RemoteProcessProxy.kernel-id",
+    "--kernel-id",
     "{kernel_id}",
+    "--port-range",
+    "{port_range}",
     "--response-address",
     "{response_address}",
     "--public-key",
     "{public_key}",
-    "--spark-context-initialization-mode",
-    "none",
     "--kernel-class-name",
     "echo_kernel.kernel.EchoKernel"
-  ]
+  ],
+  "env": {},
+  "display_name": "Echo",
+  "language": "python",
+  "interrupt_mode": "signal",
+  "metadata": {
+    "debugger": true,
+    "kernel_provisioner": {
+      "provisioner_name": "distributed-provisioner",
+      "config": {
+        "launch_timeout": 30
+      }
+    }
+  }
 }
 ```
 
-```{admonition} Important!
-The referenced `kernel-class-name` package must first be properly installed on all nodes where the associated provisioner will run.
+```{attention}
+The referenced `kernel-class-name` package must be properly installed on all nodes/images where the associated
+kernel will run.
 ```
 
-## Listening for interrupt and shutdown requests
+## Listening for Interrupt and Shutdown Requests
+
+The last task that must be performed by a kernel launcher is to listen on the communication port for work. There are
+currently two requests sent on the port, a signal event and a shutdown request.
+
+### Signal Event
+
+The signal event is of the form `{"signum": n}` where the string `'signum'` indicates a signal event and `n` is
+an integer specifying the signal number to send to the kernel. Typically, the value of `n` is `2` representing
+`SIGINT` and used to interrupt any current processing. As more kernels adopt a message-based interrupt approach,
+this will not be as common. Gateway Provisioners also use this event to perform its `poll()` implementation by
+sending `{"signum": 0}`. Raising a signal of 0 to a process is a common way to determine the process is still alive.
 
-The last task that must be performed by a kernel launcher is to listen on the communication port for work. There are currently two requests sent on the port, a signal event and a shutdown request.
+### Shutdown Request
 
-The signal event is of the form `{"signum": n}` where the string `'signum'` indicates a signal event and `'n'` is an integer specifying the signal number to send to the kernel. Typically, the value of 'n' is `2` representing `SIGINT` and used to interrupt any current processing. As more kernels adopt a message-based interrupt approach, this will not be as common. Enterprise Gateway also uses this event to perform its `poll()` implementation by sending `{"signum": 0}`. Raising a signal of 0 to a process is common way to determine the process is still alive.
+A shutdown request is sent when the Gateway Provisioners has typically terminated the kernel, and it's just performing
+its final cleanup. The form of this request is `{"shutdown": 1}`. This is what instructs the launcher to abandon
+listening on the communication socket and to exit.
 
-The event is a shutdown request. This is sent when the remote provisioner has typically terminated the kernel and it's just performing its final cleanup. The form of this request is `{"shutdown": 1}`. This is what instructs the launcher to abandon listening on the communication socket and to exit.
+Here's an example from the Python (and R) server listener code of
+[handling host-initiated requests](https://github.com/jupyter-server/gateway_provisioners/blob/9de8af8a361aa779f8eb4d10585c0d917bb3731f/gateway_provisioners/kernel-launchers/shared/scripts/server_listener.py#L231-L245).
 
-## Other parameters
+## Other Parameters
 
-Besides `--port-range`, `--public-key`, and `--response-address`, the kernel launcher needs to support `--kernel-id` that indicates the kernel's ID as known to the host server. It should also tolerate the existence of `--spark-context-initialization-mode` but, unless applicable for Spark enviornments, should only support values of `"none"` for this option.
+Besides `--port-range`, `--public-key`, and `--response-address`, the kernel launcher needs to support
+`--kernel-id` that indicates the kernel's ID as known to the host server (mostly for log reconciliation). It
+should also tolerate the existence of `--spark-context-initialization-mode` but, unless applicable for Spark
+environments, should only support values of `"none"` for this option.
```

### Comparing `gateway_provisioners-0.1.0/docs/source/developers/kernel-specification.md` & `gateway_provisioners-0.2.0/docs/source/developers/kernel-specification.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,89 +1,116 @@
-# Implementing a kernel specification
+# Implementing a Kernel Specification
 
-If you find yourself [implementing a kernel launcher](kernel-launcher.md), you'll need a way to make that kernel and kernel launcher available to applications. This is accomplished via the _kernel specification_ or _kernelspec_.
+If you find yourself [implementing a kernel launcher](kernel-launcher.md), you'll need a way to
+make that kernel and kernel launcher available to applications. This is accomplished via the
+_kernel specification_ or _kernelspec_.
+
+Kernelspecs reside in well-known directories. For multi-tenant installations, where users may share kernel
+specifications, we generally recommend they reside in `/usr/local/share/jupyter/kernels` where each entry in this
+directory is a directory representing the name of the kernel. The kernel specification is represented by the
+file `kernel.json`, the contents of which essentially indicate what environment variables should be present in
+the kernel process (via the `env` _stanza_) and which command (and arguments) should be issued to start the kernel
+process (via the `argv` _stanza_). The JSON also includes a `metadata` stanza that contains the kernel provisioner
+configuration, along with which provisioner to instantiate to help manage the kernel process's lifecycle.
+
+One approach the generated Gateway Provisioners kernel specifications take is to include a shell script that actually
+issues the `spark-submit` request. It is this shell script (typically named `run.sh`) that is referenced in the
+`argv` stanza.
 
-Kernelspecs reside in well-known directories. For Enterprise Gateway, we generally recommend they reside in `/usr/local/share/jupyter/kernels` where each entry in this directory is a directory representing the name of the kernel. The kernel specification is represented by the file `kernel.json`, the contents of which essentially indicate what environment variables should be present in the kernel process (via the `env` _stanza_) and which command (and arguments) should be issued to start the kernel process (via the `argv` _stanza_). The JSON also includes a `metadata` stanza that contains the process_proxy configuration, along with which process proxy class to instantiate to help manage the kernel process's lifecycle.
-
-One approach the sample Enterprise Gateway kernel specifications take is to include a shell script that actually issues the `spark-submit` request. It is this shell script (typically named `run.sh`) that is referenced in the `argv` stanza.
-
-Here's an example from the [`spark_python_yarn_cluster`](https://github.com/jupyter-server/enterprise_gateway/blob/main/etc/kernelspecs/spark_python_yarn_cluster/kernel.json) kernel specification:
+Here's an example from a generated kernel specification for Spark running in a Hadoop YARN cluster:
 
 ```JSON
 {
-  "language": "python",
-  "display_name": "Spark - Python (YARN Cluster Mode)",
-  "metadata": {
-    "process_proxy": {
-      "class_name": "enterprise_gateway.services.processproxies.yarn.YarnClusterProcessProxy"
-    },
-    "debugger": true
-  },
-  "env": {
-    "SPARK_HOME": "/usr/hdp/current/spark2-client",
-    "PYSPARK_PYTHON": "/opt/conda/bin/python",
-    "PYTHONPATH": "${HOME}/.local/lib/python3.7/site-packages:/usr/hdp/current/spark2-client/python:/usr/hdp/current/spark2-client/python/lib/py4j-0.10.6-src.zip",
-    "SPARK_OPTS": "--master yarn --deploy-mode cluster --name ${KERNEL_ID:-ERROR__NO__KERNEL_ID} --conf spark.yarn.submit.waitAppCompletion=false --conf spark.yarn.appMasterEnv.PYTHONUSERBASE=/home/${KERNEL_USERNAME}/.local --conf spark.yarn.appMasterEnv.PYTHONPATH=${HOME}/.local/lib/python3.7/site-packages:/usr/hdp/current/spark2-client/python:/usr/hdp/current/spark2-client/python/lib/py4j-0.10.6-src.zip --conf spark.yarn.appMasterEnv.PATH=/opt/conda/bin:$PATH ${KERNEL_EXTRA_SPARK_OPTS}",
-    "LAUNCH_OPTS": ""
-  },
   "argv": [
-    "/usr/local/share/jupyter/kernels/spark_python_yarn_cluster/bin/run.sh",
-    "--RemoteProcessProxy.kernel-id",
+    "/usr/local/share/jupyter/kernels/yarn_spark_python/bin/run.sh",
+    "--kernel-id",
     "{kernel_id}",
-    "--RemoteProcessProxy.response-address",
+    "--port-range",
+    "{port_range}",
+    "--response-address",
     "{response_address}",
-    "--RemoteProcessProxy.public-key",
+    "--public-key",
     "{public_key}",
-    "--RemoteProcessProxy.port-range",
-    "{port_range}",
-    "--RemoteProcessProxy.spark-context-initialization-mode",
-    "lazy"
-  ]
+    "--spark-context-initialization-mode",
+    "lazy",
+    "--kernel-class-name",
+    "ipykernel.ipkernel.IPythonKernel"
+  ],
+  "env": {
+    "SPARK_HOME": "/opt/spark",
+    "PYSPARK_PYTHON": "/opt/miniconda3/envs/provisioners/bin/python",
+    "PYTHONPATH": "${HOME}/.local/lib/python3.7/site-packages:/opt/spark/python",
+    "SPARK_OPTS": "--master yarn --deploy-mode cluster --name ${KERNEL_ID:-ERROR__NO__KERNEL_ID} --conf spark.yarn.submit.waitAppCompletion=false --conf spark.yarn.appMasterEnv.PYTHONUSERBASE=/home/${KERNEL_USERNAME}/.local --conf spark.yarn.appMasterEnv.PYTHONPATH=${HOME}/.local/lib/python3.7/site-packages:/opt/spark/python --conf spark.yarn.appMasterEnv.PATH=/opt/miniconda3/envs/provisioners/bin:$PATH  ${KERNEL_EXTRA_SPARK_OPTS}",
+    "LAUNCH_OPTS": ""
+  },
+  "display_name": "Spark Python (YARN Cluster)",
+  "language": "python",
+  "interrupt_mode": "signal",
+  "metadata": {
+    "kernel_provisioner": {
+      "provisioner_name": "yarn-provisioner",
+      "config": {
+        "launch_timeout": 30
+      }
+    }
+  }
 }
 ```
 
-where [`run.sh`](https://github.com/jupyter-server/enterprise_gateway/blob/main/etc/kernelspecs/spark_python_yarn_cluster/bin/run.sh) issues `spark-submit` specifying the kernel launcher as the "application":
+where [`run.sh`](https://github.com/jupyter-server/gateway_provisioners/blob/main/gateway_provisioners/kernel-specs/yarn_spark_python/bin/run.sh)
+issues `spark-submit` specifying the kernel launcher as the "application":
 
 ```bash
 eval exec \
      "${SPARK_HOME}/bin/spark-submit" \
      "${SPARK_OPTS}" \
      "${IMPERSONATION_OPTS}" \
      "${PROG_HOME}/scripts/launch_ipykernel.py" \
      "${LAUNCH_OPTS}" \
      "$@"
 ```
 
-For container-based environments, the `argv` may instead reference a script that is meant to create the container pod (for Kubernetes). For these, we use a [template file](https://github.com/jupyter-server/enterprise_gateway/blob/main/etc/kernel-launchers/kubernetes/scripts/kernel-pod.yaml.j2) that operators can adjust to meet the needs of their environment. Here's how that `kernel.json` looks:
+For container-based environments, the `argv` may instead reference a script that is meant to create the container pod
+(for Kubernetes). For these, we use a [template file](https://github.com/jupyter-server/gateway_provisioners/blob/main/gateway_provisioners/kernel-launchers/kubernetes/scripts/kernel-pod.yaml.j2)
+that operators can adjust to meet the needs of their environment. Here's how that `kernel.json` looks:
 
 ```json
 {
-  "language": "python",
-  "display_name": "Python on Kubernetes",
-  "metadata": {
-    "process_proxy": {
-      "class_name": "enterprise_gateway.services.processproxies.k8s.KubernetesProcessProxy",
-      "config": {
-        "image_name": "elyra/kernel-py:VERSION"
-      }
-    },
-    "debugger": true
-  },
-  "env": {},
   "argv": [
     "python",
-    "/usr/local/share/jupyter/kernels/python_kubernetes/scripts/launch_kubernetes.py",
-    "--RemoteProcessProxy.kernel-id",
+    "/usr/local/share/jupyter/kernels/k8s_python/scripts/launch_kubernetes.py",
+    "--kernel-id",
     "{kernel_id}",
-    "--RemoteProcessProxy.port-range",
+    "--port-range",
     "{port_range}",
-    "--RemoteProcessProxy.response-address",
+    "--response-address",
     "{response_address}",
-    "--RemoteProcessProxy.public-key",
-    "{public_key}"
-  ]
+    "--public-key",
+    "{public_key}",
+    "--kernel-class-name",
+    "ipykernel.ipkernel.IPythonKernel"
+  ],
+  "env": {},
+  "display_name": "Kubernetes Python",
+  "language": "python",
+  "interrupt_mode": "signal",
+  "metadata": {
+    "debugger": true,
+    "kernel_provisioner": {
+      "provisioner_name": "kubernetes-provisioner",
+      "config": {
+        "image_name": "elyra/kernel-py:dev",
+        "launch_timeout": 30
+      }
+    }
+  }
 }
 ```
 
-When using the `launch_ipykernel` launcher (aka the Python kernel launcher), subclasses of `ipykernel.kernelbase.Kernel` can be launched. By default, this launcher uses the classname `"ipykernel.ipkernel.IPythonKernel"`, but other subclasses of `ipykernel.kernelbase.Kernel` can be specified by adding a `--kernel-class-name` parameter to the `argv` stanza. See [Invoking subclasses of `ipykernel.kernelbase.Kernel`](kernel-launcher.md#invoking-subclasses-of-ipykernelkernelbasekernel) for more information.
+When using the `launch_ipykernel` launcher (aka the Python kernel launcher), subclasses of `ipykernel.kernelbase.Kernel`
+can be launched. By default, this launcher uses the classname `"ipykernel.ipkernel.IPythonKernel"`, but other
+subclasses of `ipykernel.kernelbase.Kernel` can be specified by adding a `--kernel-class-name` parameter to the `argv`
+stanza. See [Invoking subclasses of `ipykernel.kernelbase.Kernel`](kernel-launcher.md#invoking-subclasses-of-ipykernelkernelbasekernel)
+for more information.
 
-As should be evident, kernel specifications are highly tuned to the runtime environment so your needs may be different, but _should_ resemble the approaches we've taken so far.
+As should be evident, kernel specifications are highly tuned to the runtime environment so your needs may be different,
+but _should_ resemble the approaches we've taken so far.
```

### Comparing `gateway_provisioners-0.1.0/docs/source/operators/config-add-env.md` & `gateway_provisioners-0.2.0/docs/source/operators/config-add-env.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # Additional environment variables
 
-Besides those environment variables associated with configurable options, the following environment variables can
+In addition to those environment variables associated with configurable options, the following environment variables can
 also be used to influence functionality:
 
 ```text
   GP_DEFAULT_KERNEL_SERVICE_ACCOUNT_NAME=default
     Kubernetes Provisioners only.  This value indicates the default service account name to use for
     kernel namespaces when the KubernetesProvisioner needs to create the kernel's namespace
     and KERNEL_SERVICE_ACCOUNT_NAME has not been provided.
 
   GP_DOCKER_NETWORK=bridge
     Docker and Docker Swarm Provisioners only. Used by the docker deployment and launch
-    scripts, this indicates the name of the docker network docker network to use.  The
-    docker kernel launcher (launch_docker.py) defaults this value to 'bridge' only in
-    cases where it wasn't previously set by the deployment script.
+    scripts, this indicates the name of the docker network to use.  The docker kernel
+    launcher (launch_docker.py) defaults this value to 'bridge' only in cases where it
+    wasn't previously set by the deployment script.
 
   GP_ENABLE_TUNNELING=False
     Indicates whether tunneling (via ssh) of the kernel and communication ports
     is enabled (True) or not (False).
 
   GP_KERNEL_CLUSTER_ROLE=kernel-controller or cluster-admin
     Kubernetes Provisioners only.  The role to use when binding with the kernel service
```

### Comparing `gateway_provisioners-0.1.0/docs/source/operators/config-env-debug.md` & `gateway_provisioners-0.2.0/docs/source/operators/config-env-debug.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 ```text
   GP_DOCKER_LOG_LEVEL=WARNING
     By default, the docker client library is too verbose for its logging.  This
     value can be adjusted in situations where docker troubleshooting may be warranted.
 
   GP_KUBERNETES_LOG_LEVEL=WARNING
-    By default, the kubernetes client library is too verbose for its logging.  This
+    By default, the Kubernetes client library is too verbose for its logging.  This
     value can be adjusted in situations where kubernetes troubleshooting may be
     warranted.
 
   GP_LOG_LEVEL=10
     Used by remote launchers and server listeners (where the kernel runs), this
     indicates the level of logging used by those entities.  Level 10 (DEBUG) is
     recommended since they don't do verbose logging.
```

### Comparing `gateway_provisioners-0.1.0/docs/source/operators/config-kernel-override.md` & `gateway_provisioners-0.2.0/docs/source/operators/config-kernel-override.md`

 * *Files 5% similar despite different names*

```diff
@@ -9,42 +9,49 @@
 
 The following enumerates the set of per-kernel configuration overrides:
 
 ```{note}
 Unless noted otherwise, these values only apply to provisioners derived from `RemoteProvisioner`.
 ```
 
-- `remote_hosts`: This provisioner configuration entry can be used to override
-  `c.RemoteProvisionerConfigMixin.remote_hosts`. Any values specified in the config dictionary
-  override the globally defined values. This applies to all `DistributedProvisioner` kernels.
-- `yarn_endpoint`: This provisioner configuration entry can be used to override
-  `c.RemoteProvisionerConfigMixin.yarn_endpoint`.
-  Any values specified in the config dictionary override the globally defined values. These
-  apply to all `YarnProvisioner` kernels. Note that you'll likely be required to specify a
-  different `HADOOP_CONF_DIR` setting in the kernel.json's `env` stanza in order of the
-  `spark-submit` command to target the appropriate YARN cluster. This applies to all
-  `YarnProvisioner` kernels.
+### `RemoteProvisioner` per-kernel overrides
+
 - `authorized_users`: This provisioner configuration entry can be used to override
   `c.RemoteProvisionerConfigMixin.authorized_users`. Any values specified in the config
   dictionary override the globally defined values. Note that the typical use-case for
   this value is to not set `c.RemoteProvisionerConfigMixin.authorized_users` at the global level,
   but then restrict access at the kernel level.
 - `unauthorized_users`: This provisioner configuration entry can be used to **_amend_**
   `c.RemoteProvisionerConfigMixin.unauthorized_users`. Any values specified in the config dictionary
   are **added** to the globally defined values. As a result, once a user is denied access at the
   global level, they will _always be denied access at the kernel level_.
 - `port_range`: This remote provisioner configuration entry can be used to override
   `c.RemoteProvisionerConfigMixin.port_range`. Any values specified in the config
   dictionary override the globally defined values.
 
+### `DistributedProvisioner` per-kernel overrides
+
+- `remote_hosts`: This provisioner configuration entry can be used to override
+  `c.DistributedProvisioner.remote_hosts`. Any values specified in the config dictionary
+  override the globally defined values.
+
+### `YarnProvisioner` per-kernel overrides
+
+- `yarn_endpoint`: This provisioner configuration entry can be used to override
+  `c.RemoteProvisionerConfigMixin.yarn_endpoint`.
+  Any values specified in the config dictionary override the globally defined values. These
+  apply to all `YarnProvisioner` kernels. Note that you'll likely be required to specify a
+  different `HADOOP_CONF_DIR` setting in the kernel.json's `env` stanza in order for the
+  `spark-submit` command to target the appropriate YARN cluster.
+
 ## Per-kernel environment overrides
 
 In some cases, it is useful to allow specific values that exist in a kernel.json `env` stanza to be
 overridden on a per-kernel basis. For example, if the kernel.json supports resource limitations you
-may want to allow some requests to have access to more memory or GPUs than another. Remote Provisioners
+may want to allow some requests to have access to more memory or GPUs than another. Gateway Provisioners
 enables this capability by honoring environment variables provided in the json request over
 those same-named variables in the kernel.json `env` stanza.
 
 Environment variables for which this can occur are any variables prefixed with `KERNEL_`.
 
-See [Kernel Environment Variables](../users/kernel-envs.md) in the Users documentation
-section for a complete set of recognized `KERNEL_` variables.
+See [Kernel Environment Variables](../users/kernel-envs.md) in the Users Guide
+for a complete set of recognized `KERNEL_` variables.
```

### Comparing `gateway_provisioners-0.1.0/docs/source/operators/config-security.md` & `gateway_provisioners-0.2.0/docs/source/operators/config-security.md`

 * *Files 2% similar despite different names*

```diff
@@ -48,23 +48,23 @@
 It should be noted that the corresponding messages logged when each of the above authorization
 failures occur are slightly different. This allows the administrator to discern from which
 authorization list the failure was generated.
 
 Failures stemming from _inclusion_ in the `unauthorized_users` list will include text similar to
 the following:
 
-```
+```text
 User 'bob' is not authorized to start kernel 'Spark - Python (YARN Mode)'. Ensure
 KERNEL_USERNAME is set to an appropriate value and retry the request.
 ```
 
 Failures stemming from _exclusion_ from a non-empty `authorized_users` list will include text
 similar to the following:
 
-```
+```text
 User 'bob' is not in the set of users authorized to start kernel 'Spark - Python (YARN Mode)'. Ensure
 KERNEL_USERNAME is set to an appropriate value and retry the request.
 ```
 
 ## User Impersonation
 
 Servers using `GatewayProvisioners` can leverage other technologies to implement user impersonation
@@ -84,29 +84,29 @@
 kerberos, and thus require this security option as a pre-requisite for user impersonation. When user
 impersonation is enabled, kernels are launched with the `--proxy-user ${KERNEL_USERNAME}` which will
 tell YARN to launch the kernel in a container used by the provided username.
 
 ```{admonition} Important!
 :class: warning
 When using kerberos in a YARN managed cluster, the server's user needs to be set up as a
-`proxyuser` superuser in hadoop configuration. Please refer to the
+`proxyuser` superuser in Hadoop configuration. Please refer to the
 [Hadoop documentation](https://hadoop.apache.org/docs/current/hadoop-project-dist/hadoop-common/Superusers.html)
 regarding the proper configuration steps.
 ```
 
 ### SPNEGO Authentication to YARN APIs
 
 When kerberos is enabled in a YARN managed cluster, the administration UIs can be configured to
-require authentication/authorization via SPENEGO. When running kernels in an environment configured
+require authentication/authorization via SPNEGO. When running kernels in an environment configured
 this way, we need to convey an extra configuration to enable the proper authorization when
 communicating with YARN via the YARN APIs.
 
 `GP_YARN_ENDPOINT_SECURITY_ENABLED` indicates the requirement to use SPNEGO authentication/authorization
 when connecting with the YARN APIs and can also be conveyed via the boolean configuration option
-`c.RemoteProvisionerConfigMixin.yarn_endpoint_security_enabled` (default = False)
+`c.YarnProvisioner.yarn_endpoint_security_enabled` (default = False)
 
 ### Impersonation in Standalone or YARN Client Mode
 
 Impersonation performed in standalone or YARN client modes (via the `DistributedProvisioner`) tends
 to take the form of using `sudo` to perform the kernel launch as the target user. This can also be
 configured within the [run.sh](https://github.com/jupyter-server/enterprise_gateway/blob/main/etc/kernelspecs/spark_python_yarn_client/bin/run.sh)
 script and requires the following:
@@ -133,23 +133,23 @@
 Gateway Provisioners can be configured to perform SSH tunneling on the five ZeroMQ kernel sockets
 as well as the communication socket created within the launcher and used to perform remote and
 cross-user signalling functionality. SSH tunneling is NOT enabled by default. Tunneling can be
 enabled/disabled via the environment variable `GP_ENABLE_TUNNELING=False`. Note, there is no
 configuration file support for this variable.
 
 Note that SSH by default validates host keys before connecting to remote hosts and the connection
-will fail for invalid or unknown hosts. Remote Provisioners honors this requirement, and invalid
+will fail for invalid or unknown hosts. Gateway Provisioners honors this requirement, and invalid
 or unknown hosts will cause tunneling to fail. Please perform necessary steps to validate all
 hosts before enabling SSH tunneling, such as:
 
 - SSH to each node cluster and accept the host key properly
 - Configure SSH to disable `StrictHostKeyChecking`
 
 ## Using Generic Security Service (Kerberos)
 
 Gateway Provisioners has support for SSH connections using GSS (for example Kerberos), which
-enables its deployment without the use of an ssh key. The `RP_REMOTE_GSS_SSH` environment
+enables its deployment without the use of an ssh key. The `GP_REMOTE_GSS_SSH` environment
 variable can be used to control this behavior.
 
 ```{seealso}
 The list of [additional supported environment variables](config-add-env.md#additional-environment-variables).
 ```
```

### Comparing `gateway_provisioners-0.1.0/docs/source/operators/config-sys-env.md` & `gateway_provisioners-0.2.0/docs/source/operators/config-sys-env.md`

 * *Files identical despite different names*

### Comparing `gateway_provisioners-0.1.0/docs/source/operators/deploy-kubernetes.md` & `gateway_provisioners-0.2.0/docs/source/operators/deploy-kubernetes.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,311 +1,279 @@
 # Kubernetes deployments
 
-## Overview
+Because Gateway Provisioners is a _library package_ and not an _application_, deployment into Kubernetes
+configurations consists of ensuring that the _host application image_ has the appropriate kernel specifications in place
+and that necessary configuration items (typically environment variables in containerized deployments) are
+present in the host application.
 
-This section describes how to deploy Gateway Provisioners into an existing Kubernetes cluster.
-
-It is important that the hosting application (e.g., Jupyter Server or Kernel Gateway)
-is provisioned as a Kubernetes _deployment_ and exposed as a Kubernetes _service_.
-
-FIXME -
-(Load balancing only in EG at the moment)
-Enterprise Gateway can leverage load balancing and high availability functionality provided by
-Kubernetes (although HA cannot be fully realized until Enterprise Gateway supports persistent sessions).
-
-The following sample kernel specifications apply to Kubernetes deployments:
-
-- R_kubernetes
-- python_kubernetes
-- python_tf_gpu_kubernetes
-- python_tf_kubernetes
-- scala_kubernetes
-- spark_R_kubernetes
-- spark_python_kubernetes
-- spark_scala_kubernetes
-- spark_python_operator
-
-Enterprise Gateway deployments use the [elyra/enterprise-gateway](https://hub.docker.com/r/elyra/enterprise-gateway/)
-image from the Enterprise Gateway dockerhub organization [elyra](https://hub.docker.com/r/elyra/) along with other
-kubernetes-based images. See [Docker Images](../contributors/docker.md) for image details.
-
-When deployed within a [spark-on-kubernetes](https://spark.apache.org/docs/latest/running-on-kubernetes.html) cluster,
-Enterprise Gateway can easily support cluster-managed kernels distributed across the cluster. Enterprise Gateway
-will also provide standalone (i.e., _vanilla_) kernel invocation (where spark contexts are not automatically created)
-which also benefits from their distribution across the cluster.
-
-```{note}
-If you plan to use kernel specifications derived from the `spark_python_operator` sample, ensure that the
-[Kubernetes Operator for Apache Spark is installed](https://github.com/GoogleCloudPlatform/spark-on-k8s-operator#installation)
-in your Kubernetes cluster.
+```{tip}
+The following provides information for the kinds of tasks that should be considered when deploying applications
+that use Gateway Provisioners on Kubernetes.  See our [_Application Support_ page](https://github.com/jupyter-server/gateway_provisioners/tree/main/gateway_provisioners/app-support/README.md)
+for examples of how to configure and deploy such applications.
 ```
 
-We are using helm templates to manage Kubernetes resource configurations, which allows an end-user to easily
-customize their Enterprise Gateway deployment.
+## Generating Kernel Specifications
 
-There are two main deployment scenarios if RBAC is enabled in your Kubernetes cluster:
+Kernelspec generation for Kubernetes deployments is performed using the `jupyter-k8s-spec` command.  Because
+the host application will also reside within a docker image, the commands are usually placed into a Dockerfile
+that _extends_ an existing image.  However, some may choose to `docker exec` into a running container, perform and test
+the necessary configuration, then use `docker commit` to generate a new image.  That said, the following will assume a
+Dockerfile approach.
 
-1. Deployment user has **_Cluster Administrator Access_**. In this scenario, you have full access to the cluster and can deploy all components as needed.
-1. Deployment user has **_Namespace Administrator Access_**. This is typical for shared multi-tenant environments where each Team has control over their namespace, but not the cluster. In this scenario, your cluster Administrator can deploy the RBAC resources and Kernel Image Puller and you can deploy Enterprise Gateway.
+To generate a default kernel specification (where Python is the default kernel) enter:
 
-## Prerequisites
-
-- Install and configure [kubectl](https://kubernetes.io/docs/tasks/tools/) and [helm3](https://helm.sh/docs/intro/install/) on your workstation.
-- Create the kubernetes namespace where you want to deploy Enterprise Gateway, for example:
-  ```sh
-  kubectl create namespace enterprise-gateway
-  ```
-- If you use RBAC, you will need cluster Admin access to configure RBAC resources
-- If you plan to use Private docker registry, you will need to have credentials (see configuration steps below)
+```dockerfile
+RUN jupyter k8s-spec install
+```
 
-Once the Kubernetes cluster is configured and `kubectl` is demonstrated to be working, it is time to deploy Enterprise Gateway. There are a couple of different deployment options - using helm or kubectl.
+which produces the following output...
 
-## Gateway Provisioners Deployment Details
+```text
+[I 2023-02-16 10:39:37.538 K8sSpecInstaller] Installing kernel specification for 'Kubernetes Python'
+[I 2023-02-16 10:39:37.948 K8sSpecInstaller] Installed kernelspec k8s_python in /usr/local/share/jupyter/kernels/k8s_python
+```
 
-Enterprise Gateway is deployed as a Kubernetes deployment and exposed by a Kubernetes service. It can be accessed by the service name `enterprise-gateway` within the cluster. In addition, all objects related to Enterprise Gateway, including kernel instances, have the kubernetes label of `app=enterprise-gateway` applied.
+and the following set of files and directories:
 
-The Enterprise Gateway Kubernetes service _type_ can be:
+```text
+/usr/local/share/jupyter/kernels/k8s_python
+kernel.json logo-64x64.png
 
-- `NodePort`: allows to access Enterprise Gateway with `http://[worker IP]:[NodePort]` or having a load balancer route traffic to `http://[worker IP's]:[NodePort]`
-- `LoadBalancer`: requires appropriate network plugin available
-- `ClusterIP`: requires Kubernetes Ingress Controller
+/usr/local/share/jupyter/kernels/k8s_python/scripts:
+launch_kubernetes.py
+kernel-pod.yaml.j2
+```
 
-Kernels are stateful, therefore service is configured with a `sessionAffinity` of `ClientIP`. As a result, kernel creation requests will be routed to the same pod.
+where each provides the following function:
 
-Increase the number of `replicas` of Enterprise Gateway Deployment to improve deployment availability, but because `sessionAffinity` of `ClientIP`, traffic from the same client will be sent to the same pod of the Enterprise Gateway and if that pod goes down, client will get an error and will need to reestablish connection to another pod of the Enterprise Gateway.
+- `kernel.json` - the primary file that the host application uses to discover a given kernel's availability.
+  This file contains _stanzas_ that describe the kernel's argument vector (`argv`), its runtime environment (`env`),
+  its display name (`display_name`) and language (`language`), as
+  well as its kernel provisioner's configuration (`metadata.kernel_provisioner`) - which, in this case, will reflect the
+  `KubernetesProvisioner`.
+- `logo-64x64.png` - the icon resource corresponding to this kernel specification.  Icon resource files must be start
+  with the `logo-` prefix to be included in the kernel specification.
+- `scripts/launch_kubernetes.py` - the "launcher" for the kernel pod.  This script processes its sibling Jinja
+  templates by applying appropriate substitutes and creating each of the Kubernetes resources as described in the template.
+- `scripts/kernel-pod.yaml.j2` - the Jinja template describing the to-be-launched kernel pod corresponding to the
+  kernel image identified by the `metadata.kernel_provisioner.config.image_name` entry.  This file can be modified to
+  include instructions for volume mounts, etc., for establishing the pod's configuration.
+- `bin/run.sh` - This file will be present only when `--spark` is specified.  The first entry in the `kernel.json`'s
+  `argv` stanza will be a reference to `bin/run.sh`. This script sets up and invokes the `spark-submit` command that
+  is responsible for interacting with the Spark-on-Kubernetes resource manager.  With the introduction of Spark Pod
+  Templates, we can leverage the same templating behavior in Spark-based environments.  As a result, both the driver
+  and executor pods will have similar configurations.
 
-### Namespaces
+```{seealso}
+See [Command-line Options](#command-line-options) below for how to adjust the `image-name`, `display-name`, and
+others.
+```
 
-A best practice for Kubernetes applications running in an enterprise is to isolate applications via namespaces. Since Enterprise Gateway also requires isolation at the kernel level, it makes sense to use a namespace for each kernel, by default.
+### Deploying Custom Resource Definitions
 
-The primary namespace is created prior to the initial Helm deployment (e.g., `enterprise-gateway`). This value is communicated to Enterprise Gateway via the env variable `EG_NAMESPACE`. All Enterprise Gateway components reside in this namespace.
+Gateway Provisioners currently supports one form of Custom Resource Definitions (CRDs) via the
+[`SparkOperatorProvisioner`](../contributors/system-architecture.md#sparkoperatorprovisioner).  To generate a kernel
+specification to use `SparkOperatorProvisioner`, in addition to including the `--spark` option, you will also include the
+`--crd` option to `jupyter k8s-spec install`.
 
-By default, kernel namespaces are created when the respective kernel is launched. At that time, the kernel namespace name is computed from the kernel username (`KERNEL_USERNAME`) and its kernel ID (`KERNEL_ID`) just like the kernel pod name. Upon a kernel's termination, this namespace - provided it was created by Enterprise Gateway - will be deleted.
+```dockerfile
+RUN jupyter k8s-spec install --crd --spark
+```
 
-Installations wishing to pre-create the kernel namespace can do so by conveying the name of the kernel namespace via `KERNEL_NAMESPACE` in the `env` portion of the kernel creation request. (They must also provide the namespace's service account name via `KERNEL_SERVICE_ACCOUNT_NAME` - see next section.) When `KERNEL_NAMESPACE` is set, Enterprise Gateway will not attempt to create a kernel-specific namespace, nor will it attempt its deletion. As a result, kernel namespace lifecycle management is the user's responsibility.
+which produces the following output...
 
-```{tip}
-If you need to associate resources to users, one suggestion is to create a namespace per user and set `KERNEL_NAMESPACE = KERNEL_USERNAME` on the client (see [Kernel Environment Variables](../users/kernel-envs.md)).
+```text
+[I 2023-04-19 10:18:09.963 K8sSpecInstaller] Installing kernel specification for 'Kubernetes Spark Operator'
+[I 2023-04-19 10:18:10.360 K8sSpecInstaller] Installed kernelspec k8s_python_spark_operator in /usr/local/share/jupyter/kernels/k8s_python_spark_operator
 ```
 
-Although **not recommended**, installations requiring everything in the same namespace - Enterprise Gateway and all its kernels - can do so by setting the helm chart value `kernel.shareGatewayNamespace` to `true` - which is then set into the `EG_SHARED_NAMESPACE` env. When set, all kernels will run in the Enterprise Gateway namespace, essentially eliminating all aspects of isolation between kernel instances (and resources).
+and the following set of files and directories:
 
-### Role-Based Access Control (RBAC)
+```text
+/usr/local/share/jupyter/kernels/k8s_python_spark_operator
+kernel.json logo-64x64.png
 
-Another best practice of Kubernetes applications is to define the minimally viable set of permissions for the application. Enterprise Gateway does this by defining role-based access control (RBAC) objects for both Enterprise Gateway and kernels.
-
-Because the Enterprise Gateway pod must create kernel namespaces, pods, services (for Spark support) and role bindings, a cluster-scoped role binding is required.
+/usr/local/share/jupyter/kernels/k8s_python_spark_operator/scripts:
+launch_custom_resource.py
+sparkoperator.k8s.io-v1beta2.yaml.j2
+```
 
-The cluster role binding `enterprise-gateway-controller` also references the subject, `enterprise-gateway-sa`, which is the service account associated with the Enterprise Gateway namespace and also created by [eg-clusterrolebinding.yaml](https://github.com/jupyter-server/enterprise_gateway/blob/main/etc/kubernetes/helm/enterprise-gateway/templates/eg-clusterrolebinding.yaml)).
+There are a few things worth noting here.
 
-The [`eg-clusterrole.yaml`](https://github.com/jupyter-server/enterprise_gateway/blob/main/etc/kubernetes/helm/enterprise-gateway/templates/eg-clusterrole.yaml) defines the minimally viable roles for a kernel pod - most of which are required for Spark support.
+1. The `scripts` directory contains a different set of scripts.  This is because the SparkOperator requires a
+   slightly different launch script and its yaml definitions are different enough to warrant separation.
+1. Although this provisioner uses Spark, there is no `run` sub-directory created that contains a `spark-submit`
+   command.  Instead, the appropriate CRD is created which performs the application's submission to Spark directly.
+1. The yaml template name is a composition of the provisioner's [`group` and `version` attributes](../contributors/system-architecture.md/#sparkoperatorprovisioner).
+   In this case, the `group` is `sparkoperator.k8s.io` and `version` is `v1beta2`.
 
-Since kernels, by default, reside within their own namespace created upon their launch, a cluster role is used within a namespace-scoped role binding created when the kernel's namespace is created. The name of the kernel cluster role is `kernel-controller` and, when Enterprise Gateway creates the namespace and role binding, is also the name of the role binding instance.
+````{note}
+If you plan to use kernel specifications leveraging `SparkOperatorProvisioner`, ensure that the
+[Kubernetes Operator for Apache Spark is installed](https://github.com/GoogleCloudPlatform/spark-on-k8s-operator#installation)
+in your Kubernetes cluster.
 
-#### Kernel Service Account Name
+```{tip}
+To ensure the proper flow of environment variables to your spark operator, make sure the
+webhook server is enabled when deploying the helm chart:
 
-As noted above, installations wishing to pre-create their own kernel namespaces should provide the name of the service account associated with the namespace via `KERNEL_SERVICE_ACCOUNT_NAME` in the `env` portion of the kernel creation request (along with `KERNEL_NAMESPACE`). If not provided, the built-in namespace service account, `default`, will be referenced. In such circumstances, Enterprise Gateway will **not** create a role binding on the name for the service account, so it is the user's responsibility to ensure that the service account has the capability to perform equivalent operations as defined by the `kernel-controller` role.
+`helm install my-release spark-operator/spark-operator --namespace spark-operator --set webhook.enable=true`
+````
 
-#### Example Custom Namespace
+### Generating Multiple Specifications
 
-Here's an example of the creation of a custom namespace (`kernel-ns`) with its own service account (`kernel-sa`) and role binding (`kernel-controller`) that references the cluster-scoped role (`kernel-controller`) and includes appropriate labels to help with administration and analysis:
+Its common practice to support multiple languages or use different images for kernels of the same language.  For each
+of those differences, a separate installation command should be provided:
 
-```yaml
-apiVersion: v1
-kind: Namespace
-metadata:
-  name: kernel-ns
-  labels:
-    app: enterprise-gateway
-    component: kernel
----
-apiVersion: v1
-kind: ServiceAccount
-metadata:
-  name: kernel-sa
-  namespace: kernel-ns
-  labels:
-    app: enterprise-gateway
-    component: kernel
----
-apiVersion: rbac.authorization.k8s.io/v1
-kind: RoleBinding
-metadata:
-  name: kernel-controller
-  namespace: kernel-ns
-  labels:
-    app: enterprise-gateway
-    component: kernel
-subjects:
-  - kind: ServiceAccount
-    name: kernel-sa
-    namespace: kernel-ns
-roleRef:
-  kind: ClusterRole
-  name: kernel-controller
-  apiGroup: rbac.authorization.k8s.io
+```dockerfile
+RUN jupyter k8s-spec install --image-name my-numpy-image:dev --kernel-name my_numpy_kernel_py --display-name "My Numpy"
+RUN jupyter k8s-spec install --image-name my-tensor-image:dev --kernel-name my_tensor_kernel_py --display-name "My Tensorflow"
+RUN jupyter k8s-spec install --image-name my-R-image:dev --language R --display-name "My R Kernel"
 ```
 
-### Kernel Image Puller
+### Kubernetes Kernel Instances
 
-Kernels docker images can be big and their download from a container repository (e.g., docker.io or quay.io), which may cause slow kernel pod startup whenever the kernel image is first accessed on any given node.
+Gateway Provisioners currently supports the launching of regular (_vanilla_) and spark-based kernels within a Kubernetes cluster.
+When kernels are launched, Gateway Provisioners is responsible for creating the appropriate entities. The kind of
+entity created is a function of whether the kernel is a regular or spark-based kernel specification.
 
-To mitigate this issue, Enterprise Gateway deployment includes `kernel-image-puller` or `KIP` Kubernetes DaemonSet. This DaemonSet is responsible for polling Enterprise Gateway for the current set of configured kernelspecs, picking out any configured image name references, and pulling those images to the node on which KIP is running. Because it's a daemon set, this will also address the case when new nodes are added to a configuration (although spinning up new nodes on a kernel start request will likely time out anyway).
+Regular kernels are launched as a kernel pod based on the `scripts/kernel-pod.yaml.j2` template via the
+`scripts/launch_kubernetes.py` script, both of which are located in the `scripts` directory.  Spark-based kernels are
+launched via `spark-submit` in the `bin/run.sh` script triggering the creation of a _driver_ pod and one or more
+_executor_ pods.
 
-#### KIP Configuration
+Items worth noting:
 
-`KIP` is using same kubernetes Service Account as Enterprise Gateway itself, so it will use same credentials to access private docker registry - see helm configuration section for details.
+1. The launched pods' names will be composed of the launching username (`KERNEL_USERNAME`) and kernel-id. Some additional
+   information is added to the spark-based pod names.
+1. The pods will have 3 labels applied: `"kernel_id=<kernel-id>"`, `"component=kernel"`, and
+   `"app=gateway-provisioners"` - similar to Docker.  The `component` label on the spark-based executor pods will hold a
+   value of `worker` to distinguish them from the driver.
+1. The pods will be launched within the same Kubernetes network as the host application.
 
-`KIP_INTERVAL` - The Kernel Image Puller can be configured for the interval at which it checks for new kernelspecs
+## Namespaces
 
-`KIP_NUM_PULLERS`- the number of puller threads it will utilize per node ()
+A best practice for Kubernetes applications running in an enterprise is to isolate applications via namespaces. There are
+three ways namespaces can be used with respect to Gateway Provisioners: Shared Namespace, Bring-Your-Own Namespace,
+and Automatic Namespace.
 
-`KIP_NUM_RETRIES` - the number of retries it will attempt for a given image (),
+### Shared Namespace
 
-`KIP_PULL_POLICY` - and the pull policy () - which essentially dictates whether it will attempt to pull images that its already encountered (`Always`) vs. only pulling the image if it hasn't seen it yet (`IfNotPresent`).
+Because Gateway Provisioners is a _library package_ and not its own application, the default namespace behavior is to
+use a _shared namespace_.  That is, kernel pods launched by the application are placed into the same namespace as the
+hosting application.  This option is controlled by two environment variables: `GP_SHARED_NAMESPACE` and `GP_NAMESPACE`.
 
-If the Enterprise Gateway defines an authentication token (`EG_AUTH_TOKEN`) then that same token should be configured here as (`KIP_AUTH_TOKEN`) so that the puller can correctly authenticate its requests.
+#### `GP_SHARED_NAMESPACE`
 
-#### KIP Container Runtime
+This environment variable defaults to `True`.  When enabled, all kernel pods will be launched into the namespace
+identified by `GP_NAMESPACE`.  No attempt is made to alter the configuration of `GP_NAMESPACE`.
 
-The Kernel Image Puller also supports multiple container runtimes since Docker is no longer configured by default in Kubernetes. KIP currently supports Docker and Containerd runtimes. If another runtime is encountered, KIP will try to proceed using the Containerd client `crictl` against the configured socket. As a result, it is import that the `criSocket` value be appropriately configured relative to the container runtime. If the runtime is something other than Docker or Containerd and `crictl` isn't able to pull images, it may be necessary to manually pre-seed images or incur kernel start timeouts the first time a given node is asked to start a kernel associated with a non-resident image.
+#### `GP_NAMESPACE`
 
-KIP also supports the notion of a _default container registry_ whereby image names that do not specify a registry (e.g., `docker.io` or `quay.io`) KIP will apply the configured default. Ideally, the image name should be fully qualified.
+This environment variable identifies the namespace in which the host application is running.  It defaults to the
+namespace named `default`, but its recommended that host application deployment configure its own namespace and this
+environment variable be set to that value.
 
-### Kernelspec Modifications
+### Bring-Your-Own Namespace
 
-One of the more common areas of customization we see occurs within the kernelspec files located in `/usr/local/share/jupyter/kernels`. To accommodate the ability to customize the kernel definitions, you have two different options: NFS mounts, or custom container images. The two options are mutually exclusive, because they mount kernelspecs into the same location in the Enterprise Gateway pod.
+Users can specify their own namespace be used by setting `GP_SHARED_NAMESPACE` = `False` and specifying the
+`KERNEL_NAMESPACE` environment variable in the `env` stanza of the kernel's start request (e.g., `POST /api/kernels`).
+This namespace model is preferred in multi-tenant configurations, particularly when a Gateway server is the host
+application or, for example, in JupyterHub situations where Hub launches notebook servers into user-oriented namespaces.
+(In this case, setting `GP_NAMESPACE` to the user-oriented namespace on each JupyterLab launch and using _Shared Namespace
+modeling_, would have the same effect as setting `KERNEL_NAMESPACE` using the _Bring-Your-Own Namespace modeling_.)
 
-#### Via NFS
+When configured, Gateway Provisioners assumes the namespace identified by `KERNEL_NAMESPACE` already exists and is
+properly configured from a resources and privileges standpoint.  In addition to providing `KERNEL_NAMESPACE`, users
+must also provide the name of the service account privileged to create resources within the namespace.  The service
+account name is conveyed via `KERNEL_SERVICE_ACCOUNT_NAME`.
 
-The kernels directory can be mounted as an NFS volume into the Enterprise Gateway pod, thereby making the kernelspecs available to all EG pods within the Kubernetes cluster (provided the NFS mounts exist on all applicable nodes).
+Gateway Provisioners will not attempt to delete this namespace upon the kernel's termination.
 
-As an example, we have included the necessary entries for mounting an existing NFS mount point into the Enterprise Gateway pod. By default, these references are commented out as they require the operator to configure the appropriate NFS mounts and server IP. If you are deploying Enterprise Gateway via the helm chart, you can enable NFS directly via helm values.
+### Automatic Namespace
 
-Here you can see how `deployment.yaml` references use of the volume (ia `volumeMounts`
-for the container specification and `volumes` in the pod specification (non-applicable entries have been omitted):
+Operators wanting the finest isolation level, where each kernel pod is launched into their own namespace, can do so by
+disabling `GP_SHARED_NAMESPACE` and not setting `KERNEL_NAMESPACE`.  In these configurations, Gateway Provisioners will
+_create_ a namespace corresponding to the values of `KERNEL_USERNAME`-`KERNEL_ID`, just as the pods are named.
 
-```yaml
-spec:
-  containers:
-    # Uncomment to enable NFS-mounted kernelspecs
-    volumeMounts:
-      - name: kernelspecs
-        mountPath: "/usr/local/share/jupyter/kernels"
-  volumes:
-    - name: kernelspecs
-      nfs:
-        server: <internal-ip-of-nfs-server>
-        path: "/usr/local/share/jupyter/kernels"
-```
-
-```{tip}
-Because the kernel pod definition file, [kernel-pod.yaml](https://github.com/jupyter-server/enterprise_gateway/blob/main/etc/kernel-launchers/kubernetes/scripts/kernel-pod.yaml.j2), resides in the kernelspecs hierarchy, customizations to the deployments of future kernel instances can now also take place.  In addition, these same entries can be added to the kernel-pod.yaml definitions if access to the same or other NFS mount points are desired within kernel pods. (We'll be looking at ways to make modifications to per-kernel configurations more manageable.)
-```
+This option requires higher-level privileges on the RBAC settings of the host application as the namespace must be
+created on startup and deleted on termination.
 
-Use of more formal persistent volume types must include the [Persistent Volume](https://kubernetes.io/docs/concepts/storage/persistent-volumes) and corresponding Persistent Volume Claim stanzas.
+#### Required RBAC Settings
 
-#### Via Custom Container Image
+As noted above, the ability to create and destroy namespaces at the time of kernel launch requires additional privileges
+in the form of a `cluster-role`.  This role will require privileges to create and delete namespaces, services, and
+role-bindings, among other things.  Because a new namespace will be created, a subsequent cluster-role should exist
+that is for use by the kernel pod itself.  These two role definitions are provided below:
 
-If you are deploying Enterprise Gateway via the helm chart, then instead of using NFS, you can build your custom kernelspecs into a container image that Enterprise Gateway consumes. Here's an example Dockerfile for such a container:
+##### Application Cluster Role
 
-```
-FROM alpine:3.9
+This role is the responsibility of the host application deployment. The application name is specified here as
+`gateway-provisioners` with a suggested name of `gateway-provisioners-controller`.
 
-COPY kernels /kernels
+```yaml+jinja
+apiVersion: rbac.authorization.k8s.io/v1
+kind: ClusterRole
+metadata:
+  name: gateway-provisioners-controller
+  labels:
+    app: gateway-provisioners
+    component: gateway-provisioners
+rules:
+  - apiGroups: [""]
+    resources: ["pods", "namespaces", "services", "configmaps", "secrets", "persistentvolumes", "persistentvolumeclaims"]
+    verbs: ["get", "watch", "list", "create", "delete"]
+  - apiGroups: ["rbac.authorization.k8s.io"]
+    resources: ["rolebindings"]
+    verbs: ["get", "list", "create", "delete"]
+  - apiGroups: ["sparkoperator.k8s.io"]
+    resources: ["sparkapplications", "sparkapplications/status", "scheduledsparkapplications", "scheduledsparkapplications/status"]
+    verbs: ["get", "watch", "list", "create", "delete"]
 ```
 
-This assumes that your source contains a `kernels/` directory with all the kernelspecs you'd like to end up in the image, e.g. `kernels/python_kubernetes/kernel.json` and any associated files.
-
-Once you build your custom kernelspecs image and push it to a container registry, you can refer to it from your helm deployment. For instance:
-
-```bash
-helm upgrade --install --atomic --namespace enterprise-gateway enterprise-gateway etc/kubernetes/helm --set kernelspecs.image=your-custom-image:latest
+```{note}
+The reference to `apiGroups: ["sparkoperator.k8s.io"]` is forward-reaching as Gateway Provisioners doesn't currently
+support Spark Operators - but plans to in the near future.
 ```
 
-...where `your-custom-image:latest` is the image name and tag of your kernelspecs image. Once deployed, the helm chart copies the data from the `/kernels` directory of your container into the `/usr/local/share/jupyter/kernels` directory of the Enterprise Gateway pod. Note that when this happens, the built-in kernelspecs are no longer available. So include all kernelspecs that you want to be available in your container image.
-
-Also, you should update the helm chart `kernel.whitelist` value with the name(s) of your custom kernelspecs.
-
-## Kubernetes Kernel Instances
+##### Kernel Cluster Role
 
-There are essentially two kinds of kernels (independent of language) launched within an Enterprise Gateway Kubernetes cluster - _vanilla_ and _spark-on-kubernetes_ (if available).
+The name of this role is conveyed from the host application to Gateway Provisioners via
+the `GP_KERNEL_CLUSTER_ROLE` environment variable and defaults to `cluster-admin`, so operators are advised to create
+a specific role for these purposes.  This role is responsible for managing resources within the newly-created namespace.\
+While the role is a `cluster-role`, it is only _bound_ via a `role-binding` binding the cluster role to the namespace
+and its service account referenced by `KERNEL_SERVICE_ACCOUNT_NAME`.
 
-When _vanilla_ kernels are launched, Enterprise Gateway is responsible for creating the corresponding pod. On the other hand, _spark-on-kubernetes_ kernels are launched via `spark-submit` with a specific `master` URI - which then creates the corresponding pod(s) (including executor pods). Images can be launched using both forms provided they have the appropriate support for Spark installed.
-
-Here's the yaml configuration used when _vanilla_ kernels are launched. As noted in the `KubernetesProcessProxy` section below, this file ([kernel-pod.yaml.j2](https://github.com/jupyter-server/enterprise_gateway/blob/main/etc/kernel-launchers/kubernetes/scripts/kernel-pod.yaml.j2)) serves as a template where each of the tags surrounded with `{{` and `}}` represent variables that are substituted at the time of the kernel's launch. All `{{ kernel_xxx }}` parameters correspond to `KERNEL_XXX` environment variables that can be specified from the client in the kernel creation request's json body.
+Here is the general yaml describing this configuration and suggests a name of `kernel-controller`:
 
 ```yaml+jinja
-apiVersion: v1
-kind: Pod
+apiVersion: rbac.authorization.k8s.io/v1
+kind: ClusterRole
 metadata:
-  name: "{{ kernel_pod_name }}"
-  namespace: "{{ kernel_namespace }}"
+  # Referenced by GP_KERNEL_CLUSTER_ROLE in the Deployment
+  name: kernel-controller
   labels:
-    kernel_id: "{{ kernel_id }}"
-    app: enterprise-gateway
+    app: gateway-provisioners
     component: kernel
-spec:
-  restartPolicy: Never
-  serviceAccountName: "{{ kernel_service_account_name }}"
-  {% if kernel_uid is defined or kernel_gid is defined %}
-  securityContext:
-    {% if kernel_uid is defined %}
-    runAsUser: {{ kernel_uid | int }}
-    {% endif %}
-    {% if kernel_gid is defined %}
-    runAsGroup: {{ kernel_gid | int }}
-    {% endif %}
-    fsGroup: 100
-  {% endif %}
-  containers:
-  - env:
-    - name: EG_RESPONSE_ADDRESS
-      value: "{{ eg_response_address }}"
-    - name: EG_PUBLIC_KEY
-      value: "{{ eg_public_key }}"
-    - name: KERNEL_LANGUAGE
-      value: "{{ kernel_language }}"
-    - name: KERNEL_SPARK_CONTEXT_INIT_MODE
-      value: "{{ kernel_spark_context_init_mode }}"
-    - name: KERNEL_NAME
-      value: "{{ kernel_name }}"
-    - name: KERNEL_USERNAME
-      value: "{{ kernel_username }}"
-    - name: KERNEL_ID
-      value: "{{ kernel_id }}"
-    - name: KERNEL_NAMESPACE
-      value: "{{ kernel_namespace }}"
-    image: "{{ kernel_image }}"
-    name: "{{ kernel_pod_name }}"
-```
-
-There are a number of items worth noting:
-
-1. Kernel pods can be identified in three ways using `kubectl`:
-
-   1. By the global label `app=enterprise-gateway` - useful when needing to identify all related objects (e.g., `kubectl get all -l app=enterprise-gateway`)
-   1. By the _kernel_id_ label `kernel_id=<kernel_id>` - useful when only needing specifics about a given kernel. This label is used internally by enterprise-gateway when performing its discovery and lifecycle management operations.
-   1. By the _component_ label `component=kernel` - useful when needing to identity only kernels and not other enterprise-gateway components. (Note, the latter can be isolated via `component=enterprise-gateway`.)
-
-   Note that since kernels run in isolated namespaces by default, it's often helpful to include the clause `--all-namespaces` on commands that will span namespaces. To isolate commands to a given namespace, you'll need to add the namespace clause `--namespace <namespace-name>`.
-
-1. Each kernel pod is named by the invoking user (via the `KERNEL_USERNAME` env) and its kernel_id (env `KERNEL_ID`). This identifier also applies to those kernels launched within `spark-on-kubernetes`.
-
-1. Kernel pods use the specified `securityContext`. If env `KERNEL_UID` is not specified in the kernel creation request a default value of `1000` (the jovyan user) will be used. Similarly, for `KERNEL_GID`, whose default is `100` (the users group). In addition, Enterprise Gateway enforces a list of prohibited UID and GID values. By default, this list is initialized to the 0 (root) UID and GID. Administrators can configure the `EG_PROHIBITED_UIDS` and `EG_PROHIBITED_GIDS` environment variables via the `deployment.yaml` file with comma-separated values to alter the set of user and group ids to be prevented.
-
-1. As noted above, if `KERNEL_NAMESPACE` is not provided in the request, Enterprise Gateway will create a namespace using the same naming algorithm for the pod. In addition, the `kernel-controller` cluster role will be bound to a namespace-scoped role binding of the same name using the namespace's default service account as its subject. Users wishing to use their own kernel namespaces must provide **both** `KERNEL_NAMESPACE` and `KERNEL_SERVICE_ACCOUNT_NAME` as these are both used in the `kernel-pod.yaml.j2` as `{{ kernel_namespace }}` and `{{ kernel_service_account_name }}`, respectively.
-
-1. Kernel pods have restart policies of `Never`. This is because the Jupyter framework already has built-in logic for auto-restarting failed kernels and any other restart policy would likely interfere with the built-in behaviors.
-
-1. The parameters to the launcher that is built into the image are communicated via environment variables as noted in the `env:` section above.
+rules:
+  - apiGroups: [""]
+    resources: ["pods"]
+    verbs: ["get", "watch", "list", "create", "delete"]
+  - apiGroups: [""]
+    resources: ["configmaps"]
+    verbs: ["list", "create"]
+  - apiGroups: [""]
+    resources: ["services", "persistentvolumeclaims"]
+    verbs: ["list"]
+```
 
 ## Unconditional Volume Mounts
 
-Unconditional volume mounts can be added in the `kernel-pod.yaml.j2` template. An example of these unconditional volume mounts can be found when extending docker shared memory. For some I/O jobs the pod will need more than the default `64mb` of shared memory on the `/dev/shm` path.
+Unconditional volume mounts can be added in the `kernel-pod.yaml.j2` template. An example of these unconditional
+volume mounts can be found when extending docker shared memory. For some I/O jobs the pod will need more than
+the default `64mb` of shared memory on the `/dev/shm` path.
 
 ```yaml+jinja
 volumeMounts:
 # Define any "unconditional" mounts here, followed by "conditional" mounts that vary per client
 {% if kernel_volume_mounts is defined %}
   {% for volume_mount in kernel_volume_mounts %}
 - {{ volume_mount }}
@@ -316,15 +284,17 @@
 {% if kernel_volumes is defined %}
 {% for volume in kernel_volumes %}
 - {{ volume }}
 {% endfor %}
 {% endif %}
 ```
 
-The conditional volumes are handled by the loops inside the yaml file. Any unconditional volumes can be added before these conditions. In the scenario where the `/dev/shm` will need to be expanded the following mount has to be added.
+The conditional volumes are handled by the loops inside the yaml file. Any unconditional volumes can be added
+before these conditions. In the scenario where the `/dev/shm` will need to be expanded the following mount
+has to be added.
 
 ```yaml+jinja
 volumeMounts:
 # Define any "unconditional" mounts here, followed by "conditional" mounts that vary per client
 - mountPath: /dev/shm
   name: dshm
 {% if kernel_volume_mounts is defined %}
@@ -342,26 +312,31 @@
 - {{ volume }}
 {% endfor %}
 {% endif %}
 ```
 
 ## Kubernetes Resource Quotas
 
-When deploying kernels on a Kubernetes cluster a best practice is to define request and limit quotas for CPUs, GPUs, and Memory. These quotas can be defined from the client via KERNEL\_-prefixed environment variables which are passed through to the kernel at startup.
+When deploying kernels on a Kubernetes cluster a best practice is to define request and limit quotas for CPUs,
+GPUs, and Memory. These quotas can be defined from the client via `KERNEL_`-prefixed environment variables which are
+passed through to the kernel at startup.
 
 - `KERNEL_CPUS` - CPU Request by Kernel
 - `KERNEL_MEMORY` - MEMORY Request by Kernel
 - `KERNEL_GPUS` - GPUS Request by Kernel
 - `KERNEL_CPUS_LIMIT` - CPU Limit
 - `KERNEL_MEMORY_LIMIT` - MEMORY Limit
 - `KERNEL_GPUS_LIMIT` - GPUS Limit
 
-Memory and CPU units are based on the [Kubernetes Official Documentation](https://kubernetes.io/docs/concepts/configuration/manage-resources-containers/) while GPU is using the NVIDIA `nvidia.com/gpu` parameter. The desired units should be included in the variable's value.
+Memory and CPU units are based on the
+[Kubernetes Official Documentation](https://kubernetes.io/docs/concepts/configuration/manage-resources-containers/)
+while GPU is using the NVIDIA `nvidia.com/gpu` parameter. The desired units should be included in the variable's value.
 
-When defined, these variables are then substituted into the appropriate location of the corresponding kernel-pod.yaml.j2 template.
+When defined, these variables are then substituted into the appropriate location of the corresponding
+`kernel-pod.yaml.j2` template.
 
 ```yaml+jinja
 {% if kernel_cpus is defined or kernel_memory is defined or kernel_gpus is defined or kernel_cpus_limit is defined or kernel_memory_limit is defined or kernel_gpus_limit is defined %}
   resources:
     {% if kernel_cpus is defined or kernel_memory is defined or kernel_gpus is defined %}
     requests:
       {% if kernel_cpus is defined %}
@@ -385,164 +360,160 @@
       {% if kernel_gpus_limit is defined %}
       nvidia.com/gpu: "{{ kernel_gpus_limit }}"
       {% endif %}
     {% endif %}
   {% endif %}
 ```
 
-## KubernetesProcessProxy
-
-To indicate that a given kernel should be launched into a Kubernetes configuration, the kernel.json file's `metadata` stanza must include a `process_proxy` stanza indicating a `class_name:` of `KubernetesProcessProxy`. This ensures the appropriate lifecycle management will take place relative to a Kubernetes environment.
-
-Along with the `class_name:` entry, this process proxy stanza should also include a proxy configuration stanza which specifies the container image to associate with the kernel's pod. If this entry is not provided, the Enterprise Gateway implementation will use a default entry of `elyra/kernel-py:VERSION`. In either case, this value is made available to the rest of the parameters used to launch the kernel by way of an environment variable: `KERNEL_IMAGE`.
-
-_(Please note that the use of `VERSION` in docker image tags is a placeholder for the appropriate version-related image tag. When kernelspecs are built via the Enterprise Gateway Makefile, `VERSION` is replaced with the appropriate version denoting the target release. A full list of available image tags can be found in the dockerhub repository corresponding to each image.)_
-
-```json
-{
-  "metadata": {
-    "process_proxy": {
-      "class_name": "enterprise_gateway.services.processproxies.k8s.KubernetesProcessProxy",
-      "config": {
-        "image_name": "elyra/kernel-py:VERSION"
-      }
-    }
-  }
-}
-```
-
-As always, kernels are launched by virtue of the `argv:` stanza in their respective kernel.json files. However, when launching _vanilla_ kernels in a kubernetes environment, what gets invoked isn't the kernel's launcher, but, instead, a python script that is responsible for using the [Kubernetes Python API](https://github.com/kubernetes-client/python) to create the corresponding pod instance. The pod is _configured_ by applying the values to each of the substitution parameters into the [kernel-pod.yaml](https://github.com/jupyter-server/enterprise_gateway/blob/main/etc/kernel-launchers/kubernetes/scripts/kernel-pod.yaml.j2) file previously displayed. This file resides in the same `scripts` directory as the kubernetes launch script - `launch_kubernetes.py` - which is referenced by the kernel.json's `argv:` stanza:
-
-```json
-{
-  "argv": [
-    "python",
-    "/usr/local/share/jupyter/kernels/python_kubernetes/scripts/launch_kubernetes.py",
-    "--RemoteProcessProxy.kernel-id",
-    "{kernel_id}",
-    "--RemoteProcessProxy.response-address",
-    "{response_address}",
-    "--RemoteProcessProxy.public-key",
-    "{public_key}"
-  ]
-}
-```
-
-By default, _vanilla_ kernels use a value of `none` for the spark context initialization mode so no context will be created automatically.
-
-When the kernel is intended to target _Spark-on-kubernetes_, its launch is very much like kernels launched in YARN _cluster mode_, albeit with a completely different set of parameters. Here's an example `SPARK_OPTS` string value which best conveys the idea:
-
-```
-  "SPARK_OPTS": "--master k8s://https://${KUBERNETES_SERVICE_HOST}:${KUBERNETES_SERVICE_PORT} --deploy-mode cluster --name ${KERNEL_USERNAME}-${KERNEL_ID} --conf spark.kubernetes.driver.label.app=enterprise-gateway --conf spark.kubernetes.driver.label.kernel_id=${KERNEL_ID} --conf spark.kubernetes.executor.label.app=enterprise-gateway --conf spark.kubernetes.executor.label.kernel_id=${KERNEL_ID} --conf spark.kubernetes.driver.docker.image=${KERNEL_IMAGE} --conf spark.kubernetes.executor.docker.image=kubespark/spark-executor-py:v2.5.0-kubernetes-0.5.0 --conf spark.kubernetes.submission.waitAppCompletion=false",
-```
-
-Note that each of the labels previously discussed are also applied to the _driver_ and _executor_ pods.
-
-For these invocations, the `argv:` is nearly identical to non-kubernetes configurations, invoking a `run.sh` script which essentially holds the `spark-submit` invocation that takes the aforementioned `SPARK_OPTS` as its primary parameter:
-
-```json
-{
-  "argv": [
-    "/usr/local/share/jupyter/kernels/spark_python_kubernetes/bin/run.sh",
-    "--RemoteProcessProxy.kernel-id",
-    "{kernel_id}",
-    "--RemoteProcessProxy.response-address",
-    "{response_address}",
-    "--RemoteProcessProxy.public-key",
-    "{public_key}",
-    "--RemoteProcessProxy.spark-context-initialization-mode",
-    "lazy"
-  ]
-}
-```
-
-### Confirming deployment and the service port mapping
-
-```bash
-kubectl get all --all-namespaces -l app=enterprise-gateway
-
-NAME                        DESIRED   CURRENT   UP-TO-DATE   AVAILABLE   AGE
-deploy/enterprise-gateway   1         1         1            1           2h
-
-NAME                               DESIRED   CURRENT   READY     AGE
-rs/enterprise-gateway-74c46cb7fc   1         1         1         2h
-
-NAME                                     READY     STATUS    RESTARTS   AGE
-po/enterprise-gateway-74c46cb7fc-jrkl7   1/1       Running   0          2h
-
-NAME                     TYPE       CLUSTER-IP       EXTERNAL-IP   PORT(S)          AGE
-svc/enterprise-gateway   NodePort   10.110.253.220   <none>        8888:32422/TCP   2h
-```
-
-Of particular importance is the mapping to port `8888` (e.g.,`32422`). If you are performing this on the same host as where the notebook will run, then you will need to note the cluster-ip entry (e.g.,`10.110.253.220`).
+## Other Configuration Items
 
-(Note: if the number of replicas is > 1, then you will see two pods listed with different five-character suffixes.)
-
-```{tip}
- You can avoid the need to point at a different port each time EG is launched by adding an `externalIPs:` entry to the `spec:` section of the `service.yaml` file.  This entry can be specifed in the `values.yaml` via the `service.externalIPs.k8sMasterPublicIP` entry.
-```
-
-The value of the `JUPYTER_GATEWAY_URL` used by the gateway-enabled Notebook server will vary depending on whether you choose to define an external IP or not. If and external IP is defined, you'll set `JUPYTER_GATEWAY_URL=<externalIP>:8888` else you'll set `JUPYTER_GATEWAY_URL=<k8s-master>:32422` **but also need to restart clients each time Enterprise Gateway is started.** As a result, use of the `externalIPs:` value is highly recommended.
-
-## Kubernetes Tips
-
-The following items illustrate some useful commands for navigating Enterprise Gateway within a kubernetes environment.
-
-- All objects created on behalf of Enterprise Gateway can be located using the label `app=enterprise-gateway`. You'll probably see duplicated entries for the deployments(deploy) and replication sets (rs) - we didn't include the duplicates here.
-
-```bash
-kubectl get all -l app=enterprise-gateway --all-namespaces
-
-NAME                        DESIRED   CURRENT   UP-TO-DATE   AVAILABLE   AGE
-deploy/enterprise-gateway   1         1         1            1           3h
-
-NAME                               DESIRED   CURRENT   READY     AGE
-rs/enterprise-gateway-74c46cb7fc   1         1         1         3h
-
-NAME                                             READY     STATUS    RESTARTS   AGE
-pod/alice-5e755458-a114-4215-96b7-bcb016fc7b62   1/1       Running   0          8s
-pod/enterprise-gateway-74c46cb7fc-jrkl7          1/1       Running   0          3h
-```
-
-- All objects related to a given kernel can be located using the label `kernel_id=<kernel_id>`
-
-```bash
-kubectl get all -l kernel_id=5e755458-a114-4215-96b7-bcb016fc7b62 --all-namespaces
-
-NAME                                             READY     STATUS    RESTARTS   AGE
-pod/alice-5e755458-a114-4215-96b7-bcb016fc7b62   1/1       Running   0          28s
-```
-
-Note: because kernels are, by default, isolated to their own namespace, you could also find all objects of a
-given kernel using only the `--namespace <kernel-namespace>` clause.
-
-- To enter into a given pod (i.e., container) in order to get a better idea of what might be happening within the container, use the exec command with the pod name
-
-```bash
-kubectl exec -it enterprise-gateway-74c46cb7fc-jrkl7 /bin/bash
-```
-
-- Logs can be accessed against the pods or deployment (requires the object type prefix (e.g., `pod/`))
-
-```bash
-kubectl logs -f pod/alice-5e755458-a114-4215-96b7-bcb016fc7b62
-```
-
-Note that if using multiple replicas, commands against each pod are required.
-
-- The Kubernetes dashboard is useful as well. It's located at port `30000` of the master node
-
-```bash
-https://elyra-kube1.foo.bar.com:30000/dashboard/#!/overview?namespace=default
-```
+There are some environment variables that can be set in the host application's environment that affect how Gateway
+Provisioners operate within a Kubernetes environment.  For example, `GP_MIRROR_WORKING_DIRS` can be set
+to `True`, instructing Gateway Provisioners to set the launched container's working directory to the value of
+`KERNEL_WORKING_DIR`.  When this environment variable is enabled, it usually implies that volume mounts are in play
+such that the per-user volumes are then available to the launched container.
+
+Other [environment variables](config-add-env.md#additional-environment-variables) applicable to Kubernetes
+configurations are `GP_NAMESPACE` and `GP_PROHIBITED_UIDS`.
+
+````{seealso}
+```{eval-rst}
+See :ref:`configuring-gp`, with a focus on Kubernetes-specific options, for
+additional configuration options within the host application.
+```
+````
+
+## Command-line Options
+
+The following is produced using `jupyter k8s-spec install --help` and displays the complete set of command-line
+options:
+
+```text
+Creates a Jupyter kernel specification for use within a Kubernetes cluster.
+
+Options
+=======
+The options below are convenience aliases to configurable class-options,
+as listed in the "Equivalent to" description-line of the aliases.
+To see all configurable class-options for some <cmd>, use:
+    <cmd> --help-all
+
+--spark
+    Install kernelspec for use with Spark.  When combined with --crd,
+    will configure the SparkOperatorProvisioner for Spark Application CRDs.
+    Equivalent to: [--K8sSpecInstaller.spark=True]
+--user
+    Try to install the kernel spec to the per-user directory instead of the system or environment directory.
+    Equivalent to: [--BaseSpecApp.user=True]
+--replace
+    If a kernel specification already exists in the destination, allow for its replacement.
+    Equivalent to: [--BaseSpecApp.replace=True]
+--sys-prefix
+    Specify a prefix to install to, e.g. an env. The kernelspec will be installed in PREFIX/share/jupyter/kernels/
+    Equivalent to: [--BaseSpecApp.prefix=/opt/miniconda3/envs/provisioners]
+--debug
+    set log level to logging.DEBUG (maximize logging output)
+    Equivalent to: [--Application.log_level=10]
+--tensorflow
+    Install kernelspec for use with Tensorflow.
+    Equivalent to: [--K8sSpecInstaller.tensorflow=True]
+--crd
+    Install kernelspec for use with a Custom Resource Definition.  When combined with --spark,
+    will configure the SparkOperatorProvisioner for Spark Application CRDs.
+    Equivalent to: [--K8sSpecInstaller.crd=True]
+--image-name=<Unicode>
+    The kernel image to use for this kernel specification. If this specification
+    is enabled for Spark usage, this image will be the driver image.
+    (GP_IMAGE_NAME env var)
+    Default: None
+    Equivalent to: [--K8sSpecInstaller.image_name]
+--executor-image-name=<Unicode>
+    The executor image to use for this kernel specification.  Only applies to
+    Spark-enabled kernel specifications.  (GP_EXECUTOR_IMAGE_NAME env var)
+    Default: None
+    Equivalent to: [--K8sSpecInstaller.executor_image_name]
+--spark-home=<Unicode>
+    Specify where the spark files can be found.
+    Default: '/opt/spark'
+    Equivalent to: [--BaseSpecSparkApp.spark_home]
+--spark-init-mode=<Unicode>
+    Spark context initialization mode.  Must be one of ['lazy', 'eager', 'none'].
+        Default = lazy.
+    Default: 'lazy'
+    Equivalent to: [--BaseSpecSparkApp.spark_init_mode]
+--extra-spark-opts=<Unicode>
+    Specify additional Spark options.
+    Default: ''
+    Equivalent to: [--BaseSpecSparkApp.extra_spark_opts]
+--prefix=<Unicode>
+    Specify a prefix to install to, e.g. an env. The kernelspec will be
+    installed in PREFIX/share/jupyter/kernels/
+    Default: ''
+    Equivalent to: [--BaseSpecApp.prefix]
+--kernel-name=<Unicode>
+    Install the kernel spec into a directory with this name.
+    Default: ''
+    Equivalent to: [--BaseSpecApp.kernel_name]
+--display-name=<Unicode>
+    The display name of the kernel - used by user-facing applications.
+    Default: ''
+    Equivalent to: [--BaseSpecApp.display_name]
+--language=<Unicode>
+    The language of the kernel referenced in the kernel specification.  Must be one of
+        'Python', 'R', or 'Scala'.  Default = 'Python'.
+    Default: 'Python'
+    Equivalent to: [--BaseSpecApp.language]
+--authorized-users=<set-item-1>...
+    List of user names against which KERNEL_USERNAME will be compared. Any match
+    (case-sensitive) will allow the kernel's launch, otherwise an HTTP 403
+    (Forbidden) error will be raised.  The set of unauthorized users takes
+    precedence. This option should be used carefully as it can dramatically
+    limit who can launch kernels. To specify multiple names via the CLI,
+    separate options must be provided for each entry. (GP_AUTHORIZED_USERS env
+    var - non-bracketed, just comma-separated)
+    Default: set()
+    Equivalent to: [--BaseSpecApp.authorized_users]
+--unauthorized-users=<set-item-1>...
+    List of user names against which KERNEL_USERNAME will be compared. Any match
+    (case-sensitive) will prevent the kernel's launch and result in an HTTP 403
+    (Forbidden) error. To specify multiple names via the CLI, separate options
+    must be provided for each entry. (GP_UNAUTHORIZED_USERS env var - non-
+    bracketed, just comma-separated)
+    Default: {'root'}
+    Equivalent to: [--BaseSpecApp.unauthorized_users]
+--port-range=<Unicode>
+    Specifies the lower and upper port numbers from which ports are created. The
+    bounded values are separated by '..' (e.g., 33245..34245 specifies a range
+    of 1000 ports to be randomly selected). A range of zero (e.g., 33245..33245
+    or 0..0) disables port-range enforcement.  (GP_PORT_RANGE env var)
+    Default: '0..0'
+    Equivalent to: [--BaseSpecApp.port_range]
+--launch-timeout=<Int>
+    Number of ports to try if the specified port is not available
+    (GP_LAUNCH_TIMEOUT env var)
+    Default: 30
+    Equivalent to: [--BaseSpecApp.launch_timeout]
+--ipykernel-subclass-name=<Unicode>
+    For Python kernels, the name of the ipykernel subclass.
+    Default: 'ipykernel.ipkernel.IPythonKernel'
+    Equivalent to: [--BaseSpecApp.ipykernel_subclass_name]
+--log-level=<Enum>
+    Set the log level by value or name.
+    Choices: any of [0, 10, 20, 30, 40, 50, 'DEBUG', 'INFO', 'WARN', 'ERROR', 'CRITICAL']
+    Default: 30
+    Equivalent to: [--Application.log_level]
+--config=<Unicode>
+    Full path of a config file.
+    Default: ''
+    Equivalent to: [--JupyterApp.config_file]
+
+Examples
+--------
 
-From there, logs can be accessed by selecting the `Pods` option in the left-hand pane followed by the _lined_ icon on
-the far right.
+    jupyter-k8s-spec install --language=R --kernel-name=r_k8s --image-name=foo/my_r_kernel_image:v4_0
 
-- User "system:serviceaccount:default:default" cannot list pods in the namespace "default"
+    jupyter-k8s-spec install --language=Scala --spark --kernel-name=scala_k8s_spark --display-name='Scala on Kubernetes with Spark'
 
-On a recent deployment, Enterprise Gateway was not able to create or list kernel pods. Found
-the following command was necessary. (Kubernetes security relative to Enterprise Gateway is still under construction.)
+    jupyter-k8s-spec install --spark --crd --display-name='Python SparkOperator"
 
-```bash
-kubectl create clusterrolebinding add-on-cluster-admin --clusterrole=cluster-admin  --serviceaccount=default:default
+To see all available configurables, use `--help-all`.
 ```
```

### Comparing `gateway_provisioners-0.1.0/docs/source/operators/index.rst` & `gateway_provisioners-0.2.0/docs/source/operators/index.rst`

 * *Files 16% similar despite different names*

```diff
@@ -4,65 +4,77 @@
 These pages are targeted at *operators* that need to deploy and configure a Jupyter server instance with
 gateway provisioners.
 
 .. admonition:: Use cases
 
     - *As an operator, I want to fix the bottleneck on the local server due to large number of kernels running on it and the size of each kernel (spark driver) process, by deploying the Gateway Provisioners, such that kernels can be launched as managed resources within a Hadoop YARN cluster, distributing the resource-intensive driver processes across the cluster, while still allowing the multiple data analysts to leverage the compute power of a large cluster.*
     - *As an operator, I want to constrain applications to specific port ranges so I can more easily identify issues and manage network configurations that adhere to my corporate policy.*
-    - *As an operator, I want to constrain the number of active kernels that each of my users can have at any given time.*
 
 
 Deploying Gateway Provisioners
 ------------------------------
-The deployment of Enterprise Gateway consists of several items, depending on
-the nature of the target environment.  Because this topic differs depending on
-whether the runtime environment is targeting containers or traditional servers,
-we've separated the discussions accordingly.
+When considering the deployment and configuration of Gateway Provisioners it is important
+to understand where your users notebooks will be located relative to the compute resources
+you wish to leverage.
+
+For example, if your users use notebooks on their local desktops but
+want to leverage kernels running within a Kubernetes cluster, the deployment and configuration
+of Gateway Provisioners should take place within a Gateway server (docker image) that can be remote from the
+user's desktop.
+
+If, on the other hand, your users already run within a Kubernetes cluster via JupyterHub (for example),
+then the deployment and configuration of Gateway Provisioners would take place within the Jupyter Lab container
+image that is launched on behalf of each user.
+
+Regardless of *which* host application to update, Gateway Provisioners are deployed and configured wherever the
+kernel process is ultimately launched. In any case, the host application is using `jupyter_client` to launch kernels.
 
 Container-based deployments
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~
 Gateway Provisioners includes support for two forms of container-based environments, Kubernetes
 and Docker.
 
 .. toctree::
    :maxdepth: 1
    :name: container-deployments
 
+   installing-gp-container
+   installing-kernels-container
    deploy-kubernetes
    deploy-docker
 
 Server-based deployments
 ~~~~~~~~~~~~~~~~~~~~~~~~
-Tasks for traditional server deployments are nearly identical with respect to
-Gateway Provisioners' installation, differing slightly with how the kernel
-specifications are configured.  As a result, we marked those topics
-as "common" relative to the others.
-
-FIXME - review the "common" wording above
+Tasks for traditional server deployments are nearly identical to container-based deployments
+except the commands are not entered within a `Dockerfile`, but rather in the shell of the
+server where the host application resides.
 
 .. toctree::
    :maxdepth: 1
    :name: node-deployments
 
    installing-gp
    installing-kernels
    deploy-yarn-cluster
    deploy-distributed
 
+
+.. _configuring-gp:
+
 Configuring Gateway Provisioners
 --------------------------------
 The Gateway Provisioners package adheres to
 `Jupyter's common configuration approach <https://jupyter.readthedocs.io/en/latest/use/config.html>`_
 . However, because its a library package and not a standalone application, you must add its configurable
 items into the hosting application's configuration file (recommended) or by setting the corresponding
 environment variables.
 
 .. toctree::
    :maxdepth: 1
-   :name: configuring
+   :name: configuration
 
    config-file
    config-add-env
    config-env-debug
    config-sys-env
    config-kernel-override
    config-security
```

### Comparing `gateway_provisioners-0.1.0/docs/source/operators/installing-gp.md` & `gateway_provisioners-0.2.0/docs/source/operators/installing-gp.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,17 @@
-# Installing Gateway Provisioners
+# Installing Gateway Provisioners (Servers)
 
-Gateway Provisioners require `jupyter_client >= 7.0`. Attempts to install into existing environments
+These instructions are relative to the host application _server_.  For _container-based_ installations, see
+[Installing Gateway Provisioners (Containers)](installing-gp-container.md).
+
+```{attention}
+Gateway Provisioners require `jupyter_client >= 7.0`. Attempts to install Gateway Provisioners into existing environments
 with older versions of `jupyter_client` will be met with resolution warnings and no kernel provisioners
 (remote or local) will be used.
+```
 
 Base functionality is installed using either of the following commands...
 
 ```bash
 pip install --upgrade gateway_provisioners
 ```
 
@@ -19,55 +24,27 @@
 ```{note}
 We recommend the use of `mamba` over `conda`.  However, if you need to use `conda`, all `mamba`
 commands should be directly replacable with `conda`.
 ```
 
 ## Optional Dependencies
 
-At this point, the GatewayProvisioners provides the _ability_ to configure kernel specifications for any of its
-kernel provisioner implementations. However, because so different target configurations are supported, the
+At this point, the Gateway Provisioners provides the _ability_ to configure kernel specifications for any of its
+kernel provisioner implementations. However, because multiple target configurations are supported, the
 libraries relative to the actual target environment should also be installed using optional dependencies.
 
 ```{note}
 Attempts to create kernel specifications for environments in which the optional dependencies have not been installed
 will still generate specifications, but warning messages will also be produced as those specifications are not
 usable until their dependencies have been installed.
 ```
 
 GatewayProvisioners supports the following optional dependencies, each of which can be included in brackets on
 the installation command.
 
-### Kubernetes
-
-If you plan to target Kubernetes environments use:
-
-```bash
-pip install --upgrade gateway_provisioners[k8s]
-```
-
-or
-
-```bash
-mamba install -c conda-forge gateway_provisioners[k8s]
-```
-
-### Docker or DockerSwarm
-
-If you plan to target Docker or DockerSwarm environments use:
-
-```bash
-pip install --upgrade gateway_provisioners[docker]
-```
-
-or
-
-```bash
-mamba install -c conda-forge gateway_provisioners[docker]
-```
-
 ### Hadoop YARN
 
 If you plan to target Hadoop YARN environments use:
 
 ```bash
 pip install --upgrade gateway_provisioners[yarn]
 ```
@@ -79,22 +56,22 @@
 ```
 
 ### Distributed/SSH
 
 If you plan to target multi-node environments via SSH, nothing additional is necessary as all required libraries
 are included in the base installation.
 
-### Mixed environments
+```bash
+pip install --upgrade gateway_provisioners
+```
 
-Although unlikely, if you need to support multiple types of clusters, the optional dependencies can be combined as
-comma-seperated values. For example, to support both Kubernetes and Hadoop YARN environments from the same server,
-one would issue:
+or
 
 ```bash
-pip install --upgrade gateway_provisioners[k8s, yarn]
+mamba install -c conda-forge gateway_provisioners
 ```
 
 ## Uninstalling Gateway Provisioners
 
 To uninstall Gateway Provisioners...
 
 ```bash
@@ -103,9 +80,9 @@
 
 ```bash
 mamba uninstall gateway_provisioners
 ```
 
 ```{tip}
 To fully _complete_ the removal of gateway provisioners, any kernel specifications referencing the various
-Gateway Provisioners should be removed as well.
+Gateway Provisioners should be removed as well.  Kernel specifications can be located using `jupyter kernelspec list`.
 ```
```

### Comparing `gateway_provisioners-0.1.0/docs/source/operators/installing-kernels.md` & `gateway_provisioners-0.2.0/docs/source/operators/installing-kernels.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-# Installing supported kernels (common)
+# Installing Supported Kernels (Servers)
 
-Gateway Provisioners includes kernel specifications that support the following kernels:
+Gateway Provisioners includes tooling to create kernel specifications that support the following kernels:
 
 - IPython kernel (Python)
 - Apache Toree (Scala)
 - IRKernel (R)
 
 Refer to the following for instructions on installing the respective kernels. For cluster-based environments, these
 steps should be performed on each applicable node of the cluster, unless noted otherwise.
 
 ```{admonition} Important!
 :class: warning
-For proper operation across the _non-containerized clusters_, the IpyKernel and IRkernel packages (not the
+For proper operation across the _non-containerized clusters_, the IPyKernel and IRkernel packages (not the
 kernel specification) must be installed on every node of the cluster available to Gateway Provisioners.
 For example, run `pip install ipykernel` on each applicable node.
 
 Note: This step is **not** required for the Scala (Apache Toree) Kernel as that can be expressed as a
-dependency in the `spark_submit` invocation where the package is copied during launch.
+dependency in the `spark-submit` invocation where the package is copied during launch.
 ```
 
 ## Python Kernel (IPython kernel)
 
-The IPython kernel comes pre-installed with Anaconda and we have tested with its default version
+The IPython kernel comes pre-installed with Anaconda, and we have tested with its default version
 of [IPython kernel](https://ipython.readthedocs.io/en/stable/).
 
 ```bash
 pip install --upgrade ipykernel
 ```
 
 or
```

### Comparing `gateway_provisioners-0.1.0/docs/source/other/related-resources.md` & `gateway_provisioners-0.2.0/docs/source/contributors/related-resources.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Related Resources
 
-Here are some resources related to the Jupyter Enterprise Gateway project.
+Here are some resources related to the Gateway Provisioners project.
 
-- [Jupyter.org](https://jupyter.org)
-- [Jupyter Server Team Compass](https://github.com/jupyter-server/team-compass#jupyter-server-team-compass)
-- [Jupyter Calendar - Community Meetings](https://docs.jupyter.org/en/latest/community/content-community.html#jupyter-community-meetings)
-- [Jupyter Community Discourse Forum](https://discourse.jupyter.org/)
+- [Jupyter.org](https://jupyter.org) - the official Jupyter organization website.
+- [Jupyter Server Team Compass](https://github.com/jupyter-server/team-compass#jupyter-server-team-compass) - all things related to the Jupyter Server organization.
+- [Jupyter Calendar - Community Meetings](https://docs.jupyter.org/en/latest/community/content-community.html#jupyter-community-meetings) - the set of Jupyter-related meetings - all are welcome!
+- [Jupyter Community Discourse Forum](https://discourse.jupyter.org/) - the public forum for Jupyter-related questions, discussions, and announcements.
 - [Jupyter Enterprise Gateway Github Repo](https://github.com/jupyter-server/enterprise_gateway) - the source code for Enterprise Gateway - which supports remote kernels using Process Proxies. It's 4.0 release will support kernel provisioners and process proxy support will go away.
 - [Jupyter Kernel Gateway Github Repo](https://github.com/jupyter-server/kernel_gateway) - the source code for Kernel Gateway - which immediately supports kernel provisioners by virtue of using the base `KernelManager` class.
 - [Jupyter Server Github Repo](https://github.com/jupyter-server/jupyter_server) - the source code for the Jupyter Server.
-- [Jupyter Client Github Repo](https://github.com/jupyter/jupyter_client) - the source code for the base kernel lifecycle management and message classes. Enterprise Gateway extends the `KernelManager` classes of `jupyter_client`.
+- [Jupyter Client Github Repo](https://github.com/jupyter/jupyter_client) - the source code for the base kernel management, provisioner, and messaging (client) classes.
```

### Comparing `gateway_provisioners-0.1.0/docs/source/other/troubleshooting.md` & `gateway_provisioners-0.2.0/docs/source/operators/deploy-yarn-cluster.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,275 +1,330 @@
-# Troubleshooting Guide
+# Hadoop YARN deployments
 
-This page identifies scenarios we've encountered when running Enterprise Gateway. We also provide
-instructions for setting up a debug environment on our [Debugging Jupyter Enterprise Gateway](../contributors/debug.md) page.
-
-## Fresh Install
-
-Scenario: **I just installed Enterprise Gateway but nothing happens, how do I proceed?**
-
-Because Enterprise Gateway is one element of a networked application, there are various _touch points_ that should
-be validated independently. The following items can be used as a checklist to confirm general operability.
-
-1. Confirm that Enterprise Gateway is servicing general requests. This can be accomplished using the following
-   `curl` command, which should produce the json corresponding to the configured kernelspecs:
-   `bash curl http://<gateway_server>:<gateway_port>/api/kernelspecs `
-1. Independently validate any resource manager you're running against. Various resource managers usually provide
-   examples for how to go about validating their configuration.
-1. Confirm that the Enterprise Gateway arguments for contacting the configured resource manager are in place. These
-   should be covered in the deployment section of our Operators Guide.
-1. If using a Notebook server as your front-end, ensure that the Gateway configuration options or NB2KG extension settings are properly configured.
-   Once the notebook has started, a refresh on the tree view should issue the same `kernelspecs` request in step 1 and
-   the drop-down menu items for available kernels should reflect an entry for each kernelspec returned.
-1. **Always** consult your Enterprise Gateway log file. If you have not redirected `stdout` and `stderr` to a
-   file you are highly encouraged to do so. In addition, you should enable `DEBUG` logging at least until your
-   configuration is stable. Please note, however, that you may be asked to produce an Enterprise Gateway log with
-   `DEBUG` enabled when reporting issues.
-
-## Hadoop YARN Cluster Mode
-
-Scenario: **I'm trying to launch a (Python/Scala/R) kernel in YARN Cluster Mode, but it failed with
-a "Kernel error" and State: 'FAILED'.**
-
-1. Check the output from Enterprise Gateway for an error message. If an applicationId was
-   generated, make a note of it. For example, you can locate the applicationId
-   `application_1506552273380_0011` from the following snippet of message:
-   `[D 2017-09-28 17:13:22.675 EnterpriseGatewayApp] 13: State: 'ACCEPTED', Host: 'burna2.yourcompany.com', KernelID: '28a5e827-4676-4415-bbfc-ac30a0dcc4c3', ApplicationID: 'application_1506552273380_0011' 17/09/28 17:13:22 INFO YarnClientImpl: Submitted application application_1506552273380_0011 17/09/28 17:13:22 INFO Client: Application report for application_1506552273380_0011 (state: ACCEPTED) 17/09/28 17:13:22 INFO Client: client token: N/A diagnostics: AM container is launched, waiting for AM container to Register with RM ApplicationMaster host: N/A ApplicationMaster RPC port: -1 queue: default start time: 1506644002471 final status: UNDEFINED tracking URL: http://burna1.yourcompany.com:8088/proxy/application_1506552273380_0011/`
-1. Lookup the YARN log for that applicationId in the YARN ResourceManager UI: ![YARN ResourceManager UI](../images/yarnui.jpg)
-1. Drill down from the applicationId to find logs for the failed attempts and take appropriate
-   actions. For example, for the error below,
-   ```
-   Traceback (most recent call last):
-    File "launch_ipykernel.py", line 7, in <module>
-      from ipython_genutils.py3compat import str_to_bytes
-    ImportError: No module named ipython_genutils.py3compat
-   ```
-   Simply running "pip install ipython_genutils" should fix the problem. If Anaconda is
-   installed, make sure the environment variable for Python, i.e. `PYSPARK_PYTHON`, is
-   properly configured in the kernelspec and matches the actual Anaconda installation
-   directory.
-
-## SSH Permissions
-
-Scenario: **I'm trying to launch a (Python/Scala/R) kernel in YARN Client Mode, but it failed with
-a "Kernel error" and an `AuthenticationException`.**
-
-```
-[E 2017-09-29 11:13:23.277 EnterpriseGatewayApp] Exception 'AuthenticationException' occurred
-when creating a SSHClient connecting to 'xxx.xxx.xxx.xxx' with user 'elyra',
-message='Authentication failed.'.
-```
-
-This error indicates that the password-less ssh may not be properly configured. Password-less
-ssh needs to be configured on the node that the Enterprise Gateway is running on to all other
-worker nodes.
-
-You might also see an `SSHException` indicating a similar issue.
+Hadoop YARN deployments will utilize the `YarnProvisioner` to launch kernels across the cluster via
+the YARN resource manager.  The following assumes a Hadoop Yarn cluster has already been provisioned.
 
-```
-[E 2017-09-29 11:13:23.277 EnterpriseGatewayApp] Exception 'SSHException' occurred
-when creating a SSHClient connecting to 'xxx.xxx.xxx.xxx' with user 'elyra',
-message='No authentication methods available.'.
-```
-
-In general, you can look for more information in the kernel log for YARN Client
-kernels. The default location is /tmp with a filename of `kernel-<kernel_id>.log`. The location
-can be configured using the environment variable `EG_KERNEL_LOG_DIR` during Enterprise Gateway start up.
-
-```{seealso}
-[Operators Guide](../operators/config-add-env.md#additional-environment-variables)
-for a list of configurable environment variables.
-```
-
-## SSH Tunneling
-
-Scenario: **I'm trying to launch a (Python/Scala/R) kernel in YARN Client Mode with SSH tunneling enabled,
-but it failed with a "Kernel error" and a SSHException.**
-
-```
-[E 2017-10-26 11:48:20.922 EnterpriseGatewayApp] The following exception occurred waiting
-for connection file response for KernelId 'da3d0dde-9de1-44b1-b1b4-e6f3cf52dfb9' on host
-'remote-host-name': The authenticity of the host can't be established.
+```{note}
+In some cases, where a Spark "client mode" is desired, use of the `DistributedProvisioner`
+will be leveraged. Please refer to the [_Distributed deployments_](deploy-distributed.md) topic
+for those details.
 ```
 
-This error indicates that fingerprint for the ECDSA key of the remote host has not been added
-to the list of known hosts from where the SSH tunnel is being established.
+Steps required to complete deployment on a Hadoop YARN cluster are:
 
-For example, if the Enterprise Gateway is running on `node1` under service-user `jdoe` and
-environment variable `EG_REMOTE_HOSTS` is set to `node2,node3,node4`, then the Kernels can be
-launched on any of those hosts and a SSH tunnel will be established between `node1` and
-any of the those hosts.
+1. Install the host application on the primary node of the Hadoop YARN cluster.
+1. [Install Gateway Provisioners](installing-gp.md#hadoop-yarn) where the host application is located. Note,
+   this location is not a hard-requirement, but recommended.
+   If installed remotely, some extra configuration will be necessary relative to the Hadoop configuration.
+1. [Install the desired kernels](installing-kernels.md).
+1. Generate the desired kernel specifications ([see below](#generating-kernel-specifications)).
+1. If necessary, configure the host application and generated kernel specifications relative to the
+   `YarnProvisioner`'s [configurable options](config-file.md), [environment variables](config-add-env.md), and
+   [per-kernel overrides](config-kernel-override.md#yarnprovisioner-per-kernel-overrides).
+1. Launch the host application.
 
-To address this issue, you need to perform a one-time step that requires you to login to
-`node1` as `jdoe` and manually SSH into each of the remote hosts and accept the fingerprint
-of the ECDSA key of the remote host to be added to the list of known hosts as shown below:
+## Prerequisites
 
-```
-[jdoe@node1 ~]$ ssh node2
-The authenticity of host 'node2 (172.16.207.191)' can't be established.
-ECDSA key fingerprint is SHA256:Mqi3txf4YiRC9nXg8a/4gQq5vC4SjWmcN1V5Z0+nhZg.
-ECDSA key fingerprint is MD5:bc:4b:b2:39:07:98:c1:0b:b4:c3:24:38:92:7a:2d:ef.
-Are you sure you want to continue connecting (yes/no)? yes
-Warning: Permanently added 'node2,172.16.207.191' (ECDSA) to the list of known hosts.
-[jdoe@node2 ~] exit
-```
+The distributed capabilities are currently based on an Apache Spark cluster utilizing Hadoop
+YARN as the resource manager and thus require the following environment variables to be set
+to facilitate the integration between Apache Spark and Hadoop YARN components:
 
-Repeat the aforementioned step as `jdoe` on `node1` for each of the hosts listed in
-`EG_REMOTE_HOSTS` and restart Enterprise Gateway.
+- `SPARK_HOME` must point to the Apache Spark installation path
 
-## Kernel Encounters `TypeError`
-
-Scenario: **I'm trying to launch a (Python/Scala/R) kernel, but it failed with `TypeError: Incorrect padding`.**
-
-```
-Traceback (most recent call last):
-  File "/opt/conda/lib/python3.7/site-packages/tornado/web.py", line 1512, in _execute
-    result = yield result
-  File "/opt/conda/lib/python3.7/site-packages/tornado/gen.py", line 1055, in run
-    value = future.result()
-  ...
-  ...
-  File "/opt/conda/lib/python3.7/site-packages/enterprise_gateway/services/kernels/remotemanager.py", line 125, in _launch_kernel
-    return self.process_proxy.launch_process(kernel_cmd, **kw)
-  File "/opt/conda/lib/python3.7/site-packages/enterprise_gateway/services/processproxies/yarn.py", line 63, in launch_process
-    self.confirm_remote_startup(kernel_cmd, **kw)
-  File "/opt/conda/lib/python3.7/site-packages/enterprise_gateway/services/processproxies/yarn.py", line 174, in confirm_remote_startup
-    ready_to_connect = self.receive_connection_info()
-  File "/opt/conda/lib/python3.7/site-packages/enterprise_gateway/services/processproxies/processproxy.py", line 565, in receive_connection_info
-    raise e
-TypeError: Incorrect padding
-```
-
-To address this issue, first ensure that the launchers used for each kernel are derived
-from the same release as the Enterprise Gateway server. Next ensure that `pycryptodomex 3.9.7`
-or later is installed on all hosts using either `pip install` or `conda install` as shown below:
-
-```
-[jdoe@node1 ~]$ pip uninstall pycryptodomex
-[jdoe@node1 ~]$ pip install pycryptodomex
+```bash
+export SPARK_HOME=/usr/hdp/current/spark2-client  # For HDP distribution
 ```
 
-or
+- `GP_YARN_ENDPOINT` must point to the YARN resource manager endpoint if the host application is
+  remote from the YARN cluster
 
-```
-[jdoe@node1 ~]$ conda install pycryptodomex
+```bash
+export GP_YARN_ENDPOINT=http://${YARN_RESOURCE_MANAGER_FQDN}:8088/ws/v1/cluster
 ```
 
-This should be done on the host running Enterprise Gateway as well as all the remote hosts
-on which the kernel is launched.
-
-## Port Range
-
-Scenario: **I'm trying to launch a (Python/Scala/R) kernel with port range, but it failed with `RuntimeError: Invalid port range `.**
-
-```
-Traceback (most recent call last):
-  File "/opt/conda/lib/python3.7/site-packages/tornado/web.py", line 1511, in _execute
-    result = yield result
-  File "/opt/conda/lib/python3.7/site-packages/tornado/gen.py", line 1055, in run
-    value = future.result()
-  ....
-  ....
-  File "/opt/conda/lib/python3.7/site-packages/enterprise_gateway/services/processproxies/processproxy.py", line 478, in __init__
-    super(RemoteProcessProxy, self).__init__(kernel_manager, proxy_config)
-  File "/opt/conda/lib/python3.7/site-packages/enterprise_gateway/services/processproxies/processproxy.py", line 87, in __init__
-    self._validate_port_range(proxy_config)
-  File "/opt/conda/lib/python3.7/site-packages/enterprise_gateway/services/processproxies/processproxy.py", line 407, in _validate_port_range
-    "port numbers is (1024, 65535).".format(self.lower_port))
-RuntimeError: Invalid port range '1000..2000' specified. Range for valid port numbers is (1024, 65535).
+```{note}
+If the server is using an applicable `HADOOP_CONF_DIR` that contains a valid `yarn-site.xml` file,
+then this config value can remain unset (default = None) and the YARN client library will locate
+the appropriate resource manager from the configuration.  This is also true in cases where the
+YARN cluster is configured for high availability.
 ```
 
-To address this issue, make sure that the specified port range does not overlap with TCP's well-known
-port range of (0, 1024\].
-
-## Hadoop YARN Timeout
-
-Scenario: **I'm trying to launch a (Python/Scala/R) kernel, but it times out and the YARN application status remain `ACCEPTED`.**
-
-Enterprise Gateway log from server will look like the one below, and will complain that there are no resources:
-`launch timeout due to: YARN resources unavailable`
+If the server is remote from the YARN cluster (i.e., no `HADOOP_CONF_DIR`) and the YARN cluster is
+configured for high availability, then the alternate endpoint should also be specified...
 
 ```bash
-    State: 'ACCEPTED', Host: '', KernelID: '3181db50-8bb5-4f91-8556-988895f63efa', ApplicationID: 'application_1537119233094_0001'
-    State: 'ACCEPTED', Host: '', KernelID: '3181db50-8bb5-4f91-8556-988895f63efa', ApplicationID: 'application_1537119233094_0001'
-  ...
-  ...
-    SIGKILL signal sent to pid: 19690
-    YarnClusterProcessProxy.kill, application ID: application_1537119233094_0001, kernel ID: 3181db50-8bb5-4f91-8556-988895f63efa, state: ACCEPTED
-    KernelID: '3181db50-8bb5-4f91-8556-988895f63efa' launch timeout due to: YARN resources unavailable after 61.0 seconds for app application_1537119233094_0001, launch timeout: 60.0!  Check YARN configuration.
+export GP_ALT_YARN_ENDPOINT=http://${ALT_YARN_RESOURCE_MANAGER_FQDN}:8088/ws/v1/cluster #Common to YARN deployment
 ```
 
-The most common cause for this is that YARN Resource Managers are failing to start and the cluster see no resources available.
-Make sure YARN Resource Managerss are running ok. We have also noticed that, in Kerborized environments, sometimes there are
-issues with directory access rights that cause the YARN Resource Managers to fail to start and this can be corrected by validating
-the existence of `/hadoop/yarn` and that it's owned by `yarn: hadoop`.
+## Generating Kernel Specifications
 
-## Kernel Resources
+Gateway Provisioners provides the `jupyter-yarn-spec` to generate kernel specifications for the `YarnProvisioner`.
 
-Scenario: **My kernel keeps dying when processing jobs that require large amount of resources (e.g. large files)**
-
-This is usually seen when you are trying to use more resources then what is available for your kernel.
-To address this issue, increase the amount of memory available for your Hadoop YARN application or another
-resource manager managing the kernel. For example, on Kubernetes, this may be a time when the kernel specification's [kernel-pod.yaml.j2](https://github.com/jupyter-server/enterprise_gateway/blob/main/etc/kernel-launchers/kubernetes/scripts/kernel-pod.yaml.j2) file should be extended with resource quotas.
-
-## Spark and Python Versions
-
-Scenario: **PySpark 2.4.x fails on Python 3.8**
-
-PySpark 2.4.x fails on Python 3.8 as described in [SPARK-29536](https://issues.apache.org/jira/browse/SPARK-29536).
-Use Python 3.7.x as the issue only seems to have been resolved on Spark 3.0.
-
-## Kerberos
-
-Scenario: **I'm trying to use a notebook with user impersonation on a Kerberos enabled cluster, but it fails to authenticate.**
-
-When using user impersonation in a YARN cluster with Kerberos authentication, if Kerberos is not
-setup properly you will usually see the following warning in your Enterprise Gateway log that will keep a notebook from connecting:
+To generate a default kernel specification (where Python is the default kernel) enter:
 
 ```bash
-  WARN Client: Exception encountered while connecting to the server : javax.security.sasl.SaslException: GSS initiate failed
-    [Caused by GSSException: No valid credentials provided (Mechanism level: Failed to find any Kerberos tgt)]
+jupyter yarn-spec install
 ```
 
-The most common cause for this WARN is when the user that started Enterprise Gateway is not authenticated
-with Kerberos. This can happen when the user has either not run `kinit` or their previous ticket has expired.
+which produces the following output...
 
-## Openshift Kubernetes
+```text
+[I 2023-02-08 09:48:48.685 YarnSpecInstaller] Installing kernel specification for 'Spark Python (YARN Cluster)'
+[I 2023-02-08 09:48:49.048 YarnSpecInstaller] Installed kernelspec yarn_spark_python in /usr/local/share/jupyter/kernels/yarn_spark_python
+```
+
+and the following set of files and directories:
+
+```text
+/usr/local/share/jupyter/kernels/yarn_spark_python
+kernel.json logo-64x64.png
+
+/usr/local/share/jupyter/kernels/yarn_spark_python/bin:
+run.sh
+
+/usr/local/share/jupyter/kernels/yarn_spark_python/scripts:
+launch_ipykernel.py server_listener.py
+```
+
+where each provides the following function:
+
+- `kernel.json` - the primary file that the host application uses to discover a given kernel's availability.
+  This file contains _stanzas_ that describe the kernel's argument vector (`argv`), its runtime environment (`env`),
+  its display name (`display_name`) and language (`language`), as
+  well as its kernel provisioner's configuration (`metadata.kernel_provisioner`) - which, in this case, will reflect the
+  `YarnProvisioner`.
+- `logo-64x64.png` - the icon resource corresponding to this kernel specification.  Icon resource files must be start
+  with the `logo-` prefix to be included in the kernel specification.
+- `bin/run.sh` - the first entry in the `kernel.json`'s `argv` stanza, this script sets up and invokes the `spark-submit`
+  command that is responsible for interacting with the Hadoop Yarn Resource Manager.  The `YarnProvisioner` then
+  _discovers_ the location of where the kernel (Spark driver) was scheduled to run to complete the kernel's startup.
+- `scripts/launch_ipykernel.py` - the "launcher" for the IPyKernel kernel (or subclasses thereof).  This file is typically
+  implemented in the language of the kernel and is responsible for creating the local connection information, asynchronously
+  starting a SparkContext (if asked), spawning a listener process to receive interrupts and shutdown requests, and starting
+  the IPyKernel itself.
+- `scripts/server_listener.py` - utilized by both Python and R kernels, this file is responsible for encrypting the
+  connection information and sending it back to the host application, then listening for interrupt and shutdown requests.
+
+```{note}
+R-based kernel specifications will see a `scripts/launch_IRkernel.R` script alongside `server_listener.py`, while
+Scala-based specifications will, instead, have a `lib` directory containing jar files for both the scala launcher
+(`toree-launcher-SCALA_VERSION.jar` and includes equivalent functionality to `server_listener.py`) and the Apache
+toree kernel (`toree-assembly-TOREE_VERSION.jar`)
+```
+
+```{tip}
+For shared environments (typical in Gateway server deployments) we recommend installing kernel specifications
+into a shared folder like `/usr/local/share/jupyter/kernels` (which is the default).  This is the location in
+which they reside within container images and where many of the document references assume they'll be located.
+
+Alternate locations can be specified via option `--user` (which places the set of files within the invoking user's
+home directory structure) or option `--sys-prefix` (which places the set of files within the active python
+environment's directory structure).
+```
+
+```{admonition} Important!
+:class: warning
+With the `YarnProvisioner`, only the Python and R kernel _packages_ are required on each node,
+not the entire kernel specification (i.e., the kernel installation files).  For Scala (Apache Toree)
+kernels, the kernel package is included in the `spark-submit` command and copied to each node
+(if not already there) as noted above.
+```
+
+### Adjusting Kernel Specifications
+
+While many options can be specified via command-line options to `jupyter yarn-spec install`, there may be times when
+manual adjustments are necessary.
+
+After generating the kernel specifications, you should have a `kernel.json` that resembles the
+following (this one is relative to the Python kernel using defaulted parameters):
+
+```json
+{
+  "argv": [
+    "/usr/local/share/jupyter/kernels/yarn_spark_python/bin/run.sh",
+    "--kernel-id",
+    "{kernel_id}",
+    "--port-range",
+    "{port_range}",
+    "--response-address",
+    "{response_address}",
+    "--public-key",
+    "{public_key}",
+    "--spark-context-initialization-mode",
+    "lazy",
+    "--kernel-class-name",
+    "ipykernel.ipkernel.IPythonKernel"
+  ],
+  "env": {
+    "SPARK_HOME": "/opt/spark",
+    "PYSPARK_PYTHON": "/opt/miniconda3/envs/provisioners/bin/python",
+    "PYTHONPATH": "${HOME}/.local/lib/python3.7/site-packages:/opt/spark/python",
+    "SPARK_OPTS": "--master yarn --deploy-mode cluster --name ${KERNEL_ID:-ERROR__NO__KERNEL_ID} --conf spark.yarn.submit.waitAppCompletion=false --conf spark.yarn.appMasterEnv.PYTHONUSERBASE=/home/${KERNEL_USERNAME}/.local --conf spark.yarn.appMasterEnv.PYTHONPATH=${HOME}/.local/lib/python3.7/site-packages:/opt/spark/python --conf spark.yarn.appMasterEnv.PATH=/opt/miniconda3/envs/provisioners/bin:$PATH  ${KERNEL_EXTRA_SPARK_OPTS}",
+    "LAUNCH_OPTS": ""
+  },
+  "display_name": "Spark Python (YARN Cluster)",
+  "language": "python",
+  "interrupt_mode": "signal",
+  "metadata": {
+    "kernel_provisioner": {
+      "provisioner_name": "yarn-provisioner",
+      "config": {
+        "launch_timeout": 30
+      }
+    }
+  }
+}
+```
+
+The `metadata` and `argv` entries for each kernel specification should be nearly identical and
+not require changes. You will need to adjust the `env` entries to apply to your specific
+configuration.
+
+You should also check the same kinds of environment and path settings in the corresponding
+`bin/run.sh` file - although changes are not typically necessary.
+
+### Command-line Options
+
+The following is produced using `jupyter yarn-spec install --help` and displays the complete set of command-line
+options:
+
+```text
+Creates a Jupyter kernel specification for use within a Hadoop Yarn cluster.
+
+Options
+=======
+The options below are convenience aliases to configurable class-options,
+as listed in the "Equivalent to" description-line of the aliases.
+To see all configurable class-options for some <cmd>, use:
+    <cmd> --help-all
+
+--dask
+    Install kernelspec for Dask in Yarn cluster.
+    Equivalent to: [--YarnSpecInstaller.dask=True]
+--yarn-endpoint-security-enabled
+    Install kernelspec where Yarn API endpoint has security enabled.
+    Equivalent to: [--YarnSpecInstaller.yarn_endpoint_security_enabled=True]
+--impersonation-enabled
+    Install kernelspec to impersonate user (requires root privileges).
+    Equivalent to: [--YarnSpecInstaller.impersonation_enabled=True]
+--user
+    Install to the per-user kernel registry
+    Equivalent to: [--BaseSpecApp.user=True]
+--sys-prefix
+    Install to Python's sys.prefix. Useful in conda/virtual environments.
+    Equivalent to: [--BaseSpecApp.prefix=/opt/miniconda3/envs/provisioners]
+--spark
+    Install kernelspec with Spark support.
+    Equivalent to: [--BaseSpecApp.spark=True]
+--debug
+    set log level to logging.DEBUG (maximize logging output)
+    Equivalent to: [--Application.log_level=10]
+--yarn-endpoint=<Unicode>
+    The http url specifying the YARN Resource Manager. Note: If this value is
+    NOT set, the YARN library will use the files within the local
+    HADOOP_CONFIG_DIR to determine the active resource manager.
+    (GP_YARN_ENDPOINT env var)
+    Default: None
+    Equivalent to: [--YarnSpecInstaller.yarn_endpoint]
+--alt-yarn-endpoint=<Unicode>
+    The http url specifying the alternate YARN Resource Manager.  This value
+    should be set when YARN Resource Managers are configured for high
+    availability.  Note: If both YARN endpoints are NOT set, the YARN library
+    will use the files within the local HADOOP_CONFIG_DIR to determine the
+    active resource manager. (GP_ALT_YARN_ENDPOINT env var)
+    Default: None
+    Equivalent to: [--YarnSpecInstaller.alt_yarn_endpoint]
+--python-root=<Unicode>
+    Specify where the root of the python installation resides (parent dir of
+    bin/python).
+    Default: '/opt/miniconda3/envs/provisioners'
+    Equivalent to: [--YarnSpecInstaller.python_root]
+--extra-dask-opts=<Unicode>
+    Specify additional Dask options.
+    Default: ''
+    Equivalent to: [--YarnSpecInstaller.extra_dask_opts]
+--prefix=<Unicode>
+    Specify a prefix to install to, e.g. an env. The kernelspec will be
+    installed in PREFIX/share/jupyter/kernels/
+    Default: ''
+    Equivalent to: [--BaseSpecApp.prefix]
+--kernel-name=<Unicode>
+    Install the kernel spec into a directory with this name.
+    Default: ''
+    Equivalent to: [--BaseSpecApp.kernel_name]
+--display-name=<Unicode>
+    The display name of the kernel - used by user-facing applications.
+    Default: ''
+    Equivalent to: [--BaseSpecApp.display_name]
+--language=<Unicode>
+    The language of the kernel referenced in the kernel specification.  Must be one of
+        'Python', 'R', or 'Scala'.  Default = 'Python'.
+    Default: 'Python'
+    Equivalent to: [--BaseSpecApp.language]
+--spark-home=<Unicode>
+    Specify where the spark files can be found.
+    Default: '/opt/spark'
+    Equivalent to: [--BaseSpecApp.spark_home]
+--spark-init-mode=<Unicode>
+    Spark context initialization mode.  Must be one of ['lazy', 'eager', 'none'].
+        Default = lazy.
+    Default: 'lazy'
+    Equivalent to: [--BaseSpecApp.spark_init_mode]
+--extra-spark-opts=<Unicode>
+    Specify additional Spark options.
+    Default: ''
+    Equivalent to: [--BaseSpecApp.extra_spark_opts]
+--authorized-users=<set-item-1>...
+    List of user names against which KERNEL_USERNAME will be compared. Any match
+    (case-sensitive) will allow the kernel's launch, otherwise an HTTP 403
+    (Forbidden) error will be raised.  The set of unauthorized users takes
+    precedence. This option should be used carefully as it can dramatically
+    limit who can launch kernels. To specify multiple names via the CLI,
+    separate options must be provided for each entry. (GP_AUTHORIZED_USERS env
+    var - non-bracketed, just comma-separated)
+    Default: set()
+    Equivalent to: [--BaseSpecApp.authorized_users]
+--unauthorized-users=<set-item-1>...
+    List of user names against which KERNEL_USERNAME will be compared. Any match
+    (case-sensitive) will prevent the kernel's launch and result in an HTTP 403
+    (Forbidden) error. To specify multiple names via the CLI, separate options
+    must be provided for each entry. (GP_UNAUTHORIZED_USERS env var - non-
+    bracketed, just comma-separated)
+    Default: {'root'}
+    Equivalent to: [--BaseSpecApp.unauthorized_users]
+--port-range=<Unicode>
+    Specifies the lower and upper port numbers from which ports are created. The
+    bounded values are separated by '..' (e.g., 33245..34245 specifies a range
+    of 1000 ports to be randomly selected). A range of zero (e.g., 33245..33245
+    or 0..0) disables port-range enforcement.  (GP_PORT_RANGE env var)
+    Default: '0..0'
+    Equivalent to: [--BaseSpecApp.port_range]
+--launch-timeout=<Int>
+    Number of ports to try if the specified port is not available
+    (GP_LAUNCH_TIMEOUT env var)
+    Default: 30
+    Equivalent to: [--BaseSpecApp.launch_timeout]
+--ipykernel-subclass-name=<Unicode>
+    For Python kernels, the name of the ipykernel subclass.
+    Default: 'ipykernel.ipkernel.IPythonKernel'
+    Equivalent to: [--BaseSpecApp.ipykernel_subclass_name]
+--log-level=<Enum>
+    Set the log level by value or name.
+    Choices: any of [0, 10, 20, 30, 40, 50, 'DEBUG', 'INFO', 'WARN', 'ERROR', 'CRITICAL']
+    Default: 30
+    Equivalent to: [--Application.log_level]
+--config=<Unicode>
+    Full path of a config file.
+    Default: ''
+    Equivalent to: [--JupyterApp.config_file]
+
+Examples
+--------
 
-Scenario: **Running Jupyter Enterprise Gateway on OpenShift Kubernetes Environment fails trying to create /home/jovyan/.local**
+    jupyter-yarn-spec install --language=R --spark-home=/usr/local/spark
 
-As described [in the OpenShift Admin Guide](https://docs.openshift.com/container-platform/4.10/openshift_images/create-images.html)
-there is a need to issue the following command to enable running with `USER` in Dockerfile.
+    jupyter-yarn-spec install --kernel-name=dask_python --dask --yarn-endpoint=http://foo.bar:8088/ws/v1/cluster
 
-```bash
-oc adm policy add-scc-to-group anyuid system:authenticated
-```
-
-## Opening an issue
+    jupyter-yarn-spec install --language=Scala --spark-init-mode eager
 
-Scenario: **None of the scenarios on this page match or resolve my issue, what do I do next?**
-
-If you are unable to resolve your issue, take a look at our
-[open issues list](https://github.com/jupyter-server/enterprise_gateway/issues) to see if there is an applicable scenario
-already reported. If found, please add a comment to the issue so that we can get a sense of urgency (although all
-issues are important to us). If not found, please provide the following information if possible in a **new issue**.
-
-1. Describe the issue in as much detail as possible. This should include configuration information about your environment.
-1. Gather and _attach_ the following files to the issue. If possible, please archive the files first.
-   1. The **complete** Enterprise Gateway log file. If possible, please enable `DEBUG` logging that encompasses
-      the issue.
-   1. The log file(s) produced from the corresponding kernel. This is primarily a function of the underlying resource
-      manager.
-      - For containerized installations like Kubernetes or Docker Swarm, kernel log output can be captured by
-        running the appropriate `logs` command against the pod or container, respectively. The names of the
-        corresponding pod/container can be found in the Enterprise Gateway log.
-      - For `Hadoop YARN` environments,
-        you'll need to navigate to the appropriate log directory relative the application ID associated with the kernel.
-        The application ID can be located in the Enterprise Gateway log. If you have access to an administrative console,
-        you can usually navigate to the application logs more easily.
-   1. Although unlikely, the notebook log may also be helpful. If we find that the issue is more client-side
-      related, we may ask for `DEBUG` logging there as well.
-1. If you have altered or created new kernel specifications, the files corresponding to the failing kernels would be
-   helpful. These files could also be added to the attached archive or attached separately.
-
-Please know that we understand that some information cannot be provided due to its sensitivity. In such cases, just
-let us know and we'll be happy to approach the resolution of your issue from a different angle.
+To see all available configurables, use `--help-all`.
+```
```

### Comparing `gateway_provisioners-0.1.0/docs/source/users/kernel-envs.md` & `gateway_provisioners-0.2.0/docs/source/users/kernel-envs.md`

 * *Files 8% similar despite different names*

```diff
@@ -11,120 +11,120 @@
 others can be sent to customize behaviors. The following kernel-specific environment variables are recognized
 and used by the appropriate gateway provisioners. As mentioned above, all `KERNEL_` variables submitted
 in the kernel startup request's JSON body will be available to the kernel for its launch.
 
 ```text
   KERNEL_GID=<from user> or 100
     Container-based provisioners only. This value represents the group id in which the container
-    will run. The default value is 100 representing the users group - which is how all kernel
-    images produced by Enterprise Gateway are built.  See also KERNEL_UID.
-    Kubernetes: Warning - If KERNEL_GID is set it is strongly recommened that feature-gate
+    will run. The default value is 100 representing the users group - which is the default group ID
+    when building images from within the Gateway Provisioners project.  See also KERNEL_UID.
+    Kubernetes: Warning - If KERNEL_GID is set it is strongly recommended that feature-gate
     RunAsGroup be enabled, otherwise, this value will be ignored and the pod will run as
     the root group id.  As a result, the setting of this value into the Security Context
     of the kernel pod is commented out in the kernel-pod.yaml file and must be enabled
     by the administrator.
     Docker: Warning - This value is only added to the supplemental group ids.  As a result,
     if used with KERNEL_UID, the resulting container will run as the root group with this
     value listed in its supplemental groups.
 
-  KERNEL_EXECUTOR_IMAGE=<from kernel.json process-proxy stanza> or KERNEL_IMAGE
-    Kubernetees w/ Spark provisioners only. This indicates the image that Spark on Kubernetes
-    will use for the its executors.  Although this value could come from the user, its strongly
-    recommended that the process-proxy stanza of the corresponding kernel's kernelspec
+  KERNEL_EXECUTOR_IMAGE=<from kernel.json kernel-provisioner stanza> or KERNEL_IMAGE
+    Kubernetees w/ Spark provisioners only. This indicates the image that Spark-based Kubernetes
+    deployments will use for its executors.  Although this value could come from the user, its strongly
+    recommended that the kernel-provisioner stanza of the corresponding kernel's kernelspec
     (kernel.json) file be updated to include the image name.  If no image name is
     provided, the value of KERNEL_IMAGE will be used.
 
   KERNEL_EXTRA_SPARK_OPTS=<from user>
     Spark-based provisioners only. This variable allows users to add additional spark options
     to the current set of options specified in the corresponding kernel.json file.  This
     variable is purely optional with no default value.  In addition, it is the responsibility
     of the user setting this value to ensure the options passed are appropriate relative to
     the target environment.  Because this variable contains space-separate values, it requires
     appropriate quotation.  For example, to use with the notebook docker image
-    jupyterhub/k8s-singleuser-sample , the environment variable would look something like this:
+    jupyterhub/k8s-singleuser-sample, the environment variable would look something like this:
 
     docker run ... -e KERNEL_EXTRA_SPARK_OPTS=\"--conf spark.driver.memory=2g
     --conf spark.executor.memory=2g\" ... jupyterhub/k8s-singleuser-sample
 
   KERNEL_ID=<from user> or <system generated>
     This value represents the identifier used by the Jupyter framework to identify
     the kernel.  Although this value could be provided by the user, it is recommended
     that it be generated by the system.
 
-  KERNEL_IMAGE=<from user> or <from kernel.json process-proxy stanza>
+  KERNEL_IMAGE=<from user> or <from kernel.json kernel-provisioner stanza>
     Container-based provisioners only. This indicates the image to use for the kernel in
     containerized environments - Kubernetes or Docker.  Although it can be provided by the
-    user, it is strongly recommended that the process-proxy stanza of the corresponding
+    user, it is strongly recommended that the kernel-provisioner stanza of the corresponding
     kernel's kernelspec (kernel.json) file be updated to include the image name.
 
-  KERNEL_LAUNCH_TIMEOUT=<from user> or EG_KERNEL_LAUNCH_TIMEOUT
+  KERNEL_LAUNCH_TIMEOUT=<from user> or GP_KERNEL_LAUNCH_TIMEOUT
     Indicates the time (in seconds) to allow for a kernel's launch.  This value should
     be submitted in the kernel startup if that particular kernel's startup time is
-    expected to exceed that of the EG_KERNEL_LAUNCH_TIMEOUT set when Enterprise
-    Gateway starts.
+    expected to exceed that of the GP_KERNEL_LAUNCH_TIMEOUT set when Gateway Provisioner's
+    hosting application starts.
 
-  KERNEL_NAMESPACE=<from user> or KERNEL_POD_NAME or EG_NAMESPACE
+  KERNEL_NAMESPACE=<from user> or KERNEL_POD_NAME or GP_NAMESPACE
     Kubernetes provisioners only.  This indicates the name of the namespace to use or
     create on Kubernetes in which the kernel pod will be located.  For users wishing to
-    use a pre-created namespace, this value should be submitted in the kernel startup
-    request.  In such cases, the user must also provide KERNEL_SERVICE_ACCOUNT_NAME.
-    If not provided, Enterprise Gateway will create a new namespace for the kernel
-    whose value is derived from KERNEL_POD_NAME.  In rare cases where
-    EG_SHARED_NAMESPACE is True, this value will be set to the value of EG_NAMESPACE.
+    use a pre-created namespace, this value should be submitted in the env stanza of
+    the kernel startup request.  In such cases, the user must also provide KERNEL_SERVICE_ACCOUNT_NAME.
+    If not provided, and GP_SHARED_NAMESPACE is False, Gateway Provisioners will attempt to
+    create a new namespace for the kernel whose value is derived from KERNEL_POD_NAME.  When
+    GP_SHARED_NAMESPACE is True (the default value in Gateway Provisioners), this value will
+    be set to the value of GP_NAMESPACE.
 
-    Note that if the namespace is created by Enterprise Gateway, it will be removed
-    upon the kernel's termination.  Otherwise, the Enterprise Gateway will not
+    Note that if the namespace is created by Gateway Provisioners, it will be removed
+    upon the kernel's termination.  Otherwise, the Gateway Provisioners will not
     remove the namespace.
 
   KERNEL_POD_NAME=<from user> or KERNEL_USERNAME-KERNEL_ID
-    Kubernetes provisioners only. By default, Enterprise Gateway will use a kernel
+    Kubernetes provisioners only. By default, Gateway Provisioners will use a kernel
     pod name whose value is derived from KERNEL_USERNAME and KERNEL_ID separated by
     a hyphen ('-').  This variable is typically NOT provided by the user, but, in
-    such cases, Enterprise Gateway will honor that value.  However, when provided,
+    such cases, Gateway Provisioners will honor that value.  However, when provided,
     it is the user's responsibility that KERNEL_POD_NAME is unique relative to
     any pods in the target namespace.  In addition, the pod must NOT exist -
     unlike the case if KERNEL_NAMESPACE is provided.
 
   KERNEL_REMOTE_HOST=<remote host name>
     Distributed provisioner only.  When specified, this value will override the
     configured load-balancing algorithm.
 
-  KERNEL_SERVICE_ACCOUNT_NAME=<from user> or EG_DEFAULT_KERNEL_SERVICE_ACCOUNT_NAME
+  KERNEL_SERVICE_ACCOUNT_NAME=<from user> or GP_DEFAULT_KERNEL_SERVICE_ACCOUNT_NAME
     Kubernetes provisioners only.  This value represents the name of the service account
-    that Enterprise Gateway should equate with the kernel pod.  If Enterprise Gateway
+    that Gateway Provisioners should equate with the kernel pod.  If Gateway Provisioners
     creates the kernel's namespace, it will be associated with the cluster role
-    identified by EG_KERNEL_CLUSTER_ROLE.  If not provided, it will be derived
-    from EG_DEFAULT_KERNEL_SERVICE_ACCOUNT_NAME.
+    identified by GP_KERNEL_CLUSTER_ROLE.  If not provided, it will be derived
+    from GP_DEFAULT_KERNEL_SERVICE_ACCOUNT_NAME.
 
   KERNEL_SPARKAPP_CONFIG_MAP=<from user> or None
     SparkOperator provisioner only. The name of a Kubernetes ConfigMap which will be used to
-    configure the SparkApplication. See the SparkApplicationSpec
-    (https://googlecloudplatform.github.io/spark-on-k8s-operator/docs/api-docs.html#sparkoperator.k8s.io/v1beta2.SparkApplicationSpec)
-    sparkConfigMap for more information.
+    configure the SparkApplication. This value is used to set the `sparkConfigMap` property
+    in the spark operator's yaml template during launch.
 
   KERNEL_UID=<from user> or 1000
     Container-based provisioners only. This value represents the user id in which the container
-    will run. The default value is 1000 representing the jovyan user - which is how all kernel
-    images produced by Enterprise Gateway are built.  See also KERNEL_GID.
-    Kubernetes: Warning - If KERNEL_UID is set it is strongly recommened that feature-gate
+    will run. The default value is 1000 representing the jovyan user - which is the default user ID
+    when building images from within the Gateway Provisioners project.  See also KERNEL_GID.
+    Kubernetes: Warning - If KERNEL_UID is set it is strongly recommended that feature-gate
     RunAsGroup be enabled and KERNEL_GID also be set, otherwise, the pod will run as
     the root group id. As a result, the setting of this value into the Security Context
     of the kernel pod is commented out in the kernel-pod.yaml file and must be enabled
     by the administrator.
 
-  KERNEL_USERNAME=<from user> or <enterprise-gateway-user>
+  KERNEL_USERNAME=<from user> or <gateway-provisioner-hosting-application-user>
     This value represents the logical name of the user submitting the request to
     start the kernel. Of all the KERNEL_ variables, KERNEL_USERNAME is the one that
     should be submitted in the request. In environments in which impersonation is
     used it represents the target of the impersonation.
 
   KERNEL_WORKING_DIR=<from user> or None
     Container-based provisioners only.  This value should model the directory in which the
     active notebook file is running.   It is intended to be used in conjunction with
     appropriate volume mounts in the kernel container such that the user's notebook
     filesystem exists in the container and enables the sharing of resources used within
     the notebook. As a result, the primary use case for this is for Jupyter Hub users running
-    in Kubernetes.  When a value is provided and EG_MIRROR_WORKING_DIRS=True, Enterprise
-    Gateway will set the container's working directory to the value specified in
-    KERNEL_WORKING_DIR.  If EG_MIRROR_WORKING_DIRS is False, KERNEL_WORKING_DIR will
-    not be available for use during the kernel's launch.  See also EG_MIRROR_WORKING_DIRS.
+    in Kubernetes.  When a value is provided and GP_MIRROR_WORKING_DIRS=True, Gateway
+    Provisioners will set the container's working directory to the value specified in
+    KERNEL_WORKING_DIR.  If GP_MIRROR_WORKING_DIRS is False, KERNEL_WORKING_DIR will
+    not be available for use during the kernel's launch.  See also GP_MIRROR_WORKING_DIRS.
 ```
```

### Comparing `gateway_provisioners-0.1.0/gateway_provisioners/_version.py` & `gateway_provisioners-0.2.0/gateway_provisioners/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright (c) Jupyter Development Team.
 # Distributed under the terms of the Modified BSD License.
 import re
 from typing import List
 
 # Version string must appear intact for automatic versioning
-__version__ = "0.1.0"
+__version__ = "0.2.0"
 
 # Build up version_info tuple for backwards compatibility
 pattern = r"(?P<major>\d+).(?P<minor>\d+).(?P<patch>\d+)(?P<rest>.*)"
 match = re.match(pattern, __version__)
 assert match is not None
 parts: List[object] = [int(match[part]) for part in ["major", "minor", "patch"]]
 if match["rest"]:
```

### Comparing `gateway_provisioners-0.1.0/gateway_provisioners/config_mixin.py` & `gateway_provisioners-0.2.0/gateway_provisioners/config_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 max_poll_attempts = int(os.getenv("GP_MAX_POLL_ATTEMPTS", "10"))
 poll_interval = float(os.getenv("GP_POLL_INTERVAL", "0.5"))
 socket_timeout = float(os.getenv("GP_SOCKET_TIMEOUT", "0.01"))
 ssh_port = int(os.getenv("GP_SSH_PORT", "22"))
 
 
 class RemoteProvisionerConfigMixin(Configurable):
-
     _log_formatter_cls = LogFormatter  # traitlet default is LevelFormatter
 
     @default("log_format")
     def _default_log_format(self):
         """override default log format to include milliseconds"""
         return (
             "%(color)s[%(levelname)1.1s %(asctime)s.%(msecs).03d %(name)s]%(end_color)s %(message)s"
```

### Comparing `gateway_provisioners-0.1.0/gateway_provisioners/container.py` & `gateway_provisioners-0.2.0/gateway_provisioners/container.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,28 +34,28 @@
 
     image_name_env = "GP_IMAGE_NAME"
     image_name = Unicode(
         None,
         config=True,
         allow_none=True,
         help="""The image name to use when launching container-based kernels.
-                              (GP_IMAGE_NAME env var)""",
+(GP_IMAGE_NAME env var)""",
     )
 
     @default("image_name")
     def _image_name_default(self):
         return os.getenv(self.image_name_env)
 
     executor_image_name_env = "GP_EXECUTOR_IMAGE_NAME"
     executor_image_name = Unicode(
         None,
         config=True,
         allow_none=True,
         help="""The image name to use as the Spark executor image when launching
-                               container-based kernels within Spark environments. (GP_EXECUTOR_IMAGE_NAME env var)""",
+container-based kernels within Spark environments. (GP_EXECUTOR_IMAGE_NAME env var)""",
     )
 
     @default("executor_image_name")
     def _executor_image_name_default(self):
         return os.getenv(self.executor_image_name_env) or self.image_name
 
     def __init__(self, **kwargs):
@@ -126,15 +126,15 @@
         So will regard the container as active when no status is available or one of the initial
         phases.
         Returns None if the container cannot be found or its in an initial state. Otherwise,
         return an exit code of 0.
         """
         result = 0
 
-        container_status = await self.get_container_status(None)
+        container_status = self.get_container_status(None)
         # Do not check whether container_status is None
         # EG couldn't restart kernels although connections exists.
         # See https://github.com/jupyter/enterprise_gateway/issues/827
         if container_status in self.get_initial_states():
             result = None
 
         return result
@@ -153,15 +153,15 @@
 
     @overrides
     async def kill(self, restart: bool = False) -> None:
         """Kills a containerized kernel."""
         result = None
 
         if self.container_name:  # We only have something to terminate if we have a name
-            result = await self.terminate_container_resources(restart=restart)
+            result = self.terminate_container_resources(restart=restart)
 
         return result
 
     @overrides
     async def terminate(self, restart: bool = False) -> None:
         """Terminates a containerized kernel.
 
@@ -170,34 +170,39 @@
         """
         return await self.kill(restart=restart)
 
     @overrides
     async def shutdown_listener(self, restart: bool) -> None:
         await super().shutdown_listener(restart)
         if self.container_name:  # We only have something to terminate if we have a name
-            await self.terminate_container_resources(restart)
+            self.terminate_container_resources(restart)
 
     @overrides
     async def confirm_remote_startup(self):
         """Confirms the container has started and returned necessary connection information."""
+        self.log.debug("Trying to confirm kernel container startup status")
         self.start_time = RemoteProvisionerBase.get_current_time()
         i = 0
         ready_to_connect = False  # we're ready to connect when we have a connection file to use
         while not ready_to_connect:
             i += 1
             await self.handle_launch_timeout()
 
-            container_status = await self.get_container_status(str(i))
+            container_status = self.get_container_status(str(i))
             if container_status:
-                if self.assigned_host != "":
-                    ready_to_connect = await self.receive_connection_info()
-                    self.pid = (
-                        0  # We won't send the process signals from container-based provisioners
-                    )
-                    self.pgid = 0
+                if container_status in self.get_error_states():
+                    reason = f"Error starting kernel container; status: '{container_status}'.  Check server logs."
+                    self.log_and_raise(RuntimeError(reason))
+                else:
+                    if self.assigned_host != "":
+                        ready_to_connect = await self.receive_connection_info()
+                        self.pid = (
+                            0  # We won't send the process signals from container-based provisioners
+                        )
+                        self.pgid = 0
             else:
                 self.detect_launch_failure()
 
     @overrides
     async def get_provisioner_info(self) -> Dict[str, Any]:
         """Captures the base information necessary for kernel persistence relative to containers."""
         provisioner_info = await super().get_provisioner_info()
@@ -212,19 +217,24 @@
     async def load_provisioner_info(self, provisioner_info: dict) -> None:
         """Loads the base information necessary for kernel persistence relative to containers."""
         await super().load_provisioner_info(provisioner_info)
         self.assigned_node_ip = provisioner_info.get("assigned_node_ip")
 
     @abstractmethod
     def get_initial_states(self) -> Set[str]:
-        """Return list of states indicating container is starting (includes running)."""
+        """Return list of states (in lowercase) indicating container is starting (includes running)."""
         raise NotImplementedError
 
     @abstractmethod
-    async def get_container_status(self, iteration: Optional[str]) -> str:
+    def get_error_states(self) -> Set[str]:
+        """Returns the list of error states (in lowercase)."""
+        raise NotImplementedError
+
+    @abstractmethod
+    def get_container_status(self, iteration: Optional[str]) -> str:
         """Return current container state."""
         raise NotImplementedError
 
     @abstractmethod
-    async def terminate_container_resources(self, restart: bool = False) -> Optional[bool]:
+    def terminate_container_resources(self, restart: bool = False) -> Optional[bool]:
         """Terminate any artifacts created on behalf of the container's lifetime."""
         raise NotImplementedError
```

### Comparing `gateway_provisioners-0.1.0/gateway_provisioners/distributed.py` & `gateway_provisioners-0.2.0/gateway_provisioners/distributed.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,30 +72,28 @@
 
     remote_hosts_env = "GP_REMOTE_HOSTS"
     remote_hosts_default_value = "localhost"
     remote_hosts = List(
         default_value=[remote_hosts_default_value],
         config=True,
         help="""List of host names on which this kernel can be launched.  Multiple entries must
-                        each be specified via separate options: --remote-hosts host1 --remote-hosts host2""",
+each be specified via separate options: --remote-hosts host1 --remote-hosts host2""",
     )
 
     @default("remote_hosts")
     def _remote_hosts_default(self):
         return os.getenv(self.remote_hosts_env, self.remote_hosts_default_value).split(",")
 
     load_balancing_algorithm_env = "GP_LOAD_BALANCING_ALGORITHM"
     load_balancing_algorithm_default_value = "round-robin"
     load_balancing_algorithm = Unicode(
         load_balancing_algorithm_default_value,
         config=True,
         help="""Specifies which load balancing algorithm DistributedProvisioner should use.
-            Must be one of "round-robin" or "least-connection".  (GP_LOAD_BALANCING_ALGORITHM
-            env var)
-            """,
+Must be one of "round-robin" or "least-connection".  (GP_LOAD_BALANCING_ALGORITHM env var)""",
     )
 
     @default("load_balancing_algorithm")
     def _load_balancing_algorithm_default(self) -> str:
         return os.getenv(
             self.load_balancing_algorithm_env,
             self.load_balancing_algorithm_default_value,
@@ -120,15 +118,16 @@
         self.remote_pwd = os.getenv("GP_REMOTE_PWD")
         self.use_gss = os.getenv("GP_REMOTE_GSS_SSH", "False").lower() == "true"
         if self.use_gss:
             if self.remote_pwd or _remote_user:
                 warnings.warn(
                     "Both `GP_REMOTE_GSS_SSH` and one of `GP_REMOTE_PWD` or `GP_REMOTE_USER` is set. "
                     "Those options are mutually exclusive, you configuration may be incorrect. "
-                    "GP_REMOTE_GSS_SSH will take priority."
+                    "GP_REMOTE_GSS_SSH will take priority.",
+                    stacklevel=2,
                 )
             self.remote_user = None
         else:
             self.remote_user = _remote_user if _remote_user else getpass.getuser()
 
     @property
     @overrides
```

### Comparing `gateway_provisioners-0.1.0/gateway_provisioners/docker_swarm.py` & `gateway_provisioners-0.2.0/gateway_provisioners/docker_swarm.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,25 +47,29 @@
         return kwargs
 
     @overrides
     def get_initial_states(self) -> Set[str]:
         return {"preparing", "starting", "running"}
 
     @overrides
-    async def get_container_status(self, iteration: Optional[str]) -> str:
+    def get_error_states(self) -> Set[str]:
+        return {"failed", "rejected", "complete", "shutdown", "orphaned", "remove"}
+
+    @overrides
+    def get_container_status(self, iteration: Optional[str]) -> str:
         # Locates the kernel container using the kernel_id filter.  If the status indicates an initial state we
         # should be able to get at the NetworksAttachments and determine the associated container's IP address.
-        task_state = None
+        task_state = ""
         task_id = None
         task = self._get_task()
         if task:
             task_status = task["Status"]
             task_id = task["ID"]
             if task_status:
-                task_state = task_status["State"]
+                task_state = task_status["State"].lower()
                 if (
                     self.assigned_host == "" and task_state == "running"
                 ):  # in self.get_initial_states():
                     # get the NetworkAttachments and pick out the first of the Network and first
                     networks_attachments = task["NetworksAttachments"]
                     if len(networks_attachments) > 0:
                         address = networks_attachments[0]["Addresses"][0]
@@ -79,15 +83,15 @@
                 f"Name: '{self.container_name}', Status: '{task_state}', "
                 f"IPAddress: '{self.assigned_ip}', KernelID: '{self.kernel_id}', "
                 f"TaskID: '{task_id}'"
             )
         return task_state
 
     @overrides
-    async def terminate_container_resources(self, restart: bool = False) -> Optional[bool]:
+    def terminate_container_resources(self, restart: bool = False) -> Optional[bool]:
         # Remove the docker service.
 
         result = True  # We'll be optimistic
         service = self._get_service()
         if service:
             try:
                 service.remove()  # Service still exists, attempt removal
@@ -173,24 +177,28 @@
         return kwargs
 
     @overrides
     def get_initial_states(self) -> Set[str]:
         return {"created", "running"}
 
     @overrides
-    async def get_container_status(self, iteration: Optional[str]) -> str:
+    def get_error_states(self) -> Set[str]:
+        return {"restarting", "paused", "exited", "dead"}
+
+    @overrides
+    def get_container_status(self, iteration: Optional[str]) -> str:
         # Locates the kernel container using the kernel_id filter.  If the phase indicates Running, the pod's IP
         # is used for the assigned_ip.  Only used when docker mode == regular (non swarm)
-        container_status = None
+        container_status = ""
 
         container = self._get_container()
         if container:
             self.container_name = container.name
             if container.status:
-                container_status = container.status
+                container_status = container.status.lower()
                 if container_status == "running" and self.assigned_host == "":
                     # Container is running, capture IP
 
                     # we'll use this as a fallback in case we don't find our network
                     self.assigned_ip = container.attrs.get("NetworkSettings").get("IPAddress")
                     networks = container.attrs.get("NetworkSettings").get("Networks")
                     if len(networks) > 0:
@@ -212,24 +220,23 @@
                 f"Name: '{self.container_name}', Status: '{container_status}', "
                 f"IPAddress: '{self.assigned_ip}', KernelID: '{self.kernel_id}'"
             )
 
         return container_status
 
     @overrides
-    async def terminate_container_resources(self, restart: bool = False) -> None:
+    def terminate_container_resources(self, restart: bool = False) -> None:
         # Remove the container
 
         result = True  # Since we run containers with remove=True, we'll be optimistic
         container = self._get_container()
         if container:
             try:
                 container.remove(force=True)  # Container still exists, attempt forced removal
             except Exception as err:
-
                 self.log.debug(
                     f"Container termination for container: {container.name} raised exception: {err}"
                 )
                 if isinstance(err, NotFound):
                     pass  # okay if its not found
                 else:
                     result = False
```

### Comparing `gateway_provisioners-0.1.0/gateway_provisioners/k8s.py` & `gateway_provisioners-0.2.0/gateway_provisioners/k8s.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (c) Jupyter Development Team.
 # Distributed under the terms of the Modified BSD License.
 """Code related to managing kernels running in Kubernetes clusters."""
 
 import logging
 import os
 import re
-from typing import Any, Dict, Optional, Set
+from typing import Any, Dict, List, Optional, Set
 
 import urllib3
 from overrides import overrides
 
 try:
     from jinja2 import Environment  # noqa - used by launcher so check presence here
     from kubernetes import client, config
@@ -24,27 +24,27 @@
 
 
 from .container import ContainerProvisionerBase
 
 urllib3.disable_warnings()
 
 # Default logging level of kubernetes produces too much noise - raise to warning only.
-logging.getLogger("kubernetes").setLevel(os.environ.get("EG_KUBERNETES_LOG_LEVEL", logging.WARNING))
+logging.getLogger("kubernetes").setLevel(os.environ.get("GP_KUBERNETES_LOG_LEVEL", logging.WARNING))
 
 k8s_provisioner_namespace = os.environ.get("GP_NAMESPACE", "default")
 default_kernel_service_account_name = os.environ.get(
     "GP_DEFAULT_KERNEL_SERVICE_ACCOUNT_NAME", "default"
 )
 kernel_cluster_role = os.environ.get("GP_KERNEL_CLUSTER_ROLE", "cluster-admin")
 
-# Since provisioners are a single-user scenario (not going through EG), use a shared namespace.
+# Since provisioners are a single-user scenario (not going through EG), use a shared namespace by default.
 shared_namespace = bool(os.environ.get("GP_SHARED_NAMESPACE", "True").lower() == "true")
 kpt_dir = os.environ.get("GP_POD_TEMPLATE_DIR", "/tmp")  # noqa: S108
 
-app_name = os.environ.get("GP_APP_NAME", "k8s-provisioner")
+app_name = os.environ.get("GP_APP_NAME", "gateway-provisioners")
 
 if (
     "SPHINX_BUILD_IN_PROGRESS" not in os.environ
     and "PYTEST_CURRENT_TEST" not in os.environ
     and "PYTEST_RUN_CONFIG" not in os.environ
 ):
     if bool(os.environ.get("GP_USE_INCLUSTER_CONFIG", "True").lower() == "true"):
@@ -52,38 +52,45 @@
     else:
         config.load_kube_config()
 
 
 class KubernetesProvisioner(ContainerProvisionerBase):
     """Kernel lifecycle management for Kubernetes kernels."""
 
+    # Identifies the kind of object being managed by this provisioner.
+    # For these values we will prefer the values found in the 'kind' field
+    # of the object's metadata.  This attribute is strictly used to provide
+    # context to log messages.
+    object_kind = "Pod"
+
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
         self.kernel_pod_name = None
         self.kernel_namespace = None
         self.delete_kernel_namespace = False
         # Track if we're restarting the pod from this instance.  This will be
         # set to true when restarting kernels during the original pod's termination
         # and if the kernel resides in its own namespace.
         self.restarting = False
 
     @overrides
     async def pre_launch(self, **kwargs: Any) -> Dict[str, Any]:
-        # Set env before superclass call so we see these in the debug output
+        # Set env before superclass call, so we can see these in the debug output
 
-        # Kubernetes relies on many internal env variables.  Since we're running in a k8s pod, we will
-        # transfer its env to each launched kernel.
-        kwargs["env"] = dict(os.environ, **kwargs.get("env", {}))
+        # Kubernetes relies on internal env variables to determine its configuration.  When
+        # running within a K8s cluster, these start with KUBERNETES_SERVICE, otherwise look
+        # for envs prefixed with KUBECONFIG.
+        for key in os.environ:
+            if key.startswith("KUBECONFIG") or key.startswith("KUBERNETES_SERVICE"):
+                kwargs["env"][key] = os.environ[key]
         kwargs = await super().pre_launch(**kwargs)
-        # These must follow call to super() so that kernel_username is established
+        # Determine pod name and namespace - creating the latter if necessary
         self.kernel_pod_name = self._determine_kernel_pod_name(**kwargs)
-        self.kernel_namespace = self._determine_kernel_namespace(
-            **kwargs
-        )  # will create namespace if not provided
+        self.kernel_namespace = self._determine_kernel_namespace(**kwargs)
         return kwargs
 
     @overrides
     async def get_provisioner_info(self) -> Dict[str, Any]:
         provisioner_info = await super().get_provisioner_info()
         provisioner_info.update(
             {
@@ -97,32 +104,36 @@
     async def load_provisioner_info(self, provisioner_info: dict) -> None:
         await super().load_provisioner_info(provisioner_info)
         self.kernel_namespace = provisioner_info["kernel_ns"]
         self.delete_kernel_namespace = provisioner_info["delete_ns"]
 
     @overrides
     def get_initial_states(self) -> Set[str]:
-        return {"Pending", "Running"}
+        return {"pending", "running"}
+
+    @overrides
+    def get_error_states(self) -> Set[str]:
+        return {"failed"}
 
     @overrides
-    async def get_container_status(self, iteration: Optional[str]) -> str:
+    def get_container_status(self, iteration: Optional[str]) -> str:
         # Locates the kernel pod using the kernel_id selector.  Note that we also include 'component=kernel'
         # in the selector so that executor pods (when Spark is in use) are not considered.
         # If the phase indicates Running, the pod's IP is used for the assigned_ip.
-        pod_status = None
+        pod_status = ""
         kernel_label_selector = f"kernel_id={self.kernel_id},component=kernel"
         ret = client.CoreV1Api().list_namespaced_pod(
             namespace=self.kernel_namespace, label_selector=kernel_label_selector
         )
         if ret and ret.items:
             pod_info = ret.items[0]
             self.container_name = pod_info.metadata.name
             if pod_info.status:
-                pod_status = pod_info.status.phase
-                if pod_status == "Running" and not self.assigned_host:
+                pod_status = pod_info.status.phase.lower()
+                if pod_status == "running" and not self.assigned_host:
                     # Pod is running, capture IP
                     self.assigned_ip = pod_info.status.pod_ip
                     self.assigned_host = self.container_name
                     self.assigned_node_ip = pod_info.status.host_ip
 
         if iteration:  # only log if iteration is not None (otherwise poll() is too noisy)
             self.log.debug(
@@ -130,124 +141,138 @@
                 f"'{self.kernel_namespace}'. Name: '{self.container_name}', "
                 f"Status: '{pod_status}', Pod IP: '{self.assigned_ip}', "
                 f"KernelID: '{self.kernel_id}'"
             )
 
         return pod_status
 
-    @overrides
-    async def terminate_container_resources(self, restart: bool = False) -> Optional[bool]:
-        # Kubernetes objects don't go away on their own - so we need to tear down the namespace
-        # or pod associated with the kernel.  If we created the namespace, and we're not in the
-        # process of restarting the kernel, then that's our target, else just delete the pod.
+    def delete_managed_object(self, termination_stati: List[str]) -> bool:
+        """Deletes the object managed by this provisioner
 
-        result = False
+        A return value of True indicates the object is considered deleted,
+        otherwise a False or None value is returned.
+
+        Note: the caller is responsible for handling exceptions.
+        """
         body = client.V1DeleteOptions(grace_period_seconds=0, propagation_policy="Background")
 
-        # If this termination is due to a restart, record that fact, so we can tolerate
-        # things like the existence of pre-existing namespaces (when auto-creation is
-        # in play), etc.
-        self.restarting = restart
+        # Deleting a Pod will return a v1.Pod if found and its status will be a PodStatus containing
+        # a phase string property
+        # https://kubernetes.io/docs/reference/generated/kubernetes-api/v1.21/#podstatus-v1-core
+        v1_pod = client.CoreV1Api().delete_namespaced_pod(
+            namespace=self.kernel_namespace, body=body, name=self.container_name
+        )
+        status = None
+        if v1_pod and v1_pod.status:
+            status = v1_pod.status.phase
 
-        # Delete the pod then, if applicable, the namespace
-        try:
-            object_name = "pod"
-            status = None
-            termination_stati = ["Succeeded", "Failed", "Terminating"]
-
-            # Deleting a Pod will return a v1.Pod if found and its status will be a PodStatus containing
-            # a phase string property
-            # https://kubernetes.io/docs/reference/generated/kubernetes-api/v1.21/#podstatus-v1-core
-            v1_pod = client.CoreV1Api().delete_namespaced_pod(
-                namespace=self.kernel_namespace, body=body, name=self.container_name
-            )
-            if v1_pod and v1_pod.status:
-                status = v1_pod.status.phase
+        result = status in termination_stati
 
-            if status in termination_stati:
-                result = True
+        return result
+
+    @overrides
+    def terminate_container_resources(self, restart: bool = False) -> Optional[bool]:
+        # Kubernetes objects don't go away on their own - so we need to tear down the namespace
+        # and/or pod associated with the kernel.  We'll always target the pod first so that shutdown
+        # is perceived as happening more rapidly.  Then, if we created the namespace, and we're not
+        # in the process of restarting the kernel, we'll delete the namespace.
+        # After deleting the pod we check the container status, rather than the status returned
+        # from the pod deletion API, since it's not necessarily reflective of the actual status.
+
+        self.restarting = restart
+        result = False
+        termination_stati = ["Succeeded", "Failed", "Terminating", "Success"]
 
+        # Delete the managed object then, if applicable, the namespace
+        object_type = self.object_kind
+        try:
+            result = self.delete_managed_object(termination_stati)
             if not result:
-                # If the status indicates the pod is not terminated, capture its current status.
+                # If the status indicates the object is not terminated, capture its current status.
                 # If None, update the result to True, else issue warning that it is not YET deleted
                 # since we still have the hard termination sequence to occur.
-                cur_status = await self.get_container_status(None)
+                cur_status = self.get_container_status(None)
                 if cur_status is None:
                     result = True
                 else:
                     self.log.warning(
-                        f"Pod {self.kernel_namespace}.{self.container_name} is not yet deleted.  "
-                        f"Current status is '{cur_status}'."
+                        f"{object_type} '{self.kernel_namespace}.{self.container_name}'"
+                        f" is not yet deleted.  Current status is '{cur_status}'."
                     )
 
-            if self.delete_kernel_namespace and not self.restarting:
-                object_name = "namespace"
+            if self.delete_kernel_namespace and restart is False:
+                object_type = "Namespace"
                 # Status is a return value for calls that don't return other objects.
                 # https://kubernetes.io/docs/reference/generated/kubernetes-api/v1.21/#status-v1-meta
+                body = client.V1DeleteOptions(
+                    grace_period_seconds=0, propagation_policy="Background"
+                )
                 v1_status = client.CoreV1Api().delete_namespace(
                     name=self.kernel_namespace, body=body
                 )
+                status = None
                 if v1_status:
                     status = v1_status.status
 
-                if status:
-                    if any(s in status for s in termination_stati):
-                        result = True
+                if status and any(s in status for s in termination_stati):
+                    result = True
 
                 if not result:
                     self.log.warning(
                         f"Namespace {self.kernel_namespace} is not yet deleted.  "
                         f"Current status is '{status}'."
                     )
+
         except Exception as err:
             if isinstance(err, client.rest.ApiException) and err.status == 404:
                 result = True  # okay if it's not found
             else:
-                self.log.warning(f"Error occurred deleting {object_name}: {err}")
+                self.log.warning(f"Error occurred deleting {object_type.lower()}: {err}")
 
         if result:
             self.log.debug(
-                f"KubernetesProvisioner.terminate_container_resources, pod: {self.kernel_namespace}."
-                f"{self.container_name}, kernel ID: {self.kernel_id} has been terminated."
+                f"KubernetesProcessProxy.terminate_container_resources, "
+                f"{self.object_kind}: {self.kernel_namespace}.{self.container_name}, "
+                f"kernel ID: {self.kernel_id} has been terminated."
             )
             self.container_name = None
             result = None  # maintain jupyter contract
         else:
             self.log.warning(
-                f"KubernetesProvisioner.terminate_container_resources, pod: {self.kernel_namespace}."
-                f"{self.container_name}, kernel ID: {self.kernel_id} has not been terminated."
+                "KubernetesProcessProxy.terminate_container_resources, "
+                f"{self.object_kind}: {self.kernel_namespace}.{self.container_name}, "
+                f"kernel ID: {self.kernel_id} has not been terminated."
             )
 
         # Check if there's a kernel pod template file for this kernel and silently delete it.
-        kpt_file = f"{kpt_dir}/kpt_{self.kernel_id}"
+        kpt_file = kpt_dir + "/kpt_" + self.kernel_id
         try:
             os.remove(kpt_file)
         except OSError:
             pass
 
         return result
 
     def _determine_kernel_pod_name(self, **kwargs):
         pod_name = kwargs["env"].get("KERNEL_POD_NAME")
         if pod_name is None:
             pod_name = f"{self.kernel_username}-{self.kernel_id}"
 
         # Rewrite pod_name to be compatible with DNS name convention
         # And put back into env since kernel needs this
-        pod_name = re.sub("[^0-9a-z]+", "-", pod_name.lower())
+        pod_name = re.sub(r"[^\da-z]+", "-", pod_name.lower())
         while pod_name.startswith("-"):
             pod_name = pod_name[1:]
         while pod_name.endswith("-"):
             pod_name = pod_name[:-1]
         kwargs["env"]["KERNEL_POD_NAME"] = pod_name
 
         return pod_name
 
     def _determine_kernel_namespace(self, **kwargs):
-
         # Since we need the service account name regardless of whether we're creating the namespace or not,
         # get it now.
         service_account_name = KubernetesProvisioner._determine_kernel_service_account_name(
             **kwargs
         )
 
         # If KERNEL_NAMESPACE was provided, then we assume it already exists.  If not provided, then we'll
```

### Comparing `gateway_provisioners-0.1.0/gateway_provisioners/remote_provisioner.py` & `gateway_provisioners-0.2.0/gateway_provisioners/remote_provisioner.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,14 @@
         self._enforce_authorization(**kwargs)
 
         self.log.debug(f"RemoteProvisionerBase.pre_launch() env: {env}")
         return kwargs
 
     @overrides
     async def launch_kernel(self, cmd: List[str], **kwargs: Any) -> KernelConnectionInfo:
-
         launch_kwargs = RemoteProvisionerBase._scrub_kwargs(kwargs)
         self.local_proc = gp_launch_kernel(cmd, **launch_kwargs)
         self.pid = self.local_proc.pid
         self.ip = local_ip
 
         self.log_kernel_launch(cmd)
 
@@ -247,15 +246,14 @@
 
     @overrides
     def get_shutdown_wait_time(self, recommended: Optional[float] = 5.0) -> float:
         return recommended
 
     @overrides
     def _finalize_env(self, env: Dict[str, str]) -> None:
-
         # add the applicable kernel_id and language to the env dict
         env["KERNEL_ID"] = self.kernel_id
 
         kernel_language = "unknown-kernel-language"
         if len(self.kernel_spec.language) > 0:
             kernel_language = self.kernel_spec.language.lower()
         # if already set in env: stanza, let that override.
@@ -347,15 +345,14 @@
         Sends a shutdown request to the kernel launcher listener.
         """
         # If a comm port has been established, instruct the listener to shutdown so that proper
         # kernel termination can occur.  If not done, the listener keeps the launcher process
         # active, even after the kernel has terminated, leading to less than graceful terminations.
 
         if self.comm_port > 0:
-
             try:
                 await self._send_listener_request({"shutdown": 1}, shutdown_socket=True)
                 self.log.debug("Shutdown request sent to listener via gateway communication port.")
             except Exception as e:
                 if not isinstance(e, OSError) or e.errno != errno.ECONNREFUSED:
                     self.log.warning(
                         f"An unexpected exception occurred sending listener shutdown "
```

### Comparing `gateway_provisioners-0.1.0/gateway_provisioners/response_manager.py` & `gateway_provisioners-0.2.0/gateway_provisioners/response_manager.py`

 * *Files identical despite different names*

### Comparing `gateway_provisioners-0.1.0/gateway_provisioners/yarn.py` & `gateway_provisioners-0.2.0/gateway_provisioners/yarn.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,46 +46,46 @@
 
     yarn_endpoint_env = "GP_YARN_ENDPOINT"
     yarn_endpoint = Unicode(
         None,
         config=True,
         allow_none=True,
         help="""The http url specifying the YARN Resource Manager. Note: If this value is NOT set,
-                            the YARN library will use the files within the local HADOOP_CONFIG_DIR to determine the
-                            active resource manager. (GP_YARN_ENDPOINT env var)""",
+the YARN library will use the files within the local HADOOP_CONFIG_DIR to determine the
+active resource manager. (GP_YARN_ENDPOINT env var)""",
     )
 
     @default("yarn_endpoint")
     def _yarn_endpoint_default(self):
         return os.getenv(self.yarn_endpoint_env)
 
     # Alt Yarn endpoint
     alt_yarn_endpoint_env = "GP_ALT_YARN_ENDPOINT"
     alt_yarn_endpoint = Unicode(
         None,
         config=True,
         allow_none=True,
         help="""The http url specifying the alternate YARN Resource Manager.  This value should
-                                be set when YARN Resource Managers are configured for high availability.  Note: If both
-                                YARN endpoints are NOT set, the YARN library will use the files within the local
-                                HADOOP_CONFIG_DIR to determine the active resource manager.
-                                (GP_ALT_YARN_ENDPOINT env var)""",
+be set when YARN Resource Managers are configured for high availability.  Note: If both
+YARN endpoints are NOT set, the YARN library will use the files within the local
+HADOOP_CONFIG_DIR to determine the active resource manager.
+(GP_ALT_YARN_ENDPOINT env var)""",
     )
 
     @default("alt_yarn_endpoint")
     def _alt_yarn_endpoint_default(self):
         return os.getenv(self.alt_yarn_endpoint_env)
 
     yarn_endpoint_security_enabled_env = "GP_YARN_ENDPOINT_SECURITY_ENABLED"
     yarn_endpoint_security_enabled_default_value = False
     yarn_endpoint_security_enabled = Bool(
         yarn_endpoint_security_enabled_default_value,
         config=True,
         help="""Is YARN Kerberos/SPNEGO Security enabled (True/False).
-                                          (GP_YARN_ENDPOINT_SECURITY_ENABLED env var)""",
+(GP_YARN_ENDPOINT_SECURITY_ENABLED env var)""",
     )
 
     @default("yarn_endpoint_security_enabled")
     def _yarn_endpoint_security_enabled_default(self):
         return bool(
             os.getenv(
                 self.yarn_endpoint_security_enabled_env,
@@ -95,15 +95,15 @@
 
     # Impersonation enabled
     impersonation_enabled_env = "GP_IMPERSONATION_ENABLED"
     impersonation_enabled = Bool(
         False,
         config=True,
         help="""Indicates whether impersonation will be performed during kernel launch.
-                                 (GP_IMPERSONATION_ENABLED env var)""",
+(GP_IMPERSONATION_ENABLED env var)""",
     )
 
     @default("impersonation_enabled")
     def _impersonation_enabled_default(self):
         return bool(os.getenv(self.impersonation_enabled_env, "false").lower() == "true")
 
     initial_states = {"NEW", "SUBMITTED", "ACCEPTED", "RUNNING"}
```

### Comparing `gateway_provisioners-0.1.0/gateway_provisioners/cli/base_app.py` & `gateway_provisioners-0.2.0/gateway_provisioners/cli/base_app.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import tempfile
 from glob import glob
 from string import Template
 from typing import Any
 
 from jupyter_client.kernelspec import KernelSpec, KernelSpecManager
 from jupyter_core.application import JupyterApp, base_aliases, base_flags
+from jupyter_core.paths import SYSTEM_JUPYTER_PATH, jupyter_data_dir
 from overrides import overrides
 from traitlets import Bool, Instance, TraitError, Unicode, default, validate
 
 from .._version import __version__
 from ..config_mixin import RemoteProvisionerConfigMixin
 
 kernel_launchers_dir = os.path.join(os.path.dirname(__file__), "..", "kernel-launchers")
@@ -26,15 +27,14 @@
 launcher_dirs = ["python", "r", "scala", "kubernetes", "docker", "operators"]
 resource_dirs = ["python", "r", "scala"]
 
 KERNEL_JSON = "kernel.json"
 PYTHON = "python"
 SCALA = "scala"
 R = "r"
-DASK = "dask"
 DEFAULT_LANGUAGE = PYTHON
 SUPPORTED_LANGUAGES = [PYTHON, SCALA, R]
 DEFAULT_INIT_MODE = "lazy"
 SPARK_INIT_MODES = [DEFAULT_INIT_MODE, "eager", "none"]
 LANGUAGE_SUBSTITUTIONS = {PYTHON: PYTHON, R: "R", SCALA: SCALA}
 DEFAULT_PYTHON_KERNEL_CLASS_NAME = "ipykernel.ipkernel.IPythonKernel"
 
@@ -248,42 +248,14 @@
         return value
 
     ipykernel_subclass_name = Unicode(
         DEFAULT_PYTHON_KERNEL_CLASS_NAME,
         config=True,
         help="""For Python kernels, the name of the ipykernel subclass.""",
     )
-
-    spark_home = Unicode(
-        os.getenv("SPARK_HOME", "/opt/spark"),
-        config=True,
-        help="""Specify where the spark files can be found.""",
-    )
-
-    spark_init_mode = Unicode(
-        DEFAULT_INIT_MODE,
-        config=True,
-        help=f"""Spark context initialization mode.  Must be one of {SPARK_INIT_MODES}.
-    Default = {DEFAULT_INIT_MODE}.""",
-    )
-
-    @validate("spark_init_mode")
-    def _spark_init_mode_validate(self, proposal: dict[str, str]) -> str:
-        value = proposal["value"]
-        try:
-            assert value.lower() in SPARK_INIT_MODES
-        except AssertionError as ae:
-            err_msg = (
-                f"Invalid Spark initialization mode value '{value}', not in {SPARK_INIT_MODES}"
-            )
-            raise TraitError(err_msg) from ae
-        return value.lower()  # always use lowercase form
-
-    extra_spark_opts = Unicode("", config=True, help="Specify additional Spark options.")
-
     # Flags
     user = Bool(
         False,
         config=True,
         help="Try to install the kernel spec to the per-user directory instead of the system "
         "or environment directory.",
     )
@@ -291,44 +263,45 @@
     prefix = Unicode(
         "",
         config=True,
         help="Specify a prefix to install to, e.g. an env. The kernelspec will be "
         "installed in PREFIX/share/jupyter/kernels/",
     )
 
-    spark = Bool(False, config=True, help="Install kernel for use with Spark.")
+    replace = Bool(
+        False,
+        config=True,
+        help="If a kernel specification already exists in the destination, allow for its replacement.",
+    )
 
-    super_aliases = {
+    aliases = {
         "prefix": "BaseSpecApp.prefix",
         "kernel-name": "BaseSpecApp.kernel_name",
         "display-name": "BaseSpecApp.display_name",
         "language": "BaseSpecApp.language",
-        "spark-home": "BaseSpecApp.spark_home",
-        "spark-init-mode": "BaseSpecApp.spark_init_mode",
-        "extra-spark-opts": "BaseSpecApp.extra_spark_opts",
         "authorized-users": "BaseSpecApp.authorized_users",
         "unauthorized-users": "BaseSpecApp.unauthorized_users",
         "port-range": "BaseSpecApp.port_range",
         "launch-timeout": "BaseSpecApp.launch_timeout",
         "ipykernel-subclass-name": "BaseSpecApp.ipykernel_subclass_name",
     }
-    super_aliases.update(base_aliases)
+    aliases.update(base_aliases)
 
-    super_flags = {
+    flags = {
         "user": (
             {"BaseSpecApp": {"user": True}},
-            "Install to the per-user kernel registry",
+            user.help,
+        ),
+        "replace": (
+            {"BaseSpecApp": {"replace": True}},
+            replace.help,
         ),
         "sys-prefix": (
             {"BaseSpecApp": {"prefix": sys.prefix}},
-            "Install to Python's sys.prefix. Useful in conda/virtual environments.",
-        ),
-        "spark": (
-            {"BaseSpecApp": {"spark": True}},
-            "Install kernelspec with Spark support.",
+            prefix.help,
         ),
         "debug": base_flags["debug"],
     }
 
     @overrides
     def validate_parameters(self):
         if self.user and self.prefix:
@@ -364,42 +337,58 @@
         if self.launcher_dir_name in [R]:
             self._detect_missing_rscript()
 
     @overrides
     def install_files(self):
         """Assembles kernel-specs, launchers and resources into staging directory, then installs as kernel-spec."""
 
+        # Before setting up staging area, check if kernel spec already exists and no replacement has been requested
+        dest_dir, temp_dir = self._replace_existing()
+
         # create staging dir
         staging_dir = self._create_staging_directory()
 
         # copy appropriate resource files
         self._copy_kernel_spec_files(staging_dir)
 
-        # install to destination
-        self.log.info(f"Installing kernel specification for '{self.display_name}'")
-        self.install_dir = self.kernel_spec_manager.install_kernel_spec(
-            staging_dir,
-            kernel_name=self.kernel_name,
-            user=self.user,
-            prefix=self.prefix,
-        )
-        self._delete_directory(staging_dir)
-        # If we're installing a scala kernel and don't have the toree jar file, issue
-        # a warning indicating that the scala kernel needs that file in its kernelspec
-        # directory hierarchy.
-        if self.launcher_dir_name in [SCALA] and not self.toree_jar_path:
-            kspec_toree_jar_location = os.path.join(self.install_dir, "lib")
-            self.log.warning(
-                "The Apache Toree kernel is either not installed or it's jar file cannot be determined. "
-                f"Please ensure that the Toree jar file is placed into '{kspec_toree_jar_location}' "
-                f"prior to using the kernel."
+        try:
+            # install to destination
+            self.log.info(f"Installing kernel specification for '{self.display_name}'")
+            self.install_dir = self.kernel_spec_manager.install_kernel_spec(
+                staging_dir,
+                kernel_name=self.kernel_name,
+                user=self.user,
+                prefix=self.prefix,
             )
+            self._delete_directory(staging_dir)
+            # If we're installing a scala kernel and don't have the toree jar file, issue
+            # a warning indicating that the scala kernel needs that file in its kernelspec
+            # directory hierarchy.
+            if self.launcher_dir_name in [SCALA] and not self.toree_jar_path:
+                kspec_toree_jar_location = os.path.join(self.install_dir, "lib")
+                self.log.warning(
+                    "The Apache Toree kernel is either not installed or it's jar file cannot be determined. "
+                    f"Please ensure that the Toree jar file is placed into '{kspec_toree_jar_location}' "
+                    f"prior to using the kernel."
+                )
+            # Apply substitutions to kernel.json file
+            self._finalize_kernel_json()
 
-        # Apply substitutions to kernel.json file
-        self._finalize_kernel_json()
+        except Exception as ex:
+            # We encountered an exception.  If we're in replace mode, revert temp directory back to destination
+            if temp_dir:
+                shutil.rmtree(dest_dir)
+                shutil.copytree(src=temp_dir, dst=dest_dir, dirs_exist_ok=True)
+                self.log.warning(
+                    f"An exception was encountered while finalizing the kernel specification and "
+                    f"the previous contents have been restored. The exception was: {ex}"
+                )
+        finally:
+            if temp_dir:
+                shutil.rmtree(temp_dir)
 
     def _copy_kernel_spec_files(self, staging_dir: str):
         """Copies the launcher, resource and kernel-spec files to the staging directory."""
 
         if any(
             dir_name is None
             for dir_name in [
@@ -471,34 +460,119 @@
 
     def add_optional_config_entries(self, config_stanza: dict) -> None:
         """
         Adds optional configuration parameters to the 'config' stanza of 'kernel_provisioner'.
 
         This method is overridden by subclasses which should call super().add_optional_config_entries().
         """
-        if self.authorized_users and list(self.authorized_users) != self.authorized_users_default():
+        if (
+            self.authorized_users
+            and list(self.authorized_users) != self._authorized_users_default()
+        ):
             config_stanza["authorized_users"] = list(self.authorized_users)
         if (
             self.unauthorized_users
-            and list(self.unauthorized_users) != self.unauthorized_users_default()
+            and list(self.unauthorized_users) != self._unauthorized_users_default()
         ):
             config_stanza["unauthorized_users"] = list(self.unauthorized_users)
         if self.port_range and self.port_range != self.port_range_default_value:
             config_stanza["port_range"] = self.port_range
         if self.launch_timeout:  # Always add launch_timeout if there's a value.
             config_stanza["launch_timeout"] = self.launch_timeout
 
     def get_substitutions(self, install_dir: os.path) -> dict:
         """
         Gather substitution strings to inject into the templated files.
 
         This method is overridden by subclasses which should first call super().get_substitutions().
         """
         substitutions = {}
-        substitutions["spark_home"] = self.spark_home
-        substitutions["extra_spark_opts"] = self.extra_spark_opts
-        substitutions["spark_init_mode"] = self.spark_init_mode
         substitutions["display_name"] = self.display_name
         substitutions["install_dir"] = install_dir
         substitutions["language"] = LANGUAGE_SUBSTITUTIONS[self.language.lower()]
         substitutions["ipykernel_subclass_name"] = self.ipykernel_subclass_name
         return substitutions
+
+    def _replace_existing(self) -> tuple[str, str]:
+        temp_dir = ""
+        destination_dir = self._get_destination_dir()
+        kernel_json = os.path.join(destination_dir, "kernel.json")
+        if os.path.exists(kernel_json):
+            if not self.replace:
+                err_msg = (
+                    f"A kernel specification exists at '{destination_dir}' and '--replace' "
+                    f"has not been specified.  Terminating."
+                )
+                raise SystemExit(err_msg)
+            else:
+                temp_dir = tempfile.mkdtemp()
+                shutil.copytree(src=destination_dir, dst=temp_dir, dirs_exist_ok=True)
+        return destination_dir, temp_dir
+
+    def _get_destination_dir(self) -> str:
+        """This method is essentially oa copy of `_get_destination_dir` from jupyter_client/kernelspec.py"""
+        if self.user:
+            return os.path.join(jupyter_data_dir(), "kernels", self.kernel_name)
+        elif self.prefix:
+            return os.path.join(
+                os.path.abspath(self.prefix), "share", "jupyter", "kernels", self.kernel_name
+            )
+        else:
+            return os.path.join(SYSTEM_JUPYTER_PATH[0], "kernels", self.kernel_name)
+
+
+class BaseSpecSparkApp(BaseSpecApp):
+    spark_home = Unicode(
+        os.getenv("SPARK_HOME", "/opt/spark"),
+        config=True,
+        help="""Specify where the spark files can be found.""",
+    )
+
+    spark_init_mode = Unicode(
+        DEFAULT_INIT_MODE,
+        config=True,
+        help=f"""Spark context initialization mode.  Must be one of {SPARK_INIT_MODES}.
+    Default = {DEFAULT_INIT_MODE}.""",
+    )
+
+    @validate("spark_init_mode")
+    def _spark_init_mode_validate(self, proposal: dict[str, str]) -> str:
+        value = proposal["value"]
+        try:
+            assert value.lower() in SPARK_INIT_MODES
+        except AssertionError as ae:
+            err_msg = (
+                f"Invalid Spark initialization mode value '{value}', not in {SPARK_INIT_MODES}"
+            )
+            raise TraitError(err_msg) from ae
+        return value.lower()  # always use lowercase form
+
+    extra_spark_opts = Unicode("", config=True, help="Specify additional Spark options.")
+
+    spark = Bool(False, config=True, help="Install kernelspec for use with Spark.")
+
+    aliases = {
+        "spark-home": "BaseSpecSparkApp.spark_home",
+        "spark-init-mode": "BaseSpecSparkApp.spark_init_mode",
+        "extra-spark-opts": "BaseSpecSparkApp.extra_spark_opts",
+    }
+    aliases.update(BaseSpecApp.aliases)
+
+    flags = {
+        "spark": (
+            {"BaseSpecSparkApp": {"spark": True}},
+            spark.help,
+        ),
+    }
+    flags.update(BaseSpecApp.flags)
+
+    def get_substitutions(self, install_dir: os.path) -> dict:
+        """
+        Gather substitution strings to inject into the templated files.
+
+        This method is overridden by subclasses which should first call super().get_substitutions().
+        """
+        substitutions = super().get_substitutions(install_dir)
+        substitutions["spark_home"] = self.spark_home
+        substitutions["extra_spark_opts"] = self.extra_spark_opts
+        substitutions["spark_init_mode"] = self.spark_init_mode
+        return substitutions
```

### Comparing `gateway_provisioners-0.1.0/gateway_provisioners/cli/docker_specapp.py` & `gateway_provisioners-0.2.0/gateway_provisioners/cli/docker_specapp.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,31 +61,33 @@
     )
 
     @default("image_name")
     def _image_name_default(self):
         return os.getenv(self.image_name_env)
 
     # Flags
-    swarm = Bool(False, config=True, help="Install kernel for use within a Docker Swarm cluster.")
+    swarm = Bool(
+        False, config=True, help="Install kernelspec for use within a Docker Swarm cluster."
+    )
 
     provisioner_name = Unicode(DOCKER_PROVISIONER_NAME, config=False)
     launcher_name = Unicode(LAUNCHER_NAME, config=False)
 
     aliases = {
         "image-name": "DockerSpecInstaller.image_name",
     }
-    aliases.update(BaseSpecApp.super_aliases)
+    aliases.update(BaseSpecApp.aliases)
 
     flags = {
         "swarm": (
             {"DockerSpecInstaller": {"swarm": True}},
-            "Install kernel for use within a Docker Swarm cluster.",
+            swarm.help,
         ),
     }
-    flags.update(BaseSpecApp.super_flags)
+    flags.update(BaseSpecApp.flags)
 
     @overrides
     def detect_missing_extras(self):
         super().detect_missing_extras()
         try:
             import docker  # noqa: F401
         except ImportError:
```

### Comparing `gateway_provisioners-0.1.0/gateway_provisioners/cli/image_bootstrapapp.py` & `gateway_provisioners-0.2.0/gateway_provisioners/cli/image_bootstrapapp.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,14 @@
     }
     flags.update(BaseApp.flags)
 
     kernel_spec_install = False  # Set to false when bootstrap installation occurs
 
     @overrides
     def detect_missing_extras(self):
-
         for lang in self.languages:
             if lang.lower() == SCALA:
                 self._detect_missing_toree_jar()
             elif lang.lower() == R:
                 self._detect_missing_rscript()
 
     @overrides
```

### Comparing `gateway_provisioners-0.1.0/gateway_provisioners/cli/k8s_specapp.py` & `gateway_provisioners-0.2.0/gateway_provisioners/cli/k8s_specapp.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,26 +3,35 @@
 import os
 
 from jupyter_core.application import JupyterApp
 from overrides import overrides
 from traitlets import Bool, Unicode, default
 
 from .._version import __version__
-from .base_app import DEFAULT_LANGUAGE, PYTHON, SCALA, BaseSpecApp, R
+from .base_app import DEFAULT_LANGUAGE, PYTHON, SCALA, BaseSpecSparkApp, R
+
+SPARK_OP = "spark_operator"
 
-DEFAULT_KERNEL_NAMES = {PYTHON: "k8s_python", SCALA: "k8s_scala", R: "k8s_r"}
 KERNEL_SPEC_TEMPLATE_NAMES = {
     PYTHON: "container_python",
     SCALA: "container_scala",
     R: "container_r",
+    SPARK_OP: "k8s_python_spark_operator",
+}
+DEFAULT_KERNEL_NAMES = {
+    PYTHON: "k8s_python",
+    SCALA: "k8s_scala",
+    R: "k8s_r",
+    SPARK_OP: "k8s_python_spark_operator",
 }
 DEFAULT_DISPLAY_NAMES = {
     PYTHON: "Kubernetes Python",
     SCALA: "Kubernetes Scala",
     R: "Kubernetes R",
+    SPARK_OP: "Kubernetes Spark Operator",
 }
 DEFAULT_IMAGE_NAMES = {
     PYTHON: "elyra/kernel-py",
     SCALA: "elyra/kernel-scala",
     R: "elyra/kernel-r",
 }
 DEFAULT_SPARK_IMAGE_NAMES = {
@@ -31,29 +40,32 @@
     R: "elyra/kernel-spark-r",
 }
 
 SPARK_SUFFIX = "_spark"
 SPARK_DISPLAY_NAME_SUFFIX = " (with Spark)"
 
 PROVISIONER_NAME = "kubernetes-provisioner"
+SPARK_OP_PROVISIONER_NAME = "spark-operator-provisioner"
 LAUNCHER_NAME = "launch_kubernetes.py"
+SPARK_OP_LAUNCHER_NAME = "launch_custom_resource.py"
 
 
-class K8sSpecInstaller(BaseSpecApp):
+class K8sSpecInstaller(BaseSpecSparkApp):
     """CLI for extension management."""
 
     name = "jupyter-k8s-spec"
     description = "Creates a Jupyter kernel specification for use within a Kubernetes cluster."
     # Note that the left justification of the second example is necessary to ensure proper
     # alignment with the first example during --help output.
     examples = """
     jupyter-k8s-spec install --language=R --kernel-name=r_k8s --image-name=foo/my_r_kernel_image:v4_0
 
-jupyter-k8s-spec install --language=Scala --spark --kernel-name=scala_k8s_spark
-    --display-name='Scala on Kubernetes with Spark'
+jupyter-k8s-spec install --language=Scala --spark --kernel-name=scala_k8s_spark --display-name='Scala on Kubernetes with Spark'
+
+jupyter-k8s-spec install --spark --crd --display-name='Python SparkOperator"
     """
 
     @default("kernel_name")
     def _kernel_name_default(self) -> str:
         return DEFAULT_KERNEL_NAMES[DEFAULT_LANGUAGE]
 
     @default("display_name")
@@ -84,27 +96,55 @@
     )
 
     @default("executor_image_name")
     def _executor_image_name_default(self):
         return os.getenv(self.executor_image_name_env)
 
     # Flags
-    tensorflow = Bool(False, config=True, help="""Install kernel for use with Tensorflow.""")
-
+    tensorflow = Bool(False, config=True, help="""Install kernelspec for use with Tensorflow.""")
+    crd = Bool(
+        False,
+        config=True,
+        help="""Install kernelspec for use with a Custom Resource Definition.  When combined with --spark,
+will configure the SparkOperatorProvisioner for Spark Application CRDs.""",
+    )
+    spark = Bool(
+        False,
+        config=True,
+        help="""Install kernelspec for use with Spark.  When combined with --crd,
+will configure the SparkOperatorProvisioner for Spark Application CRDs.""",
+    )
     provisioner_name = Unicode(PROVISIONER_NAME, config=False)
     launcher_name = Unicode(LAUNCHER_NAME, config=False)
 
     aliases = {
         "image-name": "K8sSpecInstaller.image_name",
         "executor-image-name": "K8sSpecInstaller.executor_image_name",
     }
-    aliases.update(BaseSpecApp.super_aliases)
+    aliases.update(BaseSpecSparkApp.aliases)
 
     flags = {}
-    flags.update(BaseSpecApp.super_flags)
+    flags.update(BaseSpecSparkApp.flags)
+    flags.update(
+        {
+            "tensorflow": (
+                {"K8sSpecInstaller": {"tensorflow": True}},
+                tensorflow.help,
+            ),
+            "crd": (
+                {"K8sSpecInstaller": {"crd": True}},
+                crd.help,
+            ),
+            # Override the spark flag so this help string is present.
+            "spark": (
+                {"K8sSpecInstaller": {"spark": True}},
+                spark.help,
+            ),
+        }
+    )
 
     @overrides
     def detect_missing_extras(self):
         super().detect_missing_extras()
         try:
             import jinja2  # noqa: F401
             import kubernetes  # noqa: F401
@@ -115,19 +155,51 @@
                 "by specifying the extra 'k8s' (e.g., pip install 'gateway_provisioners[k8s]')."
             )
 
     @overrides
     def validate_parameters(self):
         super().validate_parameters()
 
+        entered_language = self.language
         self.language = self.language.lower()
         self.launcher_dir_name = "kubernetes"
         self.resource_dir_name = self.language
 
-        if self.spark is True:
+        if self.crd is True:
+            if self.spark is False:
+                reason = (
+                    "--crd requires a specifying option (e.g., --spark) to determine which "
+                    "CustomResourceProvisioner to configure."
+                )
+                raise RuntimeError(reason)
+            if self.language != PYTHON:
+                self.log.warning(
+                    f"CRD support only works with Python, changing language from {entered_language} to Python."
+                )
+                self.language = PYTHON
+            # if kernel and display names are still defaulted, silently convert to lang default and append spark suffix
+            if self.kernel_name == DEFAULT_KERNEL_NAMES[DEFAULT_LANGUAGE]:
+                self.kernel_name = DEFAULT_KERNEL_NAMES[SPARK_OP]
+            if self.display_name == DEFAULT_DISPLAY_NAMES[DEFAULT_LANGUAGE]:
+                self.display_name = DEFAULT_DISPLAY_NAMES[SPARK_OP]
+
+            self.kernel_spec_dir_name = KERNEL_SPEC_TEMPLATE_NAMES[SPARK_OP]
+
+            if self.image_name is None:
+                self.image_name = f"{DEFAULT_SPARK_IMAGE_NAMES[self.language]}:{self._get_tag()}"
+            if self.executor_image_name is None:
+                self.executor_image_name = self.image_name
+
+            # Spark operators use different provisioners and launchers
+            if self.provisioner_name == PROVISIONER_NAME:
+                self.provisioner_name = SPARK_OP_PROVISIONER_NAME
+            if self.launcher_name == LAUNCHER_NAME:
+                self.launcher_name = SPARK_OP_LAUNCHER_NAME
+            self.launcher_dir_name = "operators"
+        elif self.spark is True:
             # if kernel and display names are still defaulted, silently convert to lang default and append spark suffix
             if self.kernel_name == DEFAULT_KERNEL_NAMES[DEFAULT_LANGUAGE]:
                 self.kernel_name = DEFAULT_KERNEL_NAMES[self.language] + SPARK_SUFFIX
             if self.display_name == DEFAULT_DISPLAY_NAMES[DEFAULT_LANGUAGE]:
                 self.display_name = DEFAULT_DISPLAY_NAMES[self.language] + SPARK_DISPLAY_NAME_SUFFIX
 
             self.kernel_spec_dir_name = DEFAULT_KERNEL_NAMES[self.language] + SPARK_SUFFIX
@@ -169,16 +241,17 @@
 
 
 class K8sProvisionerApp(JupyterApp):
     """Application responsible for driving the creation of Kubernetes-based kernel specifications."""
 
     version = __version__
     name = "jupyter k8s-spec"
-    description = """Application used to create kernel specifications for use on Kubernetes clusters
-    via the KubernetesProvisioner kernel provisioner."""
+    description = (
+        """Application used to create kernel specifications for use on Kubernetes clusters."""
+    )
     subcommands = dict(
         {
             "install": (K8sSpecInstaller, K8sSpecInstaller.description.splitlines()[0]),
         }
     )
     aliases = {}
     flags = {}
```

### Comparing `gateway_provisioners-0.1.0/gateway_provisioners/cli/ssh_specapp.py` & `gateway_provisioners-0.2.0/gateway_provisioners/cli/ssh_specapp.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 import os
 
 from jupyter_core.application import JupyterApp
 from overrides import overrides
 from traitlets import List, Unicode, default
 
 from .._version import __version__
-from .base_app import DEFAULT_LANGUAGE, PYTHON, SCALA, BaseSpecApp, R
+from .base_app import DEFAULT_LANGUAGE, PYTHON, SCALA, BaseSpecSparkApp, R
 
 DEFAULT_KERNEL_NAMES = {PYTHON: "ssh_python", SCALA: "ssh_scala", R: "ssh_r"}
 DEFAULT_DISPLAY_NAMES = {PYTHON: "Python SSH", SCALA: "Scala SSH", R: "R SSH"}
 SPARK_SUFFIX = "_spark"
 SPARK_DISPLAY_NAME_SUFFIX = " (with Spark)"
 
 
-class SshSpecInstaller(BaseSpecApp):
+class SshSpecInstaller(BaseSpecSparkApp):
     """CLI for extension management."""
 
     name = "jupyter-ssh-spec"
     description = (
         "Creates a Jupyter kernel specification for use within a cluster of hosts via SSH."
     )
     # Note that the left justification of the second example is necessary to ensure proper
@@ -61,18 +61,18 @@
     )
     # Flags
 
     aliases = {
         "remote-hosts": "SshSpecInstaller.remote_hosts",
         "spark-master": "SshSpecInstaller.spark_master",
     }
-    aliases.update(BaseSpecApp.super_aliases)
+    aliases.update(BaseSpecSparkApp.aliases)
 
     flags = {}
-    flags.update(BaseSpecApp.super_flags)
+    flags.update(BaseSpecSparkApp.flags)
 
     @overrides
     def validate_parameters(self):
         super().validate_parameters()
 
         self.language = self.language.lower()
         self.launcher_dir_name = self.language
@@ -103,15 +103,15 @@
 
         # sanitize kernel_name
         self.kernel_name = self.kernel_name.replace(" ", "_")
 
     @overrides
     def add_optional_config_entries(self, config_stanza: dict) -> None:
         super().add_optional_config_entries(config_stanza)
-        if self.remote_hosts and list(self.remote_hosts) != self.remote_hosts_default():
+        if self.remote_hosts and list(self.remote_hosts) != self._remote_hosts_default():
             config_stanza["remote_hosts"] = list(self.remote_hosts)
 
     @overrides
     def get_substitutions(self, install_dir) -> dict:
         substitutions = super().get_substitutions(install_dir)
         substitutions["spark_master"] = self.spark_master
         return substitutions
```

### Comparing `gateway_provisioners-0.1.0/gateway_provisioners/cli/yarn_specapp.py` & `gateway_provisioners-0.2.0/gateway_provisioners/cli/yarn_specapp.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 import sys
 
 from jupyter_core.application import JupyterApp
 from overrides import overrides
 from traitlets import Bool, Unicode, default
 
 from .._version import __version__
-from .base_app import DASK, DEFAULT_LANGUAGE, PYTHON, SCALA, BaseSpecApp, R
+from .base_app import DEFAULT_LANGUAGE, PYTHON, SCALA, BaseSpecSparkApp, R
+
+DASK = "dask"
 
 DEFAULT_KERNEL_NAMES = {
     PYTHON: "yarn_spark_python",
     SCALA: "yarn_spark_scala",
     R: "yarn_spark_r",
     DASK: "yarn_dask_python",
 }
@@ -20,15 +22,15 @@
     PYTHON: "Spark Python (YARN Cluster)",
     SCALA: "Spark Scala (YARN Cluster)",
     R: "Spark R (YARN Cluster)",
     DASK: "Dask Python (YARN Cluster)",
 }
 
 
-class YarnSpecInstaller(BaseSpecApp):
+class YarnSpecInstaller(BaseSpecSparkApp):
     """CLI for extension management."""
 
     name = "jupyter-yarn-spec"
     description = "Creates a Jupyter kernel specification for use within a Hadoop Yarn cluster."
     # Note that the left justification of the second example is necessary to ensure proper
     # alignment with the first example during --help output.
     examples = """
@@ -124,31 +126,31 @@
 
     aliases = {
         "yarn-endpoint": "YarnSpecInstaller.yarn_endpoint",
         "alt-yarn-endpoint": "YarnSpecInstaller.alt_yarn_endpoint",
         "python-root": "YarnSpecInstaller.python_root",
         "extra-dask-opts": "YarnSpecInstaller.extra_dask_opts",
     }
-    aliases.update(BaseSpecApp.super_aliases)
+    aliases.update(BaseSpecSparkApp.aliases)
 
     flags = {
         "dask": (
             {"YarnSpecInstaller": {"dask": True}},
-            "Install kernelspec for Dask in Yarn cluster.",
+            dask.help,
         ),
         "yarn-endpoint-security-enabled": (
             {"YarnSpecInstaller": {"yarn_endpoint_security_enabled": True}},
-            "Install kernelspec where Yarn API endpoint has security enabled.",
+            yarn_endpoint_security_enabled.help,
         ),
         "impersonation-enabled": (
             {"YarnSpecInstaller": {"impersonation_enabled": True}},
-            "Install kernelspec to impersonate user (requires root privileges).",
+            impersonation_enabled.help,
         ),
     }
-    flags.update(BaseSpecApp.super_flags)
+    flags.update(BaseSpecSparkApp.flags)
 
     @overrides
     def detect_missing_extras(self):
         super().detect_missing_extras()
         try:
             import yarn_api_client  # noqa: F401
         except ImportError:
```

### Comparing `gateway_provisioners-0.1.0/gateway_provisioners/docker/gp-spark-base/Dockerfile` & `gateway_provisioners-0.2.0/gateway_provisioners/docker/gp-spark-base/Dockerfile`

 * *Files 6% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 
 # Spark dependencies
 # Default values can be overridden at build time
 # All ARGs following SPARK_VERSION have values that must correspond to
 # that version of Spark.  See https://spark.apache.org/downloads.html
 # (OPENJDK_VERSION can be any of 8, 11, 17)
 ARG SPARK_VERSION=${SPARK_VERSION:-3.3.1}
-ARG HADOOP_VERSION="2"
-ARG SCALA_VERSION="2.12"
-ARG SPARK_CHECKSUM="817f89d83ffacda1c2075d28d4a649bc007a0dd4b8edeac4b2c5e0365efc34fafceff0afedc809faa0e687c6aabf0ff6dbcda329e9045692d700c63018d93171"
-ARG OPENJDK_VERSION="17"
+ARG SPARK_CHECKSUM=${SPARK_CHECKSUM:-817f89d83ffacda1c2075d28d4a649bc007a0dd4b8edeac4b2c5e0365efc34fafceff0afedc809faa0e687c6aabf0ff6dbcda329e9045692d700c63018d93171}
+ARG HADOOP_VERSION=${HADOOP_VERSION:-2}
+ARG SCALA_VERSION=${SCALA_VERSION:-2.12}
+ARG OPENJDK_VERSION=${OPENJDK_VERSION:-17}
 
 # JDK installation
 RUN apt-get update --yes && \
     apt-get install --yes --no-install-recommends \
     "openjdk-${OPENJDK_VERSION}-jre-headless" \
     ca-certificates-java && \
     apt-get clean && rm -rf /var/lib/apt/lists/*
```

### Comparing `gateway_provisioners-0.1.0/gateway_provisioners/docker/kernel-image/Dockerfile` & `gateway_provisioners-0.2.0/gateway_provisioners/docker/kernel-image/Dockerfile`

 * *Files 8% similar despite different names*

```diff
@@ -114,16 +114,15 @@
 FROM kernel-${KERNEL_LANG} as kernel-image
 ARG KERNEL_LANG
 LABEL KERNEL_LANG=${KERNEL_LANG}
 
 # Build images from appropriate source - release or local
 FROM kernel-image AS package-release
 # Install remote provisioners from PYPI
-# TODO - uncomment once we have a release
-#RUN pip install gateway_provisioners
+RUN pip install gateway_provisioners
 
 # LOCAL (dev) build
 FROM kernel-image AS package-local
 # Install remote provisioners from local wheel
 COPY gateway_provisioners*.whl /tmp/
 RUN pip install /tmp/gateway_provisioners*.whl && \
 	rm -f /tmp/gateway_provisioners*.whl
```

### Comparing `gateway_provisioners-0.1.0/gateway_provisioners/kernel-launchers/R/scripts/launch_IRkernel.R` & `gateway_provisioners-0.2.0/gateway_provisioners/kernel-launchers/R/scripts/launch_IRkernel.R`

 * *Files identical despite different names*

### Comparing `gateway_provisioners-0.1.0/gateway_provisioners/kernel-launchers/bootstrap/bootstrap-kernel.sh` & `gateway_provisioners-0.2.0/gateway_provisioners/kernel-launchers/bootstrap/bootstrap-kernel.sh`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,17 @@
   # Launch the python kernel launcher - which embeds the IPython kernel and listens for interrupts
   # and shutdown requests from the server.
 
   export JPY_PARENT_PID=$$$$  # Force reset of parent pid since we're detached
 
   if [ -z "${KERNEL_CLASS_NAME}" ]
   then
-    kernel_class_option = ""
+    kernel_class_option=""
   else
-    kernel_class_option = "--kernel_class_name ${KERNEL_CLASS_NAME}"
+    kernel_class_option="--kernel_class_name ${KERNEL_CLASS_NAME}"
   fi
 
 	set -x
 	python ${KERNEL_LAUNCHERS_DIR}/python/scripts/launch_ipykernel.py --kernel-id ${KERNEL_ID} \
 	      --port-range ${PORT_RANGE} --response-address ${RESPONSE_ADDRESS} --public-key ${PUBLIC_KEY} \
 	      --spark-context-initialization-mode ${KERNEL_SPARK_CONTEXT_INIT_MODE}  ${kernel_class_option}
 	{ set +x; } 2>/dev/null
```

### Comparing `gateway_provisioners-0.1.0/gateway_provisioners/kernel-launchers/docker/scripts/launch_docker.py` & `gateway_provisioners-0.2.0/gateway_provisioners/kernel-launchers/docker/scripts/launch_docker.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     # Determine network. If EG_DOCKER_NETWORK has not been propagated, fall back to 'bridge'...
     docker_network = os.environ.get("DOCKER_NETWORK", os.environ.get("EG_DOCKER_NETWORK", "bridge"))
 
     # Build labels - these will be modelled similar to kubernetes: kernel_id, component, app, ...
     labels = {}
     labels["kernel_id"] = kernel_id
     labels["component"] = "kernel"
-    labels["app"] = "enterprise-gateway"
+    labels["app"] = "gateway-provisioners"
 
     # Capture env parameters...
     param_env = {}
     param_env["PORT_RANGE"] = port_range
     param_env["PUBLIC_KEY"] = public_key
     param_env["RESPONSE_ADDRESS"] = response_addr
     param_env["KERNEL_SPARK_CONTEXT_INIT_MODE"] = spark_context_init_mode
```

### Comparing `gateway_provisioners-0.1.0/gateway_provisioners/kernel-launchers/kubernetes/scripts/kernel-pod.yaml.j2` & `gateway_provisioners-0.2.0/gateway_provisioners/kernel-launchers/kubernetes/scripts/kernel-pod.yaml.j2`

 * *Files 5% similar despite different names*

```diff
@@ -10,17 +10,19 @@
 apiVersion: v1
 kind: Pod
 metadata:
   name: "{{ kernel_pod_name }}"
   namespace: "{{ kernel_namespace }}"
   labels:
     kernel_id: "{{ kernel_id }}"
-    app: enterprise-gateway
+    app: gateway-provisioners
     component: kernel
     source: kernel-pod.yaml
+  annotations:
+    cluster-autoscaler.kubernetes.io/safe-to-evict: "false"
 spec:
   restartPolicy: Never
   serviceAccountName: "{{ kernel_service_account_name }}"
 # NOTE: that using runAsGroup requires that feature-gate RunAsGroup be enabled.
 # WARNING: Only using runAsUser w/o runAsGroup or NOT enabling the RunAsGroup feature-gate
 # will result in the new kernel pod's effective group of 0 (root)! although the user will
 # correspond to the runAsUser value.  As a result, BOTH should be uncommented AND the feature-gate
@@ -34,35 +36,20 @@
     {% endif %}
     {% if kernel_gid is defined %}
     runAsGroup: {{ kernel_gid | int }}
     {% endif %}
     fsGroup: 100
   {% endif %}
   containers:
-  - env:
-    - name: PORT_RANGE
-      value: "{{ port_range }}"
-    - name: RESPONSE_ADDRESS
-      value: "{{ response_address }}"
-    - name: PUBLIC_KEY
-      value: "{{ public_key }}"
-    - name: KERNEL_ID
-      value: "{{ kernel_id }}"
-    - name: KERNEL_LANGUAGE
-      value: "{{ kernel_language }}"
-    - name: KERNEL_NAME
-      value: "{{ kernel_name }}"
-    - name: KERNEL_NAMESPACE
-      value: "{{ kernel_namespace }}"
-    - name: KERNEL_SPARK_CONTEXT_INIT_MODE
-      value: "{{ kernel_spark_context_init_mode }}"
-    - name: KERNEL_USERNAME
-      value: "{{ kernel_username }}"
-    image: "{{ kernel_image }}"
+  - image: "{{ kernel_image }}"
     name: "{{ kernel_pod_name }}"
+    env:
+# Add any custom envs here that aren't already configured for the kernel's environment
+#    - name: MY_CUSTOM_ENV
+#      value: "my_custom_value"
     {% if kernel_cpus is defined or kernel_memory is defined or kernel_gpus is defined or kernel_cpus_limit is defined or kernel_memory_limit is defined or kernel_gpus_limit is defined %}
     resources:
       {% if kernel_cpus is defined or kernel_memory is defined or kernel_gpus is defined %}
       requests:
         {% if kernel_cpus is defined %}
         cpu: "{{ kernel_cpus }}"
         {% endif %}
```

### Comparing `gateway_provisioners-0.1.0/gateway_provisioners/kernel-launchers/kubernetes/scripts/launch_kubernetes.py` & `gateway_provisioners-0.2.0/gateway_provisioners/kernel-launchers/kubernetes/scripts/launch_kubernetes.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 #!/opt/conda/bin/python
 # Copyright (c) Jupyter Development Team.
 # Distributed under the terms of the Modified BSD License.
 
 import argparse
 import os
 import sys
+from typing import List
 
 import urllib3
 import yaml
 from jinja2 import Environment, FileSystemLoader, select_autoescape
 from kubernetes import client, config
+from kubernetes.client.rest import ApiException
 
 urllib3.disable_warnings()
 
 KERNEL_POD_TEMPLATE_PATH = "/kernel-pod.yaml.j2"
 
 
 def generate_kernel_pod_yaml(keywords):
@@ -39,14 +41,54 @@
     # contain corresponding item. Therefore, no need to check if any are left unsubstituted.
     # Kubernetes API server will validate the pod spec instead.
     k8s_yaml = j_env.get_template(KERNEL_POD_TEMPLATE_PATH).render(**keywords)
 
     return k8s_yaml
 
 
+def extend_pod_env(pod_def: dict) -> dict:
+    """Extends the pod_def.spec.containers[0].env stanza with current environment."""
+    env_stanza = pod_def["spec"]["containers"][0].get("env") or []
+
+    # Walk current set of template env entries and replace those found in the current
+    # env with their values (and record those items).   Then add all others from the env
+    # that were not already.
+    processed_entries: List[str] = []
+    for item in env_stanza:
+        item_name = item.get("name")
+        if item_name in os.environ:
+            item["value"] = os.environ[item_name]
+            processed_entries.append(item_name)
+
+    for name, value in os.environ.items():
+        if name not in processed_entries:
+            env_stanza.append({"name": name, "value": value})
+
+    pod_def["spec"]["containers"][0]["env"] = env_stanza
+    return pod_def
+
+
+# A popular reason that lasts many APIs but is not a constant in the client lib
+K8S_ALREADY_EXIST_REASON = "AlreadyExists"
+
+
+def _parse_k8s_exception(exc: ApiException) -> str:
+    """Parse the exception and return the error message from kubernetes api
+    Args:
+        exc (Exception): Exception object
+    Returns:
+        str: Error message from kubernetes api
+    """
+    # more exception can be parsed, but at the time of implementation we only need this one
+    if exc.status == 409:
+        if exc.reason == "Conflict" and f'"reason":{K8S_ALREADY_EXIST_REASON}' in exc.body:
+            return K8S_ALREADY_EXIST_REASON
+    return ""
+
+
 def launch_kubernetes_kernel(
     kernel_id,
     port_range,
     response_addr,
     public_key,
     spark_context_init_mode,
     pod_template_file,
@@ -62,21 +104,32 @@
 
     # Capture keywords and their values.
     keywords = {}
 
     # Factory values...
     # Since jupyter lower cases the kernel directory as the kernel-name, we need to capture its case-sensitive
     # value since this is used to locate the kernel launch script within the image.
-    keywords["port_range"] = port_range
-    keywords["public_key"] = public_key
-    keywords["response_address"] = response_addr
-    keywords["kernel_id"] = kernel_id
-    keywords["kernel_name"] = os.path.basename(os.path.dirname(os.path.dirname(__file__)))
-    keywords["kernel_spark_context_init_mode"] = spark_context_init_mode
-    keywords["kernel_class_name"] = kernel_class_name
+    # Ensure these key/value pairs are reflected in the environment.  We'll add these to the container's env
+    # stanza after the pod template is generated.
+    if port_range:
+        os.environ["PORT_RANGE"] = port_range
+    if public_key:
+        os.environ["PUBLIC_KEY"] = public_key
+    if response_addr:
+        os.environ["RESPONSE_ADDRESS"] = response_addr
+    if kernel_id:
+        os.environ["KERNEL_ID"] = kernel_id
+    if spark_context_init_mode:
+        os.environ["KERNEL_SPARK_CONTEXT_INIT_MODE"] = spark_context_init_mode
+    if kernel_class_name:
+        os.environ["KERNEL_CLASS_NAME"] = kernel_class_name
+
+    os.environ["KERNEL_NAME"] = os.path.basename(
+        os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
+    )
 
     # Walk env variables looking for names prefixed with KERNEL_.  When found, set corresponding keyword value
     # with name in lower case.
     for name, value in os.environ.items():
         if name.startswith("KERNEL_"):
             keywords[name.lower()] = yaml.safe_load(value)
 
@@ -93,38 +146,62 @@
     pod_template = None
     kernel_namespace = keywords["kernel_namespace"]
     k8s_objs = yaml.safe_load_all(k8s_yaml)
     for k8s_obj in k8s_objs:
         if k8s_obj.get("kind"):
             if k8s_obj["kind"] == "Pod":
                 #  print("{}".format(k8s_obj))  # useful for debug
-                pod_template = k8s_obj
+                pod_template = extend_pod_env(k8s_obj)
                 if pod_template_file is None:
-                    client.CoreV1Api(client.ApiClient()).create_namespaced_pod(
-                        body=k8s_obj, namespace=kernel_namespace
-                    )
+                    try:
+                        client.CoreV1Api(client.ApiClient()).create_namespaced_pod(
+                            body=k8s_obj, namespace=kernel_namespace
+                        )
+                    except ApiException as exc:
+                        if _parse_k8s_exception(exc) == K8S_ALREADY_EXIST_REASON:
+                            (
+                                client.CoreV1Api(client.ApiClient())
+                                .list_namespaced_pod(
+                                    namespace=kernel_namespace,
+                                    label_selector=f"kernel_id={kernel_id}",
+                                    watch=False,
+                                )
+                                .items[0]
+                            )
+                        else:
+                            raise exc
             elif k8s_obj["kind"] == "Secret":
                 if pod_template_file is None:
                     client.CoreV1Api(client.ApiClient()).create_namespaced_secret(
                         body=k8s_obj, namespace=kernel_namespace
                     )
             elif k8s_obj["kind"] == "PersistentVolumeClaim":
                 if pod_template_file is None:
-                    client.CoreV1Api(client.ApiClient()).create_namespaced_persistent_volume_claim(
-                        body=k8s_obj, namespace=kernel_namespace
-                    )
+                    try:
+                        client.CoreV1Api(
+                            client.ApiClient()
+                        ).create_namespaced_persistent_volume_claim(
+                            body=k8s_obj, namespace=kernel_namespace
+                        )
+                    except ApiException as exc:
+                        if _parse_k8s_exception(exc) == K8S_ALREADY_EXIST_REASON:
+                            pass
+                        else:
+                            raise exc
             elif k8s_obj["kind"] == "PersistentVolume":
                 if pod_template_file is None:
                     client.CoreV1Api(client.ApiClient()).create_persistent_volume(body=k8s_obj)
             else:
                 sys.exit(
                     f"ERROR - Unhandled Kubernetes object kind '{k8s_obj['kind']}' found in yaml file - "
                     f"kernel launch terminating!"
                 )
         else:
+            print("ERROR processing Kubernetes yaml file - kernel launch terminating!")
+            print(k8s_yaml)
             sys.exit(
                 f"ERROR - Unknown Kubernetes object '{k8s_obj}' found in yaml file - kernel launch terminating!"
             )
 
     if pod_template_file:
         # TODO - construct other --conf options for things like mounts, resources, etc.
         # write yaml to file...
@@ -139,15 +216,15 @@
 
         additional_spark_opts += _get_spark_resources(pod_template)
 
         if spark_opts_out:
             with open(spark_opts_out, "w+") as soo_fd:
                 soo_fd.write(additional_spark_opts)
         else:  # If no spark_opts_out was specified, print to stdout in case this is an old caller
-            print(additional_spark_opts)  # noqa: T201
+            print(additional_spark_opts)
 
 
 def _get_spark_resources(pod_template: dict) -> str:
     # Gather up resources for cpu/memory requests/limits.  Since gpus require a "discovery script"
     # we'll leave that alone for now:
     # https://spark.apache.org/docs/latest/running-on-kubernetes.html#resource-allocation-and-configuration-overview
     #
```

### Comparing `gateway_provisioners-0.1.0/gateway_provisioners/kernel-launchers/python/scripts/launch_ipykernel.py` & `gateway_provisioners-0.2.0/gateway_provisioners/kernel-launchers/python/scripts/launch_ipykernel.py`

 * *Files identical despite different names*

### Comparing `gateway_provisioners-0.1.0/gateway_provisioners/kernel-launchers/python/scripts/server_listener.py` & `gateway_provisioners-0.2.0/gateway_provisioners/kernel-launchers/python/scripts/server_listener.py`

 * *Files identical despite different names*

### Comparing `gateway_provisioners-0.1.0/gateway_provisioners/kernel-launchers/scala/lib/toree-launcher_2.12-0.1.0.jar` & `gateway_provisioners-0.2.0/gateway_provisioners/kernel-launchers/scala/lib/toree-launcher_2.12-0.2.0.jar`

 * *Files 9% similar despite different names*

#### zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 31960 bytes, number of entries: 14
--rw----     2.0 fat      295 bX defN 23-Jan-27 15:37 META-INF/MANIFEST.MF
--rw----     1.0 fat        0 b- stor 23-Jan-27 15:37 launcher/
--rw----     1.0 fat        0 b- stor 23-Jan-27 15:37 launcher/utils/
--rw----     2.0 fat     4289 bl defN 23-Jan-27 15:37 launcher/ToreeLauncher.class
--rw----     2.0 fat     8762 bl defN 23-Jan-27 15:37 launcher/KernelProfile.class
--rw----     2.0 fat     3662 bl defN 23-Jan-27 15:37 launcher/utils/SecurityUtils$.class
--rw----     2.0 fat      925 bl defN 23-Jan-27 15:37 launcher/utils/SecurityUtils.class
--rw----     2.0 fat     6012 bl defN 23-Jan-27 15:37 launcher/utils/Payload$.class
--rw----     2.0 fat     4335 bl defN 23-Jan-27 15:37 launcher/utils/SocketUtils$.class
--rw----     2.0 fat     5348 bl defN 23-Jan-27 15:37 launcher/utils/Payload.class
--rw----     2.0 fat     1528 bl defN 23-Jan-27 15:37 launcher/utils/SocketUtils.class
--rw----     2.0 fat     8828 bl defN 23-Jan-27 15:37 launcher/KernelProfile$.class
--rw----     2.0 fat      785 bl defN 23-Jan-27 15:37 launcher/ToreeLauncher$$anon$1.class
--rw----     2.0 fat    19372 bl defN 23-Jan-27 15:37 launcher/ToreeLauncher$.class
-14 files, 64141 bytes uncompressed, 29904 bytes compressed:  53.4%
+Zip file size: 31961 bytes, number of entries: 14
+-rw----     2.0 fat      295 bX defN 23-Apr-20 22:36 META-INF/MANIFEST.MF
+-rw----     1.0 fat        0 b- stor 23-Apr-20 22:36 launcher/
+-rw----     1.0 fat        0 b- stor 23-Apr-20 22:36 launcher/utils/
+-rw----     2.0 fat    19372 bl defN 23-Apr-20 22:36 launcher/ToreeLauncher$.class
+-rw----     2.0 fat     8828 bl defN 23-Apr-20 22:36 launcher/KernelProfile$.class
+-rw----     2.0 fat     4289 bl defN 23-Apr-20 22:36 launcher/ToreeLauncher.class
+-rw----     2.0 fat     8762 bl defN 23-Apr-20 22:36 launcher/KernelProfile.class
+-rw----     2.0 fat      785 bl defN 23-Apr-20 22:36 launcher/ToreeLauncher$$anon$1.class
+-rw----     2.0 fat     6012 bl defN 23-Apr-20 22:36 launcher/utils/Payload$.class
+-rw----     2.0 fat     3662 bl defN 23-Apr-20 22:36 launcher/utils/SecurityUtils$.class
+-rw----     2.0 fat      925 bl defN 23-Apr-20 22:36 launcher/utils/SecurityUtils.class
+-rw----     2.0 fat     4335 bl defN 23-Apr-20 22:36 launcher/utils/SocketUtils$.class
+-rw----     2.0 fat     1528 bl defN 23-Apr-20 22:36 launcher/utils/SocketUtils.class
+-rw----     2.0 fat     5348 bl defN 23-Apr-20 22:36 launcher/utils/Payload.class
+14 files, 64141 bytes uncompressed, 29905 bytes compressed:  53.4%
```

#### zipnote «TEMP»/diffoscope_imnz3io0_/tmpv8pnvv74_.zip

```diff
@@ -3,41 +3,41 @@
 
 Filename: launcher/
 Comment: 
 
 Filename: launcher/utils/
 Comment: 
 
-Filename: launcher/ToreeLauncher.class
+Filename: launcher/ToreeLauncher$.class
 Comment: 
 
-Filename: launcher/KernelProfile.class
+Filename: launcher/KernelProfile$.class
 Comment: 
 
-Filename: launcher/utils/SecurityUtils$.class
+Filename: launcher/ToreeLauncher.class
 Comment: 
 
-Filename: launcher/utils/SecurityUtils.class
+Filename: launcher/KernelProfile.class
 Comment: 
 
-Filename: launcher/utils/Payload$.class
+Filename: launcher/ToreeLauncher$$anon$1.class
 Comment: 
 
-Filename: launcher/utils/SocketUtils$.class
+Filename: launcher/utils/Payload$.class
 Comment: 
 
-Filename: launcher/utils/Payload.class
+Filename: launcher/utils/SecurityUtils$.class
 Comment: 
 
-Filename: launcher/utils/SocketUtils.class
+Filename: launcher/utils/SecurityUtils.class
 Comment: 
 
-Filename: launcher/KernelProfile$.class
+Filename: launcher/utils/SocketUtils$.class
 Comment: 
 
-Filename: launcher/ToreeLauncher$$anon$1.class
+Filename: launcher/utils/SocketUtils.class
 Comment: 
 
-Filename: launcher/ToreeLauncher$.class
+Filename: launcher/utils/Payload.class
 Comment: 
 
 Zip file comment:
```

#### META-INF/MANIFEST.MF

```diff
@@ -1,10 +1,10 @@
 Manifest-Version: 1.0
 Specification-Title: toree-launcher
-Specification-Version: 0.1.0
+Specification-Version: 0.2.0
 Specification-Vendor: default
 Implementation-Title: toree-launcher
-Implementation-Version: 0.1.0
+Implementation-Version: 0.2.0
 Implementation-Vendor: default
 Implementation-Vendor-Id: default
 Main-Class: launcher.ToreeLauncher
```

### Comparing `gateway_provisioners-0.1.0/gateway_provisioners/kernel-launchers/scala/toree-launcher/build.sbt` & `gateway_provisioners-0.2.0/gateway_provisioners/kernel-launchers/scala/toree-launcher/build.sbt`

 * *Files identical despite different names*

### Comparing `gateway_provisioners-0.1.0/gateway_provisioners/kernel-launchers/scala/toree-launcher/project/scalastyle-config.xml` & `gateway_provisioners-0.2.0/gateway_provisioners/kernel-launchers/scala/toree-launcher/project/scalastyle-config.xml`

 * *Files identical despite different names*

### Comparing `gateway_provisioners-0.1.0/gateway_provisioners/kernel-launchers/scala/toree-launcher/src/main/scala/launcher/KernelProfile.scala` & `gateway_provisioners-0.2.0/gateway_provisioners/kernel-launchers/scala/toree-launcher/src/main/scala/launcher/KernelProfile.scala`

 * *Files identical despite different names*

### Comparing `gateway_provisioners-0.1.0/gateway_provisioners/kernel-launchers/scala/toree-launcher/src/main/scala/launcher/ToreeLauncher.scala` & `gateway_provisioners-0.2.0/gateway_provisioners/kernel-launchers/scala/toree-launcher/src/main/scala/launcher/ToreeLauncher.scala`

 * *Files identical despite different names*

### Comparing `gateway_provisioners-0.1.0/gateway_provisioners/kernel-launchers/scala/toree-launcher/src/main/scala/launcher/utils/SecurityUtils.scala` & `gateway_provisioners-0.2.0/gateway_provisioners/kernel-launchers/scala/toree-launcher/src/main/scala/launcher/utils/SecurityUtils.scala`

 * *Files identical despite different names*

### Comparing `gateway_provisioners-0.1.0/gateway_provisioners/kernel-launchers/scala/toree-launcher/src/main/scala/launcher/utils/SocketUtils.scala` & `gateway_provisioners-0.2.0/gateway_provisioners/kernel-launchers/scala/toree-launcher/src/main/scala/launcher/utils/SocketUtils.scala`

 * *Files identical despite different names*

### Comparing `gateway_provisioners-0.1.0/gateway_provisioners/kernel-launchers/shared/scripts/server_listener.py` & `gateway_provisioners-0.2.0/gateway_provisioners/kernel-launchers/shared/scripts/server_listener.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,14 @@
         self.public_key: bytes = public_key.encode("utf-8")
         self.cluster_type: str = cluster_type
 
         # Initialized later...
         self.comm_socket: socket | None = None
 
     def build_connection_file(self) -> None:
-
         ports: list = self._select_ports(5)
         write_connection_file(
             fname=self.conn_filename,
             ip="0.0.0.0",  # noqa: S104
             key=str(uuid.uuid4()).encode("utf-8"),  # convert to bytes,
             shell_port=ports[0],
             iopub_port=ports[1],
```

### Comparing `gateway_provisioners-0.1.0/gateway_provisioners/kernel-resources/python/logo-64x64.png` & `gateway_provisioners-0.2.0/gateway_provisioners/kernel-resources/python/logo-64x64.png`

 * *Files identical despite different names*

### Comparing `gateway_provisioners-0.1.0/gateway_provisioners/kernel-resources/r/kernel.js` & `gateway_provisioners-0.2.0/gateway_provisioners/kernel-resources/r/kernel.js`

 * *Files identical despite different names*

### Comparing `gateway_provisioners-0.1.0/gateway_provisioners/kernel-resources/r/logo-64x64.png` & `gateway_provisioners-0.2.0/gateway_provisioners/kernel-resources/r/logo-64x64.png`

 * *Files identical despite different names*

### Comparing `gateway_provisioners-0.1.0/gateway_provisioners/kernel-resources/scala/logo-64x64.png` & `gateway_provisioners-0.2.0/gateway_provisioners/kernel-resources/scala/logo-64x64.png`

 * *Files identical despite different names*

### Comparing `gateway_provisioners-0.1.0/gateway_provisioners/kernel-specs/container_python/kernel.json` & `gateway_provisioners-0.2.0/gateway_provisioners/kernel-specs/container_python/kernel.json`

 * *Files identical despite different names*

### Comparing `gateway_provisioners-0.1.0/gateway_provisioners/kernel-specs/container_r/kernel.json` & `gateway_provisioners-0.2.0/gateway_provisioners/kernel-specs/container_r/kernel.json`

 * *Files identical despite different names*

### Comparing `gateway_provisioners-0.1.0/gateway_provisioners/kernel-specs/container_scala/kernel.json` & `gateway_provisioners-0.2.0/gateway_provisioners/kernel-specs/container_scala/kernel.json`

 * *Files identical despite different names*

### Comparing `gateway_provisioners-0.1.0/gateway_provisioners/kernel-specs/k8s_python_spark/kernel.json` & `gateway_provisioners-0.2.0/gateway_provisioners/kernel-specs/k8s_python_spark/kernel.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9833333333333334%*

 * *Differences: {"'env'": "{'SPARK_OPTS': '--master "*

 * *          'k8s://https://${KUBERNETES_SERVICE_HOST}:${KUBERNETES_SERVICE_PORT} --deploy-mode '*

 * *          'cluster --name ${KERNEL_USERNAME}-${KERNEL_ID} --conf '*

 * *          'spark.kubernetes.namespace=${KERNEL_NAMESPACE} --conf '*

 * *          'spark.kubernetes.driver.label.app=kubernetes-kernel-provider --conf '*

 * *          'spark.kubernetes.driver.label.kernel_id=${KERNEL_ID} --conf '*

 * *          'spark.kubernetes.driver.label.component=kernel --conf '*

 * *          'spark.kuberne […]*

```diff
@@ -12,15 +12,15 @@
         "--kernel-class-name",
         "${ipykernel_subclass_name}"
     ],
     "display_name": "${display_name}",
     "env": {
         "LAUNCH_OPTS": "",
         "SPARK_HOME": "${spark_home}",
-        "SPARK_OPTS": "--master k8s://https://${KUBERNETES_SERVICE_HOST}:${KUBERNETES_SERVICE_PORT} --deploy-mode cluster --name ${KERNEL_USERNAME}-${KERNEL_ID} --conf spark.kubernetes.namespace=${KERNEL_NAMESPACE} --conf spark.kubernetes.driver.label.app=kubernetes-kernel-provider --conf spark.kubernetes.driver.label.kernel_id=${KERNEL_ID} --conf spark.kubernetes.driver.label.component=kernel --conf spark.kubernetes.executor.label.app=kubernetes-kernel-provider --conf spark.kubernetes.executor.label.kernel_id=${KERNEL_ID} --conf spark.kubernetes.executor.label.component=kernel --conf spark.kubernetes.driver.container.image=${KERNEL_IMAGE} --conf spark.kubernetes.executor.container.image=${KERNEL_EXECUTOR_IMAGE} --conf spark.kubernetes.authenticate.driver.serviceAccountName=${KERNEL_SERVICE_ACCOUNT_NAME} --conf spark.kubernetes.submission.waitAppCompletion=false --conf spark.kubernetes.pyspark.pythonVersion=3 ${extra_spark_opts} ${KERNEL_EXTRA_SPARK_OPTS}"
+        "SPARK_OPTS": "--master k8s://https://${KUBERNETES_SERVICE_HOST}:${KUBERNETES_SERVICE_PORT} --deploy-mode cluster --name ${KERNEL_USERNAME}-${KERNEL_ID} --conf spark.kubernetes.namespace=${KERNEL_NAMESPACE} --conf spark.kubernetes.driver.label.app=kubernetes-kernel-provider --conf spark.kubernetes.driver.label.kernel_id=${KERNEL_ID} --conf spark.kubernetes.driver.label.component=kernel --conf spark.kubernetes.executor.label.app=kubernetes-kernel-provider --conf spark.kubernetes.executor.label.kernel_id=${KERNEL_ID} --conf spark.kubernetes.executor.label.component=worker --conf spark.kubernetes.driver.container.image=${KERNEL_IMAGE} --conf spark.kubernetes.executor.container.image=${KERNEL_EXECUTOR_IMAGE} --conf spark.kubernetes.authenticate.driver.serviceAccountName=${KERNEL_SERVICE_ACCOUNT_NAME} --conf spark.kubernetes.submission.waitAppCompletion=false --conf spark.kubernetes.pyspark.pythonVersion=3 ${extra_spark_opts} ${KERNEL_EXTRA_SPARK_OPTS}"
     },
     "language": "${language}",
     "metadata": {
         "debugger": true,
         "kernel_provisioner": {
             "config": {
                 "executor_image_name": "${executor_image_name}",
```

### Comparing `gateway_provisioners-0.1.0/gateway_provisioners/kernel-specs/k8s_python_spark/bin/run.sh` & `gateway_provisioners-0.2.0/gateway_provisioners/kernel-specs/k8s_python_spark/bin/run.sh`

 * *Files identical despite different names*

### Comparing `gateway_provisioners-0.1.0/gateway_provisioners/kernel-specs/k8s_r_spark/kernel.json` & `gateway_provisioners-0.2.0/gateway_provisioners/kernel-specs/k8s_r_spark/kernel.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9833333333333334%*

 * *Differences: {"'env'": "{'SPARK_OPTS': '--master "*

 * *          'k8s://https://${KUBERNETES_SERVICE_HOST}:${KUBERNETES_SERVICE_PORT} --deploy-mode '*

 * *          'cluster --name ${KERNEL_USERNAME}-${KERNEL_ID} --conf '*

 * *          'spark.kubernetes.namespace=${KERNEL_NAMESPACE} --conf '*

 * *          'spark.kubernetes.driver.label.app=kubernetes-kernel-provider --conf '*

 * *          'spark.kubernetes.driver.label.kernel_id=${KERNEL_ID} --conf '*

 * *          'spark.kubernetes.driver.label.component=kernel --conf '*

 * *          'spark.kuberne […]*

```diff
@@ -12,15 +12,15 @@
         "--spark-context-initialization-mode",
         "${spark_init_mode}"
     ],
     "display_name": "${display_name}",
     "env": {
         "LAUNCH_OPTS": "",
         "SPARK_HOME": "${spark_home}",
-        "SPARK_OPTS": "--master k8s://https://${KUBERNETES_SERVICE_HOST}:${KUBERNETES_SERVICE_PORT} --deploy-mode cluster --name ${KERNEL_USERNAME}-${KERNEL_ID} --conf spark.kubernetes.namespace=${KERNEL_NAMESPACE} --conf spark.kubernetes.driver.label.app=kubernetes-kernel-provider --conf spark.kubernetes.driver.label.kernel_id=${KERNEL_ID} --conf spark.kubernetes.driver.label.component=kernel --conf spark.kubernetes.executor.label.app=kubernetes-kernel-provider --conf spark.kubernetes.executor.label.kernel_id=${KERNEL_ID} --conf spark.kubernetes.executor.label.component=kernel --conf spark.kubernetes.driver.container.image=${KERNEL_IMAGE} --conf spark.kubernetes.executor.container.image=${KERNEL_EXECUTOR_IMAGE} --conf spark.kubernetes.authenticate.driver.serviceAccountName=${KERNEL_SERVICE_ACCOUNT_NAME} --conf spark.kubernetes.submission.waitAppCompletion=false ${extra_spark_opts} ${KERNEL_EXTRA_SPARK_OPTS}"
+        "SPARK_OPTS": "--master k8s://https://${KUBERNETES_SERVICE_HOST}:${KUBERNETES_SERVICE_PORT} --deploy-mode cluster --name ${KERNEL_USERNAME}-${KERNEL_ID} --conf spark.kubernetes.namespace=${KERNEL_NAMESPACE} --conf spark.kubernetes.driver.label.app=kubernetes-kernel-provider --conf spark.kubernetes.driver.label.kernel_id=${KERNEL_ID} --conf spark.kubernetes.driver.label.component=kernel --conf spark.kubernetes.executor.label.app=kubernetes-kernel-provider --conf spark.kubernetes.executor.label.kernel_id=${KERNEL_ID} --conf spark.kubernetes.executor.label.component=worker --conf spark.kubernetes.driver.container.image=${KERNEL_IMAGE} --conf spark.kubernetes.executor.container.image=${KERNEL_EXECUTOR_IMAGE} --conf spark.kubernetes.authenticate.driver.serviceAccountName=${KERNEL_SERVICE_ACCOUNT_NAME} --conf spark.kubernetes.submission.waitAppCompletion=false ${extra_spark_opts} ${KERNEL_EXTRA_SPARK_OPTS}"
     },
     "language": "${language}",
     "metadata": {
         "kernel_provisioner": {
             "config": {
                 "executor_image_name": "${executor_image_name}",
                 "image_name": "${image_name}"
```

### Comparing `gateway_provisioners-0.1.0/gateway_provisioners/kernel-specs/k8s_r_spark/bin/run.sh` & `gateway_provisioners-0.2.0/gateway_provisioners/kernel-specs/k8s_r_spark/bin/run.sh`

 * *Files identical despite different names*

### Comparing `gateway_provisioners-0.1.0/gateway_provisioners/kernel-specs/k8s_scala_spark/kernel.json` & `gateway_provisioners-0.2.0/gateway_provisioners/kernel-specs/k8s_scala_spark/kernel.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.99%*

 * *Differences: {"'env'": "{'__TOREE_SPARK_OPTS__': '--master "*

 * *          'k8s://https://${KUBERNETES_SERVICE_HOST}:${KUBERNETES_SERVICE_PORT} --deploy-mode '*

 * *          'cluster --name ${KERNEL_USERNAME}-${KERNEL_ID} --conf '*

 * *          'spark.kubernetes.namespace=${KERNEL_NAMESPACE} --driver-memory 2G --conf '*

 * *          'spark.kubernetes.driver.label.app=kubernetes-kernel-provider --conf '*

 * *          'spark.kubernetes.driver.label.kernel_id=${KERNEL_ID} --conf '*

 * *          'spark.kubernetes.driver.label.component=kernel --co […]*

```diff
@@ -14,15 +14,15 @@
     ],
     "display_name": "${display_name}",
     "env": {
         "DEFAULT_INTERPRETER": "Scala",
         "LAUNCH_OPTS": "",
         "SPARK_HOME": "${spark_home}",
         "__TOREE_OPTS__": "--alternate-sigint USR2",
-        "__TOREE_SPARK_OPTS__": "--master k8s://https://${KUBERNETES_SERVICE_HOST}:${KUBERNETES_SERVICE_PORT} --deploy-mode cluster --name ${KERNEL_USERNAME}-${KERNEL_ID} --conf spark.kubernetes.namespace=${KERNEL_NAMESPACE} --driver-memory 2G --conf spark.kubernetes.driver.label.app=kubernetes-kernel-provider --conf spark.kubernetes.driver.label.kernel_id=${KERNEL_ID} --conf spark.kubernetes.driver.label.component=kernel --conf spark.kubernetes.executor.label.app=kubernetes-kernel-provider --conf spark.kubernetes.executor.label.kernel_id=${KERNEL_ID} --conf spark.kubernetes.executor.label.component=kernel --conf spark.kubernetes.driver.container.image=${KERNEL_IMAGE} --conf spark.kubernetes.executor.container.image=${KERNEL_EXECUTOR_IMAGE} --conf spark.kubernetes.authenticate.driver.serviceAccountName=${KERNEL_SERVICE_ACCOUNT_NAME} --conf spark.kubernetes.submission.waitAppCompletion=false ${extra_spark_opts} ${KERNEL_EXTRA_SPARK_OPTS}"
+        "__TOREE_SPARK_OPTS__": "--master k8s://https://${KUBERNETES_SERVICE_HOST}:${KUBERNETES_SERVICE_PORT} --deploy-mode cluster --name ${KERNEL_USERNAME}-${KERNEL_ID} --conf spark.kubernetes.namespace=${KERNEL_NAMESPACE} --driver-memory 2G --conf spark.kubernetes.driver.label.app=kubernetes-kernel-provider --conf spark.kubernetes.driver.label.kernel_id=${KERNEL_ID} --conf spark.kubernetes.driver.label.component=kernel --conf spark.kubernetes.executor.label.app=kubernetes-kernel-provider --conf spark.kubernetes.executor.label.kernel_id=${KERNEL_ID} --conf spark.kubernetes.executor.label.component=worker --conf spark.kubernetes.driver.container.image=${KERNEL_IMAGE} --conf spark.kubernetes.executor.container.image=${KERNEL_EXECUTOR_IMAGE} --conf spark.kubernetes.authenticate.driver.serviceAccountName=${KERNEL_SERVICE_ACCOUNT_NAME} --conf spark.kubernetes.submission.waitAppCompletion=false ${extra_spark_opts} ${KERNEL_EXTRA_SPARK_OPTS}"
     },
     "language": "${language}",
     "metadata": {
         "kernel_provisioner": {
             "config": {
                 "executor_image_name": "${executor_image_name}",
                 "image_name": "${image_name}"
```

### Comparing `gateway_provisioners-0.1.0/gateway_provisioners/kernel-specs/k8s_scala_spark/bin/run.sh` & `gateway_provisioners-0.2.0/gateway_provisioners/kernel-specs/k8s_scala_spark/bin/run.sh`

 * *Files identical despite different names*

### Comparing `gateway_provisioners-0.1.0/gateway_provisioners/kernel-specs/ssh_python/kernel.json` & `gateway_provisioners-0.2.0/gateway_provisioners/kernel-specs/ssh_python/kernel.json`

 * *Files identical despite different names*

### Comparing `gateway_provisioners-0.1.0/gateway_provisioners/kernel-specs/ssh_python_spark/kernel.json` & `gateway_provisioners-0.2.0/gateway_provisioners/kernel-specs/ssh_python_spark/kernel.json`

 * *Files identical despite different names*

### Comparing `gateway_provisioners-0.1.0/gateway_provisioners/kernel-specs/ssh_python_spark/bin/run.sh` & `gateway_provisioners-0.2.0/gateway_provisioners/kernel-specs/ssh_python_spark/bin/run.sh`

 * *Files identical despite different names*

### Comparing `gateway_provisioners-0.1.0/gateway_provisioners/kernel-specs/ssh_r_spark/kernel.json` & `gateway_provisioners-0.2.0/gateway_provisioners/kernel-specs/ssh_r_spark/kernel.json`

 * *Files identical despite different names*

### Comparing `gateway_provisioners-0.1.0/gateway_provisioners/kernel-specs/ssh_r_spark/bin/run.sh` & `gateway_provisioners-0.2.0/gateway_provisioners/kernel-specs/ssh_r_spark/bin/run.sh`

 * *Files identical despite different names*

### Comparing `gateway_provisioners-0.1.0/gateway_provisioners/kernel-specs/ssh_scala/kernel.json` & `gateway_provisioners-0.2.0/gateway_provisioners/kernel-specs/ssh_scala/kernel.json`

 * *Files identical despite different names*

### Comparing `gateway_provisioners-0.1.0/gateway_provisioners/kernel-specs/ssh_scala/bin/run.sh` & `gateway_provisioners-0.2.0/gateway_provisioners/kernel-specs/ssh_scala/bin/run.sh`

 * *Files identical despite different names*

### Comparing `gateway_provisioners-0.1.0/gateway_provisioners/kernel-specs/ssh_scala_spark/kernel.json` & `gateway_provisioners-0.2.0/gateway_provisioners/kernel-specs/ssh_scala_spark/kernel.json`

 * *Files identical despite different names*

### Comparing `gateway_provisioners-0.1.0/gateway_provisioners/kernel-specs/ssh_scala_spark/bin/run.sh` & `gateway_provisioners-0.2.0/gateway_provisioners/kernel-specs/ssh_scala_spark/bin/run.sh`

 * *Files identical despite different names*

### Comparing `gateway_provisioners-0.1.0/gateway_provisioners/kernel-specs/yarn_dask_python/kernel.json` & `gateway_provisioners-0.2.0/gateway_provisioners/kernel-specs/yarn_dask_python/kernel.json`

 * *Files identical despite different names*

### Comparing `gateway_provisioners-0.1.0/gateway_provisioners/kernel-specs/yarn_dask_python/bin/run.sh` & `gateway_provisioners-0.2.0/gateway_provisioners/kernel-specs/yarn_dask_python/bin/run.sh`

 * *Files identical despite different names*

### Comparing `gateway_provisioners-0.1.0/gateway_provisioners/kernel-specs/yarn_spark_python/kernel.json` & `gateway_provisioners-0.2.0/gateway_provisioners/kernel-specs/yarn_spark_python/kernel.json`

 * *Files identical despite different names*

### Comparing `gateway_provisioners-0.1.0/gateway_provisioners/kernel-specs/yarn_spark_python/bin/run.sh` & `gateway_provisioners-0.2.0/gateway_provisioners/kernel-specs/yarn_spark_python/bin/run.sh`

 * *Files identical despite different names*

### Comparing `gateway_provisioners-0.1.0/gateway_provisioners/kernel-specs/yarn_spark_r/kernel.json` & `gateway_provisioners-0.2.0/gateway_provisioners/kernel-specs/yarn_spark_r/kernel.json`

 * *Files identical despite different names*

### Comparing `gateway_provisioners-0.1.0/gateway_provisioners/kernel-specs/yarn_spark_r/bin/run.sh` & `gateway_provisioners-0.2.0/gateway_provisioners/kernel-specs/yarn_spark_r/bin/run.sh`

 * *Files identical despite different names*

### Comparing `gateway_provisioners-0.1.0/gateway_provisioners/kernel-specs/yarn_spark_scala/kernel.json` & `gateway_provisioners-0.2.0/gateway_provisioners/kernel-specs/yarn_spark_scala/kernel.json`

 * *Files identical despite different names*

### Comparing `gateway_provisioners-0.1.0/gateway_provisioners/kernel-specs/yarn_spark_scala/bin/run.sh` & `gateway_provisioners-0.2.0/gateway_provisioners/kernel-specs/yarn_spark_scala/bin/run.sh`

 * *Files identical despite different names*

### Comparing `gateway_provisioners-0.1.0/tests/conftest.py` & `gateway_provisioners-0.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gateway_provisioners-0.1.0/tests/test_docker_provisioners.py` & `gateway_provisioners-0.2.0/tests/test_docker_provisioners.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 
 
 @pytest.mark.parametrize(
     "name,seed_env",
     [("docker", {"KERNEL_USERNAME": TEST_USER}), ("docker-swarm", {"KERNEL_USERNAME": TEST_USER})],
 )
 async def test_lifecycle(init_api_mocks, response_manager, get_provisioner, name, seed_env):
-
     kernel_id = str(uuid4())
     validator = ValidatorBase.create_instance(
         name, seed_env, kernel_id=kernel_id, response_manager=response_manager
     )
     os.environ.update(seed_env)
 
     provisioner = get_provisioner(name, kernel_id)
```

### Comparing `gateway_provisioners-0.1.0/tests/test_k8s_provisioners.py` & `gateway_provisioners-0.2.0/tests/test_k8s_provisioners.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import pytest
 from jupyter_client import KernelConnectionInfo
 from validators import TEST_USER, K8sValidator
 
 
 @pytest.mark.parametrize("seed_env", [{"KERNEL_USERNAME": TEST_USER}])
 async def test_lifecycle(init_api_mocks, response_manager, get_provisioner, seed_env):
-
     name = "kubernetes"
     kernel_id = str(uuid4())
     validator = K8sValidator.create_instance(
         name, seed_env, kernel_id=kernel_id, response_manager=response_manager
     )
     os.environ.update(seed_env)
```

### Comparing `gateway_provisioners-0.1.0/tests/test_yarn_provisioners.py` & `gateway_provisioners-0.2.0/tests/test_yarn_provisioners.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,14 @@
     "GP_YARN_ENDPOINT": "my-yarn-cluster.acme.com:7777",
     "GP_ALT_YARN_ENDPOINT": "my-yarn-cluster.acme.com:8888",
 }
 
 
 @pytest.mark.parametrize("seed_env", [YARN_SEED_ENV])
 async def test_lifecycle(init_api_mocks, response_manager, get_provisioner, seed_env):
-
     name = "yarn"
     kernel_id = str(uuid4())
     validator = YarnValidator.create_instance(
         name, seed_env, kernel_id=kernel_id, response_manager=response_manager
     )
     os.environ.update(seed_env)
```

### Comparing `gateway_provisioners-0.1.0/tests/validators.py` & `gateway_provisioners-0.2.0/tests/validators.py`

 * *Files identical despite different names*

### Comparing `gateway_provisioners-0.1.0/tests/mocks/docker_client.py` & `gateway_provisioners-0.2.0/tests/mocks/docker_client.py`

 * *Files identical despite different names*

### Comparing `gateway_provisioners-0.1.0/tests/mocks/k8s_client.py` & `gateway_provisioners-0.2.0/tests/mocks/k8s_client.py`

 * *Files identical despite different names*

### Comparing `gateway_provisioners-0.1.0/tests/mocks/popen.py` & `gateway_provisioners-0.2.0/tests/mocks/popen.py`

 * *Files identical despite different names*

### Comparing `gateway_provisioners-0.1.0/tests/mocks/response_manager.py` & `gateway_provisioners-0.2.0/tests/mocks/response_manager.py`

 * *Files identical despite different names*

### Comparing `gateway_provisioners-0.1.0/tests/mocks/yarn_client.py` & `gateway_provisioners-0.2.0/tests/mocks/yarn_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,14 @@
         elif app:
             self.data["app"] = app
         elif status:
             self.data["status"] = status
 
 
 class MockResourceManager:
-
     CLUSTER_CONTAINER_MEMORY = 1024 * 1024 * 1024  # 1GB
 
     def __init__(self, **kwargs):
         self.endpoints = kwargs.get("service_endpoints")
 
     def get_active_endpoint(self):
         assert len(self.endpoints) > 0
```

### Comparing `gateway_provisioners-0.1.0/.gitignore` & `gateway_provisioners-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `gateway_provisioners-0.1.0/LICENSE.md` & `gateway_provisioners-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gateway_provisioners-0.1.0/README.md` & `gateway_provisioners-0.2.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 # Gateway Provisioners
 
-[![Build Status](https://github.com/gateway-experiments/gateway_provisioners/actions/workflows/build.yml/badge.svg?query=branch%3Amain++)](https://github.com/gateway-experiments/gateway_provisioners/actions/workflows/build.yml/badge.svg?query=branch%3Amain++)
+[![Build Status](https://github.com/jupyter-server/gateway_provisioners/actions/workflows/build.yml/badge.svg?query=branch%3Amain++)](https://github.com/jupyter-server/gateway_provisioners/actions/workflows/build.yml/badge.svg?query=branch%3Amain++)
 [![Documentation Status](https://readthedocs.org/projects/gateway_provisioners/badge/?version=latest)](https://gateway-provisioners.readthedocs.io/en/latest/?badge=latest)
 
-**NOTE: This repository is experimental and undergoing frequent changes!**
-
 Gateway Provisioners provides [kernel provisioners](https://jupyter-client.readthedocs.io/en/latest/provisioning.html)
 that interact with kernels launched into resource-managed clusters or otherwise run remotely from the launching server.
 This functionality derives from [Jupyter Enterprise Gateway's](https://github.com/jupyter-server/enterprise_gateway)
-_process proxy_ architecture. However, unlike \[process proxies\]
-(https://jupyter-enterprise-gateway.readthedocs.io/en/latest/contributors/system-architecture.html#process-proxy),
+_process proxy_ architecture. However, unlike [process proxies](https://jupyter-enterprise-gateway.readthedocs.io/en/latest/contributors/system-architecture.html#process-proxy),
 you do not need to use a gateway server to use these provisioners - although, in certain cases,
 it is recommended (for example when the launching server does not reside within the same network as the launched kernel).
 
 Here is the current set of provisioners provided by this package, many of which have their requirements conditionally
 installed:
 
 - `KubernetesProvisioner` - Kernels (residing in images) are launched as pods within a Kubernetes cluster
   - `pip install gateway_provisioners[k8s]`
 - `DockerSwarmProvisioner` - Kernels (residing in images) are launched as containers within a DockerSwarm cluster
-- `DockerProvisioner` - Kernels (residing in images) are launched as containers
+- `DockerProvisioner` - Kernels (residing in images) are launched as containers on the local server
   - `pip install gateway_provisioners[docker]`
 - `YarnProvisioner` - Kernels are launched into a Hadoop YARN cluster (primarily Spark)
   - `pip install gateway_provisioners[yarn]`
 - `DistributedProvisioner` - Kernels are launched across a set of hosts using SSH, round-robin
   - `pip install gateway_provisioners`
 
 This package also includes command-line utilities that can be used to create kernel specifications or inject bootstrap
@@ -31,37 +28,39 @@
 
 - `jupyter-k8s-spec` - for building kernel specifications relative to the `KubernetesProvisioner`
 - `jupyter-docker-spec` - for building kernel specifications relative to `DockerProvisioner` and `DockerSwarmProvisioner`
 - `jupyter-yarn-spec` - for building kernel specifications relative to the `YarnProvisioner`
 - `jupyter-ssh-spec` - for building kernel specifications relative to the `DistributedProvisioner`
 - `jupyter-image-bootstrap` - for injecting bootstrap support when building kernel-based images
 
-**NOTE: The container-based provisioners (`KubernetesProvisioner`, `DockerSwarmProvisioner`, and `DockerProvisioner`)
-require that the hosting server also be running within the same environment/network. As a result, these
-provisioners may be better suited for use by a Gateway Server (Kernel Gateway or Enterprise Gateway) so
-as to not require the Notebook/Lab server to be in a container.**
+**Note:** The container-based provisioners (`KubernetesProvisioner`, `DockerSwarmProvisioner`, and `DockerProvisioner`)
+require that the hosting server also be running within the same environment/network. As a result, these provisioners
+may be better suited for use by a Gateway Server (e.g., [Jupyter Kernel Gateway](https://github.com/jupyter-server/kernel_gateway))
+so as to not require the Notebook/Lab server also be deployed in a container.
+
+______________________________________________________________________
 
 ## Installation
 
-Detailed installation instructions are located in the
-[Operators Guide](https://gateway-provisioners.readthedocs.io/en/latest/operators/installing-gp.html)
+Detailed deployment instructions are located in the
+[Operators Guide](https://gateway-provisioners.readthedocs.io/en/latest/operators/index.html)
 of the project docs. Here's a quick start using `pip`:
 
 ```bash
 # install from pypi
 pip install --upgrade gateway-provisioners
 
 # options for the command-line utilities can be viewed using '--help-all'
-jupyter k8s-spec install --help-all
+jupyter yarn-spec install --help-all
 
-# run it with default options
-jupyter k8s-spec install
+# run it with default options to install a Python-based kernelspec for Hadoop Yarn
+jupyter yarn-spec install
 ```
 
 ## Contributing
 
 The [Contribution page](https://gateway-provisioners.readthedocs.io/en/latest/contributors/contrib.html) includes
-information about how to contribute to Gateway Provisioners. We encourage you to explore the other topics in our \[Contributor's Guide\]
-(https://gateway-provisioners.readthedocs.io/en/latest/contributors/index.html)
+information about how to contribute to Gateway Provisioners. We encourage you to explore the other topics in our
+[Contributors Guide](https://gateway-provisioners.readthedocs.io/en/latest/contributors/index.html)
 like how to [set up a development environment](https://gateway-provisioners.readthedocs.io/en/latest/contributors/devinstall.html),
-gaining an understanding of the [system architecture](https://gateway-provisioners.readthedocs.io/en/latest/contributors/system-architecture.html),
-and taking a look at the \[API documentation\[(https://gateway-provisioners.readthedocs.io/en/latest/api/modules.html), among other thigns.
+or gaining an understanding of the [system architecture](https://gateway-provisioners.readthedocs.io/en/latest/contributors/system-architecture.html),
+among other things.
```

### Comparing `gateway_provisioners-0.1.0/pyproject.toml` & `gateway_provisioners-0.2.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -30,23 +30,22 @@
 name = "Jupyter Development Team"
 email = "jupyter@googlegroups.org"
 
 [project.readme]
 file = "README.md"
 content-type = "text/markdown"
 
-
 [project.license]
 file = "LICENSE.md"
 
 [project.urls]
 Homepage = "https://jupyter.org"
 Documentation = "https://gateway-provisioners.readthedocs.io/"
-Source = "https://github.com/gateway-experiments/gateway_provisioners"
-Tracker = "https://github.com/gateway-experiments/gateway_provisioners/issues"
+Source = "https://github.com/jupyter-server/gateway_provisioners"
+Tracker = "https://github.com/jupyter-server/gateway_provisioners/issues"
 
 [project.optional-dependencies]
 test = [
   "importlib_metadata",
   "mock",
   "pre-commit",
   "pytest",
@@ -57,24 +56,24 @@
   # Install optional dependencies so all modules will load during collection
   "docker>=3.5.0",
   "yarn-api-client",
   "kubernetes>=18.20.0",
   "jinja2>=3.1",
 ]
 docs = [
-  "mistune<3",
+  "docutils<0.20",
+  "mistune<3.0.0",
   "myst-parser",
   "pydata_sphinx_theme",
-  "sphinx",
   "sphinx-copybutton",
-  "sphinx-markdown-tables",
-  "sphinx_book_theme",
-  "sphinxcontrib-mermaid",
   "sphinxcontrib-openapi",
+  "sphinxcontrib-blockdiag",
+  "sphinxcontrib-seqdiag",
   "sphinxcontrib_github_alt",
+  "sphinxcontrib-spelling",
   "sphinx-autodoc-typehints",
   "sphinxemoji",
   "tornado",
   # Install optional dependencies so all API modules will load
   "docker>=3.5.0",
   "yarn-api-client",
   "kubernetes>=18.20.0",
@@ -82,16 +81,18 @@
 ]
 dev = [
   "coverage",
   "pre-commit",
   "build",
   "twine",
 ]
-kerberos = [
-
+lint = [
+  "black[jupyter]==23.3.0",
+  "mdformat>0.7",
+  "ruff==0.0.261",
 ]
 yarn = [
     "yarn-api-client"
 ]
 k8s = [
     "kubernetes>=18.20.0",
     "jinja2>=3.1"
@@ -107,35 +108,62 @@
 jupyter-docker-spec = "gateway_provisioners.cli.docker_specapp:DockerProvisionerApp.launch_instance"
 jupyter-image-bootstrap = "gateway_provisioners.cli.image_bootstrapapp:ImageBootstrapApp.launch_instance"
 
 [project.entry-points."jupyter_client.kernel_provisioners"]
 yarn-provisioner = "gateway_provisioners.yarn:YarnProvisioner"
 distributed-provisioner = "gateway_provisioners.distributed:DistributedProvisioner"
 kubernetes-provisioner = "gateway_provisioners.k8s:KubernetesProvisioner"
+spark-operator-provisioner = "gateway_provisioners.spark_operator:SparkOperatorProvisioner"
 docker-provisioner = "gateway_provisioners.docker_swarm:DockerProvisioner"
 docker-swarm-provisioner = "gateway_provisioners.docker_swarm:DockerSwarmProvisioner"
 
 [tool.hatch.version]
 path = "gateway_provisioners/_version.py"
+validate-bump = false
 
 [tool.hatch.build]
 artifacts = ["gateway_provisioners/kernel-launchers/scala/lib"]
 
+[tool.hatch.envs.build]
+features = ["dev"]
+[tool.hatch.envs.build.scripts]
+clean = "make clean"
+lint = "make lint"
+dist = "make dist"
+all = "make clean lint dist install"
+
 [tool.hatch.envs.docs]
 features = ["docs"]
 [tool.hatch.envs.docs.scripts]
 build = "make -C docs html SPHINXOPTS='-W'"
 api = "sphinx-apidoc -o docs/source/api -f -E gateway_provisioners"
 
 [tool.hatch.envs.test]
 features = ["test"]
 [tool.hatch.envs.test.scripts]
 test = "python -m pytest -vv {args}"
 nowarn = "test -W default {args}"
 
+[tool.hatch.envs.lint]
+features = ["lint"]
+[tool.hatch.envs.lint.scripts]
+style = [
+  "ruff {args:.}",
+  "black --check --diff {args:.}",
+  "mdformat --check {args:docs/source *.md}"
+]
+fmt = [
+  "black {args:.}",
+  "ruff --fix {args:.}",
+  "mdformat {args:docs/source *.md}"
+]
+
+[tool.jupyter-releaser.hooks]
+before-build-python = ["pip install -e .[dev]", "make clean lint dist install"]
+
 [tool.jupyter-releaser.options]
 post-version-spec = "dev"
 
 [tool.mypy]
 check_untyped_defs = true
 disallow_any_generics = false
 disallow_incomplete_defs = true
@@ -182,49 +210,55 @@
 target-version = "py38"
 line-length = 100
 select = [
   "A", "B", "C", "E", "EM", "F", "FBT", "I", "N", "Q", "RUF", "S", "T",
   "UP", "W", "YTT",
 ]
 ignore = [
+  # A001/A002/A003 .. is shadowing a python builtin
+  "A001",
+  "A002",
+  "A003",
   # Allow non-abstract empty methods in abstract base classes
   "B027",
   # Ignore McCabe complexity
   "C901",
-  # Allow boolean positional values in function calls, like `dict.get(... True)`
-  "FBT003",
-  # Use of `assert` detected
-  "S101",
+  # Module level import not at top of file
+  "E402",
   # Line too long
   "E501",
-  # Relative imports are banned
-  "TID252",
   # Boolean ... in function definition
   "FBT001",
   "FBT002",
-  # Module level import not at top of file
-  "E402",
-  # A001/A002/A003 .. is shadowing a python builtin
-  "A001",
-  "A002",
-  "A003",
-  # Possible hardcoded password
-  "S105",
-  "S106",
+  # Allow boolean positional values in function calls, like `dict.get(... True)`
+  "FBT003",
   # Variable `xxx` in function should be lowercase
   "N806",
   # Exception name `KernelSessionRecordConflict` should be named with an Error suffix
   "N818",
+  # Use of `assert` detected
+  "S101",
+  # Possible hardcoded password
+  "S105",
+  "S106",
+  # Standard pseudo-random generators are not suitable for security/cryptographic purposes. (Used for port selection)
+  "S311",
+  # Relative imports are banned
+  "TID252",
 ]
 unfixable = [
   # Don't touch print statements
   "T201",
   # Don't touch unused imports
   "F401",
   # Don't touch noqa lines
   "RUF100",
 ]
 [tool.ruff.per-file-ignores]
 # T201 `print` found
 "gateway_provisioners/cli/*" = ["T201"]
+"gateway_provisioners/kernel-launchers/*" = ["T201"]
 # N802 Function name should be lowercase
 "tests/mocks/k8s_client.py" = ["N802"]
+
+[tool.check-wheel-contents]
+ignore = ["W002", "W004"]
```

### Comparing `gateway_provisioners-0.1.0/PKG-INFO` & `gateway_provisioners-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: gateway_provisioners
-Version: 0.1.0
+Version: 0.2.0
 Summary: Gateway Provisioners - a package containing kernel provisioners supporting the deployment of remote and resource-managed kernels.
 Project-URL: Homepage, https://jupyter.org
 Project-URL: Documentation, https://gateway-provisioners.readthedocs.io/
-Project-URL: Source, https://github.com/gateway-experiments/gateway_provisioners
-Project-URL: Tracker, https://github.com/gateway-experiments/gateway_provisioners/issues
+Project-URL: Source, https://github.com/jupyter-server/gateway_provisioners
+Project-URL: Tracker, https://github.com/jupyter-server/gateway_provisioners/issues
 Author-email: Jupyter Development Team <jupyter@googlegroups.org>
 License: # Licensing terms
         
         This project is licensed under the terms of the Modified BSD License
         (also known as New or Revised or 3-Clause BSD), as follows:
         
         - Copyright (c) 2001-2015, IPython Development Team
@@ -91,34 +91,37 @@
 Requires-Dist: coverage; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
 Requires-Dist: twine; extra == 'dev'
 Provides-Extra: docker
 Requires-Dist: docker>=3.5.0; extra == 'docker'
 Provides-Extra: docs
 Requires-Dist: docker>=3.5.0; extra == 'docs'
+Requires-Dist: docutils<0.20; extra == 'docs'
 Requires-Dist: jinja2>=3.1; extra == 'docs'
 Requires-Dist: kubernetes>=18.20.0; extra == 'docs'
-Requires-Dist: mistune<3; extra == 'docs'
+Requires-Dist: mistune<3.0.0; extra == 'docs'
 Requires-Dist: myst-parser; extra == 'docs'
 Requires-Dist: pydata-sphinx-theme; extra == 'docs'
-Requires-Dist: sphinx; extra == 'docs'
 Requires-Dist: sphinx-autodoc-typehints; extra == 'docs'
-Requires-Dist: sphinx-book-theme; extra == 'docs'
 Requires-Dist: sphinx-copybutton; extra == 'docs'
-Requires-Dist: sphinx-markdown-tables; extra == 'docs'
+Requires-Dist: sphinxcontrib-blockdiag; extra == 'docs'
 Requires-Dist: sphinxcontrib-github-alt; extra == 'docs'
-Requires-Dist: sphinxcontrib-mermaid; extra == 'docs'
 Requires-Dist: sphinxcontrib-openapi; extra == 'docs'
+Requires-Dist: sphinxcontrib-seqdiag; extra == 'docs'
+Requires-Dist: sphinxcontrib-spelling; extra == 'docs'
 Requires-Dist: sphinxemoji; extra == 'docs'
 Requires-Dist: tornado; extra == 'docs'
 Requires-Dist: yarn-api-client; extra == 'docs'
 Provides-Extra: k8s
 Requires-Dist: jinja2>=3.1; extra == 'k8s'
 Requires-Dist: kubernetes>=18.20.0; extra == 'k8s'
-Provides-Extra: kerberos
+Provides-Extra: lint
+Requires-Dist: black[jupyter]==23.3.0; extra == 'lint'
+Requires-Dist: mdformat>0.7; extra == 'lint'
+Requires-Dist: ruff==0.0.261; extra == 'lint'
 Provides-Extra: test
 Requires-Dist: docker>=3.5.0; extra == 'test'
 Requires-Dist: importlib-metadata; extra == 'test'
 Requires-Dist: jinja2>=3.1; extra == 'test'
 Requires-Dist: kubernetes>=18.20.0; extra == 'test'
 Requires-Dist: mock; extra == 'test'
 Requires-Dist: pre-commit; extra == 'test'
@@ -130,34 +133,31 @@
 Requires-Dist: yarn-api-client; extra == 'test'
 Provides-Extra: yarn
 Requires-Dist: yarn-api-client; extra == 'yarn'
 Description-Content-Type: text/markdown
 
 # Gateway Provisioners
 
-[![Build Status](https://github.com/gateway-experiments/gateway_provisioners/actions/workflows/build.yml/badge.svg?query=branch%3Amain++)](https://github.com/gateway-experiments/gateway_provisioners/actions/workflows/build.yml/badge.svg?query=branch%3Amain++)
+[![Build Status](https://github.com/jupyter-server/gateway_provisioners/actions/workflows/build.yml/badge.svg?query=branch%3Amain++)](https://github.com/jupyter-server/gateway_provisioners/actions/workflows/build.yml/badge.svg?query=branch%3Amain++)
 [![Documentation Status](https://readthedocs.org/projects/gateway_provisioners/badge/?version=latest)](https://gateway-provisioners.readthedocs.io/en/latest/?badge=latest)
 
-**NOTE: This repository is experimental and undergoing frequent changes!**
-
 Gateway Provisioners provides [kernel provisioners](https://jupyter-client.readthedocs.io/en/latest/provisioning.html)
 that interact with kernels launched into resource-managed clusters or otherwise run remotely from the launching server.
 This functionality derives from [Jupyter Enterprise Gateway's](https://github.com/jupyter-server/enterprise_gateway)
-_process proxy_ architecture. However, unlike \[process proxies\]
-(https://jupyter-enterprise-gateway.readthedocs.io/en/latest/contributors/system-architecture.html#process-proxy),
+_process proxy_ architecture. However, unlike [process proxies](https://jupyter-enterprise-gateway.readthedocs.io/en/latest/contributors/system-architecture.html#process-proxy),
 you do not need to use a gateway server to use these provisioners - although, in certain cases,
 it is recommended (for example when the launching server does not reside within the same network as the launched kernel).
 
 Here is the current set of provisioners provided by this package, many of which have their requirements conditionally
 installed:
 
 - `KubernetesProvisioner` - Kernels (residing in images) are launched as pods within a Kubernetes cluster
   - `pip install gateway_provisioners[k8s]`
 - `DockerSwarmProvisioner` - Kernels (residing in images) are launched as containers within a DockerSwarm cluster
-- `DockerProvisioner` - Kernels (residing in images) are launched as containers
+- `DockerProvisioner` - Kernels (residing in images) are launched as containers on the local server
   - `pip install gateway_provisioners[docker]`
 - `YarnProvisioner` - Kernels are launched into a Hadoop YARN cluster (primarily Spark)
   - `pip install gateway_provisioners[yarn]`
 - `DistributedProvisioner` - Kernels are launched across a set of hosts using SSH, round-robin
   - `pip install gateway_provisioners`
 
 This package also includes command-line utilities that can be used to create kernel specifications or inject bootstrap
@@ -165,37 +165,39 @@
 
 - `jupyter-k8s-spec` - for building kernel specifications relative to the `KubernetesProvisioner`
 - `jupyter-docker-spec` - for building kernel specifications relative to `DockerProvisioner` and `DockerSwarmProvisioner`
 - `jupyter-yarn-spec` - for building kernel specifications relative to the `YarnProvisioner`
 - `jupyter-ssh-spec` - for building kernel specifications relative to the `DistributedProvisioner`
 - `jupyter-image-bootstrap` - for injecting bootstrap support when building kernel-based images
 
-**NOTE: The container-based provisioners (`KubernetesProvisioner`, `DockerSwarmProvisioner`, and `DockerProvisioner`)
-require that the hosting server also be running within the same environment/network. As a result, these
-provisioners may be better suited for use by a Gateway Server (Kernel Gateway or Enterprise Gateway) so
-as to not require the Notebook/Lab server to be in a container.**
+**Note:** The container-based provisioners (`KubernetesProvisioner`, `DockerSwarmProvisioner`, and `DockerProvisioner`)
+require that the hosting server also be running within the same environment/network. As a result, these provisioners
+may be better suited for use by a Gateway Server (e.g., [Jupyter Kernel Gateway](https://github.com/jupyter-server/kernel_gateway))
+so as to not require the Notebook/Lab server also be deployed in a container.
+
+______________________________________________________________________
 
 ## Installation
 
-Detailed installation instructions are located in the
-[Operators Guide](https://gateway-provisioners.readthedocs.io/en/latest/operators/installing-gp.html)
+Detailed deployment instructions are located in the
+[Operators Guide](https://gateway-provisioners.readthedocs.io/en/latest/operators/index.html)
 of the project docs. Here's a quick start using `pip`:
 
 ```bash
 # install from pypi
 pip install --upgrade gateway-provisioners
 
 # options for the command-line utilities can be viewed using '--help-all'
-jupyter k8s-spec install --help-all
+jupyter yarn-spec install --help-all
 
-# run it with default options
-jupyter k8s-spec install
+# run it with default options to install a Python-based kernelspec for Hadoop Yarn
+jupyter yarn-spec install
 ```
 
 ## Contributing
 
 The [Contribution page](https://gateway-provisioners.readthedocs.io/en/latest/contributors/contrib.html) includes
-information about how to contribute to Gateway Provisioners. We encourage you to explore the other topics in our \[Contributor's Guide\]
-(https://gateway-provisioners.readthedocs.io/en/latest/contributors/index.html)
+information about how to contribute to Gateway Provisioners. We encourage you to explore the other topics in our
+[Contributors Guide](https://gateway-provisioners.readthedocs.io/en/latest/contributors/index.html)
 like how to [set up a development environment](https://gateway-provisioners.readthedocs.io/en/latest/contributors/devinstall.html),
-gaining an understanding of the [system architecture](https://gateway-provisioners.readthedocs.io/en/latest/contributors/system-architecture.html),
-and taking a look at the \[API documentation\[(https://gateway-provisioners.readthedocs.io/en/latest/api/modules.html), among other thigns.
+or gaining an understanding of the [system architecture](https://gateway-provisioners.readthedocs.io/en/latest/contributors/system-architecture.html),
+among other things.
```

