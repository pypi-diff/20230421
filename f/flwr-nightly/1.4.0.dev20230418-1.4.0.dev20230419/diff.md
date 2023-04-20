# Comparing `tmp/flwr_nightly-1.4.0.dev20230418.tar.gz` & `tmp/flwr_nightly-1.4.0.dev20230419.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flwr_nightly-1.4.0.dev20230418.tar", max compression
+gzip compressed data, was "flwr_nightly-1.4.0.dev20230419.tar", max compression
```

## Comparing `flwr_nightly-1.4.0.dev20230418.tar` & `flwr_nightly-1.4.0.dev20230419.tar`

### file list

```diff
@@ -1,103 +1,104 @@
--rw-r--r--   0        0        0    11358 2023-04-18 23:02:13.113126 flwr_nightly-1.4.0.dev20230418/LICENSE
--rw-r--r--   0        0        0    10297 2023-04-18 23:02:13.113126 flwr_nightly-1.4.0.dev20230418/README.md
--rw-r--r--   0        0        0     4269 2023-04-18 23:02:34.657409 flwr_nightly-1.4.0.dev20230418/pyproject.toml
--rw-r--r--   0        0        0      930 2023-04-18 23:02:13.361129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/__init__.py
--rw-r--r--   0        0        0     1164 2023-04-18 23:02:13.361129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/client/__init__.py
--rw-r--r--   0        0        0    12224 2023-04-18 23:02:13.361129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/client/app.py
--rw-r--r--   0        0        0     6503 2023-04-18 23:02:13.361129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/client/client.py
--rw-r--r--   0        0        0     3351 2023-04-18 23:02:13.361129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/client/dpfedavg_numpy_client.py
--rw-r--r--   0        0        0      728 2023-04-18 23:02:13.361129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/client/grpc_client/__init__.py
--rw-r--r--   0        0        0     4117 2023-04-18 23:02:13.361129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/client/grpc_client/connection.py
--rw-r--r--   0        0        0      712 2023-04-18 23:02:13.361129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/client/message_handler/__init__.py
--rw-r--r--   0        0        0     5077 2023-04-18 23:02:13.361129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/client/message_handler/message_handler.py
--rw-r--r--   0        0        0     1686 2023-04-18 23:02:13.361129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/client/message_handler/task_handler.py
--rw-r--r--   0        0        0     5100 2023-04-18 23:02:13.361129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/client/numpy_client.py
--rw-r--r--   0        0        0      728 2023-04-18 23:02:13.361129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/client/rest_client/__init__.py
--rw-r--r--   0        0        0     7455 2023-04-18 23:02:13.361129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/client/rest_client/connection.py
--rw-r--r--   0        0        0     2877 2023-04-18 23:02:13.361129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/common/__init__.py
--rw-r--r--   0        0        0     2309 2023-04-18 23:02:13.361129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/common/address.py
--rw-r--r--   0        0        0      884 2023-04-18 23:02:13.361129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/common/date.py
--rw-r--r--   0        0        0     1828 2023-04-18 23:02:13.361129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/common/dp.py
--rw-r--r--   0        0        0     1894 2023-04-18 23:02:13.361129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/common/grpc.py
--rw-r--r--   0        0        0     3483 2023-04-18 23:02:13.361129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/common/logger.py
--rw-r--r--   0        0        0     2120 2023-04-18 23:02:13.361129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/common/parameter.py
--rw-r--r--   0        0        0    16316 2023-04-18 23:02:13.361129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/common/serde.py
--rw-r--r--   0        0        0     7684 2023-04-18 23:02:13.361129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/common/telemetry.py
--rw-r--r--   0        0        0     3714 2023-04-18 23:02:13.361129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/common/typing.py
--rw-r--r--   0        0        0      848 2023-04-18 23:02:13.361129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/common/version.py
--rw-r--r--   0        0        0      769 2023-04-18 23:02:13.361129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/driver/__init__.py
--rw-r--r--   0        0        0     3909 2023-04-18 23:02:13.361129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/driver/driver.py
--rw-r--r--   0        0        0      676 2023-04-18 23:02:13.361129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/proto/__init__.py
--rw-r--r--   0        0        0     4663 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/proto/driver_pb2.py
--rw-r--r--   0        0        0     3815 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/proto/driver_pb2.pyi
--rw-r--r--   0        0        0     5727 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/proto/driver_pb2_grpc.py
--rw-r--r--   0        0        0     1617 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/proto/driver_pb2_grpc.pyi
--rw-r--r--   0        0        0     4982 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/proto/fleet_pb2.py
--rw-r--r--   0        0        0     4554 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/proto/fleet_pb2.pyi
--rw-r--r--   0        0        0     4275 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/proto/fleet_pb2_grpc.py
--rw-r--r--   0        0        0     1495 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/proto/fleet_pb2_grpc.pyi
--rw-r--r--   0        0        0     1188 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/proto/node_pb2.py
--rw-r--r--   0        0        0      751 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/proto/node_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/proto/node_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/proto/node_pb2_grpc.pyi
--rw-r--r--   0        0        0     3217 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/proto/task_pb2.py
--rw-r--r--   0        0        0     4286 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/proto/task_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/proto/task_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/proto/task_pb2_grpc.pyi
--rw-r--r--   0        0        0    18721 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/proto/transport_pb2.py
--rw-r--r--   0        0        0    21497 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/proto/transport_pb2.pyi
--rw-r--r--   0        0        0     2598 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/proto/transport_pb2_grpc.py
--rw-r--r--   0        0        0      766 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/proto/transport_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/py.typed
--rw-r--r--   0        0        0     1370 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/__init__.py
--rw-r--r--   0        0        0    19238 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/app.py
--rw-r--r--   0        0        0     5941 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/client_manager.py
--rw-r--r--   0        0        0     2228 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/client_proxy.py
--rw-r--r--   0        0        0     1058 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/criterion.py
--rw-r--r--   0        0        0      705 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/driver/__init__.py
--rw-r--r--   0        0        0     3919 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/driver/driver_servicer.py
--rw-r--r--   0        0        0      704 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/fleet/__init__.py
--rw-r--r--   0        0        0     1638 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/fleet/fleet_servicer.py
--rw-r--r--   0        0        0      728 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/grpc_server/__init__.py
--rw-r--r--   0        0        0     4450 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/grpc_server/driver_client_manager.py
--rw-r--r--   0        0        0     5594 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/grpc_server/flower_service_servicer.py
--rw-r--r--   0        0        0     6416 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/grpc_server/grpc_bridge.py
--rw-r--r--   0        0        0     4623 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/grpc_server/grpc_client_proxy.py
--rw-r--r--   0        0        0    11509 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/grpc_server/grpc_server.py
--rw-r--r--   0        0        0     6314 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/grpc_server/ins_scheduler.py
--rw-r--r--   0        0        0     4457 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/history.py
--rw-r--r--   0        0        0      728 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/rest_server/__init__.py
--rw-r--r--   0        0        0     4640 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/rest_server/rest_api.py
--rw-r--r--   0        0        0    15855 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/server.py
--rw-r--r--   0        0        0      996 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/state/__init__.py
--rw-r--r--   0        0        0     6521 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/state/in_memory_state.py
--rw-r--r--   0        0        0    19296 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/state/sqlite_state.py
--rw-r--r--   0        0        0     4805 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/state/state.py
--rw-r--r--   0        0        0     1648 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/state/state_factory.py
--rw-r--r--   0        0        0     1588 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/strategy/__init__.py
--rw-r--r--   0        0        0     4994 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/strategy/aggregate.py
--rw-r--r--   0        0        0     4519 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/strategy/dpfedavg_adaptive.py
--rw-r--r--   0        0        0     4875 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/strategy/dpfedavg_fixed.py
--rw-r--r--   0        0        0     5978 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/strategy/fault_tolerant_fedavg.py
--rw-r--r--   0        0        0     6730 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/strategy/fedadagrad.py
--rw-r--r--   0        0        0     7012 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/strategy/fedadam.py
--rw-r--r--   0        0        0    11495 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/strategy/fedavg.py
--rw-r--r--   0        0        0     9985 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/strategy/fedavg_android.py
--rw-r--r--   0        0        0     8953 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/strategy/fedavgm.py
--rw-r--r--   0        0        0     6469 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/strategy/fedmedian.py
--rw-r--r--   0        0        0     5393 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/strategy/fedopt.py
--rw-r--r--   0        0        0     7708 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/strategy/fedprox.py
--rw-r--r--   0        0        0     7772 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/strategy/fedxgb_nn_avg.py
--rw-r--r--   0        0        0     7044 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/strategy/fedyogi.py
--rw-r--r--   0        0        0     7011 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/strategy/krum.py
--rw-r--r--   0        0        0    10744 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/strategy/qfedavg.py
--rw-r--r--   0        0        0     7484 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/strategy/strategy.py
--rw-r--r--   0        0        0      901 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/utils/__init__.py
--rw-r--r--   0        0        0     5114 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/utils/tensorboard.py
--rw-r--r--   0        0        0     4941 2023-04-18 23:02:13.365129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/utils/validator.py
--rw-r--r--   0        0        0     1271 2023-04-18 23:02:13.369129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/simulation/__init__.py
--rw-r--r--   0        0        0     7773 2023-04-18 23:02:13.369129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/simulation/app.py
--rw-r--r--   0        0        0      727 2023-04-18 23:02:13.369129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/simulation/ray_transport/__init__.py
--rw-r--r--   0        0        0     5472 2023-04-18 23:02:13.369129 flwr_nightly-1.4.0.dev20230418/src/py/flwr/simulation/ray_transport/ray_client_proxy.py
--rw-r--r--   0        0        0    12316 1970-01-01 00:00:00.000000 flwr_nightly-1.4.0.dev20230418/setup.py
--rw-r--r--   0        0        0    12772 1970-01-01 00:00:00.000000 flwr_nightly-1.4.0.dev20230418/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-04-19 23:02:22.962476 flwr_nightly-1.4.0.dev20230419/LICENSE
+-rw-r--r--   0        0        0    10297 2023-04-19 23:02:22.962476 flwr_nightly-1.4.0.dev20230419/README.md
+-rw-r--r--   0        0        0     4269 2023-04-19 23:02:46.562846 flwr_nightly-1.4.0.dev20230419/pyproject.toml
+-rw-r--r--   0        0        0      930 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/__init__.py
+-rw-r--r--   0        0        0     1164 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/client/__init__.py
+-rw-r--r--   0        0        0    12441 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/client/app.py
+-rw-r--r--   0        0        0     6503 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/client/client.py
+-rw-r--r--   0        0        0     3351 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/client/dpfedavg_numpy_client.py
+-rw-r--r--   0        0        0      728 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/client/grpc_client/__init__.py
+-rw-r--r--   0        0        0     4288 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/client/grpc_client/connection.py
+-rw-r--r--   0        0        0      712 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/client/message_handler/__init__.py
+-rw-r--r--   0        0        0     5077 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/client/message_handler/message_handler.py
+-rw-r--r--   0        0        0     1686 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/client/message_handler/task_handler.py
+-rw-r--r--   0        0        0     5100 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/client/numpy_client.py
+-rw-r--r--   0        0        0      728 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/client/rest_client/__init__.py
+-rw-r--r--   0        0        0     8194 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/client/rest_client/connection.py
+-rw-r--r--   0        0        0     2877 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/common/__init__.py
+-rw-r--r--   0        0        0     1876 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/common/address.py
+-rw-r--r--   0        0        0      898 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/common/constant.py
+-rw-r--r--   0        0        0      884 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/common/date.py
+-rw-r--r--   0        0        0     1828 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/common/dp.py
+-rw-r--r--   0        0        0     1894 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/common/grpc.py
+-rw-r--r--   0        0        0     3483 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/common/logger.py
+-rw-r--r--   0        0        0     2120 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/common/parameter.py
+-rw-r--r--   0        0        0    16316 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/common/serde.py
+-rw-r--r--   0        0        0     7684 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/common/telemetry.py
+-rw-r--r--   0        0        0     3714 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/common/typing.py
+-rw-r--r--   0        0        0      848 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/common/version.py
+-rw-r--r--   0        0        0      769 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/driver/__init__.py
+-rw-r--r--   0        0        0     3909 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/driver/driver.py
+-rw-r--r--   0        0        0      676 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/proto/__init__.py
+-rw-r--r--   0        0        0     4663 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/proto/driver_pb2.py
+-rw-r--r--   0        0        0     3815 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/proto/driver_pb2.pyi
+-rw-r--r--   0        0        0     5727 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/proto/driver_pb2_grpc.py
+-rw-r--r--   0        0        0     1617 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/proto/driver_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4982 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/proto/fleet_pb2.py
+-rw-r--r--   0        0        0     4554 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/proto/fleet_pb2.pyi
+-rw-r--r--   0        0        0     4275 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/proto/fleet_pb2_grpc.py
+-rw-r--r--   0        0        0     1495 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/proto/fleet_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1188 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/proto/node_pb2.py
+-rw-r--r--   0        0        0      751 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/proto/node_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/proto/node_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/proto/node_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3217 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/proto/task_pb2.py
+-rw-r--r--   0        0        0     4286 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/proto/task_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/proto/task_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/proto/task_pb2_grpc.pyi
+-rw-r--r--   0        0        0    18721 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/proto/transport_pb2.py
+-rw-r--r--   0        0        0    21497 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/proto/transport_pb2.pyi
+-rw-r--r--   0        0        0     2598 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/proto/transport_pb2_grpc.py
+-rw-r--r--   0        0        0      766 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/proto/transport_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/py.typed
+-rw-r--r--   0        0        0     1370 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/__init__.py
+-rw-r--r--   0        0        0    21729 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/app.py
+-rw-r--r--   0        0        0     5941 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/client_manager.py
+-rw-r--r--   0        0        0     2228 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/client_proxy.py
+-rw-r--r--   0        0        0     1058 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/criterion.py
+-rw-r--r--   0        0        0      705 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/driver/__init__.py
+-rw-r--r--   0        0        0     3919 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/driver/driver_servicer.py
+-rw-r--r--   0        0        0      704 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/fleet/__init__.py
+-rw-r--r--   0        0        0     1638 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/fleet/fleet_servicer.py
+-rw-r--r--   0        0        0      728 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/grpc_server/__init__.py
+-rw-r--r--   0        0        0     4450 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/grpc_server/driver_client_manager.py
+-rw-r--r--   0        0        0     5594 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/grpc_server/flower_service_servicer.py
+-rw-r--r--   0        0        0     6416 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/grpc_server/grpc_bridge.py
+-rw-r--r--   0        0        0     4623 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/grpc_server/grpc_client_proxy.py
+-rw-r--r--   0        0        0    11509 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/grpc_server/grpc_server.py
+-rw-r--r--   0        0        0     6314 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/grpc_server/ins_scheduler.py
+-rw-r--r--   0        0        0     4457 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/history.py
+-rw-r--r--   0        0        0      728 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/rest_server/__init__.py
+-rw-r--r--   0        0        0     4564 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/rest_server/rest_api.py
+-rw-r--r--   0        0        0    15855 2023-04-19 23:02:23.214480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/server.py
+-rw-r--r--   0        0        0      996 2023-04-19 23:02:23.218480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/state/__init__.py
+-rw-r--r--   0        0        0     6521 2023-04-19 23:02:23.218480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/state/in_memory_state.py
+-rw-r--r--   0        0        0    19296 2023-04-19 23:02:23.218480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/state/sqlite_state.py
+-rw-r--r--   0        0        0     4805 2023-04-19 23:02:23.218480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/state/state.py
+-rw-r--r--   0        0        0     1648 2023-04-19 23:02:23.218480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/state/state_factory.py
+-rw-r--r--   0        0        0     1588 2023-04-19 23:02:23.218480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/strategy/__init__.py
+-rw-r--r--   0        0        0     4994 2023-04-19 23:02:23.218480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/strategy/aggregate.py
+-rw-r--r--   0        0        0     4519 2023-04-19 23:02:23.218480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/strategy/dpfedavg_adaptive.py
+-rw-r--r--   0        0        0     4875 2023-04-19 23:02:23.218480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/strategy/dpfedavg_fixed.py
+-rw-r--r--   0        0        0     5978 2023-04-19 23:02:23.218480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/strategy/fault_tolerant_fedavg.py
+-rw-r--r--   0        0        0     6730 2023-04-19 23:02:23.218480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/strategy/fedadagrad.py
+-rw-r--r--   0        0        0     7012 2023-04-19 23:02:23.218480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/strategy/fedadam.py
+-rw-r--r--   0        0        0    11495 2023-04-19 23:02:23.218480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/strategy/fedavg.py
+-rw-r--r--   0        0        0     9985 2023-04-19 23:02:23.218480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/strategy/fedavg_android.py
+-rw-r--r--   0        0        0     8953 2023-04-19 23:02:23.218480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/strategy/fedavgm.py
+-rw-r--r--   0        0        0     6469 2023-04-19 23:02:23.218480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/strategy/fedmedian.py
+-rw-r--r--   0        0        0     5393 2023-04-19 23:02:23.218480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/strategy/fedopt.py
+-rw-r--r--   0        0        0     7708 2023-04-19 23:02:23.218480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/strategy/fedprox.py
+-rw-r--r--   0        0        0     7772 2023-04-19 23:02:23.218480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/strategy/fedxgb_nn_avg.py
+-rw-r--r--   0        0        0     7044 2023-04-19 23:02:23.218480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/strategy/fedyogi.py
+-rw-r--r--   0        0        0     7011 2023-04-19 23:02:23.218480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/strategy/krum.py
+-rw-r--r--   0        0        0    10744 2023-04-19 23:02:23.218480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/strategy/qfedavg.py
+-rw-r--r--   0        0        0     7484 2023-04-19 23:02:23.218480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/strategy/strategy.py
+-rw-r--r--   0        0        0      901 2023-04-19 23:02:23.218480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/utils/__init__.py
+-rw-r--r--   0        0        0     5114 2023-04-19 23:02:23.218480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/utils/tensorboard.py
+-rw-r--r--   0        0        0     4941 2023-04-19 23:02:23.218480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/utils/validator.py
+-rw-r--r--   0        0        0     1271 2023-04-19 23:02:23.218480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/simulation/__init__.py
+-rw-r--r--   0        0        0     7773 2023-04-19 23:02:23.218480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/simulation/app.py
+-rw-r--r--   0        0        0      727 2023-04-19 23:02:23.218480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/simulation/ray_transport/__init__.py
+-rw-r--r--   0        0        0     5472 2023-04-19 23:02:23.218480 flwr_nightly-1.4.0.dev20230419/src/py/flwr/simulation/ray_transport/ray_client_proxy.py
+-rw-r--r--   0        0        0    12316 1970-01-01 00:00:00.000000 flwr_nightly-1.4.0.dev20230419/setup.py
+-rw-r--r--   0        0        0    12772 1970-01-01 00:00:00.000000 flwr_nightly-1.4.0.dev20230419/PKG-INFO
```

### Comparing `flwr_nightly-1.4.0.dev20230418/LICENSE` & `flwr_nightly-1.4.0.dev20230419/LICENSE`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/README.md` & `flwr_nightly-1.4.0.dev20230419/README.md`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/pyproject.toml` & `flwr_nightly-1.4.0.dev20230419/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.4.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "flwr-nightly"
-version = "1.4.0-dev20230418"
+version = "1.4.0-dev20230419"
 description = "Flower: A Friendly Federated Learning Framework"
 license = "Apache-2.0"
 authors = ["The Flower Authors <hello@flower.dev>"]
 readme = "README.md"
 homepage = "https://flower.dev"
 repository = "https://github.com/adap/flower"
 documentation = "https://flower.dev"
```

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/__init__.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/client/__init__.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/client/app.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/client/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     GRPC_MAX_MESSAGE_LENGTH,
     EventType,
     event,
     ndarrays_to_parameters,
     parameters_to_ndarrays,
 )
 from flwr.common.address import parse_address
+from flwr.common.constant import MISSING_EXTRA_REST
 from flwr.common.logger import log
 from flwr.common.typing import (
     Code,
     EvaluateIns,
     EvaluateRes,
     FitIns,
     FitRes,
@@ -84,18 +85,18 @@
 
 # pylint: disable=import-outside-toplevel,too-many-locals
 def start_client(
     *,
     server_address: str,
     client: Client,
     grpc_max_message_length: int = GRPC_MAX_MESSAGE_LENGTH,
-    root_certificates: Optional[bytes] = None,
+    root_certificates: Optional[Union[bytes, str]] = None,
     rest: bool = False,
 ) -> None:
-    """Start a Flower Client which connects to a gRPC server.
+    """Start a Flower client node which connects to a Flower server.
 
     Parameters
     ----------
     server_address : str
         The IPv4 or IPv6 address of the server. If the Flower
         server runs on the same machine on port 8080, then `server_address`
         would be `"[::]:8080"`.
@@ -105,33 +106,33 @@
     grpc_max_message_length : int (default: 536_870_912, this equals 512MB)
         The maximum length of gRPC messages that can be exchanged with the
         Flower server. The default should be sufficient for most models.
         Users who train very large models might need to increase this
         value. Note that the Flower server needs to be started with the
         same value (see `flwr.server.start_server`), otherwise it will not
         know about the increased limit and block larger messages.
-    root_certificates : bytes (default: None)
-        The PEM-encoded root certificates as a byte string. If provided, a secure
-        connection using the certificates will be established to a
-        SSL-enabled Flower server.
+    root_certificates : Optional[Union[bytes, str]] (default: None)
+        The PEM-encoded root certificates as a byte string or a path string.
+        If provided, a secure connection using the certificates will be
+        established to an SSL-enabled Flower server.
     rest : bool (default: False)
         Defines whether or not the client is interacting with the server using the
         experimental REST API. This feature is experimental, it might change
         considerably in future versions of Flower.
 
     Examples
     --------
-    Starting a client with insecure server connection:
+    Starting a gRPC client with an insecure server connection:
 
     >>> start_client(
     >>>     server_address=localhost:8080,
     >>>     client=FlowerClient(),
     >>> )
 
-    Starting a SSL-enabled client:
+    Starting an SSL-enabled gRPC client:
 
     >>> from pathlib import Path
     >>> start_client(
     >>>     server_address=localhost:8080,
     >>>     client=FlowerClient(),
     >>>     root_certificates=Path("/crts/root.pem").read_bytes(),
     >>> )
@@ -146,19 +147,21 @@
     host, port, is_v6 = parsed_address
     address = f"[{host}]:{port}" if is_v6 else f"{host}:{port}"
 
     # Use either gRPC bidirectional streaming or REST request/response
     if rest:
         try:
             from .rest_client.connection import http_request_response
-        except ImportError as missing_dep:
-            raise ImportError(
-                "To use the REST API you must install the "
-                "extra dependencies by running `pip install flwr['rest']`."
-            ) from missing_dep
+        except ModuleNotFoundError:
+            sys.exit(MISSING_EXTRA_REST)
+        if server_address[:4] != "http":
+            sys.exit(
+                "When using the REST API, please provide `https://` or "
+                "`http://` before the server address (e.g. `http://127.0.0.1:8080`)"
+            )
         connection = http_request_response
     else:
         connection = grpc_connection
     while True:
         sleep_duration: int = 0
         with connection(
             address,
@@ -214,17 +217,17 @@
         The maximum length of gRPC messages that can be exchanged with the
         Flower server. The default should be sufficient for most models.
         Users who train very large models might need to increase this
         value. Note that the Flower server needs to be started with the
         same value (see `flwr.server.start_server`), otherwise it will not
         know about the increased limit and block larger messages.
     root_certificates : bytes (default: None)
-        The PEM-encoded root certificates a byte string. If provided, a secure
-        connection using the certificates will be established to a
-        SSL-enabled Flower server.
+        The PEM-encoded root certificates as a byte string or a path string.
+        If provided, a secure connection using the certificates will be
+        established to an SSL-enabled Flower server.
     rest : bool (default: False)
         Defines whether or not the client is interacting with the server using the
         experimental REST API. This feature is experimental, it might be change
         considerably in future versions of Flower.
 
     Examples
     --------
```

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/client/client.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/client/client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/client/dpfedavg_numpy_client.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/client/dpfedavg_numpy_client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/client/grpc_client/__init__.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/client/grpc_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/client/grpc_client/connection.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/client/grpc_client/connection.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,16 +13,17 @@
 # limitations under the License.
 # ==============================================================================
 """Contextmanager managing a gRPC channel to the Flower server."""
 
 
 from contextlib import contextmanager
 from logging import DEBUG
+from pathlib import Path
 from queue import Queue
-from typing import Callable, Iterator, Optional, Tuple
+from typing import Callable, Iterator, Optional, Tuple, Union
 
 from flwr.common import GRPC_MAX_MESSAGE_LENGTH
 from flwr.common.grpc import create_channel
 from flwr.common.logger import log
 from flwr.proto.transport_pb2 import ClientMessage, ServerMessage
 from flwr.proto.transport_pb2_grpc import FlowerServiceStub
 
@@ -38,15 +39,15 @@
     log(DEBUG, channel_connectivity)
 
 
 @contextmanager
 def grpc_connection(
     server_address: str,
     max_message_length: int = GRPC_MAX_MESSAGE_LENGTH,
-    root_certificates: Optional[bytes] = None,
+    root_certificates: Optional[Union[bytes, str]] = None,
 ) -> Iterator[Tuple[Callable[[], ServerMessage], Callable[[ClientMessage], None]]]:
     """Establish a gRPC connection to a gRPC server.
 
     Parameters
     ----------
     server_address : str
         The IPv4 or IPv6 address of the server. If the Flower server runs on the same
@@ -57,17 +58,17 @@
         server. The default should be sufficient for most models. Users who train
         very large models might need to increase this value. Note that the Flower
         server needs to be started with the same value
         (see `flwr.server.start_server`), otherwise it will not know about the
         increased limit and block larger messages.
         (default: 536_870_912, this equals 512MB)
     root_certificates : Optional[bytes] (default: None)
-        The PEM-encoded root certificates as a byte string. If provided, a secure
-        connection using the certificates will be established to a SSL-enabled
-        Flower server.
+        The PEM-encoded root certificates as a byte string or a path string.
+        If provided, a secure connection using the certificates will be
+        established to an SSL-enabled Flower server.
 
     Returns
     -------
     receive, send : Callable, Callable
 
     Examples
     --------
@@ -80,14 +81,17 @@
     >>>     root_certificates=Path("/crts/root.pem").read_bytes(),
     >>> ) as conn:
     >>>     receive, send = conn
     >>>     server_message = receive()
     >>>     # do something here
     >>>     send(client_message)
     """
+    if isinstance(root_certificates, str):
+        root_certificates = Path(root_certificates).read_bytes()
+
     channel = create_channel(
         server_address=server_address,
         root_certificates=root_certificates,
         max_message_length=max_message_length,
     )
     channel.subscribe(on_channel_state_change)
```

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/client/message_handler/__init__.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/client/message_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/client/message_handler/message_handler.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/client/message_handler/message_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/client/message_handler/task_handler.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/client/message_handler/task_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/client/numpy_client.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/client/numpy_client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/client/rest_client/__init__.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/client/rest_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/client/rest_client/connection.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/client/rest_client/connection.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,80 +11,99 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Contextmanager managing a REST-based channel to the Flower server."""
 
 
+import sys
 from contextlib import contextmanager
 from logging import ERROR, INFO, WARN
-from typing import Callable, Dict, Iterator, Optional, Tuple
-
-try:
-    import requests
-except ImportError as missing_dep:
-    raise ImportError(
-        "To use the REST API you must install the "
-        "extra dependencies by running `pip install flwr['rest']`."
-    ) from missing_dep
+from typing import Callable, Dict, Iterator, Optional, Tuple, Union
 
 from flwr.client.message_handler.task_handler import get_server_message
 from flwr.common import GRPC_MAX_MESSAGE_LENGTH
+from flwr.common.constant import MISSING_EXTRA_REST
 from flwr.common.logger import log
 from flwr.proto.fleet_pb2 import (
     PullTaskInsRequest,
     PullTaskInsResponse,
     PushTaskResRequest,
     PushTaskResResponse,
 )
 from flwr.proto.node_pb2 import Node
 from flwr.proto.task_pb2 import Task, TaskIns, TaskRes
 from flwr.proto.transport_pb2 import ClientMessage, ServerMessage
 
+try:
+    import requests
+except ModuleNotFoundError:
+    sys.exit(MISSING_EXTRA_REST)
+
+
 PATH_PULL_TASK_INS: str = "api/v0/fleet/pull-task-ins"
 PATH_PUSH_TASK_RES: str = "api/v0/fleet/push-task-res"
 
 
 @contextmanager
 def http_request_response(
     server_address: str,
     max_message_length: int = GRPC_MAX_MESSAGE_LENGTH,  # pylint: disable=W0613
-    root_certificates: Optional[bytes] = None,  # pylint: disable=unused-argument
+    root_certificates: Optional[
+        Union[bytes, str]
+    ] = None,  # pylint: disable=unused-argument
 ) -> Iterator[
     Tuple[Callable[[], Optional[ServerMessage]], Callable[[ClientMessage], None]]
 ]:
     """Primitives for request/response-based interaction with a server.
 
     One notable difference to the grpc_connection context manager is that
     `receive` can return `None`.
 
     Parameters
     ----------
     server_address : str
-        The IPv6 address of the server. If the Flower server runs on the same machine
-        on port 8080, then `server_address` would be `"[::]:8080"`.
+        The IPv6 address of the server with `http://` or `https://`.
+        If the Flower server runs on the same machine
+        on port 8080, then `server_address` would be `"http://[::]:8080"`.
     max_message_length : int
         Ignored, only present to preserve API-compatibility.
-    root_certificates : Optional[bytes] (default: None)
-        Ignored, for now.
+    root_certificates : Optional[Union[bytes, str]] (default: None)
+        Path of the root certificate. If provided, a secure
+        connection using the certificates will be established to an SSL-enabled
+        Flower server. Bytes won't work for the REST API.
 
     Returns
     -------
     receive, send : Callable, Callable
     """
 
     log(
         WARN,
         """
         EXPERIMENTAL: `rest` is an experimental feature, it might change
         considerably in future versions of Flower
         """,
     )
 
-    base_url = f"http://{server_address}"
+    base_url = server_address
+
+    # NEVER SET VERIFY TO FALSE
+    # Otherwise any server can fake its identity
+    # Please refer to:
+    # https://requests.readthedocs.io/en/latest/user/advanced/#ssl-cert-verification
+    verify: Union[bool, str] = True
+    if isinstance(root_certificates, str):
+        verify = root_certificates
+    elif isinstance(root_certificates, bytes):
+        log(
+            ERROR,
+            "For the REST API, the root certificates "
+            "must be provided as a string path to the client.",
+        )
 
     # Necessary state to link TaskRes to TaskIns
     state: Dict[str, Optional[TaskIns]] = {"current_task_ins": None}
 
     ###########################################################################
     # receive/send functions
     ###########################################################################
@@ -102,14 +121,15 @@
         res = requests.post(
             url=f"{base_url}/{PATH_PULL_TASK_INS}",
             headers={
                 "Accept": "application/protobuf",
                 "Content-Type": "application/protobuf",
             },
             data=pull_task_ins_req_bytes,
+            verify=verify,
         )
 
         # Check status code and headers
         if res.status_code != 200:
             return None
         if "content-type" not in res.headers:
             log(
@@ -173,14 +193,15 @@
         res = requests.post(
             url=f"{base_url}/{PATH_PUSH_TASK_RES}",
             headers={
                 "Accept": "application/protobuf",
                 "Content-Type": "application/protobuf",
             },
             data=push_task_res_request_bytes,
+            verify=verify,
         )
 
         state["current_task_ins"] = None
 
         # Check status code and headers
         if res.status_code != 200:
             return
```

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/common/__init__.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/common/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/common/address.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/common/address.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,61 +10,50 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Flower IP address utils."""
 
-
-import re
 from ipaddress import ip_address
-from typing import Optional, Pattern, Tuple
+from typing import Optional, Tuple
 
 IPV6: int = 6
 
-DOMAIN_PATTERN: Pattern[str] = re.compile(
-    r"^(https?:\/\/)?(localhost)|(([a-zA-Z]{1})|([a-zA-Z]{1}[a-zA-Z]{1})|"
-    r"([a-zA-Z]{1}[0-9]{1})|([0-9]{1}[a-zA-Z]{1})|"
-    r"([a-zA-Z0-9][-_.a-zA-Z0-9]{0,61}[a-zA-Z0-9]))\."
-    r"([a-zA-Z]{2,13}|[a-zA-Z0-9-]{2,30}.[a-zA-Z]{2,3})$"
-)
-
 
 def parse_address(address: str) -> Optional[Tuple[str, int, Optional[bool]]]:
-    """Parses an IP address into a host, port, and version.
+    """Parses an IP address into host, port, and version.
 
     Parameters
     ----------
     address : str
         The string representation of a domain, an IPv4, or an IPV6 address
         with the port number.
 
         For example, '127.0.0.1:8080', or [::1]:8080.
 
     Returns
     -------
-    Optional[Tuple[str, int, bool]]
-        If the string provided is not a correct IPv6 or IPv4,
+    Optional[Tuple[str, int, Optional[bool]]]
+        If the port provided is incorrect,
         the function will return None, otherwise it will return the host,
-        as a string, the port number, as an int, and
-        a bool that is True if the address is IPv6 and False otherwise.
+        (str), port number (int), and version (bool).
     """
     try:
         raw_host, _, raw_port = address.rpartition(":")
 
-        if DOMAIN_PATTERN.match(raw_host):
-            print(raw_host)
-            host = raw_host
-            version = None
-        else:
-            host = raw_host.translate({ord(i): None for i in "[]"})
-            version = ip_address(host).version == IPV6
-
         port = int(raw_port)
 
         if port > 65535 or port < 1:
             raise ValueError("Port number is invalid.")
 
+        try:
+            host = raw_host.translate({ord(i): None for i in "[]"})
+            version = ip_address(host).version == IPV6
+        except ValueError:
+            host = raw_host
+            version = None
+
         return host, port, version
 
     except ValueError:
         return None
```

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/common/date.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/common/date.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/common/dp.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/common/dp.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/common/grpc.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/common/grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/common/logger.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/common/logger.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/common/parameter.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/common/parameter.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/common/serde.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/common/serde.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/common/telemetry.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/common/telemetry.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/common/typing.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/common/typing.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/common/version.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/common/version.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/driver/__init__.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/driver/driver.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/driver/driver.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/proto/__init__.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/proto/driver_pb2.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/proto/driver_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/proto/driver_pb2.pyi` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/proto/driver_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/proto/driver_pb2_grpc.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/proto/driver_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/proto/driver_pb2_grpc.pyi` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/proto/driver_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/proto/fleet_pb2.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/proto/fleet_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/proto/fleet_pb2.pyi` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/proto/fleet_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/proto/fleet_pb2_grpc.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/proto/fleet_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/proto/fleet_pb2_grpc.pyi` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/proto/fleet_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/proto/node_pb2.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/proto/node_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/proto/node_pb2.pyi` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/proto/node_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/proto/task_pb2.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/proto/task_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/proto/task_pb2.pyi` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/proto/task_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/proto/transport_pb2.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/proto/transport_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/proto/transport_pb2.pyi` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/proto/transport_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/proto/transport_pb2_grpc.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/proto/transport_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/proto/transport_pb2_grpc.pyi` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/proto/transport_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/__init__.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/app.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/app.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,23 +15,25 @@
 """Flower server app."""
 
 
 import argparse
 import sys
 import threading
 from dataclasses import dataclass
-from logging import INFO, WARN
+from logging import ERROR, INFO, WARN
+from os.path import isfile
 from signal import SIGINT, SIGTERM, signal
 from types import FrameType
 from typing import List, Optional, Tuple
 
 import grpc
 
 from flwr.common import GRPC_MAX_MESSAGE_LENGTH, EventType, event
 from flwr.common.address import parse_address
+from flwr.common.constant import MISSING_EXTRA_REST
 from flwr.common.logger import log
 from flwr.proto.driver_pb2_grpc import add_DriverServicer_to_server
 from flwr.proto.transport_pb2_grpc import add_FlowerServiceServicer_to_server
 from flwr.server.client_manager import ClientManager, SimpleClientManager
 from flwr.server.driver.driver_servicer import DriverServicer
 from flwr.server.grpc_server.driver_client_manager import DriverClientManager
 from flwr.server.grpc_server.flower_service_servicer import FlowerServiceServicer
@@ -276,15 +278,20 @@
         address_arg = args.rest_fleet_api_address
         parsed_address = parse_address(address_arg)
         if not parsed_address:
             sys.exit(f"Fleet IP address ({address_arg}) cannot be parsed.")
         host, port, _ = parsed_address
         fleet_thread = threading.Thread(
             target=_run_fleet_api_rest,
-            args=(host, port, state_factory),
+            args=(
+                host,
+                port,
+                state_factory,
+                args.rest_fleet_api_workers,
+            ),
         )
         fleet_thread.start()
         bckg_threads.append(fleet_thread)
     elif args.fleet_api_type == "grpc":
         address_arg = args.grpc_fleet_api_address
         parsed_address = parse_address(address_arg)
         if not parsed_address:
@@ -344,15 +351,22 @@
         address_arg = args.rest_fleet_api_address
         parsed_address = parse_address(address_arg)
         if not parsed_address:
             sys.exit(f"Fleet IP address ({address_arg}) cannot be parsed.")
         host, port, _ = parsed_address
         fleet_thread = threading.Thread(
             target=_run_fleet_api_rest,
-            args=(host, port, state_factory),
+            args=(
+                host,
+                port,
+                args.ssl_keyfile,
+                args.ssl_certfile,
+                state_factory,
+                args.rest_fleet_api_workers,
+            ),
         )
         fleet_thread.start()
         bckg_threads.append(fleet_thread)
     elif args.fleet_api_type == "grpc":
         address_arg = args.grpc_fleet_api_address
         parsed_address = parse_address(address_arg)
         if not parsed_address:
@@ -371,15 +385,20 @@
     _register_exit_handlers(
         grpc_servers=grpc_servers,
         bckg_threads=bckg_threads,
         event_type=EventType.RUN_SERVER_LEAVE,
     )
 
     # Block
-    driver_server.wait_for_termination()
+    while True:
+        if bckg_threads:
+            for thread in bckg_threads:
+                if not thread.is_alive():
+                    sys.exit(1)
+        driver_server.wait_for_termination(timeout=1)
 
 
 def _register_exit_handlers(
     grpc_servers: List[grpc.Server],
     bckg_threads: List[threading.Thread],
     event_type: EventType,
 ) -> None:
@@ -474,47 +493,87 @@
 
     log(INFO, "Flower ECE: Starting Fleet API (gRPC-bidi) on %s", address)
     fleet_grpc_server.start()
 
     return fleet_grpc_server
 
 
-# pylint: disable=import-outside-toplevel
+# pylint: disable=import-outside-toplevel,too-many-arguments
 def _run_fleet_api_rest(
     host: str,
     port: int,
+    ssl_keyfile: Optional[str],
+    ssl_certfile: Optional[str],
     state_factory: StateFactory,
+    workers: int,
 ) -> None:
     """Run Driver API (REST-based)."""
     try:
         import uvicorn
 
         from flwr.server.rest_server.rest_api import app as fast_api_app
-    except ImportError as missing_dep:
-        raise ImportError(
-            "To use the REST API you must install the "
-            "extra dependencies by running "
-            "`pip install flwr['rest']`."
-        ) from missing_dep
+    except ModuleNotFoundError:
+        sys.exit(MISSING_EXTRA_REST)
+    if workers != 1:
+        raise ValueError(
+            f"The supported number of workers for the Fleet API (REST server) is "
+            f"1. Instead given {workers}. The functionality of >1 workers will be "
+            f"added in the future releases."
+        )
     log(INFO, "Starting Flower REST server")
 
     # See: https://www.starlette.io/applications/#accessing-the-app-instance
     fast_api_app.state.STATE_FACTORY = state_factory
 
+    validation_exceptions = _validate_ssl_files(
+        ssl_certfile=ssl_certfile, ssl_keyfile=ssl_keyfile
+    )
+    if any(validation_exceptions):
+        # Starting with 3.11 we can use ExceptionGroup but for now
+        # this seems to be the reasonable approach.
+        raise ValueError(validation_exceptions)
+
     uvicorn.run(
-        # "flwr.server.rest_server.rest_api:app",
-        app=fast_api_app,
+        app="flwr.server.rest_server.rest_api:app",
         port=port,
         host=host,
         reload=False,
         access_log=True,
-        workers=1,
+        ssl_keyfile=ssl_keyfile,
+        ssl_certfile=ssl_certfile,
+        workers=workers,
     )
 
 
+def _validate_ssl_files(
+    ssl_keyfile: Optional[str], ssl_certfile: Optional[str]
+) -> List[ValueError]:
+    validation_exceptions = []
+
+    if ssl_keyfile is not None and not isfile(ssl_keyfile):
+        msg = "Path argument `--ssl-keyfile` does not point to a file."
+        log(ERROR, msg)
+        validation_exceptions.append(ValueError(msg))
+
+    if ssl_certfile is not None and not isfile(ssl_certfile):
+        msg = "Path argument `--ssl-certfile` does not point to a file."
+        log(ERROR, msg)
+        validation_exceptions.append(ValueError(msg))
+
+    if not bool(ssl_keyfile) == bool(ssl_certfile):
+        msg = (
+            "When setting one of `--ssl-keyfile` and "
+            + "`--ssl-certfile`, both have to be used."
+        )
+        log(ERROR, msg)
+        validation_exceptions.append(ValueError(msg))
+
+    return validation_exceptions
+
+
 def _parse_args_driver() -> argparse.ArgumentParser:
     """Parse command line arguments for Driver API."""
     parser = argparse.ArgumentParser(
         description="Start Flower server (Driver API)",
     )
 
     _add_args_common(parser=parser)
@@ -594,7 +653,23 @@
     # Fleet API REST options
     rest_group = parser.add_argument_group("Fleet API REST server options", "")
     rest_group.add_argument(
         "--rest-fleet-api-address",
         help=f"Fleet API REST server address. Default:'{ADDRESS_FLEET_API_REST}'",
         default=ADDRESS_FLEET_API_REST,
     )
+    rest_group.add_argument(
+        "--ssl-certfile",
+        help="Fleet API REST SSL certificate file (as a path str). Default:None",
+        default=None,
+    )
+    rest_group.add_argument(
+        "--ssl-keyfile",
+        help="Fleet API REST SSL private key file (as a path str). Default:None",
+        default=None,
+    )
+    rest_group.add_argument(
+        "--rest-fleet-api-workers",
+        help=f"Number of workers for Fleet API REST server. Default:'{1}'",
+        type=int,
+        default=1,
+    )
```

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/client_manager.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/client_manager.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/client_proxy.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/criterion.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/criterion.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/driver/__init__.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/driver/driver_servicer.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/driver/driver_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/fleet/__init__.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/fleet/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/fleet/fleet_servicer.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/fleet/fleet_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/grpc_server/__init__.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/grpc_server/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/grpc_server/driver_client_manager.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/grpc_server/driver_client_manager.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/grpc_server/flower_service_servicer.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/grpc_server/flower_service_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/grpc_server/grpc_bridge.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/grpc_server/grpc_bridge.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/grpc_server/grpc_client_proxy.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/grpc_server/grpc_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/grpc_server/grpc_server.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/grpc_server/grpc_server.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/grpc_server/ins_scheduler.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/grpc_server/ins_scheduler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/history.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/history.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/rest_server/__init__.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/rest_server/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/rest_server/rest_api.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/rest_server/rest_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,38 +11,38 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """REST API server."""
 
 
+import sys
 from logging import INFO
 from typing import List, Optional
 from uuid import UUID
 
-try:
-    from fastapi import FastAPI, HTTPException, Request, Response
-    from starlette.datastructures import Headers
-except ImportError as missing_dep:
-    raise ImportError(
-        "To use the REST API you must install the "
-        "extra dependencies by running `pip install flwr['rest']`."
-    ) from missing_dep
-
+from flwr.common.constant import MISSING_EXTRA_REST
 from flwr.common.logger import log
 from flwr.proto.fleet_pb2 import (
     PullTaskInsRequest,
     PullTaskInsResponse,
     PushTaskResRequest,
     PushTaskResResponse,
     Reconnect,
 )
 from flwr.proto.task_pb2 import TaskIns, TaskRes
 from flwr.server.state import State
 
+try:
+    from fastapi import FastAPI, HTTPException, Request, Response
+    from starlette.datastructures import Headers
+except ModuleNotFoundError:
+    sys.exit(MISSING_EXTRA_REST)
+
+
 app: FastAPI = FastAPI()
 
 
 @app.post("/api/v0/fleet/pull-task-ins", response_class=Response)  # type: ignore
 async def pull_task_ins(request: Request) -> Response:
     """Pull TaskIns."""
     _check_headers(request.headers)
```

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/server.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/server.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/state/__init__.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/state/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/state/in_memory_state.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/state/in_memory_state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/state/sqlite_state.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/state/sqlite_state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/state/state.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/state/state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/state/state_factory.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/state/state_factory.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/strategy/__init__.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/strategy/aggregate.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/strategy/aggregate.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/strategy/dpfedavg_adaptive.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/strategy/dpfedavg_adaptive.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/strategy/dpfedavg_fixed.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/strategy/dpfedavg_fixed.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/strategy/fault_tolerant_fedavg.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/strategy/fault_tolerant_fedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/strategy/fedadagrad.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/strategy/fedadagrad.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/strategy/fedadam.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/strategy/fedadam.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/strategy/fedavg.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/strategy/fedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/strategy/fedavg_android.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/strategy/fedavg_android.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/strategy/fedavgm.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/strategy/fedavgm.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/strategy/fedmedian.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/strategy/fedmedian.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/strategy/fedopt.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/strategy/fedopt.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/strategy/fedprox.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/strategy/fedprox.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/strategy/fedxgb_nn_avg.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/strategy/fedxgb_nn_avg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/strategy/fedyogi.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/strategy/fedyogi.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/strategy/krum.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/strategy/krum.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/strategy/qfedavg.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/strategy/qfedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/strategy/strategy.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/strategy/strategy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/utils/__init__.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/utils/tensorboard.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/utils/tensorboard.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/server/utils/validator.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/server/utils/validator.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/simulation/__init__.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/simulation/app.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/simulation/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/simulation/ray_transport/__init__.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/simulation/ray_transport/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/src/py/flwr/simulation/ray_transport/ray_client_proxy.py` & `flwr_nightly-1.4.0.dev20230419/src/py/flwr/simulation/ray_transport/ray_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230418/setup.py` & `flwr_nightly-1.4.0.dev20230419/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 {'console_scripts': ['flower-client = flwr.client:run_client',
                      'flower-driver-api = flwr.server:run_driver_api',
                      'flower-fleet-api = flwr.server:run_fleet_api',
                      'flower-server = flwr.server:run_server']}
 
 setup_kwargs = {
     'name': 'flwr-nightly',
-    'version': '1.4.0.dev20230418',
+    'version': '1.4.0.dev20230419',
     'description': 'Flower: A Friendly Federated Learning Framework',
     'long_description': '# Flower: A Friendly Federated Learning Framework\n\n<p align="center">\n  <a href="https://flower.dev/">\n    <img src="https://flower.dev/_next/image/?url=%2F_next%2Fstatic%2Fmedia%2Fflower_white_border.c2012e70.png&w=640&q=75" width="140px" alt="Flower Website" />\n  </a>\n</p>\n<p align="center">\n    <a href="https://flower.dev/">Website</a> |\n    <a href="https://flower.dev/blog">Blog</a> |\n    <a href="https://flower.dev/docs/">Docs</a> |\n    <a href="https://flower.dev/conf/flower-summit-2022">Conference</a> |\n    <a href="https://flower.dev/join-slack">Slack</a>\n    <br /><br />\n</p>\n\n[![GitHub license](https://img.shields.io/github/license/adap/flower)](https://github.com/adap/flower/blob/main/LICENSE)\n[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/adap/flower/blob/main/CONTRIBUTING.md)\n![Build](https://github.com/adap/flower/actions/workflows/flower.yml/badge.svg)\n![Downloads](https://pepy.tech/badge/flwr)\n[![Slack](https://img.shields.io/badge/Chat-Slack-red)](https://flower.dev/join-slack)\n\nFlower (`flwr`) is a framework for building federated learning systems. The\ndesign of Flower is based on a few guiding principles:\n\n* **Customizable**: Federated learning systems vary wildly from one use case to\n  another. Flower allows for a wide range of different configurations depending\n  on the needs of each individual use case.\n\n* **Extendable**: Flower originated from a research project at the University of\n  Oxford, so it was built with AI research in mind. Many components can be\n  extended and overridden to build new state-of-the-art systems.\n\n* **Framework-agnostic**: Different machine learning frameworks have different\n  strengths. Flower can be used with any machine learning framework, for\n  example, [PyTorch](https://pytorch.org),\n  [TensorFlow](https://tensorflow.org), [Hugging Face Transformers](https://huggingface.co/), [PyTorch Lightning](https://pytorchlightning.ai/), [MXNet](https://mxnet.apache.org/), [scikit-learn](https://scikit-learn.org/), [JAX](https://jax.readthedocs.io/), [TFLite](https://tensorflow.org/lite/), [fastai](https://www.fast.ai/), [Pandas](https://pandas.pydata.org/\n) for federated analytics, or even raw [NumPy](https://numpy.org/)\n  for users who enjoy computing gradients by hand.\n\n* **Understandable**: Flower is written with maintainability in mind. The\n  community is encouraged to both read and contribute to the codebase.\n\nMeet the Flower community on [flower.dev](https://flower.dev)!\n\n## Federated Learning Tutorial\n\nFlower\'s goal is to make federated learning accessible to everyone. This series of tutorials introduces the fundamentals of federated learning and how to implement them in Flower.\n\n0. **What is Federated Learning?**\n\n   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-0-What-is-FL.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-0-What-is-FL.ipynb))\n\n1. **An Introduction to Federated Learning**\n\n   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-1-Intro-to-FL-PyTorch.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-1-Intro-to-FL-PyTorch.ipynb))\n\n2. **Using Strategies in Federated Learning**\n\n   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-2-Strategies-in-FL-PyTorch.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-2-Strategies-in-FL-PyTorch.ipynb))\n   \n3. **Building Strategies for Federated Learning**\n\n   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-3-Building-a-Strategy-PyTorch.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-3-Building-a-Strategy-PyTorch.ipynb))\n   \n4. **Custom Clients for Federated Learning**\n\n   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-4-Client-and-NumPyClient-PyTorch.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-4-Client-and-NumPyClient-PyTorch.ipynb))\n\nStay tuned, more tutorials are coming soon. Topics include **Privacy and Security in Federated Learning**, and **Scaling Federated Learning**.\n\n## Documentation\n\n[Flower Docs](https://flower.dev/docs):\n* [Installation](https://flower.dev/docs/installation.html)\n* [Quickstart (TensorFlow)](https://flower.dev/docs/quickstart-tensorflow.html)\n* [Quickstart (PyTorch)](https://flower.dev/docs/quickstart-pytorch.html)\n* [Quickstart (Hugging Face [code example])](https://flower.dev/docs/quickstart-huggingface.html)\n* [Quickstart (PyTorch Lightning [code example])](https://flower.dev/docs/quickstart-pytorch-lightning.html)\n* [Quickstart (MXNet)](https://flower.dev/docs/example-mxnet-walk-through.html)\n* [Quickstart (Pandas)](https://flower.dev/docs/quickstart-pandas.html)\n* [Quickstart (fastai)](https://flower.dev/docs/quickstart-fastai.html)\n* [Quickstart (JAX)](https://github.com/adap/flower/tree/main/examples/quickstart_jax)\n* [Quickstart (scikit-learn)](https://github.com/adap/flower/tree/main/examples/sklearn-logreg-mnist)\n* [Quickstart (TFLite on Android [code example])](https://github.com/adap/flower/tree/main/examples/android)\n\n## Flower Baselines\n\nFlower Baselines is a collection of community-contributed experiments that reproduce the experiments performed in popular federated learning publications. Researchers can build on Flower Baselines to quickly evaluate new ideas:\n\n* [FedAvg](https://arxiv.org/abs/1602.05629):\n  * [MNIST](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/fedavg_mnist)\n* [FedProx](https://arxiv.org/abs/1812.06127):\n  * [MNIST](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/fedprox_mnist)\n* [FedBN: Federated Learning on non-IID Features via Local Batch Normalization](https://arxiv.org/abs/2102.07623):\n  * [Convergence Rate](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/fedbn/convergence_rate)\n* [Adaptive Federated Optimization](https://arxiv.org/abs/2003.00295):\n  * [CIFAR-10/100](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/adaptive_federated_optimization)\n\nCheck the Flower documentation to learn more: [Using Baselines](https://flower.dev/docs/using-baselines.html)\n\nThe Flower community loves contributions! Make your work more visible and enable others to build on it by contributing it as a baseline: [Contributing Baselines](https://flower.dev/docs/contributing-baselines.html)\n\n## Flower Usage Examples\n\nSeveral code examples show different usage scenarios of Flower (in combination with popular machine learning frameworks such as PyTorch or TensorFlow).\n\nQuickstart examples:\n\n* [Quickstart (TensorFlow)](https://github.com/adap/flower/tree/main/examples/quickstart_tensorflow)\n* [Quickstart (PyTorch)](https://github.com/adap/flower/tree/main/examples/quickstart_pytorch)\n* [Quickstart (Hugging Face)](https://github.com/adap/flower/tree/main/examples/quickstart_huggingface)\n* [Quickstart (PyTorch Lightning)](https://github.com/adap/flower/tree/main/examples/quickstart_pytorch_lightning)\n* [Quickstart (fastai)](https://github.com/adap/flower/tree/main/examples/quickstart_fastai)\n* [Quickstart (Pandas)](https://github.com/adap/flower/tree/main/examples/quickstart_pandas)\n* [Quickstart (MXNet)](https://github.com/adap/flower/tree/main/examples/quickstart_mxnet)\n* [Quickstart (JAX)](https://github.com/adap/flower/tree/main/examples/quickstart_jax)\n* [Quickstart (scikit-learn)](https://github.com/adap/flower/tree/main/examples/sklearn-logreg-mnist)\n* [Quickstart (TFLite on Android)](https://github.com/adap/flower/tree/main/examples/android)\n\nOther [examples](https://github.com/adap/flower/tree/main/examples):\n\n* [Raspberry Pi & Nvidia Jetson Tutorial](https://github.com/adap/flower/tree/main/examples/embedded_devices)\n* [Android & TFLite](https://github.com/adap/flower/tree/main/examples/android)\n* [PyTorch: From Centralized to Federated](https://github.com/adap/flower/tree/main/examples/pytorch_from_centralized_to_federated)\n* [MXNet: From Centralized to Federated](https://github.com/adap/flower/tree/main/examples/mxnet_from_centralized_to_federated)\n* [Advanced Flower with TensorFlow/Keras](https://github.com/adap/flower/tree/main/examples/advanced_tensorflow)\n* [Advanced Flower with PyTorch](https://github.com/adap/flower/tree/main/examples/advanced_pytorch)\n* Single-Machine Simulation of Federated Learning Systems ([PyTorch](https://github.com/adap/flower/tree/main/examples/simulation_pytorch)) ([Tensorflow](https://github.com/adap/flower/tree/main/examples/simulation_tensorflow))\n\n## Community\n\nFlower is built by a wonderful community of researchers and engineers. [Join Slack](https://flower.dev/join-slack) to meet them, [contributions](#contributing-to-flower) are welcome.\n\n<a href="https://github.com/adap/flower/graphs/contributors">\n  <img src="https://contrib.rocks/image?repo=adap/flower" />\n</a>\n\n## Citation\n\nIf you publish work that uses Flower, please cite Flower as follows: \n\n```bibtex\n@article{beutel2020flower,\n  title={Flower: A Friendly Federated Learning Research Framework},\n  author={Beutel, Daniel J and Topal, Taner and Mathur, Akhil and Qiu, Xinchi and Fernandez-Marques, Javier and Gao, Yan and Sani, Lorenzo and Kwing, Hei Li and Parcollet, Titouan and Gusmão, Pedro PB de and Lane, Nicholas D}, \n  journal={arXiv preprint arXiv:2007.14390},\n  year={2020}\n}\n```\n\nPlease also consider adding your publication to the list of Flower-based publications in the docs, just open a Pull Request.\n\n## Contributing to Flower\n\nWe welcome contributions. Please see [CONTRIBUTING.md](CONTRIBUTING.md) to get started!\n',
     'author': 'The Flower Authors',
     'author_email': 'hello@flower.dev',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://flower.dev',
```

#### html2text {}

```diff
@@ -10,15 +10,15 @@
 extras_require = \ {':python_version < "3.8"': ['importlib-
 metadata>=4.0.0,<5.0.0'], 'rest': ['requests>=2.28.2,<3.0.0',
 'fastapi>=0.95.0,<0.96.0', 'starlette>=0.26.1,<0.27.0', 'uvicorn
 [standard]>=0.21.1,<0.22.0'], 'simulation': ['ray[default]>=2.3.0,<3.0.0']}
 entry_points = \ {'console_scripts': ['flower-client = flwr.client:run_client',
 'flower-driver-api = flwr.server:run_driver_api', 'flower-fleet-api =
 flwr.server:run_fleet_api', 'flower-server = flwr.server:run_server']}
-setup_kwargs = { 'name': 'flwr-nightly', 'version': '1.4.0.dev20230418',
+setup_kwargs = { 'name': 'flwr-nightly', 'version': '1.4.0.dev20230419',
 'description': 'Flower: A Friendly Federated Learning Framework',
 'long_description': '# Flower: A Friendly Federated Learning Framework\n\n
                           \n \n_[Flower_Website]\n\n
 \n
            \n Website |\n Blog |\n Docs |\n Conference |\n Slack\n
 
                                       \n
```

### Comparing `flwr_nightly-1.4.0.dev20230418/PKG-INFO` & `flwr_nightly-1.4.0.dev20230419/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flwr-nightly
-Version: 1.4.0.dev20230418
+Version: 1.4.0.dev20230419
 Summary: Flower: A Friendly Federated Learning Framework
 Home-page: https://flower.dev
 License: Apache-2.0
 Author: The Flower Authors
 Author-email: hello@flower.dev
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flwr-nightly Version: 1.4.0.dev20230418 Summary:
+Metadata-Version: 2.1 Name: flwr-nightly Version: 1.4.0.dev20230419 Summary:
 Flower: A Friendly Federated Learning Framework Home-page: https://flower.dev
 License: Apache-2.0 Author: The Flower Authors Author-email: hello@flower.dev
 Requires-Python: >=3.7,<4.0 Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Science/Research Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Operating System :: MacOS :: MacOS X Classifier:
 Operating System :: POSIX :: Linux Classifier: Programming Language :: Python
```

