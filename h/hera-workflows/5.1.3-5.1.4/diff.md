# Comparing `tmp/hera_workflows-5.1.3.tar.gz` & `tmp/hera_workflows-5.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hera_workflows-5.1.3.tar", max compression
+gzip compressed data, was "hera_workflows-5.1.4.tar", max compression
```

## Comparing `hera_workflows-5.1.3.tar` & `hera_workflows-5.1.4.tar`

### file list

```diff
@@ -1,132 +1,132 @@
--rw-r--r--   0        0        0     1066 2023-04-15 21:34:41.499745 hera_workflows-5.1.3/LICENSE
--rw-r--r--   0        0        0    11696 2023-04-15 21:34:41.499745 hera_workflows-5.1.3/README.md
--rw-r--r--   0        0        0     3540 2023-04-15 21:35:04.008046 hera_workflows-5.1.3/pyproject.toml
--rw-r--r--   0        0        0      522 2023-04-15 21:34:41.511745 hera_workflows-5.1.3/src/hera/__init__.py
--rw-r--r--   0        0        0      310 2023-04-15 21:35:04.008046 hera_workflows-5.1.3/src/hera/_version.py
--rw-r--r--   0        0        0        0 2023-04-15 21:34:41.511745 hera_workflows-5.1.3/src/hera/events/__init__.py
--rw-r--r--   0        0        0     3267 2023-04-15 21:34:41.511745 hera_workflows-5.1.3/src/hera/events/models/__init__.py
--rw-r--r--   0        0        0     1418 2023-04-15 21:34:41.511745 hera_workflows-5.1.3/src/hera/events/models/eventsource.py
--rw-r--r--   0        0        0      861 2023-04-15 21:34:41.511745 hera_workflows-5.1.3/src/hera/events/models/eventsource.pyi
--rw-r--r--   0        0        0      144 2023-04-15 21:34:41.511745 hera_workflows-5.1.3/src/hera/events/models/google/__init__.py
--rw-r--r--   0        0        0      347 2023-04-15 21:34:41.511745 hera_workflows-5.1.3/src/hera/events/models/google/protobuf.py
--rw-r--r--   0        0        0      164 2023-04-15 21:34:41.511745 hera_workflows-5.1.3/src/hera/events/models/google/protobuf.pyi
--rw-r--r--   0        0        0        0 2023-04-15 21:34:41.511745 hera_workflows-5.1.3/src/hera/events/models/grpc/__init__.py
--rw-r--r--   0        0        0      144 2023-04-15 21:34:41.511745 hera_workflows-5.1.3/src/hera/events/models/grpc/gateway/__init__.py
--rw-r--r--   0        0        0      691 2023-04-15 21:34:41.511745 hera_workflows-5.1.3/src/hera/events/models/grpc/gateway/runtime.py
--rw-r--r--   0        0        0      470 2023-04-15 21:34:41.511745 hera_workflows-5.1.3/src/hera/events/models/grpc/gateway/runtime.pyi
--rw-r--r--   0        0        0        0 2023-04-15 21:34:41.511745 hera_workflows-5.1.3/src/hera/events/models/io/__init__.py
--rw-r--r--   0        0        0        0 2023-04-15 21:34:41.511745 hera_workflows-5.1.3/src/hera/events/models/io/argoproj/__init__.py
--rw-r--r--   0        0        0      144 2023-04-15 21:34:41.511745 hera_workflows-5.1.3/src/hera/events/models/io/argoproj/events/__init__.py
--rw-r--r--   0        0        0   102993 2023-04-15 21:34:41.511745 hera_workflows-5.1.3/src/hera/events/models/io/argoproj/events/v1alpha1.py
--rw-r--r--   0        0        0    25271 2023-04-15 21:34:41.511745 hera_workflows-5.1.3/src/hera/events/models/io/argoproj/events/v1alpha1.pyi
--rw-r--r--   0        0        0      144 2023-04-15 21:34:41.511745 hera_workflows-5.1.3/src/hera/events/models/io/argoproj/workflow/__init__.py
--rw-r--r--   0        0        0   144549 2023-04-15 21:34:41.511745 hera_workflows-5.1.3/src/hera/events/models/io/argoproj/workflow/v1alpha1.py
--rw-r--r--   0        0        0    31958 2023-04-15 21:34:41.511745 hera_workflows-5.1.3/src/hera/events/models/io/argoproj/workflow/v1alpha1.pyi
--rw-r--r--   0        0        0        0 2023-04-15 21:34:41.511745 hera_workflows-5.1.3/src/hera/events/models/io/k8s/__init__.py
--rw-r--r--   0        0        0        0 2023-04-15 21:34:41.511745 hera_workflows-5.1.3/src/hera/events/models/io/k8s/api/__init__.py
--rw-r--r--   0        0        0      144 2023-04-15 21:34:41.511745 hera_workflows-5.1.3/src/hera/events/models/io/k8s/api/core/__init__.py
--rw-r--r--   0        0        0   127883 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/events/models/io/k8s/api/core/v1.py
--rw-r--r--   0        0        0    18004 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/events/models/io/k8s/api/core/v1.pyi
--rw-r--r--   0        0        0      144 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/events/models/io/k8s/api/policy/__init__.py
--rw-r--r--   0        0        0     1751 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/events/models/io/k8s/api/policy/v1beta1.py
--rw-r--r--   0        0        0      376 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/events/models/io/k8s/api/policy/v1beta1.pyi
--rw-r--r--   0        0        0        0 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/events/models/io/k8s/apimachinery/__init__.py
--rw-r--r--   0        0        0        0 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/events/models/io/k8s/apimachinery/pkg/__init__.py
--rw-r--r--   0        0        0      144 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/events/models/io/k8s/apimachinery/pkg/api/__init__.py
--rw-r--r--   0        0        0     3161 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/events/models/io/k8s/apimachinery/pkg/api/resource.py
--rw-r--r--   0        0        0      105 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/events/models/io/k8s/apimachinery/pkg/api/resource.pyi
--rw-r--r--   0        0        0        0 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/events/models/io/k8s/apimachinery/pkg/apis/__init__.py
--rw-r--r--   0        0        0      144 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/__init__.py
--rw-r--r--   0        0        0    22218 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.py
--rw-r--r--   0        0        0     2064 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi
--rw-r--r--   0        0        0      144 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/events/models/io/k8s/apimachinery/pkg/util/__init__.py
--rw-r--r--   0        0        0      277 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/events/models/io/k8s/apimachinery/pkg/util/intstr.py
--rw-r--r--   0        0        0      108 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/events/models/io/k8s/apimachinery/pkg/util/intstr.pyi
--rw-r--r--   0        0        0     1453 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/events/models/sensor.py
--rw-r--r--   0        0        0      887 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/events/models/sensor.pyi
--rw-r--r--   0        0        0    26908 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/events/service.py
--rw-r--r--   0        0        0      282 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/expr/__init__.py
--rw-r--r--   0        0        0    12021 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/expr/_node.py
--rw-r--r--   0        0        0      647 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/expr/_sprig.py
--rw-r--r--   0        0        0        0 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/py.typed
--rw-r--r--   0        0        0      188 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/shared/__init__.py
--rw-r--r--   0        0        0      269 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/shared/_base_model.py
--rw-r--r--   0        0        0     4927 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/shared/_global_config.py
--rw-r--r--   0        0        0      513 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/shared/serialization.py
--rw-r--r--   0        0        0     4413 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/__init__.py
--rw-r--r--   0        0        0     2298 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/_context.py
--rw-r--r--   0        0        0    23829 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/_mixins.py
--rw-r--r--   0        0        0    32815 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/_unparse.py
--rw-r--r--   0        0        0       25 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/action.py
--rw-r--r--   0        0        0     1115 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/archive.py
--rw-r--r--   0        0        0     7697 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/artifact.py
--rw-r--r--   0        0        0     3446 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/container.py
--rw-r--r--   0        0        0     3988 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/container_set.py
--rw-r--r--   0        0        0     3763 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/cron_workflow.py
--rw-r--r--   0        0        0     2771 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/dag.py
--rw-r--r--   0        0        0     2186 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/data.py
--rw-r--r--   0        0        0     4855 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/env.py
--rw-r--r--   0        0        0     1329 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/env_from.py
--rw-r--r--   0        0        0      208 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/exceptions.py
--rw-r--r--   0        0        0     2291 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/http_template.py
--rw-r--r--   0        0        0       30 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/memoize.py
--rw-r--r--   0        0        0     6913 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/models/__init__.py
--rw-r--r--   0        0        0     1418 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/models/eventsource.py
--rw-r--r--   0        0        0      861 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/models/eventsource.pyi
--rw-r--r--   0        0        0      144 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/models/google/__init__.py
--rw-r--r--   0        0        0      347 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/models/google/protobuf.py
--rw-r--r--   0        0        0      164 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/models/google/protobuf.pyi
--rw-r--r--   0        0        0        0 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/models/grpc/__init__.py
--rw-r--r--   0        0        0      144 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/models/grpc/gateway/__init__.py
--rw-r--r--   0        0        0      691 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/models/grpc/gateway/runtime.py
--rw-r--r--   0        0        0      470 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/models/grpc/gateway/runtime.pyi
--rw-r--r--   0        0        0        0 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/models/io/__init__.py
--rw-r--r--   0        0        0        0 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/models/io/argoproj/__init__.py
--rw-r--r--   0        0        0      144 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/models/io/argoproj/events/__init__.py
--rw-r--r--   0        0        0   102993 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/models/io/argoproj/events/v1alpha1.py
--rw-r--r--   0        0        0    25271 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/models/io/argoproj/events/v1alpha1.pyi
--rw-r--r--   0        0        0      144 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/models/io/argoproj/workflow/__init__.py
--rw-r--r--   0        0        0   144549 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.py
--rw-r--r--   0        0        0    31958 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.pyi
--rw-r--r--   0        0        0        0 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/models/io/k8s/__init__.py
--rw-r--r--   0        0        0        0 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/models/io/k8s/api/__init__.py
--rw-r--r--   0        0        0      144 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/models/io/k8s/api/core/__init__.py
--rw-r--r--   0        0        0   127883 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/models/io/k8s/api/core/v1.py
--rw-r--r--   0        0        0    18004 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/models/io/k8s/api/core/v1.pyi
--rw-r--r--   0        0        0      144 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/models/io/k8s/api/policy/__init__.py
--rw-r--r--   0        0        0     1751 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/models/io/k8s/api/policy/v1beta1.py
--rw-r--r--   0        0        0      376 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/models/io/k8s/api/policy/v1beta1.pyi
--rw-r--r--   0        0        0        0 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/models/io/k8s/apimachinery/__init__.py
--rw-r--r--   0        0        0        0 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/models/io/k8s/apimachinery/pkg/__init__.py
--rw-r--r--   0        0        0      144 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/__init__.py
--rw-r--r--   0        0        0     3161 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/resource.py
--rw-r--r--   0        0        0      105 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/resource.pyi
--rw-r--r--   0        0        0        0 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/__init__.py
--rw-r--r--   0        0        0      144 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/__init__.py
--rw-r--r--   0        0        0    22218 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.py
--rw-r--r--   0        0        0     2064 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi
--rw-r--r--   0        0        0      144 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/models/io/k8s/apimachinery/pkg/util/__init__.py
--rw-r--r--   0        0        0      277 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/models/io/k8s/apimachinery/pkg/util/intstr.py
--rw-r--r--   0        0        0      108 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/models/io/k8s/apimachinery/pkg/util/intstr.pyi
--rw-r--r--   0        0        0     1453 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/models/sensor.py
--rw-r--r--   0        0        0      887 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/models/sensor.pyi
--rw-r--r--   0        0        0      722 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/operator.py
--rw-r--r--   0        0        0     4084 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/parameter.py
--rw-r--r--   0        0        0     1018 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/protocol.py
--rw-r--r--   0        0        0     2554 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/resource.py
--rw-r--r--   0        0        0     5262 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/resources.py
--rw-r--r--   0        0        0     1856 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/retry_strategy.py
--rw-r--r--   0        0        0     3707 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/runner.py
--rw-r--r--   0        0        0    14748 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/script.py
--rw-r--r--   0        0        0    49478 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/service.py
--rw-r--r--   0        0        0     9297 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/steps.py
--rw-r--r--   0        0        0     3266 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/suspend.py
--rw-r--r--   0        0        0    10495 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/task.py
--rw-r--r--   0        0        0       27 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/toleration.py
--rw-r--r--   0        0        0     2007 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/user_container.py
--rw-r--r--   0        0        0     2610 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/validators.py
--rw-r--r--   0        0        0    18656 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/volume.py
--rw-r--r--   0        0        0    15590 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/workflow.py
--rw-r--r--   0        0        0      911 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/workflow_status.py
--rw-r--r--   0        0        0     5925 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/workflow_template.py
--rw-r--r--   0        0        0    13280 1970-01-01 00:00:00.000000 hera_workflows-5.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-04-21 01:28:44.461436 hera_workflows-5.1.4/LICENSE
+-rw-r--r--   0        0        0    11696 2023-04-21 01:28:44.461436 hera_workflows-5.1.4/README.md
+-rw-r--r--   0        0        0     3540 2023-04-21 01:29:05.069782 hera_workflows-5.1.4/pyproject.toml
+-rw-r--r--   0        0        0      522 2023-04-21 01:28:44.473436 hera_workflows-5.1.4/src/hera/__init__.py
+-rw-r--r--   0        0        0      310 2023-04-21 01:29:05.073782 hera_workflows-5.1.4/src/hera/_version.py
+-rw-r--r--   0        0        0        0 2023-04-21 01:28:44.473436 hera_workflows-5.1.4/src/hera/events/__init__.py
+-rw-r--r--   0        0        0     3267 2023-04-21 01:28:44.473436 hera_workflows-5.1.4/src/hera/events/models/__init__.py
+-rw-r--r--   0        0        0     1418 2023-04-21 01:28:44.473436 hera_workflows-5.1.4/src/hera/events/models/eventsource.py
+-rw-r--r--   0        0        0      861 2023-04-21 01:28:44.473436 hera_workflows-5.1.4/src/hera/events/models/eventsource.pyi
+-rw-r--r--   0        0        0      144 2023-04-21 01:28:44.473436 hera_workflows-5.1.4/src/hera/events/models/google/__init__.py
+-rw-r--r--   0        0        0      347 2023-04-21 01:28:44.473436 hera_workflows-5.1.4/src/hera/events/models/google/protobuf.py
+-rw-r--r--   0        0        0      164 2023-04-21 01:28:44.473436 hera_workflows-5.1.4/src/hera/events/models/google/protobuf.pyi
+-rw-r--r--   0        0        0        0 2023-04-21 01:28:44.473436 hera_workflows-5.1.4/src/hera/events/models/grpc/__init__.py
+-rw-r--r--   0        0        0      144 2023-04-21 01:28:44.473436 hera_workflows-5.1.4/src/hera/events/models/grpc/gateway/__init__.py
+-rw-r--r--   0        0        0      691 2023-04-21 01:28:44.473436 hera_workflows-5.1.4/src/hera/events/models/grpc/gateway/runtime.py
+-rw-r--r--   0        0        0      470 2023-04-21 01:28:44.473436 hera_workflows-5.1.4/src/hera/events/models/grpc/gateway/runtime.pyi
+-rw-r--r--   0        0        0        0 2023-04-21 01:28:44.473436 hera_workflows-5.1.4/src/hera/events/models/io/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 01:28:44.473436 hera_workflows-5.1.4/src/hera/events/models/io/argoproj/__init__.py
+-rw-r--r--   0        0        0      144 2023-04-21 01:28:44.473436 hera_workflows-5.1.4/src/hera/events/models/io/argoproj/events/__init__.py
+-rw-r--r--   0        0        0   102993 2023-04-21 01:28:44.473436 hera_workflows-5.1.4/src/hera/events/models/io/argoproj/events/v1alpha1.py
+-rw-r--r--   0        0        0    25271 2023-04-21 01:28:44.473436 hera_workflows-5.1.4/src/hera/events/models/io/argoproj/events/v1alpha1.pyi
+-rw-r--r--   0        0        0      144 2023-04-21 01:28:44.473436 hera_workflows-5.1.4/src/hera/events/models/io/argoproj/workflow/__init__.py
+-rw-r--r--   0        0        0   144549 2023-04-21 01:28:44.473436 hera_workflows-5.1.4/src/hera/events/models/io/argoproj/workflow/v1alpha1.py
+-rw-r--r--   0        0        0    31958 2023-04-21 01:28:44.477436 hera_workflows-5.1.4/src/hera/events/models/io/argoproj/workflow/v1alpha1.pyi
+-rw-r--r--   0        0        0        0 2023-04-21 01:28:44.477436 hera_workflows-5.1.4/src/hera/events/models/io/k8s/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 01:28:44.477436 hera_workflows-5.1.4/src/hera/events/models/io/k8s/api/__init__.py
+-rw-r--r--   0        0        0      144 2023-04-21 01:28:44.477436 hera_workflows-5.1.4/src/hera/events/models/io/k8s/api/core/__init__.py
+-rw-r--r--   0        0        0   127883 2023-04-21 01:28:44.477436 hera_workflows-5.1.4/src/hera/events/models/io/k8s/api/core/v1.py
+-rw-r--r--   0        0        0    18004 2023-04-21 01:28:44.477436 hera_workflows-5.1.4/src/hera/events/models/io/k8s/api/core/v1.pyi
+-rw-r--r--   0        0        0      144 2023-04-21 01:28:44.477436 hera_workflows-5.1.4/src/hera/events/models/io/k8s/api/policy/__init__.py
+-rw-r--r--   0        0        0     1751 2023-04-21 01:28:44.477436 hera_workflows-5.1.4/src/hera/events/models/io/k8s/api/policy/v1beta1.py
+-rw-r--r--   0        0        0      376 2023-04-21 01:28:44.477436 hera_workflows-5.1.4/src/hera/events/models/io/k8s/api/policy/v1beta1.pyi
+-rw-r--r--   0        0        0        0 2023-04-21 01:28:44.477436 hera_workflows-5.1.4/src/hera/events/models/io/k8s/apimachinery/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 01:28:44.477436 hera_workflows-5.1.4/src/hera/events/models/io/k8s/apimachinery/pkg/__init__.py
+-rw-r--r--   0        0        0      144 2023-04-21 01:28:44.477436 hera_workflows-5.1.4/src/hera/events/models/io/k8s/apimachinery/pkg/api/__init__.py
+-rw-r--r--   0        0        0     3161 2023-04-21 01:28:44.477436 hera_workflows-5.1.4/src/hera/events/models/io/k8s/apimachinery/pkg/api/resource.py
+-rw-r--r--   0        0        0      105 2023-04-21 01:28:44.477436 hera_workflows-5.1.4/src/hera/events/models/io/k8s/apimachinery/pkg/api/resource.pyi
+-rw-r--r--   0        0        0        0 2023-04-21 01:28:44.477436 hera_workflows-5.1.4/src/hera/events/models/io/k8s/apimachinery/pkg/apis/__init__.py
+-rw-r--r--   0        0        0      144 2023-04-21 01:28:44.477436 hera_workflows-5.1.4/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/__init__.py
+-rw-r--r--   0        0        0    22218 2023-04-21 01:28:44.477436 hera_workflows-5.1.4/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.py
+-rw-r--r--   0        0        0     2064 2023-04-21 01:28:44.477436 hera_workflows-5.1.4/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi
+-rw-r--r--   0        0        0      144 2023-04-21 01:28:44.477436 hera_workflows-5.1.4/src/hera/events/models/io/k8s/apimachinery/pkg/util/__init__.py
+-rw-r--r--   0        0        0      277 2023-04-21 01:28:44.477436 hera_workflows-5.1.4/src/hera/events/models/io/k8s/apimachinery/pkg/util/intstr.py
+-rw-r--r--   0        0        0      108 2023-04-21 01:28:44.477436 hera_workflows-5.1.4/src/hera/events/models/io/k8s/apimachinery/pkg/util/intstr.pyi
+-rw-r--r--   0        0        0     1453 2023-04-21 01:28:44.477436 hera_workflows-5.1.4/src/hera/events/models/sensor.py
+-rw-r--r--   0        0        0      887 2023-04-21 01:28:44.477436 hera_workflows-5.1.4/src/hera/events/models/sensor.pyi
+-rw-r--r--   0        0        0    26811 2023-04-21 01:28:44.477436 hera_workflows-5.1.4/src/hera/events/service.py
+-rw-r--r--   0        0        0      282 2023-04-21 01:28:44.477436 hera_workflows-5.1.4/src/hera/expr/__init__.py
+-rw-r--r--   0        0        0    12021 2023-04-21 01:28:44.477436 hera_workflows-5.1.4/src/hera/expr/_node.py
+-rw-r--r--   0        0        0      647 2023-04-21 01:28:44.477436 hera_workflows-5.1.4/src/hera/expr/_sprig.py
+-rw-r--r--   0        0        0        0 2023-04-21 01:28:44.477436 hera_workflows-5.1.4/src/hera/py.typed
+-rw-r--r--   0        0        0      188 2023-04-21 01:28:44.477436 hera_workflows-5.1.4/src/hera/shared/__init__.py
+-rw-r--r--   0        0        0      269 2023-04-21 01:28:44.477436 hera_workflows-5.1.4/src/hera/shared/_base_model.py
+-rw-r--r--   0        0        0     4927 2023-04-21 01:28:44.477436 hera_workflows-5.1.4/src/hera/shared/_global_config.py
+-rw-r--r--   0        0        0      513 2023-04-21 01:28:44.477436 hera_workflows-5.1.4/src/hera/shared/serialization.py
+-rw-r--r--   0        0        0     4413 2023-04-21 01:28:44.477436 hera_workflows-5.1.4/src/hera/workflows/__init__.py
+-rw-r--r--   0        0        0     2298 2023-04-21 01:28:44.477436 hera_workflows-5.1.4/src/hera/workflows/_context.py
+-rw-r--r--   0        0        0    23864 2023-04-21 01:28:44.477436 hera_workflows-5.1.4/src/hera/workflows/_mixins.py
+-rw-r--r--   0        0        0    32815 2023-04-21 01:28:44.477436 hera_workflows-5.1.4/src/hera/workflows/_unparse.py
+-rw-r--r--   0        0        0       25 2023-04-21 01:28:44.477436 hera_workflows-5.1.4/src/hera/workflows/action.py
+-rw-r--r--   0        0        0     1115 2023-04-21 01:28:44.477436 hera_workflows-5.1.4/src/hera/workflows/archive.py
+-rw-r--r--   0        0        0     7697 2023-04-21 01:28:44.477436 hera_workflows-5.1.4/src/hera/workflows/artifact.py
+-rw-r--r--   0        0        0     3446 2023-04-21 01:28:44.477436 hera_workflows-5.1.4/src/hera/workflows/container.py
+-rw-r--r--   0        0        0     3988 2023-04-21 01:28:44.477436 hera_workflows-5.1.4/src/hera/workflows/container_set.py
+-rw-r--r--   0        0        0     3763 2023-04-21 01:28:44.477436 hera_workflows-5.1.4/src/hera/workflows/cron_workflow.py
+-rw-r--r--   0        0        0     2771 2023-04-21 01:28:44.477436 hera_workflows-5.1.4/src/hera/workflows/dag.py
+-rw-r--r--   0        0        0     2186 2023-04-21 01:28:44.477436 hera_workflows-5.1.4/src/hera/workflows/data.py
+-rw-r--r--   0        0        0     4855 2023-04-21 01:28:44.477436 hera_workflows-5.1.4/src/hera/workflows/env.py
+-rw-r--r--   0        0        0     1329 2023-04-21 01:28:44.477436 hera_workflows-5.1.4/src/hera/workflows/env_from.py
+-rw-r--r--   0        0        0      208 2023-04-21 01:28:44.477436 hera_workflows-5.1.4/src/hera/workflows/exceptions.py
+-rw-r--r--   0        0        0     2291 2023-04-21 01:28:44.477436 hera_workflows-5.1.4/src/hera/workflows/http_template.py
+-rw-r--r--   0        0        0       30 2023-04-21 01:28:44.477436 hera_workflows-5.1.4/src/hera/workflows/memoize.py
+-rw-r--r--   0        0        0     6913 2023-04-21 01:28:44.477436 hera_workflows-5.1.4/src/hera/workflows/models/__init__.py
+-rw-r--r--   0        0        0     1418 2023-04-21 01:28:44.477436 hera_workflows-5.1.4/src/hera/workflows/models/eventsource.py
+-rw-r--r--   0        0        0      861 2023-04-21 01:28:44.477436 hera_workflows-5.1.4/src/hera/workflows/models/eventsource.pyi
+-rw-r--r--   0        0        0      144 2023-04-21 01:28:44.477436 hera_workflows-5.1.4/src/hera/workflows/models/google/__init__.py
+-rw-r--r--   0        0        0      347 2023-04-21 01:28:44.477436 hera_workflows-5.1.4/src/hera/workflows/models/google/protobuf.py
+-rw-r--r--   0        0        0      164 2023-04-21 01:28:44.477436 hera_workflows-5.1.4/src/hera/workflows/models/google/protobuf.pyi
+-rw-r--r--   0        0        0        0 2023-04-21 01:28:44.477436 hera_workflows-5.1.4/src/hera/workflows/models/grpc/__init__.py
+-rw-r--r--   0        0        0      144 2023-04-21 01:28:44.477436 hera_workflows-5.1.4/src/hera/workflows/models/grpc/gateway/__init__.py
+-rw-r--r--   0        0        0      691 2023-04-21 01:28:44.477436 hera_workflows-5.1.4/src/hera/workflows/models/grpc/gateway/runtime.py
+-rw-r--r--   0        0        0      470 2023-04-21 01:28:44.477436 hera_workflows-5.1.4/src/hera/workflows/models/grpc/gateway/runtime.pyi
+-rw-r--r--   0        0        0        0 2023-04-21 01:28:44.477436 hera_workflows-5.1.4/src/hera/workflows/models/io/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 01:28:44.477436 hera_workflows-5.1.4/src/hera/workflows/models/io/argoproj/__init__.py
+-rw-r--r--   0        0        0      144 2023-04-21 01:28:44.477436 hera_workflows-5.1.4/src/hera/workflows/models/io/argoproj/events/__init__.py
+-rw-r--r--   0        0        0   102993 2023-04-21 01:28:44.481436 hera_workflows-5.1.4/src/hera/workflows/models/io/argoproj/events/v1alpha1.py
+-rw-r--r--   0        0        0    25271 2023-04-21 01:28:44.481436 hera_workflows-5.1.4/src/hera/workflows/models/io/argoproj/events/v1alpha1.pyi
+-rw-r--r--   0        0        0      144 2023-04-21 01:28:44.481436 hera_workflows-5.1.4/src/hera/workflows/models/io/argoproj/workflow/__init__.py
+-rw-r--r--   0        0        0   144549 2023-04-21 01:28:44.481436 hera_workflows-5.1.4/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.py
+-rw-r--r--   0        0        0    31958 2023-04-21 01:28:44.481436 hera_workflows-5.1.4/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.pyi
+-rw-r--r--   0        0        0        0 2023-04-21 01:28:44.481436 hera_workflows-5.1.4/src/hera/workflows/models/io/k8s/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 01:28:44.481436 hera_workflows-5.1.4/src/hera/workflows/models/io/k8s/api/__init__.py
+-rw-r--r--   0        0        0      144 2023-04-21 01:28:44.481436 hera_workflows-5.1.4/src/hera/workflows/models/io/k8s/api/core/__init__.py
+-rw-r--r--   0        0        0   127883 2023-04-21 01:28:44.481436 hera_workflows-5.1.4/src/hera/workflows/models/io/k8s/api/core/v1.py
+-rw-r--r--   0        0        0    18004 2023-04-21 01:28:44.481436 hera_workflows-5.1.4/src/hera/workflows/models/io/k8s/api/core/v1.pyi
+-rw-r--r--   0        0        0      144 2023-04-21 01:28:44.481436 hera_workflows-5.1.4/src/hera/workflows/models/io/k8s/api/policy/__init__.py
+-rw-r--r--   0        0        0     1751 2023-04-21 01:28:44.481436 hera_workflows-5.1.4/src/hera/workflows/models/io/k8s/api/policy/v1beta1.py
+-rw-r--r--   0        0        0      376 2023-04-21 01:28:44.481436 hera_workflows-5.1.4/src/hera/workflows/models/io/k8s/api/policy/v1beta1.pyi
+-rw-r--r--   0        0        0        0 2023-04-21 01:28:44.481436 hera_workflows-5.1.4/src/hera/workflows/models/io/k8s/apimachinery/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 01:28:44.481436 hera_workflows-5.1.4/src/hera/workflows/models/io/k8s/apimachinery/pkg/__init__.py
+-rw-r--r--   0        0        0      144 2023-04-21 01:28:44.481436 hera_workflows-5.1.4/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/__init__.py
+-rw-r--r--   0        0        0     3161 2023-04-21 01:28:44.481436 hera_workflows-5.1.4/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/resource.py
+-rw-r--r--   0        0        0      105 2023-04-21 01:28:44.481436 hera_workflows-5.1.4/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/resource.pyi
+-rw-r--r--   0        0        0        0 2023-04-21 01:28:44.481436 hera_workflows-5.1.4/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/__init__.py
+-rw-r--r--   0        0        0      144 2023-04-21 01:28:44.481436 hera_workflows-5.1.4/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/__init__.py
+-rw-r--r--   0        0        0    22218 2023-04-21 01:28:44.481436 hera_workflows-5.1.4/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.py
+-rw-r--r--   0        0        0     2064 2023-04-21 01:28:44.481436 hera_workflows-5.1.4/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi
+-rw-r--r--   0        0        0      144 2023-04-21 01:28:44.481436 hera_workflows-5.1.4/src/hera/workflows/models/io/k8s/apimachinery/pkg/util/__init__.py
+-rw-r--r--   0        0        0      277 2023-04-21 01:28:44.481436 hera_workflows-5.1.4/src/hera/workflows/models/io/k8s/apimachinery/pkg/util/intstr.py
+-rw-r--r--   0        0        0      108 2023-04-21 01:28:44.481436 hera_workflows-5.1.4/src/hera/workflows/models/io/k8s/apimachinery/pkg/util/intstr.pyi
+-rw-r--r--   0        0        0     1453 2023-04-21 01:28:44.481436 hera_workflows-5.1.4/src/hera/workflows/models/sensor.py
+-rw-r--r--   0        0        0      887 2023-04-21 01:28:44.481436 hera_workflows-5.1.4/src/hera/workflows/models/sensor.pyi
+-rw-r--r--   0        0        0      722 2023-04-21 01:28:44.481436 hera_workflows-5.1.4/src/hera/workflows/operator.py
+-rw-r--r--   0        0        0     4084 2023-04-21 01:28:44.481436 hera_workflows-5.1.4/src/hera/workflows/parameter.py
+-rw-r--r--   0        0        0     1018 2023-04-21 01:28:44.481436 hera_workflows-5.1.4/src/hera/workflows/protocol.py
+-rw-r--r--   0        0        0     2554 2023-04-21 01:28:44.481436 hera_workflows-5.1.4/src/hera/workflows/resource.py
+-rw-r--r--   0        0        0     5262 2023-04-21 01:28:44.481436 hera_workflows-5.1.4/src/hera/workflows/resources.py
+-rw-r--r--   0        0        0     1856 2023-04-21 01:28:44.481436 hera_workflows-5.1.4/src/hera/workflows/retry_strategy.py
+-rw-r--r--   0        0        0     3707 2023-04-21 01:28:44.481436 hera_workflows-5.1.4/src/hera/workflows/runner.py
+-rw-r--r--   0        0        0    14748 2023-04-21 01:28:44.481436 hera_workflows-5.1.4/src/hera/workflows/script.py
+-rw-r--r--   0        0        0    49251 2023-04-21 01:28:44.481436 hera_workflows-5.1.4/src/hera/workflows/service.py
+-rw-r--r--   0        0        0     9297 2023-04-21 01:28:44.481436 hera_workflows-5.1.4/src/hera/workflows/steps.py
+-rw-r--r--   0        0        0     3266 2023-04-21 01:28:44.481436 hera_workflows-5.1.4/src/hera/workflows/suspend.py
+-rw-r--r--   0        0        0    10501 2023-04-21 01:28:44.481436 hera_workflows-5.1.4/src/hera/workflows/task.py
+-rw-r--r--   0        0        0       27 2023-04-21 01:28:44.481436 hera_workflows-5.1.4/src/hera/workflows/toleration.py
+-rw-r--r--   0        0        0     2007 2023-04-21 01:28:44.481436 hera_workflows-5.1.4/src/hera/workflows/user_container.py
+-rw-r--r--   0        0        0     2610 2023-04-21 01:28:44.481436 hera_workflows-5.1.4/src/hera/workflows/validators.py
+-rw-r--r--   0        0        0    18656 2023-04-21 01:28:44.481436 hera_workflows-5.1.4/src/hera/workflows/volume.py
+-rw-r--r--   0        0        0    15590 2023-04-21 01:28:44.481436 hera_workflows-5.1.4/src/hera/workflows/workflow.py
+-rw-r--r--   0        0        0      911 2023-04-21 01:28:44.481436 hera_workflows-5.1.4/src/hera/workflows/workflow_status.py
+-rw-r--r--   0        0        0     5925 2023-04-21 01:28:44.481436 hera_workflows-5.1.4/src/hera/workflows/workflow_template.py
+-rw-r--r--   0        0        0    13280 1970-01-01 00:00:00.000000 hera_workflows-5.1.4/PKG-INFO
```

### Comparing `hera_workflows-5.1.3/LICENSE` & `hera_workflows-5.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/README.md` & `hera_workflows-5.1.4/README.md`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/pyproject.toml` & `hera_workflows-5.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "hera-workflows"  # project-name
 # The version is automatically substituted by the CI
-version = "5.1.3"
+version = "5.1.4"
 description = "Hera is a Python framework for constructing and submitting Argo Workflows. The main goal of Hera is to make Argo Workflows more accessible by abstracting away some setup that is typically necessary for constructing Argo workflows."
 authors = ["Flaviu Vadan <flaviu.vadan@dynotx.com>", "Sambhav Kothari <sambhavs.email@gmail.com>", "Elliot Gunton <elliotgunton@gmail.com>"]
 maintainers = ["Flaviu Vadan <flaviu.vadan@dynotx.com>", "Sambhav Kothari <sambhavs.email@gmail.com>", "Elliot Gunton <elliotgunton@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/argoproj-labs/hera"
 repository = "https://github.com/argoproj-labs/hera"
```

### Comparing `hera_workflows-5.1.3/src/hera/__init__.py` & `hera_workflows-5.1.4/src/hera/__init__.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/events/models/__init__.py` & `hera_workflows-5.1.4/src/hera/events/models/__init__.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/events/models/eventsource.py` & `hera_workflows-5.1.4/src/hera/events/models/eventsource.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/events/models/eventsource.pyi` & `hera_workflows-5.1.4/src/hera/events/models/eventsource.pyi`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/events/models/grpc/gateway/runtime.py` & `hera_workflows-5.1.4/src/hera/events/models/grpc/gateway/runtime.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/events/models/io/argoproj/events/v1alpha1.py` & `hera_workflows-5.1.4/src/hera/events/models/io/argoproj/events/v1alpha1.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/events/models/io/argoproj/events/v1alpha1.pyi` & `hera_workflows-5.1.4/src/hera/events/models/io/argoproj/events/v1alpha1.pyi`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/events/models/io/argoproj/workflow/v1alpha1.py` & `hera_workflows-5.1.4/src/hera/events/models/io/argoproj/workflow/v1alpha1.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/events/models/io/argoproj/workflow/v1alpha1.pyi` & `hera_workflows-5.1.4/src/hera/events/models/io/argoproj/workflow/v1alpha1.pyi`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/events/models/io/k8s/api/core/v1.py` & `hera_workflows-5.1.4/src/hera/events/models/io/k8s/api/core/v1.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/events/models/io/k8s/api/core/v1.pyi` & `hera_workflows-5.1.4/src/hera/events/models/io/k8s/api/core/v1.pyi`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/events/models/io/k8s/api/policy/v1beta1.py` & `hera_workflows-5.1.4/src/hera/events/models/io/k8s/api/policy/v1beta1.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/events/models/io/k8s/apimachinery/pkg/api/resource.py` & `hera_workflows-5.1.4/src/hera/events/models/io/k8s/apimachinery/pkg/api/resource.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.py` & `hera_workflows-5.1.4/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi` & `hera_workflows-5.1.4/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/events/models/sensor.py` & `hera_workflows-5.1.4/src/hera/events/models/sensor.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/events/models/sensor.pyi` & `hera_workflows-5.1.4/src/hera/events/models/sensor.pyi`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/events/service.py` & `hera_workflows-5.1.4/src/hera/events/service.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import os
 from typing import Optional, cast
+from urllib.parse import urljoin
 
 import requests
 
 from hera.events.models import (
     CreateEventSourceRequest,
     CreateSensorRequest,
     DeleteSensorResponse,
@@ -51,15 +51,15 @@
         resource_version: Optional[str] = None,
         resource_version_match: Optional[str] = None,
         timeout_seconds: Optional[str] = None,
         limit: Optional[str] = None,
         continue_: Optional[str] = None,
     ) -> EventSourceList:
         resp = requests.get(
-            url=os.path.join(self.host, "api/v1/event-sources/{namespace}").format(
+            url=urljoin(self.host, "api/v1/event-sources/{namespace}").format(
                 namespace=namespace if namespace is not None else self.namespace
             ),
             params={
                 "listOptions.labelSelector": label_selector,
                 "listOptions.fieldSelector": field_selector,
                 "listOptions.watch": watch,
                 "listOptions.allowWatchBookmarks": allow_watch_bookmarks,
@@ -77,15 +77,15 @@
         if resp.ok:
             return EventSourceList(**resp.json())
         else:
             raise Exception(f"Server returned status code {resp.status_code} with error: {resp.json()}")
 
     def create_event_source(self, req: CreateEventSourceRequest, namespace: Optional[str] = None) -> EventSource:
         resp = requests.post(
-            url=os.path.join(self.host, "api/v1/event-sources/{namespace}").format(
+            url=urljoin(self.host, "api/v1/event-sources/{namespace}").format(
                 namespace=namespace if namespace is not None else self.namespace
             ),
             params=None,
             headers={"Authorization": f"Bearer {self.token}"},
             data=req.json(
                 exclude_none=True, by_alias=True, skip_defaults=True, exclude_unset=True, exclude_defaults=True
             ),
@@ -95,15 +95,15 @@
         if resp.ok:
             return EventSource(**resp.json())
         else:
             raise Exception(f"Server returned status code {resp.status_code} with error: {resp.json()}")
 
     def get_event_source(self, name: str, namespace: Optional[str] = None) -> EventSource:
         resp = requests.get(
-            url=os.path.join(self.host, "api/v1/event-sources/{namespace}/{name}").format(
+            url=urljoin(self.host, "api/v1/event-sources/{namespace}/{name}").format(
                 name=name, namespace=namespace if namespace is not None else self.namespace
             ),
             params=None,
             headers={"Authorization": f"Bearer {self.token}"},
             data=None,
             verify=self.verify_ssl,
         )
@@ -113,15 +113,15 @@
         else:
             raise Exception(f"Server returned status code {resp.status_code} with error: {resp.json()}")
 
     def update_event_source(
         self, name: str, req: UpdateEventSourceRequest, namespace: Optional[str] = None
     ) -> EventSource:
         resp = requests.put(
-            url=os.path.join(self.host, "api/v1/event-sources/{namespace}/{name}").format(
+            url=urljoin(self.host, "api/v1/event-sources/{namespace}/{name}").format(
                 name=name, namespace=namespace if namespace is not None else self.namespace
             ),
             params=None,
             headers={"Authorization": f"Bearer {self.token}"},
             data=req.json(
                 exclude_none=True, by_alias=True, skip_defaults=True, exclude_unset=True, exclude_defaults=True
             ),
@@ -141,15 +141,15 @@
         uid: Optional[str] = None,
         resource_version: Optional[str] = None,
         orphan_dependents: Optional[bool] = None,
         propagation_policy: Optional[str] = None,
         dry_run: Optional[list] = None,
     ) -> EventSourceDeletedResponse:
         resp = requests.delete(
-            url=os.path.join(self.host, "api/v1/event-sources/{namespace}/{name}").format(
+            url=urljoin(self.host, "api/v1/event-sources/{namespace}/{name}").format(
                 name=name, namespace=namespace if namespace is not None else self.namespace
             ),
             params={
                 "deleteOptions.gracePeriodSeconds": grace_period_seconds,
                 "deleteOptions.preconditions.uid": uid,
                 "deleteOptions.preconditions.resourceVersion": resource_version,
                 "deleteOptions.orphanDependents": orphan_dependents,
@@ -164,15 +164,15 @@
         if resp.ok:
             return EventSourceDeletedResponse()
         else:
             raise Exception(f"Server returned status code {resp.status_code} with error: {resp.json()}")
 
     def receive_event(self, discriminator: str, req: Item, namespace: Optional[str] = None) -> EventResponse:
         resp = requests.post(
-            url=os.path.join(self.host, "api/v1/events/{namespace}/{discriminator}").format(
+            url=urljoin(self.host, "api/v1/events/{namespace}/{discriminator}").format(
                 discriminator=discriminator, namespace=namespace if namespace is not None else self.namespace
             ),
             params=None,
             headers={"Authorization": f"Bearer {self.token}"},
             data=req.json(
                 exclude_none=True, by_alias=True, skip_defaults=True, exclude_unset=True, exclude_defaults=True
             ),
@@ -182,15 +182,15 @@
         if resp.ok:
             return EventResponse()
         else:
             raise Exception(f"Server returned status code {resp.status_code} with error: {resp.json()}")
 
     def get_info(self) -> InfoResponse:
         resp = requests.get(
-            url=os.path.join(self.host, "api/v1/info"),
+            url=urljoin(self.host, "api/v1/info"),
             params=None,
             headers={"Authorization": f"Bearer {self.token}"},
             data=None,
             verify=self.verify_ssl,
         )
 
         if resp.ok:
@@ -208,15 +208,15 @@
         resource_version: Optional[str] = None,
         resource_version_match: Optional[str] = None,
         timeout_seconds: Optional[str] = None,
         limit: Optional[str] = None,
         continue_: Optional[str] = None,
     ) -> SensorList:
         resp = requests.get(
-            url=os.path.join(self.host, "api/v1/sensors/{namespace}").format(
+            url=urljoin(self.host, "api/v1/sensors/{namespace}").format(
                 namespace=namespace if namespace is not None else self.namespace
             ),
             params={
                 "listOptions.labelSelector": label_selector,
                 "listOptions.fieldSelector": field_selector,
                 "listOptions.watch": watch,
                 "listOptions.allowWatchBookmarks": allow_watch_bookmarks,
@@ -234,15 +234,15 @@
         if resp.ok:
             return SensorList(**resp.json())
         else:
             raise Exception(f"Server returned status code {resp.status_code} with error: {resp.json()}")
 
     def create_sensor(self, req: CreateSensorRequest, namespace: Optional[str] = None) -> Sensor:
         resp = requests.post(
-            url=os.path.join(self.host, "api/v1/sensors/{namespace}").format(
+            url=urljoin(self.host, "api/v1/sensors/{namespace}").format(
                 namespace=namespace if namespace is not None else self.namespace
             ),
             params=None,
             headers={"Authorization": f"Bearer {self.token}"},
             data=req.json(
                 exclude_none=True, by_alias=True, skip_defaults=True, exclude_unset=True, exclude_defaults=True
             ),
@@ -252,15 +252,15 @@
         if resp.ok:
             return Sensor(**resp.json())
         else:
             raise Exception(f"Server returned status code {resp.status_code} with error: {resp.json()}")
 
     def get_sensor(self, name: str, namespace: Optional[str] = None, resource_version: Optional[str] = None) -> Sensor:
         resp = requests.get(
-            url=os.path.join(self.host, "api/v1/sensors/{namespace}/{name}").format(
+            url=urljoin(self.host, "api/v1/sensors/{namespace}/{name}").format(
                 name=name, namespace=namespace if namespace is not None else self.namespace
             ),
             params={"getOptions.resourceVersion": resource_version},
             headers={"Authorization": f"Bearer {self.token}"},
             data=None,
             verify=self.verify_ssl,
         )
@@ -268,15 +268,15 @@
         if resp.ok:
             return Sensor(**resp.json())
         else:
             raise Exception(f"Server returned status code {resp.status_code} with error: {resp.json()}")
 
     def update_sensor(self, name: str, req: UpdateSensorRequest, namespace: Optional[str] = None) -> Sensor:
         resp = requests.put(
-            url=os.path.join(self.host, "api/v1/sensors/{namespace}/{name}").format(
+            url=urljoin(self.host, "api/v1/sensors/{namespace}/{name}").format(
                 name=name, namespace=namespace if namespace is not None else self.namespace
             ),
             params=None,
             headers={"Authorization": f"Bearer {self.token}"},
             data=req.json(
                 exclude_none=True, by_alias=True, skip_defaults=True, exclude_unset=True, exclude_defaults=True
             ),
@@ -296,15 +296,15 @@
         uid: Optional[str] = None,
         resource_version: Optional[str] = None,
         orphan_dependents: Optional[bool] = None,
         propagation_policy: Optional[str] = None,
         dry_run: Optional[list] = None,
     ) -> DeleteSensorResponse:
         resp = requests.delete(
-            url=os.path.join(self.host, "api/v1/sensors/{namespace}/{name}").format(
+            url=urljoin(self.host, "api/v1/sensors/{namespace}/{name}").format(
                 name=name, namespace=namespace if namespace is not None else self.namespace
             ),
             params={
                 "deleteOptions.gracePeriodSeconds": grace_period_seconds,
                 "deleteOptions.preconditions.uid": uid,
                 "deleteOptions.preconditions.resourceVersion": resource_version,
                 "deleteOptions.orphanDependents": orphan_dependents,
@@ -331,15 +331,15 @@
         resource_version: Optional[str] = None,
         resource_version_match: Optional[str] = None,
         timeout_seconds: Optional[str] = None,
         limit: Optional[str] = None,
         continue_: Optional[str] = None,
     ) -> EventSourceWatchEvent:
         resp = requests.get(
-            url=os.path.join(self.host, "api/v1/stream/event-sources/{namespace}").format(
+            url=urljoin(self.host, "api/v1/stream/event-sources/{namespace}").format(
                 namespace=namespace if namespace is not None else self.namespace
             ),
             params={
                 "listOptions.labelSelector": label_selector,
                 "listOptions.fieldSelector": field_selector,
                 "listOptions.watch": watch,
                 "listOptions.allowWatchBookmarks": allow_watch_bookmarks,
@@ -374,15 +374,15 @@
         nanos: Optional[int] = None,
         timestamps: Optional[bool] = None,
         tail_lines: Optional[str] = None,
         limit_bytes: Optional[str] = None,
         insecure_skip_tls_verify_backend: Optional[bool] = None,
     ) -> EventsourceLogEntry:
         resp = requests.get(
-            url=os.path.join(self.host, "api/v1/stream/event-sources/{namespace}/logs").format(
+            url=urljoin(self.host, "api/v1/stream/event-sources/{namespace}/logs").format(
                 namespace=namespace if namespace is not None else self.namespace
             ),
             params={
                 "name": name,
                 "eventSourceType": event_source_type,
                 "eventName": event_name,
                 "grep": grep,
@@ -417,15 +417,15 @@
         resource_version: Optional[str] = None,
         resource_version_match: Optional[str] = None,
         timeout_seconds: Optional[str] = None,
         limit: Optional[str] = None,
         continue_: Optional[str] = None,
     ) -> Event:
         resp = requests.get(
-            url=os.path.join(self.host, "api/v1/stream/events/{namespace}").format(
+            url=urljoin(self.host, "api/v1/stream/events/{namespace}").format(
                 namespace=namespace if namespace is not None else self.namespace
             ),
             params={
                 "listOptions.labelSelector": label_selector,
                 "listOptions.fieldSelector": field_selector,
                 "listOptions.watch": watch,
                 "listOptions.allowWatchBookmarks": allow_watch_bookmarks,
@@ -455,15 +455,15 @@
         resource_version: Optional[str] = None,
         resource_version_match: Optional[str] = None,
         timeout_seconds: Optional[str] = None,
         limit: Optional[str] = None,
         continue_: Optional[str] = None,
     ) -> SensorWatchEvent:
         resp = requests.get(
-            url=os.path.join(self.host, "api/v1/stream/sensors/{namespace}").format(
+            url=urljoin(self.host, "api/v1/stream/sensors/{namespace}").format(
                 namespace=namespace if namespace is not None else self.namespace
             ),
             params={
                 "listOptions.labelSelector": label_selector,
                 "listOptions.fieldSelector": field_selector,
                 "listOptions.watch": watch,
                 "listOptions.allowWatchBookmarks": allow_watch_bookmarks,
@@ -497,15 +497,15 @@
         nanos: Optional[int] = None,
         timestamps: Optional[bool] = None,
         tail_lines: Optional[str] = None,
         limit_bytes: Optional[str] = None,
         insecure_skip_tls_verify_backend: Optional[bool] = None,
     ) -> SensorLogEntry:
         resp = requests.get(
-            url=os.path.join(self.host, "api/v1/stream/sensors/{namespace}/logs").format(
+            url=urljoin(self.host, "api/v1/stream/sensors/{namespace}/logs").format(
                 namespace=namespace if namespace is not None else self.namespace
             ),
             params={
                 "name": name,
                 "triggerName": trigger_name,
                 "grep": grep,
                 "podLogOptions.container": container,
@@ -527,29 +527,29 @@
         if resp.ok:
             return SensorLogEntry(**resp.json())
         else:
             raise Exception(f"Server returned status code {resp.status_code} with error: {resp.json()}")
 
     def get_user_info(self) -> GetUserInfoResponse:
         resp = requests.get(
-            url=os.path.join(self.host, "api/v1/userinfo"),
+            url=urljoin(self.host, "api/v1/userinfo"),
             params=None,
             headers={"Authorization": f"Bearer {self.token}"},
             data=None,
             verify=self.verify_ssl,
         )
 
         if resp.ok:
             return GetUserInfoResponse()
         else:
             raise Exception(f"Server returned status code {resp.status_code} with error: {resp.json()}")
 
     def get_version(self) -> Version:
         resp = requests.get(
-            url=os.path.join(self.host, "api/v1/version"),
+            url=urljoin(self.host, "api/v1/version"),
             params=None,
             headers={"Authorization": f"Bearer {self.token}"},
             data=None,
             verify=self.verify_ssl,
         )
 
         if resp.ok:
@@ -564,15 +564,15 @@
         node_id: str,
         artifact_name: str,
         artifact_discriminator: str,
         namespace: Optional[str] = None,
     ) -> str:
         """Get an artifact."""
         resp = requests.get(
-            url=os.path.join(
+            url=urljoin(
                 self.host,
                 "artifact-files/{namespace}/{idDiscriminator}/{id}/{nodeId}/{artifactDiscriminator}/{artifactName}",
             ).format(
                 idDiscriminator=id_discriminator,
                 id=id_,
                 nodeId=node_id,
                 artifactName=artifact_name,
@@ -589,15 +589,15 @@
             return str(resp.content)
         else:
             raise Exception(f"Server returned status code {resp.status_code} with error: {resp.json()}")
 
     def get_output_artifact_by_uid(self, uid: str, node_id: str, artifact_name: str) -> str:
         """Get an output artifact by UID."""
         resp = requests.get(
-            url=os.path.join(self.host, "artifacts-by-uid/{uid}/{nodeId}/{artifactName}").format(
+            url=urljoin(self.host, "artifacts-by-uid/{uid}/{nodeId}/{artifactName}").format(
                 uid=uid, nodeId=node_id, artifactName=artifact_name
             ),
             params=None,
             headers={"Authorization": f"Bearer {self.token}"},
             data=None,
             verify=self.verify_ssl,
         )
@@ -606,15 +606,15 @@
             return str(resp.content)
         else:
             raise Exception(f"Server returned status code {resp.status_code} with error: {resp.json()}")
 
     def get_output_artifact(self, name: str, node_id: str, artifact_name: str, namespace: Optional[str] = None) -> str:
         """Get an output artifact."""
         resp = requests.get(
-            url=os.path.join(self.host, "artifacts/{namespace}/{name}/{nodeId}/{artifactName}").format(
+            url=urljoin(self.host, "artifacts/{namespace}/{name}/{nodeId}/{artifactName}").format(
                 name=name,
                 nodeId=node_id,
                 artifactName=artifact_name,
                 namespace=namespace if namespace is not None else self.namespace,
             ),
             params=None,
             headers={"Authorization": f"Bearer {self.token}"},
@@ -626,15 +626,15 @@
             return str(resp.content)
         else:
             raise Exception(f"Server returned status code {resp.status_code} with error: {resp.json()}")
 
     def get_input_artifact_by_uid(self, uid: str, node_id: str, artifact_name: str) -> str:
         """Get an input artifact by UID."""
         resp = requests.get(
-            url=os.path.join(self.host, "input-artifacts-by-uid/{uid}/{nodeId}/{artifactName}").format(
+            url=urljoin(self.host, "input-artifacts-by-uid/{uid}/{nodeId}/{artifactName}").format(
                 uid=uid, nodeId=node_id, artifactName=artifact_name
             ),
             params=None,
             headers={"Authorization": f"Bearer {self.token}"},
             data=None,
             verify=self.verify_ssl,
         )
@@ -643,15 +643,15 @@
             return str(resp.content)
         else:
             raise Exception(f"Server returned status code {resp.status_code} with error: {resp.json()}")
 
     def get_input_artifact(self, name: str, node_id: str, artifact_name: str, namespace: Optional[str] = None) -> str:
         """Get an input artifact."""
         resp = requests.get(
-            url=os.path.join(self.host, "input-artifacts/{namespace}/{name}/{nodeId}/{artifactName}").format(
+            url=urljoin(self.host, "input-artifacts/{namespace}/{name}/{nodeId}/{artifactName}").format(
                 name=name,
                 nodeId=node_id,
                 artifactName=artifact_name,
                 namespace=namespace if namespace is not None else self.namespace,
             ),
             params=None,
             headers={"Authorization": f"Bearer {self.token}"},
```

### Comparing `hera_workflows-5.1.3/src/hera/expr/_node.py` & `hera_workflows-5.1.4/src/hera/expr/_node.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/expr/_sprig.py` & `hera_workflows-5.1.4/src/hera/expr/_sprig.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/shared/_global_config.py` & `hera_workflows-5.1.4/src/hera/shared/_global_config.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/shared/serialization.py` & `hera_workflows-5.1.4/src/hera/shared/serialization.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/workflows/__init__.py` & `hera_workflows-5.1.4/src/hera/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/workflows/_context.py` & `hera_workflows-5.1.4/src/hera/workflows/_context.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/workflows/_mixins.py` & `hera_workflows-5.1.4/src/hera/workflows/_mixins.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,18 +132,20 @@
     startup_probe: Optional[Probe] = None
     stdin: Optional[bool] = None
     stdin_once: Optional[bool] = None
     termination_message_path: Optional[str] = None
     termination_message_policy: Optional[TerminationMessagePolicy] = None
     tty: Optional[bool] = None
 
-    def _build_image_pull_policy(self) -> Optional[ImagePullPolicy]:
-        if self.image_pull_policy is None or isinstance(self.image_pull_policy, ImagePullPolicy):
-            return self.image_pull_policy
-        return ImagePullPolicy[self.image_pull_policy.lower()]
+    def _build_image_pull_policy(self) -> Optional[str]:
+        if self.image_pull_policy is None:
+            return None
+        elif isinstance(self.image_pull_policy, ImagePullPolicy):
+            return self.image_pull_policy.value
+        return ImagePullPolicy[self.image_pull_policy.lower()].value
 
     @validator("image", pre=True, always=True)
     def _set_image(cls, v):
         if v is None:
             return global_config.image
         return v
```

### Comparing `hera_workflows-5.1.3/src/hera/workflows/_unparse.py` & `hera_workflows-5.1.4/src/hera/workflows/_unparse.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/workflows/archive.py` & `hera_workflows-5.1.4/src/hera/workflows/archive.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/workflows/artifact.py` & `hera_workflows-5.1.4/src/hera/workflows/artifact.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/workflows/container.py` & `hera_workflows-5.1.4/src/hera/workflows/container.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/workflows/container_set.py` & `hera_workflows-5.1.4/src/hera/workflows/container_set.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/workflows/cron_workflow.py` & `hera_workflows-5.1.4/src/hera/workflows/cron_workflow.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/workflows/dag.py` & `hera_workflows-5.1.4/src/hera/workflows/dag.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/workflows/data.py` & `hera_workflows-5.1.4/src/hera/workflows/data.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/workflows/env.py` & `hera_workflows-5.1.4/src/hera/workflows/env.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/workflows/env_from.py` & `hera_workflows-5.1.4/src/hera/workflows/env_from.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/workflows/http_template.py` & `hera_workflows-5.1.4/src/hera/workflows/http_template.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/workflows/models/__init__.py` & `hera_workflows-5.1.4/src/hera/workflows/models/__init__.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/workflows/models/eventsource.py` & `hera_workflows-5.1.4/src/hera/workflows/models/eventsource.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/workflows/models/eventsource.pyi` & `hera_workflows-5.1.4/src/hera/workflows/models/eventsource.pyi`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/workflows/models/grpc/gateway/runtime.py` & `hera_workflows-5.1.4/src/hera/workflows/models/grpc/gateway/runtime.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/workflows/models/io/argoproj/events/v1alpha1.py` & `hera_workflows-5.1.4/src/hera/workflows/models/io/argoproj/events/v1alpha1.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/workflows/models/io/argoproj/events/v1alpha1.pyi` & `hera_workflows-5.1.4/src/hera/workflows/models/io/argoproj/events/v1alpha1.pyi`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.py` & `hera_workflows-5.1.4/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.pyi` & `hera_workflows-5.1.4/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.pyi`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/workflows/models/io/k8s/api/core/v1.py` & `hera_workflows-5.1.4/src/hera/workflows/models/io/k8s/api/core/v1.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/workflows/models/io/k8s/api/core/v1.pyi` & `hera_workflows-5.1.4/src/hera/workflows/models/io/k8s/api/core/v1.pyi`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/workflows/models/io/k8s/api/policy/v1beta1.py` & `hera_workflows-5.1.4/src/hera/workflows/models/io/k8s/api/policy/v1beta1.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/resource.py` & `hera_workflows-5.1.4/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/resource.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.py` & `hera_workflows-5.1.4/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi` & `hera_workflows-5.1.4/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/workflows/models/sensor.py` & `hera_workflows-5.1.4/src/hera/workflows/models/sensor.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/workflows/models/sensor.pyi` & `hera_workflows-5.1.4/src/hera/workflows/models/sensor.pyi`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/workflows/operator.py` & `hera_workflows-5.1.4/src/hera/workflows/operator.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/workflows/parameter.py` & `hera_workflows-5.1.4/src/hera/workflows/parameter.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/workflows/protocol.py` & `hera_workflows-5.1.4/src/hera/workflows/protocol.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/workflows/resource.py` & `hera_workflows-5.1.4/src/hera/workflows/resource.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/workflows/resources.py` & `hera_workflows-5.1.4/src/hera/workflows/resources.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/workflows/retry_strategy.py` & `hera_workflows-5.1.4/src/hera/workflows/retry_strategy.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/workflows/runner.py` & `hera_workflows-5.1.4/src/hera/workflows/runner.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/workflows/script.py` & `hera_workflows-5.1.4/src/hera/workflows/script.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/workflows/service.py` & `hera_workflows-5.1.4/src/hera/workflows/service.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import os
 from typing import Optional, cast
+from urllib.parse import urljoin
 
 import requests
 
 from hera.shared import global_config
 from hera.workflows.models import (
     ArchivedWorkflowDeletedResponse,
     ClusterWorkflowTemplate,
@@ -73,15 +73,15 @@
         resource_version_match: Optional[str] = None,
         timeout_seconds: Optional[str] = None,
         limit: Optional[str] = None,
         continue_: Optional[str] = None,
         name_prefix: Optional[str] = None,
     ) -> WorkflowList:
         resp = requests.get(
-            url=os.path.join(self.host, "api/v1/archived-workflows"),
+            url=urljoin(self.host, "api/v1/archived-workflows"),
             params={
                 "listOptions.labelSelector": label_selector,
                 "listOptions.fieldSelector": field_selector,
                 "listOptions.watch": watch,
                 "listOptions.allowWatchBookmarks": allow_watch_bookmarks,
                 "listOptions.resourceVersion": resource_version,
                 "listOptions.resourceVersionMatch": resource_version_match,
@@ -98,15 +98,15 @@
         if resp.ok:
             return WorkflowList(**resp.json())
         else:
             raise Exception(f"Server returned status code {resp.status_code} with error: {resp.json()}")
 
     def list_archived_workflow_label_keys(self) -> LabelKeys:
         resp = requests.get(
-            url=os.path.join(self.host, "api/v1/archived-workflows-label-keys"),
+            url=urljoin(self.host, "api/v1/archived-workflows-label-keys"),
             params=None,
             headers={"Authorization": f"Bearer {self.token}"},
             data=None,
             verify=self.verify_ssl,
         )
 
         if resp.ok:
@@ -123,15 +123,15 @@
         resource_version: Optional[str] = None,
         resource_version_match: Optional[str] = None,
         timeout_seconds: Optional[str] = None,
         limit: Optional[str] = None,
         continue_: Optional[str] = None,
     ) -> LabelValues:
         resp = requests.get(
-            url=os.path.join(self.host, "api/v1/archived-workflows-label-values"),
+            url=urljoin(self.host, "api/v1/archived-workflows-label-values"),
             params={
                 "listOptions.labelSelector": label_selector,
                 "listOptions.fieldSelector": field_selector,
                 "listOptions.watch": watch,
                 "listOptions.allowWatchBookmarks": allow_watch_bookmarks,
                 "listOptions.resourceVersion": resource_version,
                 "listOptions.resourceVersionMatch": resource_version_match,
@@ -147,43 +147,43 @@
         if resp.ok:
             return LabelValues(**resp.json())
         else:
             raise Exception(f"Server returned status code {resp.status_code} with error: {resp.json()}")
 
     def get_archived_workflow(self, uid: str) -> Workflow:
         resp = requests.get(
-            url=os.path.join(self.host, "api/v1/archived-workflows/{uid}").format(uid=uid),
+            url=urljoin(self.host, "api/v1/archived-workflows/{uid}").format(uid=uid),
             params=None,
             headers={"Authorization": f"Bearer {self.token}"},
             data=None,
             verify=self.verify_ssl,
         )
 
         if resp.ok:
             return Workflow(**resp.json())
         else:
             raise Exception(f"Server returned status code {resp.status_code} with error: {resp.json()}")
 
     def delete_archived_workflow(self, uid: str) -> ArchivedWorkflowDeletedResponse:
         resp = requests.delete(
-            url=os.path.join(self.host, "api/v1/archived-workflows/{uid}").format(uid=uid),
+            url=urljoin(self.host, "api/v1/archived-workflows/{uid}").format(uid=uid),
             params=None,
             headers={"Authorization": f"Bearer {self.token}"},
             data=None,
             verify=self.verify_ssl,
         )
 
         if resp.ok:
             return ArchivedWorkflowDeletedResponse()
         else:
             raise Exception(f"Server returned status code {resp.status_code} with error: {resp.json()}")
 
     def resubmit_archived_workflow(self, uid: str, req: ResubmitArchivedWorkflowRequest) -> Workflow:
         resp = requests.put(
-            url=os.path.join(self.host, "api/v1/archived-workflows/{uid}/resubmit").format(uid=uid),
+            url=urljoin(self.host, "api/v1/archived-workflows/{uid}/resubmit").format(uid=uid),
             params=None,
             headers={"Authorization": f"Bearer {self.token}"},
             data=req.json(
                 exclude_none=True, by_alias=True, skip_defaults=True, exclude_unset=True, exclude_defaults=True
             ),
             verify=self.verify_ssl,
         )
@@ -191,15 +191,15 @@
         if resp.ok:
             return Workflow(**resp.json())
         else:
             raise Exception(f"Server returned status code {resp.status_code} with error: {resp.json()}")
 
     def retry_archived_workflow(self, uid: str, req: RetryArchivedWorkflowRequest) -> Workflow:
         resp = requests.put(
-            url=os.path.join(self.host, "api/v1/archived-workflows/{uid}/retry").format(uid=uid),
+            url=urljoin(self.host, "api/v1/archived-workflows/{uid}/retry").format(uid=uid),
             params=None,
             headers={"Authorization": f"Bearer {self.token}"},
             data=req.json(
                 exclude_none=True, by_alias=True, skip_defaults=True, exclude_unset=True, exclude_defaults=True
             ),
             verify=self.verify_ssl,
         )
@@ -218,15 +218,15 @@
         resource_version: Optional[str] = None,
         resource_version_match: Optional[str] = None,
         timeout_seconds: Optional[str] = None,
         limit: Optional[str] = None,
         continue_: Optional[str] = None,
     ) -> ClusterWorkflowTemplateList:
         resp = requests.get(
-            url=os.path.join(self.host, "api/v1/cluster-workflow-templates"),
+            url=urljoin(self.host, "api/v1/cluster-workflow-templates"),
             params={
                 "listOptions.labelSelector": label_selector,
                 "listOptions.fieldSelector": field_selector,
                 "listOptions.watch": watch,
                 "listOptions.allowWatchBookmarks": allow_watch_bookmarks,
                 "listOptions.resourceVersion": resource_version,
                 "listOptions.resourceVersionMatch": resource_version_match,
@@ -242,15 +242,15 @@
         if resp.ok:
             return ClusterWorkflowTemplateList(**resp.json())
         else:
             raise Exception(f"Server returned status code {resp.status_code} with error: {resp.json()}")
 
     def create_cluster_workflow_template(self, req: ClusterWorkflowTemplateCreateRequest) -> ClusterWorkflowTemplate:
         resp = requests.post(
-            url=os.path.join(self.host, "api/v1/cluster-workflow-templates"),
+            url=urljoin(self.host, "api/v1/cluster-workflow-templates"),
             params=None,
             headers={"Authorization": f"Bearer {self.token}"},
             data=req.json(
                 exclude_none=True, by_alias=True, skip_defaults=True, exclude_unset=True, exclude_defaults=True
             ),
             verify=self.verify_ssl,
         )
@@ -258,15 +258,15 @@
         if resp.ok:
             return ClusterWorkflowTemplate(**resp.json())
         else:
             raise Exception(f"Server returned status code {resp.status_code} with error: {resp.json()}")
 
     def lint_cluster_workflow_template(self, req: ClusterWorkflowTemplateLintRequest) -> ClusterWorkflowTemplate:
         resp = requests.post(
-            url=os.path.join(self.host, "api/v1/cluster-workflow-templates/lint"),
+            url=urljoin(self.host, "api/v1/cluster-workflow-templates/lint"),
             params=None,
             headers={"Authorization": f"Bearer {self.token}"},
             data=req.json(
                 exclude_none=True, by_alias=True, skip_defaults=True, exclude_unset=True, exclude_defaults=True
             ),
             verify=self.verify_ssl,
         )
@@ -276,15 +276,15 @@
         else:
             raise Exception(f"Server returned status code {resp.status_code} with error: {resp.json()}")
 
     def get_cluster_workflow_template(
         self, name: str, resource_version: Optional[str] = None
     ) -> ClusterWorkflowTemplate:
         resp = requests.get(
-            url=os.path.join(self.host, "api/v1/cluster-workflow-templates/{name}").format(name=name),
+            url=urljoin(self.host, "api/v1/cluster-workflow-templates/{name}").format(name=name),
             params={"getOptions.resourceVersion": resource_version},
             headers={"Authorization": f"Bearer {self.token}"},
             data=None,
             verify=self.verify_ssl,
         )
 
         if resp.ok:
@@ -292,15 +292,15 @@
         else:
             raise Exception(f"Server returned status code {resp.status_code} with error: {resp.json()}")
 
     def update_cluster_workflow_template(
         self, name: str, req: ClusterWorkflowTemplateUpdateRequest
     ) -> ClusterWorkflowTemplate:
         resp = requests.put(
-            url=os.path.join(self.host, "api/v1/cluster-workflow-templates/{name}").format(name=name),
+            url=urljoin(self.host, "api/v1/cluster-workflow-templates/{name}").format(name=name),
             params=None,
             headers={"Authorization": f"Bearer {self.token}"},
             data=req.json(
                 exclude_none=True, by_alias=True, skip_defaults=True, exclude_unset=True, exclude_defaults=True
             ),
             verify=self.verify_ssl,
         )
@@ -317,15 +317,15 @@
         uid: Optional[str] = None,
         resource_version: Optional[str] = None,
         orphan_dependents: Optional[bool] = None,
         propagation_policy: Optional[str] = None,
         dry_run: Optional[list] = None,
     ) -> ClusterWorkflowTemplateDeleteResponse:
         resp = requests.delete(
-            url=os.path.join(self.host, "api/v1/cluster-workflow-templates/{name}").format(name=name),
+            url=urljoin(self.host, "api/v1/cluster-workflow-templates/{name}").format(name=name),
             params={
                 "deleteOptions.gracePeriodSeconds": grace_period_seconds,
                 "deleteOptions.preconditions.uid": uid,
                 "deleteOptions.preconditions.resourceVersion": resource_version,
                 "deleteOptions.orphanDependents": orphan_dependents,
                 "deleteOptions.propagationPolicy": propagation_policy,
                 "deleteOptions.dryRun": dry_run,
@@ -350,15 +350,15 @@
         resource_version: Optional[str] = None,
         resource_version_match: Optional[str] = None,
         timeout_seconds: Optional[str] = None,
         limit: Optional[str] = None,
         continue_: Optional[str] = None,
     ) -> CronWorkflowList:
         resp = requests.get(
-            url=os.path.join(self.host, "api/v1/cron-workflows/{namespace}").format(
+            url=urljoin(self.host, "api/v1/cron-workflows/{namespace}").format(
                 namespace=namespace if namespace is not None else self.namespace
             ),
             params={
                 "listOptions.labelSelector": label_selector,
                 "listOptions.fieldSelector": field_selector,
                 "listOptions.watch": watch,
                 "listOptions.allowWatchBookmarks": allow_watch_bookmarks,
@@ -376,15 +376,15 @@
         if resp.ok:
             return CronWorkflowList(**resp.json())
         else:
             raise Exception(f"Server returned status code {resp.status_code} with error: {resp.json()}")
 
     def create_cron_workflow(self, req: CreateCronWorkflowRequest, namespace: Optional[str] = None) -> CronWorkflow:
         resp = requests.post(
-            url=os.path.join(self.host, "api/v1/cron-workflows/{namespace}").format(
+            url=urljoin(self.host, "api/v1/cron-workflows/{namespace}").format(
                 namespace=namespace if namespace is not None else self.namespace
             ),
             params=None,
             headers={"Authorization": f"Bearer {self.token}"},
             data=req.json(
                 exclude_none=True, by_alias=True, skip_defaults=True, exclude_unset=True, exclude_defaults=True
             ),
@@ -394,15 +394,15 @@
         if resp.ok:
             return CronWorkflow(**resp.json())
         else:
             raise Exception(f"Server returned status code {resp.status_code} with error: {resp.json()}")
 
     def lint_cron_workflow(self, req: LintCronWorkflowRequest, namespace: Optional[str] = None) -> CronWorkflow:
         resp = requests.post(
-            url=os.path.join(self.host, "api/v1/cron-workflows/{namespace}/lint").format(
+            url=urljoin(self.host, "api/v1/cron-workflows/{namespace}/lint").format(
                 namespace=namespace if namespace is not None else self.namespace
             ),
             params=None,
             headers={"Authorization": f"Bearer {self.token}"},
             data=req.json(
                 exclude_none=True, by_alias=True, skip_defaults=True, exclude_unset=True, exclude_defaults=True
             ),
@@ -414,15 +414,15 @@
         else:
             raise Exception(f"Server returned status code {resp.status_code} with error: {resp.json()}")
 
     def get_cron_workflow(
         self, name: str, namespace: Optional[str] = None, resource_version: Optional[str] = None
     ) -> CronWorkflow:
         resp = requests.get(
-            url=os.path.join(self.host, "api/v1/cron-workflows/{namespace}/{name}").format(
+            url=urljoin(self.host, "api/v1/cron-workflows/{namespace}/{name}").format(
                 name=name, namespace=namespace if namespace is not None else self.namespace
             ),
             params={"getOptions.resourceVersion": resource_version},
             headers={"Authorization": f"Bearer {self.token}"},
             data=None,
             verify=self.verify_ssl,
         )
@@ -432,15 +432,15 @@
         else:
             raise Exception(f"Server returned status code {resp.status_code} with error: {resp.json()}")
 
     def update_cron_workflow(
         self, name: str, req: UpdateCronWorkflowRequest, namespace: Optional[str] = None
     ) -> CronWorkflow:
         resp = requests.put(
-            url=os.path.join(self.host, "api/v1/cron-workflows/{namespace}/{name}").format(
+            url=urljoin(self.host, "api/v1/cron-workflows/{namespace}/{name}").format(
                 name=name, namespace=namespace if namespace is not None else self.namespace
             ),
             params=None,
             headers={"Authorization": f"Bearer {self.token}"},
             data=req.json(
                 exclude_none=True, by_alias=True, skip_defaults=True, exclude_unset=True, exclude_defaults=True
             ),
@@ -460,15 +460,15 @@
         uid: Optional[str] = None,
         resource_version: Optional[str] = None,
         orphan_dependents: Optional[bool] = None,
         propagation_policy: Optional[str] = None,
         dry_run: Optional[list] = None,
     ) -> CronWorkflowDeletedResponse:
         resp = requests.delete(
-            url=os.path.join(self.host, "api/v1/cron-workflows/{namespace}/{name}").format(
+            url=urljoin(self.host, "api/v1/cron-workflows/{namespace}/{name}").format(
                 name=name, namespace=namespace if namespace is not None else self.namespace
             ),
             params={
                 "deleteOptions.gracePeriodSeconds": grace_period_seconds,
                 "deleteOptions.preconditions.uid": uid,
                 "deleteOptions.preconditions.resourceVersion": resource_version,
                 "deleteOptions.orphanDependents": orphan_dependents,
@@ -485,15 +485,15 @@
         else:
             raise Exception(f"Server returned status code {resp.status_code} with error: {resp.json()}")
 
     def resume_cron_workflow(
         self, name: str, req: CronWorkflowResumeRequest, namespace: Optional[str] = None
     ) -> CronWorkflow:
         resp = requests.put(
-            url=os.path.join(self.host, "api/v1/cron-workflows/{namespace}/{name}/resume").format(
+            url=urljoin(self.host, "api/v1/cron-workflows/{namespace}/{name}/resume").format(
                 name=name, namespace=namespace if namespace is not None else self.namespace
             ),
             params=None,
             headers={"Authorization": f"Bearer {self.token}"},
             data=req.json(
                 exclude_none=True, by_alias=True, skip_defaults=True, exclude_unset=True, exclude_defaults=True
             ),
@@ -505,15 +505,15 @@
         else:
             raise Exception(f"Server returned status code {resp.status_code} with error: {resp.json()}")
 
     def suspend_cron_workflow(
         self, name: str, req: CronWorkflowSuspendRequest, namespace: Optional[str] = None
     ) -> CronWorkflow:
         resp = requests.put(
-            url=os.path.join(self.host, "api/v1/cron-workflows/{namespace}/{name}/suspend").format(
+            url=urljoin(self.host, "api/v1/cron-workflows/{namespace}/{name}/suspend").format(
                 name=name, namespace=namespace if namespace is not None else self.namespace
             ),
             params=None,
             headers={"Authorization": f"Bearer {self.token}"},
             data=req.json(
                 exclude_none=True, by_alias=True, skip_defaults=True, exclude_unset=True, exclude_defaults=True
             ),
@@ -523,43 +523,43 @@
         if resp.ok:
             return CronWorkflow(**resp.json())
         else:
             raise Exception(f"Server returned status code {resp.status_code} with error: {resp.json()}")
 
     def get_info(self) -> InfoResponse:
         resp = requests.get(
-            url=os.path.join(self.host, "api/v1/info"),
+            url=urljoin(self.host, "api/v1/info"),
             params=None,
             headers={"Authorization": f"Bearer {self.token}"},
             data=None,
             verify=self.verify_ssl,
         )
 
         if resp.ok:
             return InfoResponse()
         else:
             raise Exception(f"Server returned status code {resp.status_code} with error: {resp.json()}")
 
     def get_user_info(self) -> GetUserInfoResponse:
         resp = requests.get(
-            url=os.path.join(self.host, "api/v1/userinfo"),
+            url=urljoin(self.host, "api/v1/userinfo"),
             params=None,
             headers={"Authorization": f"Bearer {self.token}"},
             data=None,
             verify=self.verify_ssl,
         )
 
         if resp.ok:
             return GetUserInfoResponse()
         else:
             raise Exception(f"Server returned status code {resp.status_code} with error: {resp.json()}")
 
     def get_version(self) -> Version:
         resp = requests.get(
-            url=os.path.join(self.host, "api/v1/version"),
+            url=urljoin(self.host, "api/v1/version"),
             params=None,
             headers={"Authorization": f"Bearer {self.token}"},
             data=None,
             verify=self.verify_ssl,
         )
 
         if resp.ok:
@@ -577,15 +577,15 @@
         resource_version: Optional[str] = None,
         resource_version_match: Optional[str] = None,
         timeout_seconds: Optional[str] = None,
         limit: Optional[str] = None,
         continue_: Optional[str] = None,
     ) -> WorkflowTemplateList:
         resp = requests.get(
-            url=os.path.join(self.host, "api/v1/workflow-templates/{namespace}").format(
+            url=urljoin(self.host, "api/v1/workflow-templates/{namespace}").format(
                 namespace=namespace if namespace is not None else self.namespace
             ),
             params={
                 "listOptions.labelSelector": label_selector,
                 "listOptions.fieldSelector": field_selector,
                 "listOptions.watch": watch,
                 "listOptions.allowWatchBookmarks": allow_watch_bookmarks,
@@ -605,15 +605,15 @@
         else:
             raise Exception(f"Server returned status code {resp.status_code} with error: {resp.json()}")
 
     def create_workflow_template(
         self, req: WorkflowTemplateCreateRequest, namespace: Optional[str] = None
     ) -> WorkflowTemplate:
         resp = requests.post(
-            url=os.path.join(self.host, "api/v1/workflow-templates/{namespace}").format(
+            url=urljoin(self.host, "api/v1/workflow-templates/{namespace}").format(
                 namespace=namespace if namespace is not None else self.namespace
             ),
             params=None,
             headers={"Authorization": f"Bearer {self.token}"},
             data=req.json(
                 exclude_none=True, by_alias=True, skip_defaults=True, exclude_unset=True, exclude_defaults=True
             ),
@@ -625,15 +625,15 @@
         else:
             raise Exception(f"Server returned status code {resp.status_code} with error: {resp.json()}")
 
     def lint_workflow_template(
         self, req: WorkflowTemplateLintRequest, namespace: Optional[str] = None
     ) -> WorkflowTemplate:
         resp = requests.post(
-            url=os.path.join(self.host, "api/v1/workflow-templates/{namespace}/lint").format(
+            url=urljoin(self.host, "api/v1/workflow-templates/{namespace}/lint").format(
                 namespace=namespace if namespace is not None else self.namespace
             ),
             params=None,
             headers={"Authorization": f"Bearer {self.token}"},
             data=req.json(
                 exclude_none=True, by_alias=True, skip_defaults=True, exclude_unset=True, exclude_defaults=True
             ),
@@ -645,15 +645,15 @@
         else:
             raise Exception(f"Server returned status code {resp.status_code} with error: {resp.json()}")
 
     def get_workflow_template(
         self, name: str, namespace: Optional[str] = None, resource_version: Optional[str] = None
     ) -> WorkflowTemplate:
         resp = requests.get(
-            url=os.path.join(self.host, "api/v1/workflow-templates/{namespace}/{name}").format(
+            url=urljoin(self.host, "api/v1/workflow-templates/{namespace}/{name}").format(
                 name=name, namespace=namespace if namespace is not None else self.namespace
             ),
             params={"getOptions.resourceVersion": resource_version},
             headers={"Authorization": f"Bearer {self.token}"},
             data=None,
             verify=self.verify_ssl,
         )
@@ -663,15 +663,15 @@
         else:
             raise Exception(f"Server returned status code {resp.status_code} with error: {resp.json()}")
 
     def update_workflow_template(
         self, name: str, req: WorkflowTemplateUpdateRequest, namespace: Optional[str] = None
     ) -> WorkflowTemplate:
         resp = requests.put(
-            url=os.path.join(self.host, "api/v1/workflow-templates/{namespace}/{name}").format(
+            url=urljoin(self.host, "api/v1/workflow-templates/{namespace}/{name}").format(
                 name=name, namespace=namespace if namespace is not None else self.namespace
             ),
             params=None,
             headers={"Authorization": f"Bearer {self.token}"},
             data=req.json(
                 exclude_none=True, by_alias=True, skip_defaults=True, exclude_unset=True, exclude_defaults=True
             ),
@@ -691,15 +691,15 @@
         uid: Optional[str] = None,
         resource_version: Optional[str] = None,
         orphan_dependents: Optional[bool] = None,
         propagation_policy: Optional[str] = None,
         dry_run: Optional[list] = None,
     ) -> WorkflowTemplateDeleteResponse:
         resp = requests.delete(
-            url=os.path.join(self.host, "api/v1/workflow-templates/{namespace}/{name}").format(
+            url=urljoin(self.host, "api/v1/workflow-templates/{namespace}/{name}").format(
                 name=name, namespace=namespace if namespace is not None else self.namespace
             ),
             params={
                 "deleteOptions.gracePeriodSeconds": grace_period_seconds,
                 "deleteOptions.preconditions.uid": uid,
                 "deleteOptions.preconditions.resourceVersion": resource_version,
                 "deleteOptions.orphanDependents": orphan_dependents,
@@ -727,15 +727,15 @@
         resource_version_match: Optional[str] = None,
         timeout_seconds: Optional[str] = None,
         limit: Optional[str] = None,
         continue_: Optional[str] = None,
         fields: Optional[str] = None,
     ) -> WorkflowList:
         resp = requests.get(
-            url=os.path.join(self.host, "api/v1/workflows/{namespace}").format(
+            url=urljoin(self.host, "api/v1/workflows/{namespace}").format(
                 namespace=namespace if namespace is not None else self.namespace
             ),
             params={
                 "listOptions.labelSelector": label_selector,
                 "listOptions.fieldSelector": field_selector,
                 "listOptions.watch": watch,
                 "listOptions.allowWatchBookmarks": allow_watch_bookmarks,
@@ -754,15 +754,15 @@
         if resp.ok:
             return WorkflowList(**resp.json())
         else:
             raise Exception(f"Server returned status code {resp.status_code} with error: {resp.json()}")
 
     def create_workflow(self, req: WorkflowCreateRequest, namespace: Optional[str] = None) -> Workflow:
         resp = requests.post(
-            url=os.path.join(self.host, "api/v1/workflows/{namespace}").format(
+            url=urljoin(self.host, "api/v1/workflows/{namespace}").format(
                 namespace=namespace if namespace is not None else self.namespace
             ),
             params=None,
             headers={"Authorization": f"Bearer {self.token}"},
             data=req.json(
                 exclude_none=True, by_alias=True, skip_defaults=True, exclude_unset=True, exclude_defaults=True
             ),
@@ -772,15 +772,15 @@
         if resp.ok:
             return Workflow(**resp.json())
         else:
             raise Exception(f"Server returned status code {resp.status_code} with error: {resp.json()}")
 
     def lint_workflow(self, req: WorkflowLintRequest, namespace: Optional[str] = None) -> Workflow:
         resp = requests.post(
-            url=os.path.join(self.host, "api/v1/workflows/{namespace}/lint").format(
+            url=urljoin(self.host, "api/v1/workflows/{namespace}/lint").format(
                 namespace=namespace if namespace is not None else self.namespace
             ),
             params=None,
             headers={"Authorization": f"Bearer {self.token}"},
             data=req.json(
                 exclude_none=True, by_alias=True, skip_defaults=True, exclude_unset=True, exclude_defaults=True
             ),
@@ -790,15 +790,15 @@
         if resp.ok:
             return Workflow(**resp.json())
         else:
             raise Exception(f"Server returned status code {resp.status_code} with error: {resp.json()}")
 
     def submit_workflow(self, req: WorkflowSubmitRequest, namespace: Optional[str] = None) -> Workflow:
         resp = requests.post(
-            url=os.path.join(self.host, "api/v1/workflows/{namespace}/submit").format(
+            url=urljoin(self.host, "api/v1/workflows/{namespace}/submit").format(
                 namespace=namespace if namespace is not None else self.namespace
             ),
             params=None,
             headers={"Authorization": f"Bearer {self.token}"},
             data=req.json(
                 exclude_none=True, by_alias=True, skip_defaults=True, exclude_unset=True, exclude_defaults=True
             ),
@@ -814,15 +814,15 @@
         self,
         name: str,
         namespace: Optional[str] = None,
         resource_version: Optional[str] = None,
         fields: Optional[str] = None,
     ) -> Workflow:
         resp = requests.get(
-            url=os.path.join(self.host, "api/v1/workflows/{namespace}/{name}").format(
+            url=urljoin(self.host, "api/v1/workflows/{namespace}/{name}").format(
                 name=name, namespace=namespace if namespace is not None else self.namespace
             ),
             params={"getOptions.resourceVersion": resource_version, "fields": fields},
             headers={"Authorization": f"Bearer {self.token}"},
             data=None,
             verify=self.verify_ssl,
         )
@@ -841,15 +841,15 @@
         resource_version: Optional[str] = None,
         orphan_dependents: Optional[bool] = None,
         propagation_policy: Optional[str] = None,
         dry_run: Optional[list] = None,
         force: Optional[bool] = None,
     ) -> WorkflowDeleteResponse:
         resp = requests.delete(
-            url=os.path.join(self.host, "api/v1/workflows/{namespace}/{name}").format(
+            url=urljoin(self.host, "api/v1/workflows/{namespace}/{name}").format(
                 name=name, namespace=namespace if namespace is not None else self.namespace
             ),
             params={
                 "deleteOptions.gracePeriodSeconds": grace_period_seconds,
                 "deleteOptions.preconditions.uid": uid,
                 "deleteOptions.preconditions.resourceVersion": resource_version,
                 "deleteOptions.orphanDependents": orphan_dependents,
@@ -882,15 +882,15 @@
         tail_lines: Optional[str] = None,
         limit_bytes: Optional[str] = None,
         insecure_skip_tls_verify_backend: Optional[bool] = None,
         grep: Optional[str] = None,
         selector: Optional[str] = None,
     ) -> V1alpha1LogEntry:
         resp = requests.get(
-            url=os.path.join(self.host, "api/v1/workflows/{namespace}/{name}/log").format(
+            url=urljoin(self.host, "api/v1/workflows/{namespace}/{name}/log").format(
                 name=name, namespace=namespace if namespace is not None else self.namespace
             ),
             params={
                 "podName": pod_name,
                 "logOptions.container": container,
                 "logOptions.follow": follow,
                 "logOptions.previous": previous,
@@ -912,15 +912,15 @@
         if resp.ok:
             return V1alpha1LogEntry(**resp.json())
         else:
             raise Exception(f"Server returned status code {resp.status_code} with error: {resp.json()}")
 
     def resubmit_workflow(self, name: str, req: WorkflowResubmitRequest, namespace: Optional[str] = None) -> Workflow:
         resp = requests.put(
-            url=os.path.join(self.host, "api/v1/workflows/{namespace}/{name}/resubmit").format(
+            url=urljoin(self.host, "api/v1/workflows/{namespace}/{name}/resubmit").format(
                 name=name, namespace=namespace if namespace is not None else self.namespace
             ),
             params=None,
             headers={"Authorization": f"Bearer {self.token}"},
             data=req.json(
                 exclude_none=True, by_alias=True, skip_defaults=True, exclude_unset=True, exclude_defaults=True
             ),
@@ -930,15 +930,15 @@
         if resp.ok:
             return Workflow(**resp.json())
         else:
             raise Exception(f"Server returned status code {resp.status_code} with error: {resp.json()}")
 
     def resume_workflow(self, name: str, req: WorkflowResumeRequest, namespace: Optional[str] = None) -> Workflow:
         resp = requests.put(
-            url=os.path.join(self.host, "api/v1/workflows/{namespace}/{name}/resume").format(
+            url=urljoin(self.host, "api/v1/workflows/{namespace}/{name}/resume").format(
                 name=name, namespace=namespace if namespace is not None else self.namespace
             ),
             params=None,
             headers={"Authorization": f"Bearer {self.token}"},
             data=req.json(
                 exclude_none=True, by_alias=True, skip_defaults=True, exclude_unset=True, exclude_defaults=True
             ),
@@ -948,15 +948,15 @@
         if resp.ok:
             return Workflow(**resp.json())
         else:
             raise Exception(f"Server returned status code {resp.status_code} with error: {resp.json()}")
 
     def retry_workflow(self, name: str, req: WorkflowRetryRequest, namespace: Optional[str] = None) -> Workflow:
         resp = requests.put(
-            url=os.path.join(self.host, "api/v1/workflows/{namespace}/{name}/retry").format(
+            url=urljoin(self.host, "api/v1/workflows/{namespace}/{name}/retry").format(
                 name=name, namespace=namespace if namespace is not None else self.namespace
             ),
             params=None,
             headers={"Authorization": f"Bearer {self.token}"},
             data=req.json(
                 exclude_none=True, by_alias=True, skip_defaults=True, exclude_unset=True, exclude_defaults=True
             ),
@@ -966,15 +966,15 @@
         if resp.ok:
             return Workflow(**resp.json())
         else:
             raise Exception(f"Server returned status code {resp.status_code} with error: {resp.json()}")
 
     def set_workflow(self, name: str, req: WorkflowSetRequest, namespace: Optional[str] = None) -> Workflow:
         resp = requests.put(
-            url=os.path.join(self.host, "api/v1/workflows/{namespace}/{name}/set").format(
+            url=urljoin(self.host, "api/v1/workflows/{namespace}/{name}/set").format(
                 name=name, namespace=namespace if namespace is not None else self.namespace
             ),
             params=None,
             headers={"Authorization": f"Bearer {self.token}"},
             data=req.json(
                 exclude_none=True, by_alias=True, skip_defaults=True, exclude_unset=True, exclude_defaults=True
             ),
@@ -984,15 +984,15 @@
         if resp.ok:
             return Workflow(**resp.json())
         else:
             raise Exception(f"Server returned status code {resp.status_code} with error: {resp.json()}")
 
     def stop_workflow(self, name: str, req: WorkflowStopRequest, namespace: Optional[str] = None) -> Workflow:
         resp = requests.put(
-            url=os.path.join(self.host, "api/v1/workflows/{namespace}/{name}/stop").format(
+            url=urljoin(self.host, "api/v1/workflows/{namespace}/{name}/stop").format(
                 name=name, namespace=namespace if namespace is not None else self.namespace
             ),
             params=None,
             headers={"Authorization": f"Bearer {self.token}"},
             data=req.json(
                 exclude_none=True, by_alias=True, skip_defaults=True, exclude_unset=True, exclude_defaults=True
             ),
@@ -1002,15 +1002,15 @@
         if resp.ok:
             return Workflow(**resp.json())
         else:
             raise Exception(f"Server returned status code {resp.status_code} with error: {resp.json()}")
 
     def suspend_workflow(self, name: str, req: WorkflowSuspendRequest, namespace: Optional[str] = None) -> Workflow:
         resp = requests.put(
-            url=os.path.join(self.host, "api/v1/workflows/{namespace}/{name}/suspend").format(
+            url=urljoin(self.host, "api/v1/workflows/{namespace}/{name}/suspend").format(
                 name=name, namespace=namespace if namespace is not None else self.namespace
             ),
             params=None,
             headers={"Authorization": f"Bearer {self.token}"},
             data=req.json(
                 exclude_none=True, by_alias=True, skip_defaults=True, exclude_unset=True, exclude_defaults=True
             ),
@@ -1022,15 +1022,15 @@
         else:
             raise Exception(f"Server returned status code {resp.status_code} with error: {resp.json()}")
 
     def terminate_workflow(
         self, name: str, req: WorkflowTerminateRequest, namespace: Optional[str] = None
     ) -> Workflow:
         resp = requests.put(
-            url=os.path.join(self.host, "api/v1/workflows/{namespace}/{name}/terminate").format(
+            url=urljoin(self.host, "api/v1/workflows/{namespace}/{name}/terminate").format(
                 name=name, namespace=namespace if namespace is not None else self.namespace
             ),
             params=None,
             headers={"Authorization": f"Bearer {self.token}"},
             data=req.json(
                 exclude_none=True, by_alias=True, skip_defaults=True, exclude_unset=True, exclude_defaults=True
             ),
@@ -1058,15 +1058,15 @@
         limit_bytes: Optional[str] = None,
         insecure_skip_tls_verify_backend: Optional[bool] = None,
         grep: Optional[str] = None,
         selector: Optional[str] = None,
     ) -> V1alpha1LogEntry:
         """DEPRECATED: Cannot work via HTTP if podName is an empty string. Use WorkflowLogs."""
         resp = requests.get(
-            url=os.path.join(self.host, "api/v1/workflows/{namespace}/{name}/{podName}/log").format(
+            url=urljoin(self.host, "api/v1/workflows/{namespace}/{name}/{podName}/log").format(
                 name=name, podName=pod_name, namespace=namespace if namespace is not None else self.namespace
             ),
             params={
                 "logOptions.container": container,
                 "logOptions.follow": follow,
                 "logOptions.previous": previous,
                 "logOptions.sinceSeconds": since_seconds,
@@ -1096,15 +1096,15 @@
         node_id: str,
         artifact_name: str,
         artifact_discriminator: str,
         namespace: Optional[str] = None,
     ) -> str:
         """Get an artifact."""
         resp = requests.get(
-            url=os.path.join(
+            url=urljoin(
                 self.host,
                 "artifact-files/{namespace}/{idDiscriminator}/{id}/{nodeId}/{artifactDiscriminator}/{artifactName}",
             ).format(
                 idDiscriminator=id_discriminator,
                 id=id_,
                 nodeId=node_id,
                 artifactName=artifact_name,
@@ -1121,15 +1121,15 @@
             return str(resp.content)
         else:
             raise Exception(f"Server returned status code {resp.status_code} with error: {resp.json()}")
 
     def get_output_artifact_by_uid(self, uid: str, node_id: str, artifact_name: str) -> str:
         """Get an output artifact by UID."""
         resp = requests.get(
-            url=os.path.join(self.host, "artifacts-by-uid/{uid}/{nodeId}/{artifactName}").format(
+            url=urljoin(self.host, "artifacts-by-uid/{uid}/{nodeId}/{artifactName}").format(
                 uid=uid, nodeId=node_id, artifactName=artifact_name
             ),
             params=None,
             headers={"Authorization": f"Bearer {self.token}"},
             data=None,
             verify=self.verify_ssl,
         )
@@ -1138,15 +1138,15 @@
             return str(resp.content)
         else:
             raise Exception(f"Server returned status code {resp.status_code} with error: {resp.json()}")
 
     def get_output_artifact(self, name: str, node_id: str, artifact_name: str, namespace: Optional[str] = None) -> str:
         """Get an output artifact."""
         resp = requests.get(
-            url=os.path.join(self.host, "artifacts/{namespace}/{name}/{nodeId}/{artifactName}").format(
+            url=urljoin(self.host, "artifacts/{namespace}/{name}/{nodeId}/{artifactName}").format(
                 name=name,
                 nodeId=node_id,
                 artifactName=artifact_name,
                 namespace=namespace if namespace is not None else self.namespace,
             ),
             params=None,
             headers={"Authorization": f"Bearer {self.token}"},
@@ -1158,15 +1158,15 @@
             return str(resp.content)
         else:
             raise Exception(f"Server returned status code {resp.status_code} with error: {resp.json()}")
 
     def get_input_artifact_by_uid(self, uid: str, node_id: str, artifact_name: str) -> str:
         """Get an input artifact by UID."""
         resp = requests.get(
-            url=os.path.join(self.host, "input-artifacts-by-uid/{uid}/{nodeId}/{artifactName}").format(
+            url=urljoin(self.host, "input-artifacts-by-uid/{uid}/{nodeId}/{artifactName}").format(
                 uid=uid, nodeId=node_id, artifactName=artifact_name
             ),
             params=None,
             headers={"Authorization": f"Bearer {self.token}"},
             data=None,
             verify=self.verify_ssl,
         )
@@ -1175,15 +1175,15 @@
             return str(resp.content)
         else:
             raise Exception(f"Server returned status code {resp.status_code} with error: {resp.json()}")
 
     def get_input_artifact(self, name: str, node_id: str, artifact_name: str, namespace: Optional[str] = None) -> str:
         """Get an input artifact."""
         resp = requests.get(
-            url=os.path.join(self.host, "input-artifacts/{namespace}/{name}/{nodeId}/{artifactName}").format(
+            url=urljoin(self.host, "input-artifacts/{namespace}/{name}/{nodeId}/{artifactName}").format(
                 name=name,
                 nodeId=node_id,
                 artifactName=artifact_name,
                 namespace=namespace if namespace is not None else self.namespace,
             ),
             params=None,
             headers={"Authorization": f"Bearer {self.token}"},
```

### Comparing `hera_workflows-5.1.3/src/hera/workflows/steps.py` & `hera_workflows-5.1.4/src/hera/workflows/steps.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/workflows/suspend.py` & `hera_workflows-5.1.4/src/hera/workflows/suspend.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/workflows/task.py` & `hera_workflows-5.1.4/src/hera/workflows/task.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,15 +187,15 @@
             )
         raise KeyError(f"No output parameter named `{name}` found")
 
     def next(self, other: Task, operator: Operator = Operator.and_, on: Optional[TaskResult] = None) -> Task:
         """Set self as a dependency of `other`."""
         assert issubclass(other.__class__, Task)
 
-        condition = f".{on}" if on else ""
+        condition = f".{on.value}" if on else ""
 
         if other.depends is None:
             # First dependency
             other.depends = self.name + condition
         elif self.name in other._get_dependency_tasks():
             raise ValueError(f"{self.name} already in {other.name}'s depends: {other.depends}")
         else:
```

### Comparing `hera_workflows-5.1.3/src/hera/workflows/user_container.py` & `hera_workflows-5.1.4/src/hera/workflows/user_container.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/workflows/validators.py` & `hera_workflows-5.1.4/src/hera/workflows/validators.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/workflows/volume.py` & `hera_workflows-5.1.4/src/hera/workflows/volume.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/workflows/workflow.py` & `hera_workflows-5.1.4/src/hera/workflows/workflow.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/workflows/workflow_status.py` & `hera_workflows-5.1.4/src/hera/workflows/workflow_status.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/src/hera/workflows/workflow_template.py` & `hera_workflows-5.1.4/src/hera/workflows/workflow_template.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.3/PKG-INFO` & `hera_workflows-5.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hera-workflows
-Version: 5.1.3
+Version: 5.1.4
 Summary: Hera is a Python framework for constructing and submitting Argo Workflows. The main goal of Hera is to make Argo Workflows more accessible by abstracting away some setup that is typically necessary for constructing Argo workflows.
 Home-page: https://github.com/argoproj-labs/hera
 License: MIT
 Author: Flaviu Vadan
 Author-email: flaviu.vadan@dynotx.com
 Maintainer: Flaviu Vadan
 Maintainer-email: flaviu.vadan@dynotx.com
```

