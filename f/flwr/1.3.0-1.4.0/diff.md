# Comparing `tmp/flwr-1.3.0.tar.gz` & `tmp/flwr-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flwr-1.3.0.tar", max compression
+gzip compressed data, was "flwr-1.4.0.tar", max compression
```

## Comparing `flwr-1.3.0.tar` & `flwr-1.4.0.tar`

### file list

```diff
@@ -1,92 +1,104 @@
--rw-r--r--   0        0        0    11358 2021-12-13 18:43:20.949296 flwr-1.3.0/LICENSE
--rw-r--r--   0        0        0     9703 2023-02-03 23:47:01.045135 flwr-1.3.0/README.md
--rw-r--r--   0        0        0     3947 2023-02-06 19:58:33.321264 flwr-1.3.0/pyproject.toml
--rw-r--r--   0        0        0      907 2023-01-28 04:18:48.877907 flwr-1.3.0/src/py/flwr/__init__.py
--rw-r--r--   0        0        0     1164 2022-10-31 15:06:38.979249 flwr-1.3.0/src/py/flwr/client/__init__.py
--rw-r--r--   0        0        0    10706 2023-02-06 08:22:42.786442 flwr-1.3.0/src/py/flwr/client/app.py
--rw-r--r--   0        0        0     6503 2022-10-31 15:06:38.980034 flwr-1.3.0/src/py/flwr/client/client.py
--rw-r--r--   0        0        0     3352 2022-10-31 15:06:38.980470 flwr-1.3.0/src/py/flwr/client/dpfedavg_numpy_client.py
--rw-r--r--   0        0        0      728 2022-10-31 15:06:38.980743 flwr-1.3.0/src/py/flwr/client/grpc_client/__init__.py
--rw-r--r--   0        0        0     4117 2022-10-31 15:06:38.981201 flwr-1.3.0/src/py/flwr/client/grpc_client/connection.py
--rw-r--r--   0        0        0      712 2022-10-31 15:06:38.981668 flwr-1.3.0/src/py/flwr/client/message_handler/__init__.py
--rw-r--r--   0        0        0     5077 2022-10-31 15:06:38.981911 flwr-1.3.0/src/py/flwr/client/message_handler/message_handler.py
--rw-r--r--   0        0        0     5100 2022-10-31 15:06:38.982323 flwr-1.3.0/src/py/flwr/client/numpy_client.py
--rw-r--r--   0        0        0     2734 2023-01-28 04:18:48.878227 flwr-1.3.0/src/py/flwr/common/__init__.py
--rw-r--r--   0        0        0     1827 2022-10-31 15:06:38.983200 flwr-1.3.0/src/py/flwr/common/dp.py
--rw-r--r--   0        0        0     1894 2022-10-31 15:06:38.983584 flwr-1.3.0/src/py/flwr/common/grpc.py
--rw-r--r--   0        0        0     3481 2023-01-28 04:18:48.878461 flwr-1.3.0/src/py/flwr/common/logger.py
--rw-r--r--   0        0        0     2120 2022-10-31 15:06:38.983691 flwr-1.3.0/src/py/flwr/common/parameter.py
--rw-r--r--   0        0        0    16316 2022-10-31 15:06:38.984261 flwr-1.3.0/src/py/flwr/common/serde.py
--rw-r--r--   0        0        0     7499 2023-02-06 05:13:22.247252 flwr-1.3.0/src/py/flwr/common/telemetry.py
--rw-r--r--   0        0        0     3714 2022-10-31 15:06:38.985055 flwr-1.3.0/src/py/flwr/common/typing.py
--rw-r--r--   0        0        0      846 2023-01-28 04:18:48.878815 flwr-1.3.0/src/py/flwr/common/version.py
--rw-r--r--   0        0        0      769 2023-01-28 04:18:48.879074 flwr-1.3.0/src/py/flwr/driver/__init__.py
--rw-r--r--   0        0        0     3909 2023-02-03 23:55:07.871253 flwr-1.3.0/src/py/flwr/driver/driver.py
--rw-r--r--   0        0        0      676 2021-12-13 18:43:21.067065 flwr-1.3.0/src/py/flwr/proto/__init__.py
--rw-r--r--   0        0        0    11023 2023-01-28 04:18:48.879372 flwr-1.3.0/src/py/flwr/proto/driver_pb2.py
--rw-r--r--   0        0        0     3815 2023-01-28 04:18:48.879518 flwr-1.3.0/src/py/flwr/proto/driver_pb2.pyi
--rw-r--r--   0        0        0     5727 2023-01-28 04:18:48.879859 flwr-1.3.0/src/py/flwr/proto/driver_pb2_grpc.py
--rw-r--r--   0        0        0     1617 2023-01-28 04:18:48.880099 flwr-1.3.0/src/py/flwr/proto/driver_pb2_grpc.pyi
--rw-r--r--   0        0        0    12936 2023-01-28 04:18:48.880237 flwr-1.3.0/src/py/flwr/proto/fleet_pb2.py
--rw-r--r--   0        0        0     4554 2023-01-28 04:18:48.880355 flwr-1.3.0/src/py/flwr/proto/fleet_pb2.pyi
--rw-r--r--   0        0        0     4275 2023-01-28 04:18:48.880592 flwr-1.3.0/src/py/flwr/proto/fleet_pb2_grpc.py
--rw-r--r--   0        0        0     1495 2023-01-28 04:18:48.880789 flwr-1.3.0/src/py/flwr/proto/fleet_pb2_grpc.pyi
--rw-r--r--   0        0        0     2412 2023-01-28 04:18:48.881000 flwr-1.3.0/src/py/flwr/proto/node_pb2.py
--rw-r--r--   0        0        0      751 2023-01-28 04:18:48.881137 flwr-1.3.0/src/py/flwr/proto/node_pb2.pyi
--rw-r--r--   0        0        0      159 2023-01-28 04:18:48.881351 flwr-1.3.0/src/py/flwr/proto/node_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-01-28 04:18:48.881565 flwr-1.3.0/src/py/flwr/proto/node_pb2_grpc.pyi
--rw-r--r--   0        0        0    11502 2023-01-28 04:18:48.881718 flwr-1.3.0/src/py/flwr/proto/task_pb2.py
--rw-r--r--   0        0        0     4286 2023-01-28 04:18:48.881864 flwr-1.3.0/src/py/flwr/proto/task_pb2.pyi
--rw-r--r--   0        0        0      159 2023-01-24 23:54:51.068583 flwr-1.3.0/src/py/flwr/proto/task_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-01-24 23:54:51.068641 flwr-1.3.0/src/py/flwr/proto/task_pb2_grpc.pyi
--rw-r--r--   0        0        0    58682 2023-01-24 23:54:51.068727 flwr-1.3.0/src/py/flwr/proto/transport_pb2.py
--rw-r--r--   0        0        0    21497 2023-01-24 23:54:51.068787 flwr-1.3.0/src/py/flwr/proto/transport_pb2.pyi
--rw-r--r--   0        0        0     2598 2023-01-24 23:54:51.068839 flwr-1.3.0/src/py/flwr/proto/transport_pb2_grpc.py
--rw-r--r--   0        0        0      766 2023-01-24 23:54:51.068884 flwr-1.3.0/src/py/flwr/proto/transport_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2022-10-31 15:06:38.992384 flwr-1.3.0/src/py/flwr/py.typed
--rw-r--r--   0        0        0     1190 2022-10-31 15:06:38.992652 flwr-1.3.0/src/py/flwr/server/__init__.py
--rw-r--r--   0        0        0    11063 2023-02-06 08:22:42.786683 flwr-1.3.0/src/py/flwr/server/app.py
--rw-r--r--   0        0        0     5941 2023-01-28 04:18:48.882410 flwr-1.3.0/src/py/flwr/server/client_manager.py
--rw-r--r--   0        0        0     2228 2023-01-28 04:18:48.882779 flwr-1.3.0/src/py/flwr/server/client_proxy.py
--rw-r--r--   0        0        0     1058 2021-12-13 18:43:21.067866 flwr-1.3.0/src/py/flwr/server/criterion.py
--rw-r--r--   0        0        0      705 2022-10-31 15:06:38.994058 flwr-1.3.0/src/py/flwr/server/driver/__init__.py
--rw-r--r--   0        0        0     4814 2023-02-06 03:53:52.201871 flwr-1.3.0/src/py/flwr/server/driver/driver_servicer.py
--rw-r--r--   0        0        0      704 2022-10-31 15:06:38.994845 flwr-1.3.0/src/py/flwr/server/fleet/__init__.py
--rw-r--r--   0        0        0     1638 2023-02-06 03:53:52.202051 flwr-1.3.0/src/py/flwr/server/fleet/fleet_servicer.py
--rw-r--r--   0        0        0      728 2022-10-31 15:06:38.995604 flwr-1.3.0/src/py/flwr/server/grpc_server/__init__.py
--rw-r--r--   0        0        0     4295 2023-02-06 03:53:52.202263 flwr-1.3.0/src/py/flwr/server/grpc_server/driver_client_manager.py
--rw-r--r--   0        0        0     5594 2023-01-28 04:18:48.884893 flwr-1.3.0/src/py/flwr/server/grpc_server/flower_service_servicer.py
--rw-r--r--   0        0        0     6416 2023-01-28 04:18:48.885665 flwr-1.3.0/src/py/flwr/server/grpc_server/grpc_bridge.py
--rw-r--r--   0        0        0     4623 2023-01-28 04:18:48.886497 flwr-1.3.0/src/py/flwr/server/grpc_server/grpc_client_proxy.py
--rw-r--r--   0        0        0    11509 2022-10-31 15:06:38.996931 flwr-1.3.0/src/py/flwr/server/grpc_server/grpc_server.py
--rw-r--r--   0        0        0     6146 2023-02-06 03:53:52.202433 flwr-1.3.0/src/py/flwr/server/grpc_server/ins_scheduler.py
--rw-r--r--   0        0        0     3623 2022-10-31 15:06:38.997043 flwr-1.3.0/src/py/flwr/server/history.py
--rw-r--r--   0        0        0    15706 2022-10-31 15:06:38.997529 flwr-1.3.0/src/py/flwr/server/server.py
--rw-r--r--   0        0        0      822 2023-02-06 03:53:52.202611 flwr-1.3.0/src/py/flwr/server/state/__init__.py
--rw-r--r--   0        0        0     5179 2023-02-06 03:53:52.202740 flwr-1.3.0/src/py/flwr/server/state/in_memory_state.py
--rw-r--r--   0        0        0     1847 2023-02-06 03:53:52.203015 flwr-1.3.0/src/py/flwr/server/state/state.py
--rw-r--r--   0        0        0     1515 2023-02-03 23:47:01.047050 flwr-1.3.0/src/py/flwr/server/strategy/__init__.py
--rw-r--r--   0        0        0     4994 2023-01-28 04:18:48.886988 flwr-1.3.0/src/py/flwr/server/strategy/aggregate.py
--rw-r--r--   0        0        0     4519 2022-10-31 15:06:38.998480 flwr-1.3.0/src/py/flwr/server/strategy/dpfedavg_adaptive.py
--rw-r--r--   0        0        0     4874 2022-10-31 15:06:38.998798 flwr-1.3.0/src/py/flwr/server/strategy/dpfedavg_fixed.py
--rw-r--r--   0        0        0     5978 2022-10-31 15:06:38.999096 flwr-1.3.0/src/py/flwr/server/strategy/fault_tolerant_fedavg.py
--rw-r--r--   0        0        0     6740 2022-10-31 15:06:38.999704 flwr-1.3.0/src/py/flwr/server/strategy/fedadagrad.py
--rw-r--r--   0        0        0     7022 2022-10-31 15:06:39.000070 flwr-1.3.0/src/py/flwr/server/strategy/fedadam.py
--rw-r--r--   0        0        0    11494 2022-10-31 15:06:39.000562 flwr-1.3.0/src/py/flwr/server/strategy/fedavg.py
--rw-r--r--   0        0        0     9985 2022-10-31 15:06:39.001040 flwr-1.3.0/src/py/flwr/server/strategy/fedavg_android.py
--rw-r--r--   0        0        0     8952 2022-10-31 15:06:39.001421 flwr-1.3.0/src/py/flwr/server/strategy/fedavgm.py
--rw-r--r--   0        0        0     6468 2023-01-28 04:18:48.887193 flwr-1.3.0/src/py/flwr/server/strategy/fedmedian.py
--rw-r--r--   0        0        0     5403 2022-10-31 15:06:39.001841 flwr-1.3.0/src/py/flwr/server/strategy/fedopt.py
--rw-r--r--   0        0        0     7707 2023-02-03 23:47:01.047128 flwr-1.3.0/src/py/flwr/server/strategy/fedprox.py
--rw-r--r--   0        0        0     7054 2022-10-31 15:06:39.002043 flwr-1.3.0/src/py/flwr/server/strategy/fedyogi.py
--rw-r--r--   0        0        0     7010 2023-01-28 04:18:48.887431 flwr-1.3.0/src/py/flwr/server/strategy/krum.py
--rw-r--r--   0        0        0    10744 2022-10-31 15:06:39.002341 flwr-1.3.0/src/py/flwr/server/strategy/qfedavg.py
--rw-r--r--   0        0        0     7484 2022-10-31 15:06:39.002465 flwr-1.3.0/src/py/flwr/server/strategy/strategy.py
--rw-r--r--   0        0        0      845 2021-12-13 18:43:21.070523 flwr-1.3.0/src/py/flwr/server/utils/__init__.py
--rw-r--r--   0        0        0     5112 2022-10-31 15:06:39.003013 flwr-1.3.0/src/py/flwr/server/utils/tensorboard.py
--rw-r--r--   0        0        0     1270 2022-10-31 15:06:39.003243 flwr-1.3.0/src/py/flwr/simulation/__init__.py
--rw-r--r--   0        0        0     7801 2023-02-06 05:13:22.247570 flwr-1.3.0/src/py/flwr/simulation/app.py
--rw-r--r--   0        0        0      727 2021-12-13 18:43:21.071065 flwr-1.3.0/src/py/flwr/simulation/ray_transport/__init__.py
--rw-r--r--   0        0        0     5536 2023-01-28 04:18:48.887855 flwr-1.3.0/src/py/flwr/simulation/ray_transport/ray_client_proxy.py
--rw-r--r--   0        0        0    11497 1970-01-01 00:00:00.000000 flwr-1.3.0/setup.py
--rw-r--r--   0        0        0    12096 1970-01-01 00:00:00.000000 flwr-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2021-12-13 18:43:20.949296 flwr-1.4.0/LICENSE
+-rw-r--r--   0        0        0    10297 2023-04-20 21:34:06.864418 flwr-1.4.0/README.md
+-rw-r--r--   0        0        0     4249 2023-04-21 07:38:16.652350 flwr-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0      930 2023-04-19 19:48:18.749574 flwr-1.4.0/src/py/flwr/__init__.py
+-rw-r--r--   0        0        0     1164 2022-10-31 15:06:38.979249 flwr-1.4.0/src/py/flwr/client/__init__.py
+-rw-r--r--   0        0        0    12441 2023-04-19 19:51:43.062560 flwr-1.4.0/src/py/flwr/client/app.py
+-rw-r--r--   0        0        0     6503 2023-04-09 17:40:02.229435 flwr-1.4.0/src/py/flwr/client/client.py
+-rw-r--r--   0        0        0     3351 2023-02-12 07:14:44.610718 flwr-1.4.0/src/py/flwr/client/dpfedavg_numpy_client.py
+-rw-r--r--   0        0        0      728 2022-10-31 15:06:38.980743 flwr-1.4.0/src/py/flwr/client/grpc_client/__init__.py
+-rw-r--r--   0        0        0     4288 2023-04-19 19:48:18.750067 flwr-1.4.0/src/py/flwr/client/grpc_client/connection.py
+-rw-r--r--   0        0        0      712 2022-10-31 15:06:38.981668 flwr-1.4.0/src/py/flwr/client/message_handler/__init__.py
+-rw-r--r--   0        0        0     5077 2022-10-31 15:06:38.981911 flwr-1.4.0/src/py/flwr/client/message_handler/message_handler.py
+-rw-r--r--   0        0        0     1686 2023-02-26 21:43:11.338717 flwr-1.4.0/src/py/flwr/client/message_handler/task_handler.py
+-rw-r--r--   0        0        0     5100 2023-04-09 17:40:02.229887 flwr-1.4.0/src/py/flwr/client/numpy_client.py
+-rw-r--r--   0        0        0      728 2023-02-26 21:43:11.339004 flwr-1.4.0/src/py/flwr/client/rest_client/__init__.py
+-rw-r--r--   0        0        0     8194 2023-04-19 19:51:43.062801 flwr-1.4.0/src/py/flwr/client/rest_client/connection.py
+-rw-r--r--   0        0        0     2877 2023-04-19 19:48:18.750789 flwr-1.4.0/src/py/flwr/common/__init__.py
+-rw-r--r--   0        0        0     1876 2023-04-19 19:51:43.062999 flwr-1.4.0/src/py/flwr/common/address.py
+-rw-r--r--   0        0        0      898 2023-04-19 19:51:43.063344 flwr-1.4.0/src/py/flwr/common/constant.py
+-rw-r--r--   0        0        0      884 2023-02-20 20:54:47.584164 flwr-1.4.0/src/py/flwr/common/date.py
+-rw-r--r--   0        0        0     1828 2023-04-19 19:48:18.751606 flwr-1.4.0/src/py/flwr/common/dp.py
+-rw-r--r--   0        0        0     1894 2022-10-31 15:06:38.983584 flwr-1.4.0/src/py/flwr/common/grpc.py
+-rw-r--r--   0        0        0     3483 2023-04-19 19:48:18.751732 flwr-1.4.0/src/py/flwr/common/logger.py
+-rw-r--r--   0        0        0     2120 2022-10-31 15:06:38.983691 flwr-1.4.0/src/py/flwr/common/parameter.py
+-rw-r--r--   0        0        0    16316 2023-04-09 17:40:02.230731 flwr-1.4.0/src/py/flwr/common/serde.py
+-rw-r--r--   0        0        0     7684 2023-04-19 19:48:18.751869 flwr-1.4.0/src/py/flwr/common/telemetry.py
+-rw-r--r--   0        0        0     3714 2022-10-31 15:06:38.985055 flwr-1.4.0/src/py/flwr/common/typing.py
+-rw-r--r--   0        0        0      848 2023-04-19 19:48:18.752227 flwr-1.4.0/src/py/flwr/common/version.py
+-rw-r--r--   0        0        0      769 2023-04-19 19:51:40.382732 flwr-1.4.0/src/py/flwr/driver/__init__.py
+-rw-r--r--   0        0        0     3909 2023-04-19 19:51:40.382871 flwr-1.4.0/src/py/flwr/driver/driver.py
+-rw-r--r--   0        0        0      676 2021-12-13 18:43:21.067065 flwr-1.4.0/src/py/flwr/proto/__init__.py
+-rw-r--r--   0        0        0     4663 2023-04-09 17:12:07.193366 flwr-1.4.0/src/py/flwr/proto/driver_pb2.py
+-rw-r--r--   0        0        0     3815 2023-04-08 20:10:22.055622 flwr-1.4.0/src/py/flwr/proto/driver_pb2.pyi
+-rw-r--r--   0        0        0     5727 2023-04-08 20:10:22.055705 flwr-1.4.0/src/py/flwr/proto/driver_pb2_grpc.py
+-rw-r--r--   0        0        0     1617 2023-04-08 20:10:22.055804 flwr-1.4.0/src/py/flwr/proto/driver_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4982 2023-04-09 17:12:07.193560 flwr-1.4.0/src/py/flwr/proto/fleet_pb2.py
+-rw-r--r--   0        0        0     4554 2023-04-08 20:10:22.055948 flwr-1.4.0/src/py/flwr/proto/fleet_pb2.pyi
+-rw-r--r--   0        0        0     4275 2023-04-08 20:10:22.056042 flwr-1.4.0/src/py/flwr/proto/fleet_pb2_grpc.py
+-rw-r--r--   0        0        0     1495 2023-04-08 20:10:22.056138 flwr-1.4.0/src/py/flwr/proto/fleet_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1188 2023-04-09 17:12:07.193731 flwr-1.4.0/src/py/flwr/proto/node_pb2.py
+-rw-r--r--   0        0        0      751 2023-04-08 20:10:22.056255 flwr-1.4.0/src/py/flwr/proto/node_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-08 20:10:22.056304 flwr-1.4.0/src/py/flwr/proto/node_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-04-08 20:10:22.056351 flwr-1.4.0/src/py/flwr/proto/node_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3217 2023-04-09 17:12:07.193901 flwr-1.4.0/src/py/flwr/proto/task_pb2.py
+-rw-r--r--   0        0        0     4286 2023-04-08 20:10:22.056444 flwr-1.4.0/src/py/flwr/proto/task_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-08 20:10:22.056542 flwr-1.4.0/src/py/flwr/proto/task_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-04-08 20:10:22.056592 flwr-1.4.0/src/py/flwr/proto/task_pb2_grpc.pyi
+-rw-r--r--   0        0        0    18721 2023-04-09 17:12:07.194123 flwr-1.4.0/src/py/flwr/proto/transport_pb2.py
+-rw-r--r--   0        0        0    21497 2023-04-08 20:10:22.056752 flwr-1.4.0/src/py/flwr/proto/transport_pb2.pyi
+-rw-r--r--   0        0        0     2598 2023-04-08 20:10:22.056825 flwr-1.4.0/src/py/flwr/proto/transport_pb2_grpc.py
+-rw-r--r--   0        0        0      766 2023-04-08 20:10:22.056930 flwr-1.4.0/src/py/flwr/proto/transport_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2022-10-31 15:06:38.992384 flwr-1.4.0/src/py/flwr/py.typed
+-rw-r--r--   0        0        0     1370 2023-04-19 19:48:18.752412 flwr-1.4.0/src/py/flwr/server/__init__.py
+-rw-r--r--   0        0        0    22380 2023-04-20 21:33:15.721524 flwr-1.4.0/src/py/flwr/server/app.py
+-rw-r--r--   0        0        0     5941 2023-04-09 17:40:02.231925 flwr-1.4.0/src/py/flwr/server/client_manager.py
+-rw-r--r--   0        0        0     2228 2023-01-28 04:18:48.882779 flwr-1.4.0/src/py/flwr/server/client_proxy.py
+-rw-r--r--   0        0        0     1058 2021-12-13 18:43:21.067866 flwr-1.4.0/src/py/flwr/server/criterion.py
+-rw-r--r--   0        0        0      705 2022-10-31 15:06:38.994058 flwr-1.4.0/src/py/flwr/server/driver/__init__.py
+-rw-r--r--   0        0        0     3919 2023-03-01 10:00:15.303758 flwr-1.4.0/src/py/flwr/server/driver/driver_servicer.py
+-rw-r--r--   0        0        0      704 2022-10-31 15:06:38.994845 flwr-1.4.0/src/py/flwr/server/fleet/__init__.py
+-rw-r--r--   0        0        0     1638 2023-02-06 03:53:52.202051 flwr-1.4.0/src/py/flwr/server/fleet/fleet_servicer.py
+-rw-r--r--   0        0        0      728 2022-10-31 15:06:38.995604 flwr-1.4.0/src/py/flwr/server/grpc_server/__init__.py
+-rw-r--r--   0        0        0     4467 2023-04-20 21:33:15.721689 flwr-1.4.0/src/py/flwr/server/grpc_server/driver_client_manager.py
+-rw-r--r--   0        0        0     5594 2023-01-28 04:18:48.884893 flwr-1.4.0/src/py/flwr/server/grpc_server/flower_service_servicer.py
+-rw-r--r--   0        0        0     6416 2023-01-28 04:18:48.885665 flwr-1.4.0/src/py/flwr/server/grpc_server/grpc_bridge.py
+-rw-r--r--   0        0        0     4623 2023-01-28 04:18:48.886497 flwr-1.4.0/src/py/flwr/server/grpc_server/grpc_client_proxy.py
+-rw-r--r--   0        0        0    11509 2022-10-31 15:06:38.996931 flwr-1.4.0/src/py/flwr/server/grpc_server/grpc_server.py
+-rw-r--r--   0        0        0     6314 2023-02-26 21:43:11.340590 flwr-1.4.0/src/py/flwr/server/grpc_server/ins_scheduler.py
+-rw-r--r--   0        0        0     4457 2023-04-19 19:48:18.753127 flwr-1.4.0/src/py/flwr/server/history.py
+-rw-r--r--   0        0        0      728 2023-02-26 21:43:11.340677 flwr-1.4.0/src/py/flwr/server/rest_server/__init__.py
+-rw-r--r--   0        0        0     4564 2023-04-19 19:51:43.063986 flwr-1.4.0/src/py/flwr/server/rest_server/rest_api.py
+-rw-r--r--   0        0        0    15855 2023-04-09 17:40:02.232464 flwr-1.4.0/src/py/flwr/server/server.py
+-rw-r--r--   0        0        0      996 2023-04-19 19:48:18.753433 flwr-1.4.0/src/py/flwr/server/state/__init__.py
+-rw-r--r--   0        0        0     6521 2023-04-09 17:40:02.232848 flwr-1.4.0/src/py/flwr/server/state/in_memory_state.py
+-rw-r--r--   0        0        0    19296 2023-02-24 01:24:59.843933 flwr-1.4.0/src/py/flwr/server/state/sqlite_state.py
+-rw-r--r--   0        0        0     4805 2023-04-09 17:40:02.233178 flwr-1.4.0/src/py/flwr/server/state/state.py
+-rw-r--r--   0        0        0     1648 2023-04-09 17:40:02.233334 flwr-1.4.0/src/py/flwr/server/state/state_factory.py
+-rw-r--r--   0        0        0     1588 2023-03-19 07:16:33.599546 flwr-1.4.0/src/py/flwr/server/strategy/__init__.py
+-rw-r--r--   0        0        0     4994 2023-01-28 04:18:48.886988 flwr-1.4.0/src/py/flwr/server/strategy/aggregate.py
+-rw-r--r--   0        0        0     4519 2022-10-31 15:06:38.998480 flwr-1.4.0/src/py/flwr/server/strategy/dpfedavg_adaptive.py
+-rw-r--r--   0        0        0     4875 2023-04-19 19:48:18.753564 flwr-1.4.0/src/py/flwr/server/strategy/dpfedavg_fixed.py
+-rw-r--r--   0        0        0     5978 2022-10-31 15:06:38.999096 flwr-1.4.0/src/py/flwr/server/strategy/fault_tolerant_fedavg.py
+-rw-r--r--   0        0        0     6730 2023-03-19 07:16:33.599708 flwr-1.4.0/src/py/flwr/server/strategy/fedadagrad.py
+-rw-r--r--   0        0        0     7012 2023-03-19 07:16:33.599816 flwr-1.4.0/src/py/flwr/server/strategy/fedadam.py
+-rw-r--r--   0        0        0    11495 2023-02-12 07:14:44.611220 flwr-1.4.0/src/py/flwr/server/strategy/fedavg.py
+-rw-r--r--   0        0        0     9985 2022-10-31 15:06:39.001040 flwr-1.4.0/src/py/flwr/server/strategy/fedavg_android.py
+-rw-r--r--   0        0        0     8953 2023-02-12 07:14:44.611321 flwr-1.4.0/src/py/flwr/server/strategy/fedavgm.py
+-rw-r--r--   0        0        0     6469 2023-02-12 07:14:44.611413 flwr-1.4.0/src/py/flwr/server/strategy/fedmedian.py
+-rw-r--r--   0        0        0     5393 2023-03-19 07:16:33.599932 flwr-1.4.0/src/py/flwr/server/strategy/fedopt.py
+-rw-r--r--   0        0        0     7708 2023-02-12 07:14:44.611516 flwr-1.4.0/src/py/flwr/server/strategy/fedprox.py
+-rw-r--r--   0        0        0     7772 2023-04-05 05:35:07.206662 flwr-1.4.0/src/py/flwr/server/strategy/fedxgb_nn_avg.py
+-rw-r--r--   0        0        0     7044 2023-03-19 07:16:33.600255 flwr-1.4.0/src/py/flwr/server/strategy/fedyogi.py
+-rw-r--r--   0        0        0     7011 2023-02-12 07:14:44.611649 flwr-1.4.0/src/py/flwr/server/strategy/krum.py
+-rw-r--r--   0        0        0    10744 2022-10-31 15:06:39.002341 flwr-1.4.0/src/py/flwr/server/strategy/qfedavg.py
+-rw-r--r--   0        0        0     7484 2022-10-31 15:06:39.002465 flwr-1.4.0/src/py/flwr/server/strategy/strategy.py
+-rw-r--r--   0        0        0      901 2023-02-26 21:43:11.342381 flwr-1.4.0/src/py/flwr/server/utils/__init__.py
+-rw-r--r--   0        0        0     5114 2023-04-19 19:48:18.754078 flwr-1.4.0/src/py/flwr/server/utils/tensorboard.py
+-rw-r--r--   0        0        0     4941 2023-04-19 19:48:18.754177 flwr-1.4.0/src/py/flwr/server/utils/validator.py
+-rw-r--r--   0        0        0     1271 2023-04-19 19:48:18.754537 flwr-1.4.0/src/py/flwr/simulation/__init__.py
+-rw-r--r--   0        0        0     7773 2023-04-05 05:35:07.206767 flwr-1.4.0/src/py/flwr/simulation/app.py
+-rw-r--r--   0        0        0      727 2021-12-13 18:43:21.071065 flwr-1.4.0/src/py/flwr/simulation/ray_transport/__init__.py
+-rw-r--r--   0        0        0     5472 2023-04-05 05:35:07.206865 flwr-1.4.0/src/py/flwr/simulation/ray_transport/ray_client_proxy.py
+-rw-r--r--   0        0        0    12296 1970-01-01 00:00:00.000000 flwr-1.4.0/setup.py
+-rw-r--r--   0        0        0    12752 1970-01-01 00:00:00.000000 flwr-1.4.0/PKG-INFO
```

### Comparing `flwr-1.3.0/LICENSE` & `flwr-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flwr-1.3.0/README.md` & `flwr-1.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,18 @@
 
 Meet the Flower community on [flower.dev](https://flower.dev)!
 
 ## Federated Learning Tutorial
 
 Flower's goal is to make federated learning accessible to everyone. This series of tutorials introduces the fundamentals of federated learning and how to implement them in Flower.
 
+0. **What is Federated Learning?**
+
+   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-0-What-is-FL.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-0-What-is-FL.ipynb))
+
 1. **An Introduction to Federated Learning**
 
    [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-1-Intro-to-FL-PyTorch.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-1-Intro-to-FL-PyTorch.ipynb))
 
 2. **Using Strategies in Federated Learning**
 
    [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-2-Strategies-in-FL-PyTorch.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-2-Strategies-in-FL-PyTorch.ipynb))
@@ -80,19 +84,21 @@
 * [Quickstart (scikit-learn)](https://github.com/adap/flower/tree/main/examples/sklearn-logreg-mnist)
 * [Quickstart (TFLite on Android [code example])](https://github.com/adap/flower/tree/main/examples/android)
 
 ## Flower Baselines
 
 Flower Baselines is a collection of community-contributed experiments that reproduce the experiments performed in popular federated learning publications. Researchers can build on Flower Baselines to quickly evaluate new ideas:
 
-* [FedAvg](https://arxiv.org/pdf/1602.05629.pdf):
+* [FedAvg](https://arxiv.org/abs/1602.05629):
   * [MNIST](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/fedavg_mnist)
-* [FedBN: Federated Learning on non-IID Features via Local Batch Normalization](https://arxiv.org/pdf/2102.07623.pdf):
+* [FedProx](https://arxiv.org/abs/1812.06127):
+  * [MNIST](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/fedprox_mnist)
+* [FedBN: Federated Learning on non-IID Features via Local Batch Normalization](https://arxiv.org/abs/2102.07623):
   * [Convergence Rate](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/fedbn/convergence_rate)
-* [Adaptive Federated Optimization](https://arxiv.org/pdf/2003.00295.pdf):
+* [Adaptive Federated Optimization](https://arxiv.org/abs/2003.00295):
   * [CIFAR-10/100](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/adaptive_federated_optimization)
 
 Check the Flower documentation to learn more: [Using Baselines](https://flower.dev/docs/using-baselines.html)
 
 The Flower community loves contributions! Make your work more visible and enable others to build on it by contributing it as a baseline: [Contributing Baselines](https://flower.dev/docs/contributing-baselines.html)
 
 ## Flower Usage Examples
@@ -133,15 +139,15 @@
 ## Citation
 
 If you publish work that uses Flower, please cite Flower as follows: 
 
 ```bibtex
 @article{beutel2020flower,
   title={Flower: A Friendly Federated Learning Research Framework},
-  author={Beutel, Daniel J and Topal, Taner and Mathur, Akhil and Qiu, Xinchi and Parcollet, Titouan and Lane, Nicholas D},
+  author={Beutel, Daniel J and Topal, Taner and Mathur, Akhil and Qiu, Xinchi and Fernandez-Marques, Javier and Gao, Yan and Sani, Lorenzo and Kwing, Hei Li and Parcollet, Titouan and Gusmão, Pedro PB de and Lane, Nicholas D}, 
   journal={arXiv preprint arXiv:2007.14390},
   year={2020}
 }
 ```
 
 Please also consider adding your publication to the list of Flower-based publications in the docs, just open a Pull Request.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -25,22 +25,27 @@
 www.fast.ai/), [Pandas](https://pandas.pydata.org/ ) for federated analytics,
 or even raw [NumPy](https://numpy.org/) for users who enjoy computing gradients
 by hand. * **Understandable**: Flower is written with maintainability in mind.
 The community is encouraged to both read and contribute to the codebase. Meet
 the Flower community on [flower.dev](https://flower.dev)! ## Federated Learning
 Tutorial Flower's goal is to make federated learning accessible to everyone.
 This series of tutorials introduces the fundamentals of federated learning and
-how to implement them in Flower. 1. **An Introduction to Federated Learning**
-[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)]
-(https://colab.research.google.com/github/adap/flower/blob/main/doc/source/
-tutorial/Flower-1-Intro-to-FL-PyTorch.ipynb) (or open the [Jupyter Notebook]
-(https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-1-Intro-
-to-FL-PyTorch.ipynb)) 2. **Using Strategies in Federated Learning** [![Open in
+how to implement them in Flower. 0. **What is Federated Learning?** [![Open in
 Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/
+Flower-0-What-is-FL.ipynb) (or open the [Jupyter Notebook](https://github.com/
+adap/flower/blob/main/doc/source/tutorial/Flower-0-What-is-FL.ipynb)) 1. **An
+Introduction to Federated Learning** [![Open in Colab](https://
+colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/
+Flower-1-Intro-to-FL-PyTorch.ipynb) (or open the [Jupyter Notebook](https://
+github.com/adap/flower/blob/main/doc/source/tutorial/Flower-1-Intro-to-FL-
+PyTorch.ipynb)) 2. **Using Strategies in Federated Learning** [![Open in Colab]
+(https://colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/
 Flower-2-Strategies-in-FL-PyTorch.ipynb) (or open the [Jupyter Notebook](https:
 //github.com/adap/flower/blob/main/doc/source/tutorial/Flower-2-Strategies-in-
 FL-PyTorch.ipynb)) 3. **Building Strategies for Federated Learning** [![Open in
 Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/
 Flower-3-Building-a-Strategy-PyTorch.ipynb) (or open the [Jupyter Notebook]
 (https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-3-
@@ -64,47 +69,49 @@
 [Quickstart (JAX)](https://github.com/adap/flower/tree/main/examples/
 quickstart_jax) * [Quickstart (scikit-learn)](https://github.com/adap/flower/
 tree/main/examples/sklearn-logreg-mnist) * [Quickstart (TFLite on Android [code
 example])](https://github.com/adap/flower/tree/main/examples/android) ## Flower
 Baselines Flower Baselines is a collection of community-contributed experiments
 that reproduce the experiments performed in popular federated learning
 publications. Researchers can build on Flower Baselines to quickly evaluate new
-ideas: * [FedAvg](https://arxiv.org/pdf/1602.05629.pdf): * [MNIST](https://
+ideas: * [FedAvg](https://arxiv.org/abs/1602.05629): * [MNIST](https://
 github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/
-fedavg_mnist) * [FedBN: Federated Learning on non-IID Features via Local Batch
-Normalization](https://arxiv.org/pdf/2102.07623.pdf): * [Convergence Rate]
-(https://github.com/adap/flower/tree/main/baselines/flwr_baselines/
-publications/fedbn/convergence_rate) * [Adaptive Federated Optimization](https:
-//arxiv.org/pdf/2003.00295.pdf): * [CIFAR-10/100](https://github.com/adap/
-flower/tree/main/baselines/flwr_baselines/publications/
-adaptive_federated_optimization) Check the Flower documentation to learn more:
-[Using Baselines](https://flower.dev/docs/using-baselines.html) The Flower
-community loves contributions! Make your work more visible and enable others to
-build on it by contributing it as a baseline: [Contributing Baselines](https://
-flower.dev/docs/contributing-baselines.html) ## Flower Usage Examples Several
-code examples show different usage scenarios of Flower (in combination with
-popular machine learning frameworks such as PyTorch or TensorFlow). Quickstart
-examples: * [Quickstart (TensorFlow)](https://github.com/adap/flower/tree/main/
-examples/quickstart_tensorflow) * [Quickstart (PyTorch)](https://github.com/
-adap/flower/tree/main/examples/quickstart_pytorch) * [Quickstart (Hugging
-Face)](https://github.com/adap/flower/tree/main/examples/
-quickstart_huggingface) * [Quickstart (PyTorch Lightning)](https://github.com/
-adap/flower/tree/main/examples/quickstart_pytorch_lightning) * [Quickstart
-(fastai)](https://github.com/adap/flower/tree/main/examples/quickstart_fastai)
-* [Quickstart (Pandas)](https://github.com/adap/flower/tree/main/examples/
-quickstart_pandas) * [Quickstart (MXNet)](https://github.com/adap/flower/tree/
-main/examples/quickstart_mxnet) * [Quickstart (JAX)](https://github.com/adap/
-flower/tree/main/examples/quickstart_jax) * [Quickstart (scikit-learn)](https:/
-/github.com/adap/flower/tree/main/examples/sklearn-logreg-mnist) * [Quickstart
-(TFLite on Android)](https://github.com/adap/flower/tree/main/examples/android)
-Other [examples](https://github.com/adap/flower/tree/main/examples): *
-[Raspberry Pi & Nvidia Jetson Tutorial](https://github.com/adap/flower/tree/
-main/examples/embedded_devices) * [Android & TFLite](https://github.com/adap/
-flower/tree/main/examples/android) * [PyTorch: From Centralized to Federated]
-(https://github.com/adap/flower/tree/main/examples/
+fedavg_mnist) * [FedProx](https://arxiv.org/abs/1812.06127): * [MNIST](https://
+github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/
+fedprox_mnist) * [FedBN: Federated Learning on non-IID Features via Local Batch
+Normalization](https://arxiv.org/abs/2102.07623): * [Convergence Rate](https://
+github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/fedbn/
+convergence_rate) * [Adaptive Federated Optimization](https://arxiv.org/abs/
+2003.00295): * [CIFAR-10/100](https://github.com/adap/flower/tree/main/
+baselines/flwr_baselines/publications/adaptive_federated_optimization) Check
+the Flower documentation to learn more: [Using Baselines](https://flower.dev/
+docs/using-baselines.html) The Flower community loves contributions! Make your
+work more visible and enable others to build on it by contributing it as a
+baseline: [Contributing Baselines](https://flower.dev/docs/contributing-
+baselines.html) ## Flower Usage Examples Several code examples show different
+usage scenarios of Flower (in combination with popular machine learning
+frameworks such as PyTorch or TensorFlow). Quickstart examples: * [Quickstart
+(TensorFlow)](https://github.com/adap/flower/tree/main/examples/
+quickstart_tensorflow) * [Quickstart (PyTorch)](https://github.com/adap/flower/
+tree/main/examples/quickstart_pytorch) * [Quickstart (Hugging Face)](https://
+github.com/adap/flower/tree/main/examples/quickstart_huggingface) * [Quickstart
+(PyTorch Lightning)](https://github.com/adap/flower/tree/main/examples/
+quickstart_pytorch_lightning) * [Quickstart (fastai)](https://github.com/adap/
+flower/tree/main/examples/quickstart_fastai) * [Quickstart (Pandas)](https://
+github.com/adap/flower/tree/main/examples/quickstart_pandas) * [Quickstart
+(MXNet)](https://github.com/adap/flower/tree/main/examples/quickstart_mxnet) *
+[Quickstart (JAX)](https://github.com/adap/flower/tree/main/examples/
+quickstart_jax) * [Quickstart (scikit-learn)](https://github.com/adap/flower/
+tree/main/examples/sklearn-logreg-mnist) * [Quickstart (TFLite on Android)]
+(https://github.com/adap/flower/tree/main/examples/android) Other [examples]
+(https://github.com/adap/flower/tree/main/examples): * [Raspberry Pi & Nvidia
+Jetson Tutorial](https://github.com/adap/flower/tree/main/examples/
+embedded_devices) * [Android & TFLite](https://github.com/adap/flower/tree/
+main/examples/android) * [PyTorch: From Centralized to Federated](https://
+github.com/adap/flower/tree/main/examples/
 pytorch_from_centralized_to_federated) * [MXNet: From Centralized to Federated]
 (https://github.com/adap/flower/tree/main/examples/
 mxnet_from_centralized_to_federated) * [Advanced Flower with TensorFlow/Keras]
 (https://github.com/adap/flower/tree/main/examples/advanced_tensorflow) *
 [Advanced Flower with PyTorch](https://github.com/adap/flower/tree/main/
 examples/advanced_pytorch) * Single-Machine Simulation of Federated Learning
 Systems ([PyTorch](https://github.com/adap/flower/tree/main/examples/
@@ -112,12 +119,14 @@
 examples/simulation_tensorflow)) ## Community Flower is built by a wonderful
 community of researchers and engineers. [Join Slack](https://flower.dev/join-
 slack) to meet them, [contributions](#contributing-to-flower) are welcome.
 [https://contrib.rocks/image?repo=adap/flower] ## Citation If you publish work
 that uses Flower, please cite Flower as follows: ```bibtex @article
 {beutel2020flower, title={Flower: A Friendly Federated Learning Research
 Framework}, author={Beutel, Daniel J and Topal, Taner and Mathur, Akhil and
-Qiu, Xinchi and Parcollet, Titouan and Lane, Nicholas D}, journal={arXiv
-preprint arXiv:2007.14390}, year={2020} } ``` Please also consider adding your
-publication to the list of Flower-based publications in the docs, just open a
-Pull Request. ## Contributing to Flower We welcome contributions. Please see
-[CONTRIBUTING.md](CONTRIBUTING.md) to get started!
+Qiu, Xinchi and Fernandez-Marques, Javier and Gao, Yan and Sani, Lorenzo and
+Kwing, Hei Li and Parcollet, Titouan and GusmÃ£o, Pedro PB de and Lane,
+Nicholas D}, journal={arXiv preprint arXiv:2007.14390}, year={2020} } ```
+Please also consider adding your publication to the list of Flower-based
+publications in the docs, just open a Pull Request. ## Contributing to Flower
+We welcome contributions. Please see [CONTRIBUTING.md](CONTRIBUTING.md) to get
+started!
```

### Comparing `flwr-1.3.0/pyproject.toml` & `flwr-1.4.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.4.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "flwr"
-version = "1.3.0"
+version = "1.4.0"
 description = "Flower: A Friendly Federated Learning Framework"
 license = "Apache-2.0"
 authors = ["The Flower Authors <hello@flower.dev>"]
 readme = "README.md"
 homepage = "https://flower.dev"
 repository = "https://github.com/adap/flower"
 documentation = "https://flower.dev"
@@ -40,64 +40,69 @@
     { include = "flwr", from = "src/py" },
 ]
 exclude = [
     "src/py/**/*_test.py",
 ]
 
 [tool.poetry.scripts]
+flower-driver-api = "flwr.server:run_driver_api"
+flower-fleet-api = "flwr.server:run_fleet_api"
 flower-server = "flwr.server:run_server"
 flower-client = "flwr.client:run_client"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 # Mandatory dependencies
 numpy = "^1.21.0"
-grpcio = "^1.43.0,!=1.52.0"
+grpcio = "^1.48.2,!=1.52.0"
 protobuf = "^3.19.0"
 importlib-metadata = { version = "^4.0.0", markers = "python_version < '3.8'" }
 iterators = "^0.0.2"
 # Optional dependencies (VCE)
-ray = { extras = ["default"], version = "~2.2.0", optional = true }
+ray = { version = "^2.3.0", extras = ["default"], optional = true }
 # Optional dependencies (REST transport layer)
-requests = "^2.28.1"
-fastapi = "^0.89.1"
-uvicorn = {extras = ["standard"], version = "^0.20.0"}
+requests = { version = "^2.28.2", optional = true }
+fastapi = { version = "^0.95.0", optional = true }
+starlette = { version = "^0.26.1", optional = true }
+uvicorn = { version = "^0.21.1", extras = ["standard"], optional = true }
 
 [tool.poetry.extras]
 simulation = ["ray"]
-rest = ["fastapi", "requests", "uvicorn"]
+rest = ["fastapi", "requests", "starlette", "uvicorn"]
 
-[tool.poetry.dev-dependencies]
-types-dataclasses = "==0.6.5"
+[tool.poetry.group.dev.dependencies]
+types-dataclasses = "==0.6.6"
 types-protobuf = "==3.19.18"
-types-requests = "==2.28.11.7"
+types-requests = "==2.28.11.17"
 types-setuptools = "==57.4.14"
 clang-format = "==15.0.6"
-isort = "==5.10.1"
-black = "==22.8.0"
-docformatter = "==1.5.0"
+isort = "==5.11.5"
+black = "==23.1.0"
+docformatter = "==1.5.1"
 mypy = "==0.961"
 pylint = "==2.13.8"
 flake8 = "==3.9.2"
 pytest = "==7.1.2"
 pytest-cov = "==3.0.0"
 pytest-watch = "==4.2.0"
-grpcio-tools = "==1.43.0"
+grpcio-tools = "==1.48.2"
 mypy-protobuf = "==3.2.0"
-jupyterlab = "==3.3.2"
+jupyterlab = "==3.5.3"
 rope = "==0.19.0"
 semver = "==2.13.0"
-sphinx = "==5.1.1"
-myst-parser = "==0.18.0"
+sphinx = "==5.3.0"
+myst-parser = "==0.18.1"
 sphinx-design = "==0.3.0"
-sphinx-copybutton = "==0.5.0"
+sphinx-copybutton = "==0.5.1"
 sphinxcontrib-mermaid = "==0.7.1"
-furo = "==2022.6.21"
+furo = "==2022.12.7"
 sphinx-reredirects = "==0.1.1"
-nbsphinx = "==0.8.9"
+nbsphinx = "==0.8.12"
+nbstripout = "==0.6.1"
+sphinx-argparse = "==0.4.0"
 
 [tool.isort]
 line_length = 88
 indent = "    "
 multi_line_output = 3
 include_trailing_comma = true
 force_grid_wrap = 0
```

### Comparing `flwr-1.3.0/src/py/flwr/__init__.py` & `flwr-1.4.0/src/py/flwr/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,18 +10,20 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Flower main package."""
 
+
 from flwr.common.version import package_version as _package_version
 
-from . import client, server, simulation
+from . import client, common, server, simulation
 
 __all__ = [
     "client",
+    "common",
     "server",
     "simulation",
 ]
 
 __version__ = _package_version
```

### Comparing `flwr-1.3.0/src/py/flwr/client/__init__.py` & `flwr-1.4.0/src/py/flwr/client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr-1.3.0/src/py/flwr/client/app.py` & `flwr-1.4.0/src/py/flwr/client/app.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,25 +11,28 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Flower client app."""
 
 
+import sys
 import time
 from logging import INFO
 from typing import Callable, Dict, Optional, Union
 
 from flwr.common import (
     GRPC_MAX_MESSAGE_LENGTH,
     EventType,
     event,
     ndarrays_to_parameters,
     parameters_to_ndarrays,
 )
+from flwr.common.address import parse_address
+from flwr.common.constant import MISSING_EXTRA_REST
 from flwr.common.logger import log
 from flwr.common.typing import (
     Code,
     EvaluateIns,
     EvaluateRes,
     FitIns,
     FitRes,
@@ -76,77 +79,106 @@
 
 """
 
 
 ClientLike = Union[Client, NumPyClient]
 
 
+# pylint: disable=import-outside-toplevel,too-many-locals
 def start_client(
     *,
     server_address: str,
     client: Client,
     grpc_max_message_length: int = GRPC_MAX_MESSAGE_LENGTH,
-    root_certificates: Optional[bytes] = None,
+    root_certificates: Optional[Union[bytes, str]] = None,
+    rest: bool = False,
 ) -> None:
-    """Start a Flower Client which connects to a gRPC server.
+    """Start a Flower client node which connects to a Flower server.
 
     Parameters
     ----------
-        server_address: str. The IPv6 address of the server. If the Flower
-            server runs on the same machine on port 8080, then `server_address`
-            would be `"[::]:8080"`.
-        client: flwr.client.Client. An implementation of the abstract base
-            class `flwr.client.Client`.
-        grpc_max_message_length: int (default: 536_870_912, this equals 512MB).
-            The maximum length of gRPC messages that can be exchanged with the
-            Flower server. The default should be sufficient for most models.
-            Users who train very large models might need to increase this
-            value. Note that the Flower server needs to be started with the
-            same value (see `flwr.server.start_server`), otherwise it will not
-            know about the increased limit and block larger messages.
-        root_certificates: bytes (default: None)
-            The PEM-encoded root certificates as a byte string. If provided, a secure
-            connection using the certificates will be established to a
-            SSL-enabled Flower server.
-
-    Returns
-    -------
-        None
+    server_address : str
+        The IPv4 or IPv6 address of the server. If the Flower
+        server runs on the same machine on port 8080, then `server_address`
+        would be `"[::]:8080"`.
+    client : flwr.client.Client
+        An implementation of the abstract base
+        class `flwr.client.Client`.
+    grpc_max_message_length : int (default: 536_870_912, this equals 512MB)
+        The maximum length of gRPC messages that can be exchanged with the
+        Flower server. The default should be sufficient for most models.
+        Users who train very large models might need to increase this
+        value. Note that the Flower server needs to be started with the
+        same value (see `flwr.server.start_server`), otherwise it will not
+        know about the increased limit and block larger messages.
+    root_certificates : Optional[Union[bytes, str]] (default: None)
+        The PEM-encoded root certificates as a byte string or a path string.
+        If provided, a secure connection using the certificates will be
+        established to an SSL-enabled Flower server.
+    rest : bool (default: False)
+        Defines whether or not the client is interacting with the server using the
+        experimental REST API. This feature is experimental, it might change
+        considerably in future versions of Flower.
 
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
     """
+
     event(EventType.START_CLIENT_ENTER)
 
+    # Parse IP address
+    parsed_address = parse_address(server_address)
+    if not parsed_address:
+        sys.exit(f"Server address ({server_address}) cannot be parsed.")
+    host, port, is_v6 = parsed_address
+    address = f"[{host}]:{port}" if is_v6 else f"{host}:{port}"
+
+    # Use either gRPC bidirectional streaming or REST request/response
+    if rest:
+        try:
+            from .rest_client.connection import http_request_response
+        except ModuleNotFoundError:
+            sys.exit(MISSING_EXTRA_REST)
+        if server_address[:4] != "http":
+            sys.exit(
+                "When using the REST API, please provide `https://` or "
+                "`http://` before the server address (e.g. `http://127.0.0.1:8080`)"
+            )
+        connection = http_request_response
+    else:
+        connection = grpc_connection
     while True:
         sleep_duration: int = 0
-        with grpc_connection(
-            server_address,
+        with connection(
+            address,
             max_message_length=grpc_max_message_length,
             root_certificates=root_certificates,
         ) as conn:
             receive, send = conn
 
             while True:
                 server_message = receive()
+                if server_message is None:
+                    time.sleep(3)  # Wait for 3s before asking again
+                    continue
                 client_message, sleep_duration, keep_going = handle(
                     client, server_message
                 )
                 send(client_message)
                 if not keep_going:
                     break
         if sleep_duration == 0:
@@ -165,35 +197,41 @@
 
 def start_numpy_client(
     *,
     server_address: str,
     client: NumPyClient,
     grpc_max_message_length: int = GRPC_MAX_MESSAGE_LENGTH,
     root_certificates: Optional[bytes] = None,
+    rest: bool = False,
 ) -> None:
     """Start a Flower NumPyClient which connects to a gRPC server.
 
     Parameters
     ----------
     server_address : str
-        The IPv6 address of the server. If the Flower server runs on the same
-        machine on port 8080, then `server_address` would be `"[::]:8080"`.
+        The IPv4 or IPv6 address of the server. If the Flower server runs on
+        the same machine on port 8080, then `server_address` would be
+        `"[::]:8080"`.
     client : flwr.client.NumPyClient
         An implementation of the abstract base class `flwr.client.NumPyClient`.
     grpc_max_message_length : int (default: 536_870_912, this equals 512MB)
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
+    rest : bool (default: False)
+        Defines whether or not the client is interacting with the server using the
+        experimental REST API. This feature is experimental, it might be change
+        considerably in future versions of Flower.
 
     Examples
     --------
     Starting a client with an insecure server connection:
 
     >>> start_client(
     >>>     server_address=localhost:8080,
@@ -212,14 +250,15 @@
 
     # Start
     start_client(
         server_address=server_address,
         client=_wrap_numpy_client(client=client),
         grpc_max_message_length=grpc_max_message_length,
         root_certificates=root_certificates,
+        rest=rest,
     )
 
 
 def to_client(client_like: ClientLike) -> Client:
     """Take any Client-like object and return it as a Client."""
     if isinstance(client_like, NumPyClient):
         return _wrap_numpy_client(client=client_like)
```

### Comparing `flwr-1.3.0/src/py/flwr/client/client.py` & `flwr-1.4.0/src/py/flwr/client/client.py`

 * *Files identical despite different names*

### Comparing `flwr-1.3.0/src/py/flwr/client/dpfedavg_numpy_client.py` & `flwr-1.4.0/src/py/flwr/client/dpfedavg_numpy_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 
     def get_parameters(self, config: Dict[str, Scalar]) -> NDArrays:
         return self.client.get_parameters(config)
 
     def fit(
         self, parameters: NDArrays, config: Dict[str, Scalar]
     ) -> Tuple[NDArrays, int, Dict[str, Scalar]]:
-
         original_params = copy.deepcopy(parameters)
         # Getting the updated model from the wrapped client
         updated_params, num_examples, metrics = self.client.fit(parameters, config)
 
         # Update = updated model - original model
         update = [np.subtract(x, y) for (x, y) in zip(updated_params, original_params)]
```

### Comparing `flwr-1.3.0/src/py/flwr/client/grpc_client/__init__.py` & `flwr-1.4.0/src/py/flwr/client/grpc_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr-1.3.0/src/py/flwr/client/grpc_client/connection.py` & `flwr-1.4.0/src/py/flwr/client/grpc_client/connection.py`

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

### Comparing `flwr-1.3.0/src/py/flwr/client/message_handler/__init__.py` & `flwr-1.4.0/src/py/flwr/client/message_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr-1.3.0/src/py/flwr/client/message_handler/message_handler.py` & `flwr-1.4.0/src/py/flwr/client/message_handler/message_handler.py`

 * *Files identical despite different names*

### Comparing `flwr-1.3.0/src/py/flwr/client/numpy_client.py` & `flwr-1.4.0/src/py/flwr/client/numpy_client.py`

 * *Files identical despite different names*

### Comparing `flwr-1.3.0/src/py/flwr/common/__init__.py` & `flwr-1.4.0/src/py/flwr/common/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,18 +8,21 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Flower utilities shared between server and client."""
+"""Common components shared between server and client."""
 
 
+from .date import now as now
 from .grpc import GRPC_MAX_MESSAGE_LENGTH
+from .logger import configure as configure
+from .logger import log as log
 from .parameter import bytes_to_ndarray as bytes_to_ndarray
 from .parameter import ndarray_to_bytes as ndarray_to_bytes
 from .parameter import ndarrays_to_parameters as ndarrays_to_parameters
 from .parameter import parameters_to_ndarrays as parameters_to_ndarrays
 from .telemetry import EventType as EventType
 from .telemetry import event as event
 from .typing import ClientMessage as ClientMessage
@@ -46,29 +49,32 @@
 from .typing import Status as Status
 
 __all__ = [
     "bytes_to_ndarray",
     "ClientMessage",
     "Code",
     "Config",
+    "configure",
     "DisconnectRes",
     "EvaluateIns",
     "EvaluateRes",
     "event",
     "EventType",
     "FitIns",
     "FitRes",
     "GetParametersIns",
     "GetParametersRes",
     "GetPropertiesIns",
     "GetPropertiesRes",
     "GRPC_MAX_MESSAGE_LENGTH",
+    "log",
     "Metrics",
     "MetricsAggregationFn",
     "ndarray_to_bytes",
+    "now",
     "NDArray",
     "NDArrays",
     "ndarrays_to_parameters",
     "Parameters",
     "parameters_to_ndarrays",
     "Properties",
     "ReconnectIns",
```

### Comparing `flwr-1.3.0/src/py/flwr/common/dp.py` & `flwr-1.4.0/src/py/flwr/common/dp.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Building block functions for DP algorithms."""
 
+
 from typing import Tuple
 
 import numpy as np
 
 from flwr.common.typing import NDArrays
```

### Comparing `flwr-1.3.0/src/py/flwr/common/grpc.py` & `flwr-1.4.0/src/py/flwr/common/grpc.py`

 * *Files identical despite different names*

### Comparing `flwr-1.3.0/src/py/flwr/common/logger.py` & `flwr-1.4.0/src/py/flwr/common/logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Flower Logger."""
+
+
 import logging
 from logging import LogRecord
 from logging.handlers import HTTPHandler
 from typing import Any, Dict, Optional, Tuple
 
 # Create logger
 LOGGER_NAME = "flwr"
```

### Comparing `flwr-1.3.0/src/py/flwr/common/parameter.py` & `flwr-1.4.0/src/py/flwr/common/parameter.py`

 * *Files identical despite different names*

### Comparing `flwr-1.3.0/src/py/flwr/common/serde.py` & `flwr-1.4.0/src/py/flwr/common/serde.py`

 * *Files identical despite different names*

### Comparing `flwr-1.3.0/src/py/flwr/common/telemetry.py` & `flwr-1.4.0/src/py/flwr/common/telemetry.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Flower telemetry."""
 
+
 import datetime
 import json
 import logging
 import os
 import platform
 import urllib.request
 import uuid
@@ -123,15 +124,23 @@
     START_CLIENT_ENTER = auto()
     START_CLIENT_LEAVE = auto()
 
     # Server
     START_SERVER_ENTER = auto()
     START_SERVER_LEAVE = auto()
 
-    # New Server
+    # Driver API
+    RUN_DRIVER_API_ENTER = auto()
+    RUN_DRIVER_API_LEAVE = auto()
+
+    # Fleet API
+    RUN_FLEET_API_ENTER = auto()
+    RUN_FLEET_API_LEAVE = auto()
+
+    # Driver API and Fleet API
     RUN_SERVER_ENTER = auto()
     RUN_SERVER_LEAVE = auto()
 
     # Simulation
     START_SIMULATION_ENTER = auto()
     START_SIMULATION_LEAVE = auto()
 
@@ -146,14 +155,15 @@
     # Will be assigned ThreadPoolExecutor(max_workers=1)
     # in event() the first time it's required
     "executor": None,
     "source": None,
     "cluster": None,
 }
 
+
 # In Python 3.7 pylint will throw an error stating that
 # "Value 'Future' is unsubscriptable".
 # This pylint disable line can be remove when dropping support
 # for Python 3.7
 # pylint: disable-next=unsubscriptable-object
 def event(
     event_type: EventType,
```

### Comparing `flwr-1.3.0/src/py/flwr/common/typing.py` & `flwr-1.4.0/src/py/flwr/common/typing.py`

 * *Files identical despite different names*

### Comparing `flwr-1.3.0/src/py/flwr/common/version.py` & `flwr-1.4.0/src/py/flwr/common/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 """Flower package version helper."""
+
+
 import sys
 from typing import Tuple
 
 # pylint: disable=import-error, no-name-in-module
 if sys.version_info < (3, 8):
     import importlib_metadata
 else:
```

### Comparing `flwr-1.3.0/src/py/flwr/driver/__init__.py` & `flwr-1.4.0/src/py/flwr/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr-1.3.0/src/py/flwr/driver/driver.py` & `flwr-1.4.0/src/py/flwr/driver/driver.py`

 * *Files identical despite different names*

### Comparing `flwr-1.3.0/src/py/flwr/proto/__init__.py` & `flwr-1.4.0/src/py/flwr/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr-1.3.0/src/py/flwr/proto/driver_pb2.pyi` & `flwr-1.4.0/src/py/flwr/proto/driver_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr-1.3.0/src/py/flwr/proto/driver_pb2_grpc.py` & `flwr-1.4.0/src/py/flwr/proto/driver_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr-1.3.0/src/py/flwr/proto/driver_pb2_grpc.pyi` & `flwr-1.4.0/src/py/flwr/proto/driver_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr-1.3.0/src/py/flwr/proto/fleet_pb2.pyi` & `flwr-1.4.0/src/py/flwr/proto/fleet_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr-1.3.0/src/py/flwr/proto/fleet_pb2_grpc.py` & `flwr-1.4.0/src/py/flwr/proto/fleet_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr-1.3.0/src/py/flwr/proto/fleet_pb2_grpc.pyi` & `flwr-1.4.0/src/py/flwr/proto/fleet_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr-1.3.0/src/py/flwr/proto/node_pb2.pyi` & `flwr-1.4.0/src/py/flwr/proto/node_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr-1.3.0/src/py/flwr/proto/task_pb2.pyi` & `flwr-1.4.0/src/py/flwr/proto/task_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr-1.3.0/src/py/flwr/proto/transport_pb2.pyi` & `flwr-1.4.0/src/py/flwr/proto/transport_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr-1.3.0/src/py/flwr/proto/transport_pb2_grpc.py` & `flwr-1.4.0/src/py/flwr/proto/transport_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr-1.3.0/src/py/flwr/proto/transport_pb2_grpc.pyi` & `flwr-1.4.0/src/py/flwr/proto/transport_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr-1.3.0/src/py/flwr/server/__init__.py` & `flwr-1.4.0/src/py/flwr/server/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,24 +11,30 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Flower server."""
 
 
+from . import strategy
 from .app import ServerConfig as ServerConfig
+from .app import run_driver_api as run_driver_api
+from .app import run_fleet_api as run_fleet_api
 from .app import run_server as run_server
 from .app import start_server as start_server
 from .client_manager import ClientManager as ClientManager
 from .client_manager import SimpleClientManager as SimpleClientManager
 from .history import History as History
 from .server import Server as Server
 
 __all__ = [
     "ClientManager",
-    "ServerConfig",
     "History",
+    "run_driver_api",
+    "run_fleet_api",
     "run_server",
     "Server",
+    "ServerConfig",
     "SimpleClientManager",
     "start_server",
+    "strategy",
 ]
```

### Comparing `flwr-1.3.0/src/py/flwr/server/client_manager.py` & `flwr-1.4.0/src/py/flwr/server/client_manager.py`

 * *Files identical despite different names*

### Comparing `flwr-1.3.0/src/py/flwr/server/client_proxy.py` & `flwr-1.4.0/src/py/flwr/server/client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr-1.3.0/src/py/flwr/server/criterion.py` & `flwr-1.4.0/src/py/flwr/server/criterion.py`

 * *Files identical despite different names*

### Comparing `flwr-1.3.0/src/py/flwr/server/driver/__init__.py` & `flwr-1.4.0/src/py/flwr/server/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr-1.3.0/src/py/flwr/server/fleet/__init__.py` & `flwr-1.4.0/src/py/flwr/server/fleet/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr-1.3.0/src/py/flwr/server/fleet/fleet_servicer.py` & `flwr-1.4.0/src/py/flwr/server/fleet/fleet_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr-1.3.0/src/py/flwr/server/grpc_server/__init__.py` & `flwr-1.4.0/src/py/flwr/server/grpc_server/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr-1.3.0/src/py/flwr/server/grpc_server/driver_client_manager.py` & `flwr-1.4.0/src/py/flwr/server/grpc_server/driver_client_manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,33 +11,33 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Flower DriverClientManager."""
 
 
+import random
 import threading
-import uuid
 from typing import Dict, List, Optional, Set, Tuple
 
 from flwr.server.client_manager import ClientManager
 from flwr.server.client_proxy import ClientProxy
 from flwr.server.criterion import Criterion
-from flwr.server.state import State
+from flwr.server.state import State, StateFactory
 
 from .ins_scheduler import InsScheduler
 
 
 class DriverClientManager(ClientManager):
     """Provides a pool of available clients."""
 
-    def __init__(self, state: State) -> None:
+    def __init__(self, state_factory: StateFactory) -> None:
         self._cv = threading.Condition()
         self.nodes: Dict[str, Tuple[int, InsScheduler]] = {}
-        self.state = state
+        self.state_factory = state_factory
 
     def __len__(self) -> int:
         """Return the number of available clients.
 
         Returns
         -------
         num_available : int
@@ -68,24 +68,25 @@
             Indicating if registration was successful. False if ClientProxy is
             already registered or can not be registered for any reason.
         """
         if client.cid in self.nodes:
             return False
 
         # Generate random integer ID
-        random_node_id: int = uuid.uuid1().int >> 64
+        random_node_id: int = random.randrange(9223372036854775808)
         client.node_id = random_node_id
 
         # Register node_id in with State
-        self.state.register_node(node_id=random_node_id)
+        state: State = self.state_factory.state()
+        state.register_node(node_id=random_node_id)
 
         # Create and start the instruction scheduler
         ins_scheduler = InsScheduler(
             client_proxy=client,
-            state=self.state,
+            state_factory=self.state_factory,
         )
         ins_scheduler.start()
 
         # Store cid, node_id, and InsScheduler
         self.nodes[client.cid] = (random_node_id, ins_scheduler)
 
         with self._cv:
@@ -104,15 +105,16 @@
         """
         if client.cid in self.nodes:
             node_id, ins_scheduler = self.nodes[client.cid]
             del self.nodes[client.cid]
             ins_scheduler.stop()
 
             # Unregister node_id in with State
-            self.state.unregister_node(node_id=node_id)
+            state: State = self.state_factory.state()
+            state.unregister_node(node_id=node_id)
 
             with self._cv:
                 self._cv.notify_all()
 
     def all_ids(self) -> Set[int]:
         """Return all available node ids.
```

### Comparing `flwr-1.3.0/src/py/flwr/server/grpc_server/flower_service_servicer.py` & `flwr-1.4.0/src/py/flwr/server/grpc_server/flower_service_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr-1.3.0/src/py/flwr/server/grpc_server/grpc_bridge.py` & `flwr-1.4.0/src/py/flwr/server/grpc_server/grpc_bridge.py`

 * *Files identical despite different names*

### Comparing `flwr-1.3.0/src/py/flwr/server/grpc_server/grpc_client_proxy.py` & `flwr-1.4.0/src/py/flwr/server/grpc_server/grpc_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr-1.3.0/src/py/flwr/server/grpc_server/grpc_server.py` & `flwr-1.4.0/src/py/flwr/server/grpc_server/grpc_server.py`

 * *Files identical despite different names*

### Comparing `flwr-1.3.0/src/py/flwr/server/grpc_server/ins_scheduler.py` & `flwr-1.4.0/src/py/flwr/server/grpc_server/ins_scheduler.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,34 +22,34 @@
 
 from flwr.common import EvaluateRes, FitRes, GetParametersRes, GetPropertiesRes, serde
 from flwr.common.logger import log
 from flwr.proto.node_pb2 import Node
 from flwr.proto.task_pb2 import Task, TaskIns, TaskRes
 from flwr.proto.transport_pb2 import ClientMessage, ServerMessage
 from flwr.server.client_proxy import ClientProxy
-from flwr.server.state import State
+from flwr.server.state import State, StateFactory
 
 
 class InsScheduler:
     """Schedule ClientProxy calls on a background thread."""
 
-    def __init__(self, client_proxy: ClientProxy, state: State):
+    def __init__(self, client_proxy: ClientProxy, state_factory: StateFactory):
         self.client_proxy = client_proxy
-        self.state = state
+        self.state_factory = state_factory
         self.worker_thread: Optional[threading.Thread] = None
         self.shared_memory_state = {"stop": False}
 
     def start(self) -> None:
         """Start the worker thread."""
         self.worker_thread = threading.Thread(
             target=_worker,
             args=(
                 self.client_proxy,
                 self.shared_memory_state,
-                self.state,
+                self.state_factory,
             ),
         )
         self.worker_thread.start()
 
     def stop(self) -> None:
         """Stop the worker thread."""
         if self.worker_thread is None:
@@ -60,18 +60,20 @@
         self.worker_thread = None
         self.shared_memory_state["stop"] = False
 
 
 def _worker(
     client_proxy: ClientProxy,
     shared_memory_state: Dict[str, bool],
-    state: State,
+    state_factory: StateFactory,
 ) -> None:
     """Sequentially call ClientProxy methods to process outstanding tasks."""
     log(DEBUG, "Worker for node %i started", client_proxy.node_id)
+
+    state: State = state_factory.state()
     while not shared_memory_state["stop"]:
         log(DEBUG, "Worker for node %i checking state", client_proxy.node_id)
 
         # Step 1: pull *Ins (next task) out of `state`
         task_ins_list: List[TaskIns] = state.get_task_ins(
             node_id=client_proxy.node_id,
             limit=1,
@@ -100,14 +102,15 @@
         # Step 3: wrap FitRes in a ServerMessage in a Task in a TaskRes
         task_res = TaskRes(
             task_id="",  # Will be created and set by the State
             group_id="",
             workload_id="",
             task=Task(
                 producer=Node(node_id=client_proxy.node_id, anonymous=False),
+                consumer=Node(node_id=0, anonymous=True),
                 legacy_client_message=client_message_proto,
                 ancestry=[task_ins.task_id],
             ),
         )
 
         # Step 4: write *Res (result) back to `state`
         state.store_task_res(task_res=task_res)
```

### Comparing `flwr-1.3.0/src/py/flwr/server/history.py` & `flwr-1.4.0/src/py/flwr/server/history.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,37 +10,50 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Training history."""
 
+
 from functools import reduce
 from typing import Dict, List, Tuple
 
 from flwr.common.typing import Scalar
 
 
 class History:
     """History class for training and/or evaluation metrics collection."""
 
     def __init__(self) -> None:
         self.losses_distributed: List[Tuple[int, float]] = []
         self.losses_centralized: List[Tuple[int, float]] = []
+        self.metrics_distributed_fit: Dict[str, List[Tuple[int, Scalar]]] = {}
         self.metrics_distributed: Dict[str, List[Tuple[int, Scalar]]] = {}
         self.metrics_centralized: Dict[str, List[Tuple[int, Scalar]]] = {}
 
     def add_loss_distributed(self, server_round: int, loss: float) -> None:
         """Add one loss entry (from distributed evaluation)."""
         self.losses_distributed.append((server_round, loss))
 
     def add_loss_centralized(self, server_round: int, loss: float) -> None:
         """Add one loss entry (from centralized evaluation)."""
         self.losses_centralized.append((server_round, loss))
 
+    def add_metrics_distributed_fit(
+        self, server_round: int, metrics: Dict[str, Scalar]
+    ) -> None:
+        """Add metrics entries (from distributed fit)."""
+        for key in metrics:
+            # if not (isinstance(metrics[key], float) or isinstance(metrics[key], int)):
+            #     continue  # ignore non-numeric key/value pairs
+            if key not in self.metrics_distributed_fit:
+                self.metrics_distributed_fit[key] = []
+            self.metrics_distributed_fit[key].append((server_round, metrics[key]))
+
     def add_metrics_distributed(
         self, server_round: int, metrics: Dict[str, Scalar]
     ) -> None:
         """Add metrics entries (from distributed evaluation)."""
         for key in metrics:
             # if not (isinstance(metrics[key], float) or isinstance(metrics[key], int)):
             #     continue  # ignore non-numeric key/value pairs
@@ -73,12 +86,18 @@
             rep += "History (loss, centralized):\n" + reduce(
                 lambda a, b: a + b,
                 [
                     f"\tround {server_round}: {loss}\n"
                     for server_round, loss in self.losses_centralized
                 ],
             )
+        if self.metrics_distributed_fit:
+            rep += "History (metrics, distributed, fit):\n" + str(
+                self.metrics_distributed_fit
+            )
         if self.metrics_distributed:
-            rep += "History (metrics, distributed):\n" + str(self.metrics_distributed)
+            rep += "History (metrics, distributed, evaluate):\n" + str(
+                self.metrics_distributed
+            )
         if self.metrics_centralized:
             rep += "History (metrics, centralized):\n" + str(self.metrics_centralized)
         return rep
```

### Comparing `flwr-1.3.0/src/py/flwr/server/server.py` & `flwr-1.4.0/src/py/flwr/server/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,17 +101,20 @@
         log(INFO, "FL starting")
         start_time = timeit.default_timer()
 
         for current_round in range(1, num_rounds + 1):
             # Train model and replace previous global model
             res_fit = self.fit_round(server_round=current_round, timeout=timeout)
             if res_fit:
-                parameters_prime, _, _ = res_fit  # fit_metrics_aggregated
+                parameters_prime, fit_metrics, _ = res_fit  # fit_metrics_aggregated
                 if parameters_prime:
                     self.parameters = parameters_prime
+                history.add_metrics_distributed_fit(
+                    server_round=current_round, metrics=fit_metrics
+                )
 
             # Evaluate model using strategy implementation
             res_cen = self.strategy.evaluate(current_round, parameters=self.parameters)
             if res_cen is not None:
                 loss_cen, metrics_cen = res_cen
                 log(
                     INFO,
```

### Comparing `flwr-1.3.0/src/py/flwr/server/state/__init__.py` & `flwr-1.4.0/src/py/flwr/common/date.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-# Copyright 2023 Adap GmbH. All Rights Reserved.
+# Copyright 2020 Adap GmbH. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Flower server state."""
+"""Flower date utils."""
 
 
-from .in_memory_state import InMemoryState
-from .state import State
+from datetime import datetime, timezone
 
-__all__ = [
-    "InMemoryState",
-    "State",
-]
+
+def now() -> datetime:
+    """Construct a datetime from time.time() with time zone set to UTC."""
+    return datetime.now(tz=timezone.utc)
```

### Comparing `flwr-1.3.0/src/py/flwr/server/state/in_memory_state.py` & `flwr-1.4.0/src/py/flwr/server/state/in_memory_state.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,43 +11,49 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """In-memory State implementation."""
 
 
-from datetime import datetime, timedelta, timezone
+from datetime import datetime, timedelta
+from logging import ERROR
 from typing import Dict, List, Optional, Set
 from uuid import UUID, uuid4
 
+from flwr.common import log, now
 from flwr.proto.task_pb2 import TaskIns, TaskRes
-
-from .state import State
+from flwr.server.state.state import State
+from flwr.server.utils import validate_task_ins_or_res
 
 
 class InMemoryState(State):
     """In-memory State implementation."""
 
     def __init__(self) -> None:
         self.node_ids: Set[int] = set()
         self.task_ins_store: Dict[UUID, TaskIns] = {}
         self.task_res_store: Dict[UUID, TaskRes] = {}
 
     def store_task_ins(self, task_ins: TaskIns) -> Optional[UUID]:
         """Store one TaskIns."""
 
-        # Create and set task_id
-        task_id = uuid4()
-        task_ins.task_id = str(task_id)
+        # Validate task
+        errors = validate_task_ins_or_res(task_ins)
+        if any(errors):
+            log(ERROR, errors)
+            return None
 
-        # Set created_at
-        created_at: datetime = _now()
+        # Create task_id, created_at and ttl
+        task_id = uuid4()
+        created_at: datetime = now()
         ttl: datetime = created_at + timedelta(hours=24)
 
         # Store TaskIns
+        task_ins.task_id = str(task_id)
         task_ins.task.created_at = created_at.isoformat()
         task_ins.task.ttl = ttl.isoformat()
         self.task_ins_store[task_id] = task_ins
 
         # Return the new task_id
         return task_id
 
@@ -75,33 +81,37 @@
                 and task_ins.task.delivered_at == ""
             ):
                 task_ins_list.append(task_ins)
             if limit and len(task_ins_list) == limit:
                 break
 
         # Mark all of them as delivered
-        delivered_at = _now().isoformat()
+        delivered_at = now().isoformat()
         for task_ins in task_ins_list:
             task_ins.task.delivered_at = delivered_at
 
         # Return TaskIns
         return task_ins_list
 
     def store_task_res(self, task_res: TaskRes) -> Optional[UUID]:
         """Store one TaskRes."""
 
-        # Create and set task_id
-        task_id = uuid4()
-        task_res.task_id = str(task_id)
+        # Validate task
+        errors = validate_task_ins_or_res(task_res)
+        if any(errors):
+            log(ERROR, errors)
+            return None
 
-        # Set created_at
-        created_at: datetime = _now()
+        # Create task_id, created_at and ttl
+        task_id = uuid4()
+        created_at: datetime = now()
         ttl: datetime = created_at + timedelta(hours=24)
 
         # Store TaskRes
+        task_res.task_id = str(task_id)
         task_res.task.created_at = created_at.isoformat()
         task_res.task.ttl = ttl.isoformat()
         self.task_res_store[task_id] = task_res
 
         # Return the new task_id
         return task_id
 
@@ -119,21 +129,49 @@
                 and task_res.task.delivered_at == ""
             ):
                 task_res_list.append(task_res)
             if limit and len(task_res_list) == limit:
                 break
 
         # Mark all of them as delivered
-        delivered_at = _now().isoformat()
+        delivered_at = now().isoformat()
         for task_res in task_res_list:
             task_res.task.delivered_at = delivered_at
 
         # Return TaskRes
         return task_res_list
 
+    def delete_tasks(self, task_ids: Set[UUID]) -> None:
+        """Delete all delivered TaskIns/TaskRes pairs."""
+
+        task_ins_to_be_deleted: Set[UUID] = set()
+        task_res_to_be_deleted: Set[UUID] = set()
+
+        for task_ins_id in task_ids:
+            # Find the task_id of the matching task_res
+            for task_res_id, task_res in self.task_res_store.items():
+                if UUID(task_res.task.ancestry[0]) != task_ins_id:
+                    continue
+                if task_res.task.delivered_at == "":
+                    continue
+
+                task_ins_to_be_deleted.add(task_ins_id)
+                task_res_to_be_deleted.add(task_res_id)
+
+        for task_id in task_ins_to_be_deleted:
+            del self.task_ins_store[task_id]
+        for task_id in task_res_to_be_deleted:
+            del self.task_res_store[task_id]
+
+    def num_task_ins(self) -> int:
+        return len(self.task_ins_store)
+
+    def num_task_res(self) -> int:
+        return len(self.task_res_store)
+
     def register_node(self, node_id: int) -> None:
         """Register a client node."""
         if node_id in self.node_ids:
             raise ValueError(f"Node {node_id} is already registered")
         self.node_ids.add(node_id)
 
     def unregister_node(self, node_id: int) -> None:
@@ -141,11 +179,7 @@
         if node_id not in self.node_ids:
             raise ValueError(f"Node {node_id} is not registered")
         self.node_ids.remove(node_id)
 
     def get_nodes(self) -> Set[int]:
         """Return all available client nodes."""
         return self.node_ids
-
-
-def _now() -> datetime:
-    return datetime.now(tz=timezone.utc)
```

### Comparing `flwr-1.3.0/src/py/flwr/server/strategy/__init__.py` & `flwr-1.4.0/src/py/flwr/server/strategy/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,23 +20,25 @@
 from .fedadam import FedAdam as FedAdam
 from .fedavg import FedAvg as FedAvg
 from .fedavg_android import FedAvgAndroid as FedAvgAndroid
 from .fedavgm import FedAvgM as FedAvgM
 from .fedmedian import FedMedian as FedMedian
 from .fedopt import FedOpt as FedOpt
 from .fedprox import FedProx as FedProx
+from .fedxgb_nn_avg import FedXgbNnAvg as FedXgbNnAvg
 from .fedyogi import FedYogi as FedYogi
 from .qfedavg import QFedAvg as QFedAvg
 from .strategy import Strategy as Strategy
 
 __all__ = [
     "FaultTolerantFedAvg",
     "FedAdagrad",
     "FedAdam",
     "FedAvg",
+    "FedXgbNnAvg",
     "FedAvgAndroid",
     "FedAvgM",
     "FedOpt",
     "FedProx",
     "FedYogi",
     "QFedAvg",
     "FedMedian",
```

### Comparing `flwr-1.3.0/src/py/flwr/server/strategy/aggregate.py` & `flwr-1.4.0/src/py/flwr/server/strategy/aggregate.py`

 * *Files identical despite different names*

### Comparing `flwr-1.3.0/src/py/flwr/server/strategy/dpfedavg_adaptive.py` & `flwr-1.4.0/src/py/flwr/server/strategy/dpfedavg_adaptive.py`

 * *Files identical despite different names*

### Comparing `flwr-1.3.0/src/py/flwr/server/strategy/dpfedavg_fixed.py` & `flwr-1.4.0/src/py/flwr/server/strategy/dpfedavg_fixed.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # limitations under the License.
 # ==============================================================================
 """DP-FedAvg [McMahan et al., 2018] strategy.
 
 Paper: https://arxiv.org/pdf/1710.06963.pdf
 """
 
+
 from typing import Dict, List, Optional, Tuple, Union
 
 from flwr.common import EvaluateIns, EvaluateRes, FitIns, FitRes, Parameters, Scalar
 from flwr.common.dp import add_gaussian_noise
 from flwr.common.parameter import ndarrays_to_parameters, parameters_to_ndarrays
 from flwr.server.client_manager import ClientManager
 from flwr.server.client_proxy import ClientProxy
```

### Comparing `flwr-1.3.0/src/py/flwr/server/strategy/fault_tolerant_fedavg.py` & `flwr-1.4.0/src/py/flwr/server/strategy/fault_tolerant_fedavg.py`

 * *Files identical despite different names*

### Comparing `flwr-1.3.0/src/py/flwr/server/strategy/fedadagrad.py` & `flwr-1.4.0/src/py/flwr/server/strategy/fedadagrad.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
             Function used to configure validation. Defaults to None.
         fit_metrics_aggregation_fn : Optional[MetricsAggregationFn]
             Metrics aggregation function, optional.
         evaluate_metrics_aggregation_fn: Optional[MetricsAggregationFn]
             Metrics aggregation function, optional.
         accept_failures : bool, optional
             Whether or not accept rounds containing failures. Defaults to True.
-        initial_parameters : Parameters, optional
+        initial_parameters : Parameters
             Initial global model parameters.
         eta : float, optional
             Server-side learning rate. Defaults to 1e-1.
         eta_l : float, optional
             Client-side learning rate. Defaults to 1e-1.
         tau : float, optional
             Controls the algorithm's degree of adaptability. Defaults to 1e-9.
```

### Comparing `flwr-1.3.0/src/py/flwr/server/strategy/fedadam.py` & `flwr-1.4.0/src/py/flwr/server/strategy/fedadam.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
             Optional function used for validation. Defaults to None.
         on_fit_config_fn : Callable[[int], Dict[str, Scalar]], optional
             Function used to configure training. Defaults to None.
         on_evaluate_config_fn : Callable[[int], Dict[str, Scalar]], optional
             Function used to configure validation. Defaults to None.
         accept_failures : bool, optional
             Whether or not accept rounds containing failures. Defaults to True.
-        initial_parameters : Parameters, optional
+        initial_parameters : Parameters
             Initial global model parameters.
         fit_metrics_aggregation_fn : Optional[MetricsAggregationFn]
             Metrics aggregation function, optional.
         evaluate_metrics_aggregation_fn: Optional[MetricsAggregationFn]
             Metrics aggregation function, optional.
         eta : float, optional
             Server-side learning rate. Defaults to 1e-1.
```

### Comparing `flwr-1.3.0/src/py/flwr/server/strategy/fedavg.py` & `flwr-1.4.0/src/py/flwr/server/strategy/fedavg.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 WARNING_MIN_AVAILABLE_CLIENTS_TOO_LOW = """
 Setting `min_available_clients` lower than `min_fit_clients` or
 `min_evaluate_clients` can cause the server to fail when there are too few clients
 connected to the server. `min_available_clients` must be set to a value larger
 than or equal to the values of `min_fit_clients` and `min_evaluate_clients`.
 """
 
+
 # flake8: noqa: E501
 class FedAvg(Strategy):
     """Configurable FedAvg strategy implementation."""
 
     # pylint: disable=too-many-arguments,too-many-instance-attributes,line-too-long
     def __init__(
         self,
```

### Comparing `flwr-1.3.0/src/py/flwr/server/strategy/fedavg_android.py` & `flwr-1.4.0/src/py/flwr/server/strategy/fedavg_android.py`

 * *Files identical despite different names*

### Comparing `flwr-1.3.0/src/py/flwr/server/strategy/fedavgm.py` & `flwr-1.4.0/src/py/flwr/server/strategy/fedavgm.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 WARNING_MIN_AVAILABLE_CLIENTS_TOO_LOW = """
 Setting `min_available_clients` lower than `min_fit_clients` or
 `min_evaluate_clients` can cause the server to fail when there are too few clients
 connected to the server. `min_available_clients` must be set to a value larger
 than or equal to the values of `min_fit_clients` and `min_evaluate_clients`.
 """
 
+
 # flake8: noqa: E501
 class FedAvgM(FedAvg):
     """Configurable FedAvg with Momentum strategy implementation."""
 
     # pylint: disable=too-many-arguments,too-many-instance-attributes,line-too-long
     def __init__(
         self,
```

### Comparing `flwr-1.3.0/src/py/flwr/server/strategy/fedmedian.py` & `flwr-1.4.0/src/py/flwr/server/strategy/fedmedian.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 WARNING_MIN_AVAILABLE_CLIENTS_TOO_LOW = """
 Setting `min_available_clients` lower than `min_fit_clients` or
 `min_evaluate_clients` can cause the server to fail when there are too few clients
 connected to the server. `min_available_clients` must be set to a value larger
 than or equal to the values of `min_fit_clients` and `min_evaluate_clients`.
 """
 
+
 # flake8: noqa: E501
 class FedMedian(FedAvg):
     """Configurable FedAvg with Momentum strategy implementation."""
 
     # pylint: disable=too-many-arguments,too-many-instance-attributes,line-too-long
     def __init__(
         self,
```

### Comparing `flwr-1.3.0/src/py/flwr/server/strategy/fedopt.py` & `flwr-1.4.0/src/py/flwr/server/strategy/fedopt.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
             Optional function used for validation. Defaults to None.
         on_fit_config_fn : Callable[[int], Dict[str, Scalar]], optional
             Function used to configure training. Defaults to None.
         on_evaluate_config_fn : Callable[[int], Dict[str, Scalar]], optional
             Function used to configure validation. Defaults to None.
         accept_failures : bool, optional
             Whether or not accept rounds containing failures. Defaults to True.
-        initial_parameters : Parameters, optional
+        initial_parameters : Parameters
             Initial global model parameters.
         fit_metrics_aggregation_fn : Optional[MetricsAggregationFn]
             Metrics aggregation function, optional.
         evaluate_metrics_aggregation_fn: Optional[MetricsAggregationFn]
             Metrics aggregation function, optional.
         eta : float, optional
             Server-side learning rate. Defaults to 1e-1.
```

### Comparing `flwr-1.3.0/src/py/flwr/server/strategy/fedprox.py` & `flwr-1.4.0/src/py/flwr/server/strategy/fedprox.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 WARNING_MIN_AVAILABLE_CLIENTS_TOO_LOW = """
 Setting `min_available_clients` lower than `min_fit_clients` or
 `min_evaluate_clients` can cause the server to fail when there are too few clients
 connected to the server. `min_available_clients` must be set to a value larger
 than or equal to the values of `min_fit_clients` and `min_evaluate_clients`.
 """
 
+
 # flake8: noqa: E501
 class FedProx(FedAvg):
     """Configurable FedProx strategy implementation."""
 
     # pylint: disable=too-many-arguments,too-many-instance-attributes,line-too-long
     def __init__(
         self,
```

### Comparing `flwr-1.3.0/src/py/flwr/server/strategy/fedyogi.py` & `flwr-1.4.0/src/py/flwr/server/strategy/fedyogi.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
             Optional function used for validation. Defaults to None.
         on_fit_config_fn : Callable[[int], Dict[str, Scalar]], optional
             Function used to configure training. Defaults to None.
         on_evaluate_config_fn : Callable[[int], Dict[str, Scalar]], optional
             Function used to configure validation. Defaults to None.
         accept_failures : bool, optional
             Whether or not accept rounds containing failures. Defaults to True.
-        initial_parameters : Parameters, optional
+        initial_parameters : Parameters
             Initial global model parameters.
         fit_metrics_aggregation_fn : Optional[MetricsAggregationFn]
             Metrics aggregation function, optional.
         evaluate_metrics_aggregation_fn: Optional[MetricsAggregationFn]
             Metrics aggregation function, optional.
         eta : float, optional
             Server-side learning rate. Defaults to 1e-1.
```

### Comparing `flwr-1.3.0/src/py/flwr/server/strategy/krum.py` & `flwr-1.4.0/src/py/flwr/server/strategy/krum.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 WARNING_MIN_AVAILABLE_CLIENTS_TOO_LOW = """
 Setting `min_available_clients` lower than `min_fit_clients` or
 `min_evaluate_clients` can cause the server to fail when there are too few clients
 connected to the server. `min_available_clients` must be set to a value larger
 than or equal to the values of `min_fit_clients` and `min_evaluate_clients`.
 """
 
+
 # flake8: noqa: E501
 class Krum(FedAvg):
     """Configurable Krum strategy implementation."""
 
     # pylint: disable=too-many-arguments,too-many-instance-attributes,line-too-long
     def __init__(
         self,
```

### Comparing `flwr-1.3.0/src/py/flwr/server/strategy/qfedavg.py` & `flwr-1.4.0/src/py/flwr/server/strategy/qfedavg.py`

 * *Files identical despite different names*

### Comparing `flwr-1.3.0/src/py/flwr/server/strategy/strategy.py` & `flwr-1.4.0/src/py/flwr/server/strategy/strategy.py`

 * *Files identical despite different names*

### Comparing `flwr-1.3.0/src/py/flwr/server/utils/__init__.py` & `flwr-1.4.0/src/py/flwr/simulation/ray_transport/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,14 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Contains server side utilities to be used in combination with various
-components."""
-
-
-from .tensorboard import tensorboard as tensorboard
-
-__all__ = ["tensorboard"]
+"""Ray-based Flower ClientProxy implementation."""
```

### Comparing `flwr-1.3.0/src/py/flwr/server/utils/tensorboard.py` & `flwr-1.4.0/src/py/flwr/server/utils/tensorboard.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Flower TensorBoard utilities."""
+
+
 import os
 from datetime import datetime
 from typing import Callable, Dict, List, Optional, Tuple, TypeVar, Union, cast
 
 try:
     import tensorflow as tf
 except ImportError:
```

### Comparing `flwr-1.3.0/src/py/flwr/simulation/__init__.py` & `flwr-1.4.0/src/py/flwr/simulation/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Flower simulation."""
 
+
 import importlib
 
 is_ray_installed = importlib.util.find_spec("ray") is not None
 
 if is_ray_installed:
     from flwr.simulation.app import start_simulation
 else:
```

### Comparing `flwr-1.3.0/src/py/flwr/simulation/app.py` & `flwr-1.4.0/src/py/flwr/simulation/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 import sys
 from logging import ERROR, INFO
 from typing import Any, Callable, Dict, List, Optional
 
 import ray
 
-from flwr.client.client import Client
+from flwr.client import ClientLike
 from flwr.common import EventType, event
 from flwr.common.logger import log
 from flwr.server import Server
 from flwr.server.app import ServerConfig, _fl, _init_defaults
 from flwr.server.client_manager import ClientManager
 from flwr.server.history import History
 from flwr.server.strategy import Strategy
@@ -34,15 +34,15 @@
 INVALID_ARGUMENTS_START_SIMULATION = """
 INVALID ARGUMENTS ERROR
 
 Invalid Arguments in method:
 
 `start_simulation(
     *,
-    client_fn: Callable[[str], Client],
+    client_fn: Callable[[str], ClientLike],
     num_clients: Optional[int] = None,
     clients_ids: Optional[List[str]] = None,
     client_resources: Optional[Dict[str, float]] = None,
     server: Optional[Server] = None,
     config: ServerConfig = None,
     strategy: Optional[Strategy] = None,
     client_manager: Optional[ClientManager] = None,
@@ -57,39 +57,40 @@
         - `len(clients_ids)` == `num_clients`
 
 """
 
 
 def start_simulation(  # pylint: disable=too-many-arguments
     *,
-    client_fn: Callable[[str], Client],
+    client_fn: Callable[[str], ClientLike],
     num_clients: Optional[int] = None,
     clients_ids: Optional[List[str]] = None,
     client_resources: Optional[Dict[str, float]] = None,
     server: Optional[Server] = None,
     config: Optional[ServerConfig] = None,
     strategy: Optional[Strategy] = None,
     client_manager: Optional[ClientManager] = None,
     ray_init_args: Optional[Dict[str, Any]] = None,
     keep_initialised: Optional[bool] = False,
 ) -> History:
     """Start a Ray-based Flower simulation server.
 
     Parameters
     ----------
-    client_fn : Callable[[str], Client]
+    client_fn : Callable[[str], ClientLike]
         A function creating client instances. The function must take a single
-        str argument called `cid`. It should return a single client instance.
-        Note that the created client instances are ephemeral and will often be
-        destroyed after a single method invocation. Since client instances are
-        not long-lived, they should not attempt to carry state over method
-        invocations. Any state required by the instance (model, dataset,
-        hyperparameters, ...) should be (re-)created in either the call to
-        `client_fn` or the call to any of the client methods (e.g., load
-        evaluation data in the `evaluate` method itself).
+        str argument called `cid`. It should return a single client instance
+        of type ClientLike. Note that the created client instances
+        are ephemeral and will often be destroyed after a single method
+        invocation. Since client instances are not long-lived, they should not
+         attempt to carry state over method invocations. Any state required by
+        the instance (model, dataset,hyperparameters, ...) should be
+        (re-)created in either the call to `client_fn` or the call to any of
+        the client methods (e.g., load evaluation data in the `evaluate`
+        method itself).
     num_clients : Optional[int]
         The total number of clients in this simulation. This must be set if
         `clients_ids` is not set and vice-versa.
     clients_ids : Optional[List[str]]
         List `client_id`s for each client. This is only required if
         `num_clients` is not set. Setting both `num_clients` and `clients_ids`
         with `len(clients_ids)` not equal to `num_clients` generates an error.
@@ -167,23 +168,23 @@
     if not ray_init_args:
         ray_init_args = {
             "ignore_reinit_error": True,
             "include_dashboard": False,
         }
 
     # Shut down Ray if it has already been initialized (unless asked not to)
-    if ray.is_initialized() and not keep_initialised:  # type: ignore
-        ray.shutdown()  # type: ignore
+    if ray.is_initialized() and not keep_initialised:
+        ray.shutdown()
 
     # Initialize Ray
-    ray.init(**ray_init_args)  # type: ignore
+    ray.init(**ray_init_args)
     log(
         INFO,
         "Flower VCE: Ray initialized with resources: %s",
-        ray.cluster_resources(),  # type: ignore
+        ray.cluster_resources(),
     )
 
     # Register one RayClientProxy object for each client with the ClientManager
     resources = client_resources if client_resources is not None else {}
     for cid in cids:
         client_proxy = RayClientProxy(
             client_fn=client_fn,
```

### Comparing `flwr-1.3.0/src/py/flwr/simulation/ray_transport/__init__.py` & `flwr-1.4.0/src/py/flwr/server/rest_server/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Ray-based Flower ClientProxy implementation."""
+"""Server-side part of the REST transport layer."""
```

### Comparing `flwr-1.3.0/src/py/flwr/simulation/ray_transport/ray_client_proxy.py` & `flwr-1.4.0/src/py/flwr/simulation/ray_transport/ray_client_proxy.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Ray-based Flower ClientProxy implementation."""
 
 
-from logging import DEBUG
+from logging import ERROR
 from typing import Callable, Dict, Optional, cast
 
 import ray
 
 from flwr import common
 from flwr.client import Client, ClientLike, to_client
 from flwr.client.client import (
@@ -42,120 +42,120 @@
         self.client_fn = client_fn
         self.resources = resources
 
     def get_properties(
         self, ins: common.GetPropertiesIns, timeout: Optional[float]
     ) -> common.GetPropertiesRes:
         """Returns client's properties."""
-        future_get_properties_res = launch_and_get_properties.options(
+        future_get_properties_res = launch_and_get_properties.options(  # type: ignore
             **self.resources,
         ).remote(self.client_fn, self.cid, ins)
         try:
-            res = ray.get(future_get_properties_res, timeout=timeout)  # type: ignore
+            res = ray.get(future_get_properties_res, timeout=timeout)
         except Exception as ex:
-            log(DEBUG, ex)
+            log(ERROR, ex)
             raise ex
         return cast(
             common.GetPropertiesRes,
             res,
         )
 
     def get_parameters(
         self, ins: common.GetParametersIns, timeout: Optional[float]
     ) -> common.GetParametersRes:
         """Return the current local model parameters."""
-        future_paramseters_res = launch_and_get_parameters.options(
+        future_paramseters_res = launch_and_get_parameters.options(  # type: ignore
             **self.resources,
         ).remote(self.client_fn, self.cid, ins)
         try:
-            res = ray.get(future_paramseters_res, timeout=timeout)  # type: ignore
+            res = ray.get(future_paramseters_res, timeout=timeout)
         except Exception as ex:
-            log(DEBUG, ex)
+            log(ERROR, ex)
             raise ex
         return cast(
             common.GetParametersRes,
             res,
         )
 
     def fit(self, ins: common.FitIns, timeout: Optional[float]) -> common.FitRes:
         """Train model parameters on the locally held dataset."""
-        future_fit_res = launch_and_fit.options(
+        future_fit_res = launch_and_fit.options(  # type: ignore
             **self.resources,
         ).remote(self.client_fn, self.cid, ins)
         try:
-            res = ray.get(future_fit_res, timeout=timeout)  # type: ignore
+            res = ray.get(future_fit_res, timeout=timeout)
         except Exception as ex:
-            log(DEBUG, ex)
+            log(ERROR, ex)
             raise ex
         return cast(
             common.FitRes,
             res,
         )
 
     def evaluate(
         self, ins: common.EvaluateIns, timeout: Optional[float]
     ) -> common.EvaluateRes:
         """Evaluate model parameters on the locally held dataset."""
-        future_evaluate_res = launch_and_evaluate.options(
+        future_evaluate_res = launch_and_evaluate.options(  # type: ignore
             **self.resources,
         ).remote(self.client_fn, self.cid, ins)
         try:
-            res = ray.get(future_evaluate_res, timeout=timeout)  # type: ignore
+            res = ray.get(future_evaluate_res, timeout=timeout)
         except Exception as ex:
-            log(DEBUG, ex)
+            log(ERROR, ex)
             raise ex
         return cast(
             common.EvaluateRes,
             res,
         )
 
     def reconnect(
         self, ins: common.ReconnectIns, timeout: Optional[float]
     ) -> common.DisconnectRes:
         """Disconnect and (optionally) reconnect later."""
         return common.DisconnectRes(reason="")  # Nothing to do here (yet)
 
 
-@ray.remote  # type: ignore
+@ray.remote
 def launch_and_get_properties(
     client_fn: ClientFn, cid: str, get_properties_ins: common.GetPropertiesIns
 ) -> common.GetPropertiesRes:
     """Exectue get_properties remotely."""
     client: Client = _create_client(client_fn, cid)
     return maybe_call_get_properties(
         client=client,
         get_properties_ins=get_properties_ins,
     )
 
 
-@ray.remote  # type: ignore
+@ray.remote
 def launch_and_get_parameters(
     client_fn: ClientFn, cid: str, get_parameters_ins: common.GetParametersIns
 ) -> common.GetParametersRes:
     """Exectue get_parameters remotely."""
     client: Client = _create_client(client_fn, cid)
     return maybe_call_get_parameters(
         client=client,
         get_parameters_ins=get_parameters_ins,
     )
 
 
-@ray.remote  # type: ignore
+@ray.remote
 def launch_and_fit(
     client_fn: ClientFn, cid: str, fit_ins: common.FitIns
 ) -> common.FitRes:
     """Exectue fit remotely."""
     client: Client = _create_client(client_fn, cid)
     return maybe_call_fit(
         client=client,
         fit_ins=fit_ins,
     )
 
 
-@ray.remote  # type: ignore
+@ray.remote
 def launch_and_evaluate(
     client_fn: ClientFn, cid: str, evaluate_ins: common.EvaluateIns
 ) -> common.EvaluateRes:
     """Exectue evaluate remotely."""
     client: Client = _create_client(client_fn, cid)
     return maybe_call_evaluate(
         client=client,
```

### Comparing `flwr-1.3.0/setup.py` & `flwr-1.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,52 +5,57 @@
 {'': 'src/py'}
 
 packages = \
 ['flwr',
  'flwr.client',
  'flwr.client.grpc_client',
  'flwr.client.message_handler',
+ 'flwr.client.rest_client',
  'flwr.common',
  'flwr.driver',
  'flwr.proto',
  'flwr.server',
  'flwr.server.driver',
  'flwr.server.fleet',
  'flwr.server.grpc_server',
+ 'flwr.server.rest_server',
  'flwr.server.state',
  'flwr.server.strategy',
  'flwr.server.utils',
  'flwr.simulation',
  'flwr.simulation.ray_transport']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['grpcio>=1.43.0,<2.0.0,!=1.52.0',
+['grpcio>=1.48.2,<2.0.0,!=1.52.0',
  'iterators>=0.0.2,<0.0.3',
  'numpy>=1.21.0,<2.0.0',
  'protobuf>=3.19.0,<4.0.0']
 
 extras_require = \
-{':extra == "rest"': ['requests>=2.28.1,<3.0.0',
-                      'fastapi>=0.89.1,<0.90.0',
-                      'uvicorn[standard]>=0.20.0,<0.21.0'],
- ':python_version < "3.8"': ['importlib-metadata>=4.0.0,<5.0.0'],
- 'simulation': ['ray[default]>=2.2.0,<2.3.0']}
+{':python_version < "3.8"': ['importlib-metadata>=4.0.0,<5.0.0'],
+ 'rest': ['requests>=2.28.2,<3.0.0',
+          'fastapi>=0.95.0,<0.96.0',
+          'starlette>=0.26.1,<0.27.0',
+          'uvicorn[standard]>=0.21.1,<0.22.0'],
+ 'simulation': ['ray[default]>=2.3.0,<3.0.0']}
 
 entry_points = \
 {'console_scripts': ['flower-client = flwr.client:run_client',
+                     'flower-driver-api = flwr.server:run_driver_api',
+                     'flower-fleet-api = flwr.server:run_fleet_api',
                      'flower-server = flwr.server:run_server']}
 
 setup_kwargs = {
     'name': 'flwr',
-    'version': '1.3.0',
+    'version': '1.4.0',
     'description': 'Flower: A Friendly Federated Learning Framework',
-    'long_description': '# Flower: A Friendly Federated Learning Framework\n\n<p align="center">\n  <a href="https://flower.dev/">\n    <img src="https://flower.dev/_next/image/?url=%2F_next%2Fstatic%2Fmedia%2Fflower_white_border.c2012e70.png&w=640&q=75" width="140px" alt="Flower Website" />\n  </a>\n</p>\n<p align="center">\n    <a href="https://flower.dev/">Website</a> |\n    <a href="https://flower.dev/blog">Blog</a> |\n    <a href="https://flower.dev/docs/">Docs</a> |\n    <a href="https://flower.dev/conf/flower-summit-2022">Conference</a> |\n    <a href="https://flower.dev/join-slack">Slack</a>\n    <br /><br />\n</p>\n\n[![GitHub license](https://img.shields.io/github/license/adap/flower)](https://github.com/adap/flower/blob/main/LICENSE)\n[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/adap/flower/blob/main/CONTRIBUTING.md)\n![Build](https://github.com/adap/flower/actions/workflows/flower.yml/badge.svg)\n![Downloads](https://pepy.tech/badge/flwr)\n[![Slack](https://img.shields.io/badge/Chat-Slack-red)](https://flower.dev/join-slack)\n\nFlower (`flwr`) is a framework for building federated learning systems. The\ndesign of Flower is based on a few guiding principles:\n\n* **Customizable**: Federated learning systems vary wildly from one use case to\n  another. Flower allows for a wide range of different configurations depending\n  on the needs of each individual use case.\n\n* **Extendable**: Flower originated from a research project at the University of\n  Oxford, so it was built with AI research in mind. Many components can be\n  extended and overridden to build new state-of-the-art systems.\n\n* **Framework-agnostic**: Different machine learning frameworks have different\n  strengths. Flower can be used with any machine learning framework, for\n  example, [PyTorch](https://pytorch.org),\n  [TensorFlow](https://tensorflow.org), [Hugging Face Transformers](https://huggingface.co/), [PyTorch Lightning](https://pytorchlightning.ai/), [MXNet](https://mxnet.apache.org/), [scikit-learn](https://scikit-learn.org/), [JAX](https://jax.readthedocs.io/), [TFLite](https://tensorflow.org/lite/), [fastai](https://www.fast.ai/), [Pandas](https://pandas.pydata.org/\n) for federated analytics, or even raw [NumPy](https://numpy.org/)\n  for users who enjoy computing gradients by hand.\n\n* **Understandable**: Flower is written with maintainability in mind. The\n  community is encouraged to both read and contribute to the codebase.\n\nMeet the Flower community on [flower.dev](https://flower.dev)!\n\n## Federated Learning Tutorial\n\nFlower\'s goal is to make federated learning accessible to everyone. This series of tutorials introduces the fundamentals of federated learning and how to implement them in Flower.\n\n1. **An Introduction to Federated Learning**\n\n   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-1-Intro-to-FL-PyTorch.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-1-Intro-to-FL-PyTorch.ipynb))\n\n2. **Using Strategies in Federated Learning**\n\n   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-2-Strategies-in-FL-PyTorch.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-2-Strategies-in-FL-PyTorch.ipynb))\n   \n3. **Building Strategies for Federated Learning**\n\n   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-3-Building-a-Strategy-PyTorch.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-3-Building-a-Strategy-PyTorch.ipynb))\n   \n4. **Custom Clients for Federated Learning**\n\n   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-4-Client-and-NumPyClient-PyTorch.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-4-Client-and-NumPyClient-PyTorch.ipynb))\n\nStay tuned, more tutorials are coming soon. Topics include **Privacy and Security in Federated Learning**, and **Scaling Federated Learning**.\n\n## Documentation\n\n[Flower Docs](https://flower.dev/docs):\n* [Installation](https://flower.dev/docs/installation.html)\n* [Quickstart (TensorFlow)](https://flower.dev/docs/quickstart-tensorflow.html)\n* [Quickstart (PyTorch)](https://flower.dev/docs/quickstart-pytorch.html)\n* [Quickstart (Hugging Face [code example])](https://flower.dev/docs/quickstart-huggingface.html)\n* [Quickstart (PyTorch Lightning [code example])](https://flower.dev/docs/quickstart-pytorch-lightning.html)\n* [Quickstart (MXNet)](https://flower.dev/docs/example-mxnet-walk-through.html)\n* [Quickstart (Pandas)](https://flower.dev/docs/quickstart-pandas.html)\n* [Quickstart (fastai)](https://flower.dev/docs/quickstart-fastai.html)\n* [Quickstart (JAX)](https://github.com/adap/flower/tree/main/examples/quickstart_jax)\n* [Quickstart (scikit-learn)](https://github.com/adap/flower/tree/main/examples/sklearn-logreg-mnist)\n* [Quickstart (TFLite on Android [code example])](https://github.com/adap/flower/tree/main/examples/android)\n\n## Flower Baselines\n\nFlower Baselines is a collection of community-contributed experiments that reproduce the experiments performed in popular federated learning publications. Researchers can build on Flower Baselines to quickly evaluate new ideas:\n\n* [FedAvg](https://arxiv.org/pdf/1602.05629.pdf):\n  * [MNIST](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/fedavg_mnist)\n* [FedBN: Federated Learning on non-IID Features via Local Batch Normalization](https://arxiv.org/pdf/2102.07623.pdf):\n  * [Convergence Rate](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/fedbn/convergence_rate)\n* [Adaptive Federated Optimization](https://arxiv.org/pdf/2003.00295.pdf):\n  * [CIFAR-10/100](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/adaptive_federated_optimization)\n\nCheck the Flower documentation to learn more: [Using Baselines](https://flower.dev/docs/using-baselines.html)\n\nThe Flower community loves contributions! Make your work more visible and enable others to build on it by contributing it as a baseline: [Contributing Baselines](https://flower.dev/docs/contributing-baselines.html)\n\n## Flower Usage Examples\n\nSeveral code examples show different usage scenarios of Flower (in combination with popular machine learning frameworks such as PyTorch or TensorFlow).\n\nQuickstart examples:\n\n* [Quickstart (TensorFlow)](https://github.com/adap/flower/tree/main/examples/quickstart_tensorflow)\n* [Quickstart (PyTorch)](https://github.com/adap/flower/tree/main/examples/quickstart_pytorch)\n* [Quickstart (Hugging Face)](https://github.com/adap/flower/tree/main/examples/quickstart_huggingface)\n* [Quickstart (PyTorch Lightning)](https://github.com/adap/flower/tree/main/examples/quickstart_pytorch_lightning)\n* [Quickstart (fastai)](https://github.com/adap/flower/tree/main/examples/quickstart_fastai)\n* [Quickstart (Pandas)](https://github.com/adap/flower/tree/main/examples/quickstart_pandas)\n* [Quickstart (MXNet)](https://github.com/adap/flower/tree/main/examples/quickstart_mxnet)\n* [Quickstart (JAX)](https://github.com/adap/flower/tree/main/examples/quickstart_jax)\n* [Quickstart (scikit-learn)](https://github.com/adap/flower/tree/main/examples/sklearn-logreg-mnist)\n* [Quickstart (TFLite on Android)](https://github.com/adap/flower/tree/main/examples/android)\n\nOther [examples](https://github.com/adap/flower/tree/main/examples):\n\n* [Raspberry Pi & Nvidia Jetson Tutorial](https://github.com/adap/flower/tree/main/examples/embedded_devices)\n* [Android & TFLite](https://github.com/adap/flower/tree/main/examples/android)\n* [PyTorch: From Centralized to Federated](https://github.com/adap/flower/tree/main/examples/pytorch_from_centralized_to_federated)\n* [MXNet: From Centralized to Federated](https://github.com/adap/flower/tree/main/examples/mxnet_from_centralized_to_federated)\n* [Advanced Flower with TensorFlow/Keras](https://github.com/adap/flower/tree/main/examples/advanced_tensorflow)\n* [Advanced Flower with PyTorch](https://github.com/adap/flower/tree/main/examples/advanced_pytorch)\n* Single-Machine Simulation of Federated Learning Systems ([PyTorch](https://github.com/adap/flower/tree/main/examples/simulation_pytorch)) ([Tensorflow](https://github.com/adap/flower/tree/main/examples/simulation_tensorflow))\n\n## Community\n\nFlower is built by a wonderful community of researchers and engineers. [Join Slack](https://flower.dev/join-slack) to meet them, [contributions](#contributing-to-flower) are welcome.\n\n<a href="https://github.com/adap/flower/graphs/contributors">\n  <img src="https://contrib.rocks/image?repo=adap/flower" />\n</a>\n\n## Citation\n\nIf you publish work that uses Flower, please cite Flower as follows: \n\n```bibtex\n@article{beutel2020flower,\n  title={Flower: A Friendly Federated Learning Research Framework},\n  author={Beutel, Daniel J and Topal, Taner and Mathur, Akhil and Qiu, Xinchi and Parcollet, Titouan and Lane, Nicholas D},\n  journal={arXiv preprint arXiv:2007.14390},\n  year={2020}\n}\n```\n\nPlease also consider adding your publication to the list of Flower-based publications in the docs, just open a Pull Request.\n\n## Contributing to Flower\n\nWe welcome contributions. Please see [CONTRIBUTING.md](CONTRIBUTING.md) to get started!\n',
+    'long_description': '# Flower: A Friendly Federated Learning Framework\n\n<p align="center">\n  <a href="https://flower.dev/">\n    <img src="https://flower.dev/_next/image/?url=%2F_next%2Fstatic%2Fmedia%2Fflower_white_border.c2012e70.png&w=640&q=75" width="140px" alt="Flower Website" />\n  </a>\n</p>\n<p align="center">\n    <a href="https://flower.dev/">Website</a> |\n    <a href="https://flower.dev/blog">Blog</a> |\n    <a href="https://flower.dev/docs/">Docs</a> |\n    <a href="https://flower.dev/conf/flower-summit-2022">Conference</a> |\n    <a href="https://flower.dev/join-slack">Slack</a>\n    <br /><br />\n</p>\n\n[![GitHub license](https://img.shields.io/github/license/adap/flower)](https://github.com/adap/flower/blob/main/LICENSE)\n[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/adap/flower/blob/main/CONTRIBUTING.md)\n![Build](https://github.com/adap/flower/actions/workflows/flower.yml/badge.svg)\n![Downloads](https://pepy.tech/badge/flwr)\n[![Slack](https://img.shields.io/badge/Chat-Slack-red)](https://flower.dev/join-slack)\n\nFlower (`flwr`) is a framework for building federated learning systems. The\ndesign of Flower is based on a few guiding principles:\n\n* **Customizable**: Federated learning systems vary wildly from one use case to\n  another. Flower allows for a wide range of different configurations depending\n  on the needs of each individual use case.\n\n* **Extendable**: Flower originated from a research project at the University of\n  Oxford, so it was built with AI research in mind. Many components can be\n  extended and overridden to build new state-of-the-art systems.\n\n* **Framework-agnostic**: Different machine learning frameworks have different\n  strengths. Flower can be used with any machine learning framework, for\n  example, [PyTorch](https://pytorch.org),\n  [TensorFlow](https://tensorflow.org), [Hugging Face Transformers](https://huggingface.co/), [PyTorch Lightning](https://pytorchlightning.ai/), [MXNet](https://mxnet.apache.org/), [scikit-learn](https://scikit-learn.org/), [JAX](https://jax.readthedocs.io/), [TFLite](https://tensorflow.org/lite/), [fastai](https://www.fast.ai/), [Pandas](https://pandas.pydata.org/\n) for federated analytics, or even raw [NumPy](https://numpy.org/)\n  for users who enjoy computing gradients by hand.\n\n* **Understandable**: Flower is written with maintainability in mind. The\n  community is encouraged to both read and contribute to the codebase.\n\nMeet the Flower community on [flower.dev](https://flower.dev)!\n\n## Federated Learning Tutorial\n\nFlower\'s goal is to make federated learning accessible to everyone. This series of tutorials introduces the fundamentals of federated learning and how to implement them in Flower.\n\n0. **What is Federated Learning?**\n\n   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-0-What-is-FL.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-0-What-is-FL.ipynb))\n\n1. **An Introduction to Federated Learning**\n\n   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-1-Intro-to-FL-PyTorch.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-1-Intro-to-FL-PyTorch.ipynb))\n\n2. **Using Strategies in Federated Learning**\n\n   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-2-Strategies-in-FL-PyTorch.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-2-Strategies-in-FL-PyTorch.ipynb))\n   \n3. **Building Strategies for Federated Learning**\n\n   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-3-Building-a-Strategy-PyTorch.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-3-Building-a-Strategy-PyTorch.ipynb))\n   \n4. **Custom Clients for Federated Learning**\n\n   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-4-Client-and-NumPyClient-PyTorch.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-4-Client-and-NumPyClient-PyTorch.ipynb))\n\nStay tuned, more tutorials are coming soon. Topics include **Privacy and Security in Federated Learning**, and **Scaling Federated Learning**.\n\n## Documentation\n\n[Flower Docs](https://flower.dev/docs):\n* [Installation](https://flower.dev/docs/installation.html)\n* [Quickstart (TensorFlow)](https://flower.dev/docs/quickstart-tensorflow.html)\n* [Quickstart (PyTorch)](https://flower.dev/docs/quickstart-pytorch.html)\n* [Quickstart (Hugging Face [code example])](https://flower.dev/docs/quickstart-huggingface.html)\n* [Quickstart (PyTorch Lightning [code example])](https://flower.dev/docs/quickstart-pytorch-lightning.html)\n* [Quickstart (MXNet)](https://flower.dev/docs/example-mxnet-walk-through.html)\n* [Quickstart (Pandas)](https://flower.dev/docs/quickstart-pandas.html)\n* [Quickstart (fastai)](https://flower.dev/docs/quickstart-fastai.html)\n* [Quickstart (JAX)](https://github.com/adap/flower/tree/main/examples/quickstart_jax)\n* [Quickstart (scikit-learn)](https://github.com/adap/flower/tree/main/examples/sklearn-logreg-mnist)\n* [Quickstart (TFLite on Android [code example])](https://github.com/adap/flower/tree/main/examples/android)\n\n## Flower Baselines\n\nFlower Baselines is a collection of community-contributed experiments that reproduce the experiments performed in popular federated learning publications. Researchers can build on Flower Baselines to quickly evaluate new ideas:\n\n* [FedAvg](https://arxiv.org/abs/1602.05629):\n  * [MNIST](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/fedavg_mnist)\n* [FedProx](https://arxiv.org/abs/1812.06127):\n  * [MNIST](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/fedprox_mnist)\n* [FedBN: Federated Learning on non-IID Features via Local Batch Normalization](https://arxiv.org/abs/2102.07623):\n  * [Convergence Rate](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/fedbn/convergence_rate)\n* [Adaptive Federated Optimization](https://arxiv.org/abs/2003.00295):\n  * [CIFAR-10/100](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/adaptive_federated_optimization)\n\nCheck the Flower documentation to learn more: [Using Baselines](https://flower.dev/docs/using-baselines.html)\n\nThe Flower community loves contributions! Make your work more visible and enable others to build on it by contributing it as a baseline: [Contributing Baselines](https://flower.dev/docs/contributing-baselines.html)\n\n## Flower Usage Examples\n\nSeveral code examples show different usage scenarios of Flower (in combination with popular machine learning frameworks such as PyTorch or TensorFlow).\n\nQuickstart examples:\n\n* [Quickstart (TensorFlow)](https://github.com/adap/flower/tree/main/examples/quickstart_tensorflow)\n* [Quickstart (PyTorch)](https://github.com/adap/flower/tree/main/examples/quickstart_pytorch)\n* [Quickstart (Hugging Face)](https://github.com/adap/flower/tree/main/examples/quickstart_huggingface)\n* [Quickstart (PyTorch Lightning)](https://github.com/adap/flower/tree/main/examples/quickstart_pytorch_lightning)\n* [Quickstart (fastai)](https://github.com/adap/flower/tree/main/examples/quickstart_fastai)\n* [Quickstart (Pandas)](https://github.com/adap/flower/tree/main/examples/quickstart_pandas)\n* [Quickstart (MXNet)](https://github.com/adap/flower/tree/main/examples/quickstart_mxnet)\n* [Quickstart (JAX)](https://github.com/adap/flower/tree/main/examples/quickstart_jax)\n* [Quickstart (scikit-learn)](https://github.com/adap/flower/tree/main/examples/sklearn-logreg-mnist)\n* [Quickstart (TFLite on Android)](https://github.com/adap/flower/tree/main/examples/android)\n\nOther [examples](https://github.com/adap/flower/tree/main/examples):\n\n* [Raspberry Pi & Nvidia Jetson Tutorial](https://github.com/adap/flower/tree/main/examples/embedded_devices)\n* [Android & TFLite](https://github.com/adap/flower/tree/main/examples/android)\n* [PyTorch: From Centralized to Federated](https://github.com/adap/flower/tree/main/examples/pytorch_from_centralized_to_federated)\n* [MXNet: From Centralized to Federated](https://github.com/adap/flower/tree/main/examples/mxnet_from_centralized_to_federated)\n* [Advanced Flower with TensorFlow/Keras](https://github.com/adap/flower/tree/main/examples/advanced_tensorflow)\n* [Advanced Flower with PyTorch](https://github.com/adap/flower/tree/main/examples/advanced_pytorch)\n* Single-Machine Simulation of Federated Learning Systems ([PyTorch](https://github.com/adap/flower/tree/main/examples/simulation_pytorch)) ([Tensorflow](https://github.com/adap/flower/tree/main/examples/simulation_tensorflow))\n\n## Community\n\nFlower is built by a wonderful community of researchers and engineers. [Join Slack](https://flower.dev/join-slack) to meet them, [contributions](#contributing-to-flower) are welcome.\n\n<a href="https://github.com/adap/flower/graphs/contributors">\n  <img src="https://contrib.rocks/image?repo=adap/flower" />\n</a>\n\n## Citation\n\nIf you publish work that uses Flower, please cite Flower as follows: \n\n```bibtex\n@article{beutel2020flower,\n  title={Flower: A Friendly Federated Learning Research Framework},\n  author={Beutel, Daniel J and Topal, Taner and Mathur, Akhil and Qiu, Xinchi and Fernandez-Marques, Javier and Gao, Yan and Sani, Lorenzo and Kwing, Hei Li and Parcollet, Titouan and Gusmão, Pedro PB de and Lane, Nicholas D}, \n  journal={arXiv preprint arXiv:2007.14390},\n  year={2020}\n}\n```\n\nPlease also consider adding your publication to the list of Flower-based publications in the docs, just open a Pull Request.\n\n## Contributing to Flower\n\nWe welcome contributions. Please see [CONTRIBUTING.md](CONTRIBUTING.md) to get started!\n',
     'author': 'The Flower Authors',
     'author_email': 'hello@flower.dev',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://flower.dev',
     'package_dir': package_dir,
     'packages': packages,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,24 +1,26 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'': 'src/
 py'} packages = \ ['flwr', 'flwr.client', 'flwr.client.grpc_client',
-'flwr.client.message_handler', 'flwr.common', 'flwr.driver', 'flwr.proto',
-'flwr.server', 'flwr.server.driver', 'flwr.server.fleet',
-'flwr.server.grpc_server', 'flwr.server.state', 'flwr.server.strategy',
-'flwr.server.utils', 'flwr.simulation', 'flwr.simulation.ray_transport']
-package_data = \ {'': ['*']} install_requires = \
-['grpcio>=1.43.0,<2.0.0,!=1.52.0', 'iterators>=0.0.2,<0.0.3',
-'numpy>=1.21.0,<2.0.0', 'protobuf>=3.19.0,<4.0.0'] extras_require = \ {':extra
-== "rest"': ['requests>=2.28.1,<3.0.0', 'fastapi>=0.89.1,<0.90.0', 'uvicorn
-[standard]>=0.20.0,<0.21.0'], ':python_version < "3.8"': ['importlib-
-metadata>=4.0.0,<5.0.0'], 'simulation': ['ray[default]>=2.2.0,<2.3.0']}
+'flwr.client.message_handler', 'flwr.client.rest_client', 'flwr.common',
+'flwr.driver', 'flwr.proto', 'flwr.server', 'flwr.server.driver',
+'flwr.server.fleet', 'flwr.server.grpc_server', 'flwr.server.rest_server',
+'flwr.server.state', 'flwr.server.strategy', 'flwr.server.utils',
+'flwr.simulation', 'flwr.simulation.ray_transport'] package_data = \ {'':
+['*']} install_requires = \ ['grpcio>=1.48.2,<2.0.0,!=1.52.0',
+'iterators>=0.0.2,<0.0.3', 'numpy>=1.21.0,<2.0.0', 'protobuf>=3.19.0,<4.0.0']
+extras_require = \ {':python_version < "3.8"': ['importlib-
+metadata>=4.0.0,<5.0.0'], 'rest': ['requests>=2.28.2,<3.0.0',
+'fastapi>=0.95.0,<0.96.0', 'starlette>=0.26.1,<0.27.0', 'uvicorn
+[standard]>=0.21.1,<0.22.0'], 'simulation': ['ray[default]>=2.3.0,<3.0.0']}
 entry_points = \ {'console_scripts': ['flower-client = flwr.client:run_client',
-'flower-server = flwr.server:run_server']} setup_kwargs = { 'name': 'flwr',
-'version': '1.3.0', 'description': 'Flower: A Friendly Federated Learning
-Framework', 'long_description': '# Flower: A Friendly Federated Learning
-Framework\n\n
+'flower-driver-api = flwr.server:run_driver_api', 'flower-fleet-api =
+flwr.server:run_fleet_api', 'flower-server = flwr.server:run_server']}
+setup_kwargs = { 'name': 'flwr', 'version': '1.4.0', 'description': 'Flower: A
+Friendly Federated Learning Framework', 'long_description': '# Flower: A
+Friendly Federated Learning Framework\n\n
                           \n \n_[Flower_Website]\n\n
 \n
            \n Website |\n Blog |\n Docs |\n Conference |\n Slack\n
 
                                       \n
 \n\n[![GitHub license](https://img.shields.io/github/license/adap/flower)]
 (https://github.com/adap/flower/blob/main/LICENSE)\n[![PRs Welcome](https://
@@ -44,67 +46,74 @@
 //pandas.pydata.org/\n) for federated analytics, or even raw [NumPy](https://
 numpy.org/)\n for users who enjoy computing gradients by hand.\n\n*
 **Understandable**: Flower is written with maintainability in mind. The\n
 community is encouraged to both read and contribute to the codebase.\n\nMeet
 the Flower community on [flower.dev](https://flower.dev)!\n\n## Federated
 Learning Tutorial\n\nFlower\'s goal is to make federated learning accessible to
 everyone. This series of tutorials introduces the fundamentals of federated
-learning and how to implement them in Flower.\n\n1. **An Introduction to
-Federated Learning**\n\n [![Open in Colab](https://colab.research.google.com/
-assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/
-blob/main/doc/source/tutorial/Flower-1-Intro-to-FL-PyTorch.ipynb) (or open the
-[Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/
-tutorial/Flower-1-Intro-to-FL-PyTorch.ipynb))\n\n2. **Using Strategies in
-Federated Learning**\n\n [![Open in Colab](https://colab.research.google.com/
-assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/
-blob/main/doc/source/tutorial/Flower-2-Strategies-in-FL-PyTorch.ipynb) (or open
+learning and how to implement them in Flower.\n\n0. **What is Federated
+Learning?**\n\n [![Open in Colab](https://colab.research.google.com/assets/
+colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/
+main/doc/source/tutorial/Flower-0-What-is-FL.ipynb) (or open the [Jupyter
+Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-
+0-What-is-FL.ipynb))\n\n1. **An Introduction to Federated Learning**\n\n [!
+[Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)]
+(https://colab.research.google.com/github/adap/flower/blob/main/doc/source/
+tutorial/Flower-1-Intro-to-FL-PyTorch.ipynb) (or open the [Jupyter Notebook]
+(https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-1-Intro-
+to-FL-PyTorch.ipynb))\n\n2. **Using Strategies in Federated Learning**\n\n [!
+[Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)]
+(https://colab.research.google.com/github/adap/flower/blob/main/doc/source/
+tutorial/Flower-2-Strategies-in-FL-PyTorch.ipynb) (or open the [Jupyter
+Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-
+2-Strategies-in-FL-PyTorch.ipynb))\n \n3. **Building Strategies for Federated
+Learning**\n\n [![Open in Colab](https://colab.research.google.com/assets/
+colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/
+main/doc/source/tutorial/Flower-3-Building-a-Strategy-PyTorch.ipynb) (or open
 the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/
-tutorial/Flower-2-Strategies-in-FL-PyTorch.ipynb))\n \n3. **Building Strategies
+tutorial/Flower-3-Building-a-Strategy-PyTorch.ipynb))\n \n4. **Custom Clients
 for Federated Learning**\n\n [![Open in Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/
-Flower-3-Building-a-Strategy-PyTorch.ipynb) (or open the [Jupyter Notebook]
-(https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-3-
-Building-a-Strategy-PyTorch.ipynb))\n \n4. **Custom Clients for Federated
-Learning**\n\n [![Open in Colab](https://colab.research.google.com/assets/
-colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/
-main/doc/source/tutorial/Flower-4-Client-and-NumPyClient-PyTorch.ipynb) (or
-open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/
-source/tutorial/Flower-4-Client-and-NumPyClient-PyTorch.ipynb))\n\nStay tuned,
-more tutorials are coming soon. Topics include **Privacy and Security in
-Federated Learning**, and **Scaling Federated Learning**.\n\n##
-Documentation\n\n[Flower Docs](https://flower.dev/docs):\n* [Installation]
-(https://flower.dev/docs/installation.html)\n* [Quickstart (TensorFlow)](https:
-//flower.dev/docs/quickstart-tensorflow.html)\n* [Quickstart (PyTorch)](https:/
-/flower.dev/docs/quickstart-pytorch.html)\n* [Quickstart (Hugging Face [code
-example])](https://flower.dev/docs/quickstart-huggingface.html)\n* [Quickstart
-(PyTorch Lightning [code example])](https://flower.dev/docs/quickstart-pytorch-
-lightning.html)\n* [Quickstart (MXNet)](https://flower.dev/docs/example-mxnet-
-walk-through.html)\n* [Quickstart (Pandas)](https://flower.dev/docs/quickstart-
+Flower-4-Client-and-NumPyClient-PyTorch.ipynb) (or open the [Jupyter Notebook]
+(https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-4-Client-
+and-NumPyClient-PyTorch.ipynb))\n\nStay tuned, more tutorials are coming soon.
+Topics include **Privacy and Security in Federated Learning**, and **Scaling
+Federated Learning**.\n\n## Documentation\n\n[Flower Docs](https://flower.dev/
+docs):\n* [Installation](https://flower.dev/docs/installation.html)\n*
+[Quickstart (TensorFlow)](https://flower.dev/docs/quickstart-
+tensorflow.html)\n* [Quickstart (PyTorch)](https://flower.dev/docs/quickstart-
+pytorch.html)\n* [Quickstart (Hugging Face [code example])](https://flower.dev/
+docs/quickstart-huggingface.html)\n* [Quickstart (PyTorch Lightning [code
+example])](https://flower.dev/docs/quickstart-pytorch-lightning.html)\n*
+[Quickstart (MXNet)](https://flower.dev/docs/example-mxnet-walk-
+through.html)\n* [Quickstart (Pandas)](https://flower.dev/docs/quickstart-
 pandas.html)\n* [Quickstart (fastai)](https://flower.dev/docs/quickstart-
 fastai.html)\n* [Quickstart (JAX)](https://github.com/adap/flower/tree/main/
 examples/quickstart_jax)\n* [Quickstart (scikit-learn)](https://github.com/
 adap/flower/tree/main/examples/sklearn-logreg-mnist)\n* [Quickstart (TFLite on
 Android [code example])](https://github.com/adap/flower/tree/main/examples/
 android)\n\n## Flower Baselines\n\nFlower Baselines is a collection of
 community-contributed experiments that reproduce the experiments performed in
 popular federated learning publications. Researchers can build on Flower
-Baselines to quickly evaluate new ideas:\n\n* [FedAvg](https://arxiv.org/pdf/
-1602.05629.pdf):\n * [MNIST](https://github.com/adap/flower/tree/main/
-baselines/flwr_baselines/publications/fedavg_mnist)\n* [FedBN: Federated
-Learning on non-IID Features via Local Batch Normalization](https://arxiv.org/
-pdf/2102.07623.pdf):\n * [Convergence Rate](https://github.com/adap/flower/
-tree/main/baselines/flwr_baselines/publications/fedbn/convergence_rate)\n*
-[Adaptive Federated Optimization](https://arxiv.org/pdf/2003.00295.pdf):\n *
-[CIFAR-10/100](https://github.com/adap/flower/tree/main/baselines/
-flwr_baselines/publications/adaptive_federated_optimization)\n\nCheck the
-Flower documentation to learn more: [Using Baselines](https://flower.dev/docs/
-using-baselines.html)\n\nThe Flower community loves contributions! Make your
-work more visible and enable others to build on it by contributing it as a
-baseline: [Contributing Baselines](https://flower.dev/docs/contributing-
+Baselines to quickly evaluate new ideas:\n\n* [FedAvg](https://arxiv.org/abs/
+1602.05629):\n * [MNIST](https://github.com/adap/flower/tree/main/baselines/
+flwr_baselines/publications/fedavg_mnist)\n* [FedProx](https://arxiv.org/abs/
+1812.06127):\n * [MNIST](https://github.com/adap/flower/tree/main/baselines/
+flwr_baselines/publications/fedprox_mnist)\n* [FedBN: Federated Learning on
+non-IID Features via Local Batch Normalization](https://arxiv.org/abs/
+2102.07623):\n * [Convergence Rate](https://github.com/adap/flower/tree/main/
+baselines/flwr_baselines/publications/fedbn/convergence_rate)\n* [Adaptive
+Federated Optimization](https://arxiv.org/abs/2003.00295):\n * [CIFAR-10/100]
+(https://github.com/adap/flower/tree/main/baselines/flwr_baselines/
+publications/adaptive_federated_optimization)\n\nCheck the Flower documentation
+to learn more: [Using Baselines](https://flower.dev/docs/using-
+baselines.html)\n\nThe Flower community loves contributions! Make your work
+more visible and enable others to build on it by contributing it as a baseline:
+[Contributing Baselines](https://flower.dev/docs/contributing-
 baselines.html)\n\n## Flower Usage Examples\n\nSeveral code examples show
 different usage scenarios of Flower (in combination with popular machine
 learning frameworks such as PyTorch or TensorFlow).\n\nQuickstart examples:
 \n\n* [Quickstart (TensorFlow)](https://github.com/adap/flower/tree/main/
 examples/quickstart_tensorflow)\n* [Quickstart (PyTorch)](https://github.com/
 adap/flower/tree/main/examples/quickstart_pytorch)\n* [Quickstart (Hugging
 Face)](https://github.com/adap/flower/tree/main/examples/
@@ -133,19 +142,20 @@
 tree/main/examples/simulation_tensorflow))\n\n## Community\n\nFlower is built
 by a wonderful community of researchers and engineers. [Join Slack](https://
 flower.dev/join-slack) to meet them, [contributions](#contributing-to-flower)
 are welcome.\n\n\n_[https://contrib.rocks/image?repo=adap/flower]\n\n\n##
 Citation\n\nIf you publish work that uses Flower, please cite Flower as
 follows: \n\n```bibtex\n@article{beutel2020flower,\n title={Flower: A Friendly
 Federated Learning Research Framework},\n author={Beutel, Daniel J and Topal,
-Taner and Mathur, Akhil and Qiu, Xinchi and Parcollet, Titouan and Lane,
-Nicholas D},\n journal={arXiv preprint arXiv:2007.14390},\n year=
-{2020}\n}\n```\n\nPlease also consider adding your publication to the list of
-Flower-based publications in the docs, just open a Pull Request.\n\n##
-Contributing to Flower\n\nWe welcome contributions. Please see
-[CONTRIBUTING.md](CONTRIBUTING.md) to get started!\n', 'author': 'The Flower
-Authors', 'author_email': 'hello@flower.dev', 'maintainer': 'None',
+Taner and Mathur, Akhil and Qiu, Xinchi and Fernandez-Marques, Javier and Gao,
+Yan and Sani, Lorenzo and Kwing, Hei Li and Parcollet, Titouan and GusmÃ£o,
+Pedro PB de and Lane, Nicholas D}, \n journal={arXiv preprint arXiv:
+2007.14390},\n year={2020}\n}\n```\n\nPlease also consider adding your
+publication to the list of Flower-based publications in the docs, just open a
+Pull Request.\n\n## Contributing to Flower\n\nWe welcome contributions. Please
+see [CONTRIBUTING.md](CONTRIBUTING.md) to get started!\n', 'author': 'The
+Flower Authors', 'author_email': 'hello@flower.dev', 'maintainer': 'None',
 'maintainer_email': 'None', 'url': 'https://flower.dev', 'package_dir':
 package_dir, 'packages': packages, 'package_data': package_data,
 'install_requires': install_requires, 'extras_require': extras_require,
 'entry_points': entry_points, 'python_requires': '>=3.7,<4.0', } setup
 (**setup_kwargs)
```

### Comparing `flwr-1.3.0/PKG-INFO` & `flwr-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flwr
-Version: 1.3.0
+Version: 1.4.0
 Summary: Flower: A Friendly Federated Learning Framework
 Home-page: https://flower.dev
 License: Apache-2.0
 Author: The Flower Authors
 Author-email: hello@flower.dev
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -33,23 +33,24 @@
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Provides-Extra: rest
 Provides-Extra: simulation
-Requires-Dist: fastapi (>=0.89.1,<0.90.0) ; extra == "rest"
-Requires-Dist: grpcio (>=1.43.0,<2.0.0,!=1.52.0)
+Requires-Dist: fastapi (>=0.95.0,<0.96.0) ; extra == "rest"
+Requires-Dist: grpcio (>=1.48.2,<2.0.0,!=1.52.0)
 Requires-Dist: importlib-metadata (>=4.0.0,<5.0.0) ; python_version < "3.8"
 Requires-Dist: iterators (>=0.0.2,<0.0.3)
 Requires-Dist: numpy (>=1.21.0,<2.0.0)
 Requires-Dist: protobuf (>=3.19.0,<4.0.0)
-Requires-Dist: ray[default] (>=2.2.0,<2.3.0) ; extra == "simulation"
-Requires-Dist: requests (>=2.28.1,<3.0.0) ; extra == "rest"
-Requires-Dist: uvicorn[standard] (>=0.20.0,<0.21.0) ; extra == "rest"
+Requires-Dist: ray[default] (>=2.3.0,<3.0.0) ; extra == "simulation"
+Requires-Dist: requests (>=2.28.2,<3.0.0) ; extra == "rest"
+Requires-Dist: starlette (>=0.26.1,<0.27.0) ; extra == "rest"
+Requires-Dist: uvicorn[standard] (>=0.21.1,<0.22.0) ; extra == "rest"
 Project-URL: Documentation, https://flower.dev
 Project-URL: Repository, https://github.com/adap/flower
 Description-Content-Type: text/markdown
 
 # Flower: A Friendly Federated Learning Framework
 
 <p align="center">
@@ -95,14 +96,18 @@
 
 Meet the Flower community on [flower.dev](https://flower.dev)!
 
 ## Federated Learning Tutorial
 
 Flower's goal is to make federated learning accessible to everyone. This series of tutorials introduces the fundamentals of federated learning and how to implement them in Flower.
 
+0. **What is Federated Learning?**
+
+   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-0-What-is-FL.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-0-What-is-FL.ipynb))
+
 1. **An Introduction to Federated Learning**
 
    [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-1-Intro-to-FL-PyTorch.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-1-Intro-to-FL-PyTorch.ipynb))
 
 2. **Using Strategies in Federated Learning**
 
    [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-2-Strategies-in-FL-PyTorch.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-2-Strategies-in-FL-PyTorch.ipynb))
@@ -132,19 +137,21 @@
 * [Quickstart (scikit-learn)](https://github.com/adap/flower/tree/main/examples/sklearn-logreg-mnist)
 * [Quickstart (TFLite on Android [code example])](https://github.com/adap/flower/tree/main/examples/android)
 
 ## Flower Baselines
 
 Flower Baselines is a collection of community-contributed experiments that reproduce the experiments performed in popular federated learning publications. Researchers can build on Flower Baselines to quickly evaluate new ideas:
 
-* [FedAvg](https://arxiv.org/pdf/1602.05629.pdf):
+* [FedAvg](https://arxiv.org/abs/1602.05629):
   * [MNIST](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/fedavg_mnist)
-* [FedBN: Federated Learning on non-IID Features via Local Batch Normalization](https://arxiv.org/pdf/2102.07623.pdf):
+* [FedProx](https://arxiv.org/abs/1812.06127):
+  * [MNIST](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/fedprox_mnist)
+* [FedBN: Federated Learning on non-IID Features via Local Batch Normalization](https://arxiv.org/abs/2102.07623):
   * [Convergence Rate](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/fedbn/convergence_rate)
-* [Adaptive Federated Optimization](https://arxiv.org/pdf/2003.00295.pdf):
+* [Adaptive Federated Optimization](https://arxiv.org/abs/2003.00295):
   * [CIFAR-10/100](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/adaptive_federated_optimization)
 
 Check the Flower documentation to learn more: [Using Baselines](https://flower.dev/docs/using-baselines.html)
 
 The Flower community loves contributions! Make your work more visible and enable others to build on it by contributing it as a baseline: [Contributing Baselines](https://flower.dev/docs/contributing-baselines.html)
 
 ## Flower Usage Examples
@@ -185,15 +192,15 @@
 ## Citation
 
 If you publish work that uses Flower, please cite Flower as follows: 
 
 ```bibtex
 @article{beutel2020flower,
   title={Flower: A Friendly Federated Learning Research Framework},
-  author={Beutel, Daniel J and Topal, Taner and Mathur, Akhil and Qiu, Xinchi and Parcollet, Titouan and Lane, Nicholas D},
+  author={Beutel, Daniel J and Topal, Taner and Mathur, Akhil and Qiu, Xinchi and Fernandez-Marques, Javier and Gao, Yan and Sani, Lorenzo and Kwing, Hei Li and Parcollet, Titouan and Gusmão, Pedro PB de and Lane, Nicholas D}, 
   journal={arXiv preprint arXiv:2007.14390},
   year={2020}
 }
 ```
 
 Please also consider adding your publication to the list of Flower-based publications in the docs, just open a Pull Request.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flwr Version: 1.3.0 Summary: Flower: A Friendly
+Metadata-Version: 2.1 Name: flwr Version: 1.4.0 Summary: Flower: A Friendly
 Federated Learning Framework Home-page: https://flower.dev License: Apache-2.0
 Author: The Flower Authors Author-email: hello@flower.dev Requires-Python:
 >=3.7,<4.0 Classifier: Development Status :: 5 - Production/Stable Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: Science/
 Research Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: POSIX :: Linux Classifier: Programming Language :: Python Classifier:
@@ -17,24 +17,25 @@
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: Implementation :: CPython Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Mathematics Classifier: Topic ::
 Software Development Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed Provides-Extra: rest Provides-Extra: simulation
-Requires-Dist: fastapi (>=0.89.1,<0.90.0) ; extra == "rest" Requires-Dist:
-grpcio (>=1.43.0,<2.0.0,!=1.52.0) Requires-Dist: importlib-metadata
+Requires-Dist: fastapi (>=0.95.0,<0.96.0) ; extra == "rest" Requires-Dist:
+grpcio (>=1.48.2,<2.0.0,!=1.52.0) Requires-Dist: importlib-metadata
 (>=4.0.0,<5.0.0) ; python_version < "3.8" Requires-Dist: iterators
 (>=0.0.2,<0.0.3) Requires-Dist: numpy (>=1.21.0,<2.0.0) Requires-Dist: protobuf
-(>=3.19.0,<4.0.0) Requires-Dist: ray[default] (>=2.2.0,<2.3.0) ; extra ==
-"simulation" Requires-Dist: requests (>=2.28.1,<3.0.0) ; extra == "rest"
-Requires-Dist: uvicorn[standard] (>=0.20.0,<0.21.0) ; extra == "rest" Project-
-URL: Documentation, https://flower.dev Project-URL: Repository, https://
-github.com/adap/flower Description-Content-Type: text/markdown # Flower: A
-Friendly Federated Learning Framework
+(>=3.19.0,<4.0.0) Requires-Dist: ray[default] (>=2.3.0,<3.0.0) ; extra ==
+"simulation" Requires-Dist: requests (>=2.28.2,<3.0.0) ; extra == "rest"
+Requires-Dist: starlette (>=0.26.1,<0.27.0) ; extra == "rest" Requires-Dist:
+uvicorn[standard] (>=0.21.1,<0.22.0) ; extra == "rest" Project-URL:
+Documentation, https://flower.dev Project-URL: Repository, https://github.com/
+adap/flower Description-Content-Type: text/markdown # Flower: A Friendly
+Federated Learning Framework
                                [Flower_Website]
                   Website | Blog | Docs | Conference | Slack
 
 [![GitHub license](https://img.shields.io/github/license/adap/flower)](https://
 github.com/adap/flower/blob/main/LICENSE) [![PRs Welcome](https://
 img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/adap/
 flower/blob/main/CONTRIBUTING.md) ![Build](https://github.com/adap/flower/
@@ -57,22 +58,27 @@
 www.fast.ai/), [Pandas](https://pandas.pydata.org/ ) for federated analytics,
 or even raw [NumPy](https://numpy.org/) for users who enjoy computing gradients
 by hand. * **Understandable**: Flower is written with maintainability in mind.
 The community is encouraged to both read and contribute to the codebase. Meet
 the Flower community on [flower.dev](https://flower.dev)! ## Federated Learning
 Tutorial Flower's goal is to make federated learning accessible to everyone.
 This series of tutorials introduces the fundamentals of federated learning and
-how to implement them in Flower. 1. **An Introduction to Federated Learning**
-[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)]
-(https://colab.research.google.com/github/adap/flower/blob/main/doc/source/
-tutorial/Flower-1-Intro-to-FL-PyTorch.ipynb) (or open the [Jupyter Notebook]
-(https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-1-Intro-
-to-FL-PyTorch.ipynb)) 2. **Using Strategies in Federated Learning** [![Open in
+how to implement them in Flower. 0. **What is Federated Learning?** [![Open in
 Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/
+Flower-0-What-is-FL.ipynb) (or open the [Jupyter Notebook](https://github.com/
+adap/flower/blob/main/doc/source/tutorial/Flower-0-What-is-FL.ipynb)) 1. **An
+Introduction to Federated Learning** [![Open in Colab](https://
+colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/
+Flower-1-Intro-to-FL-PyTorch.ipynb) (or open the [Jupyter Notebook](https://
+github.com/adap/flower/blob/main/doc/source/tutorial/Flower-1-Intro-to-FL-
+PyTorch.ipynb)) 2. **Using Strategies in Federated Learning** [![Open in Colab]
+(https://colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/
 Flower-2-Strategies-in-FL-PyTorch.ipynb) (or open the [Jupyter Notebook](https:
 //github.com/adap/flower/blob/main/doc/source/tutorial/Flower-2-Strategies-in-
 FL-PyTorch.ipynb)) 3. **Building Strategies for Federated Learning** [![Open in
 Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/
 Flower-3-Building-a-Strategy-PyTorch.ipynb) (or open the [Jupyter Notebook]
 (https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-3-
@@ -96,47 +102,49 @@
 [Quickstart (JAX)](https://github.com/adap/flower/tree/main/examples/
 quickstart_jax) * [Quickstart (scikit-learn)](https://github.com/adap/flower/
 tree/main/examples/sklearn-logreg-mnist) * [Quickstart (TFLite on Android [code
 example])](https://github.com/adap/flower/tree/main/examples/android) ## Flower
 Baselines Flower Baselines is a collection of community-contributed experiments
 that reproduce the experiments performed in popular federated learning
 publications. Researchers can build on Flower Baselines to quickly evaluate new
-ideas: * [FedAvg](https://arxiv.org/pdf/1602.05629.pdf): * [MNIST](https://
+ideas: * [FedAvg](https://arxiv.org/abs/1602.05629): * [MNIST](https://
 github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/
-fedavg_mnist) * [FedBN: Federated Learning on non-IID Features via Local Batch
-Normalization](https://arxiv.org/pdf/2102.07623.pdf): * [Convergence Rate]
-(https://github.com/adap/flower/tree/main/baselines/flwr_baselines/
-publications/fedbn/convergence_rate) * [Adaptive Federated Optimization](https:
-//arxiv.org/pdf/2003.00295.pdf): * [CIFAR-10/100](https://github.com/adap/
-flower/tree/main/baselines/flwr_baselines/publications/
-adaptive_federated_optimization) Check the Flower documentation to learn more:
-[Using Baselines](https://flower.dev/docs/using-baselines.html) The Flower
-community loves contributions! Make your work more visible and enable others to
-build on it by contributing it as a baseline: [Contributing Baselines](https://
-flower.dev/docs/contributing-baselines.html) ## Flower Usage Examples Several
-code examples show different usage scenarios of Flower (in combination with
-popular machine learning frameworks such as PyTorch or TensorFlow). Quickstart
-examples: * [Quickstart (TensorFlow)](https://github.com/adap/flower/tree/main/
-examples/quickstart_tensorflow) * [Quickstart (PyTorch)](https://github.com/
-adap/flower/tree/main/examples/quickstart_pytorch) * [Quickstart (Hugging
-Face)](https://github.com/adap/flower/tree/main/examples/
-quickstart_huggingface) * [Quickstart (PyTorch Lightning)](https://github.com/
-adap/flower/tree/main/examples/quickstart_pytorch_lightning) * [Quickstart
-(fastai)](https://github.com/adap/flower/tree/main/examples/quickstart_fastai)
-* [Quickstart (Pandas)](https://github.com/adap/flower/tree/main/examples/
-quickstart_pandas) * [Quickstart (MXNet)](https://github.com/adap/flower/tree/
-main/examples/quickstart_mxnet) * [Quickstart (JAX)](https://github.com/adap/
-flower/tree/main/examples/quickstart_jax) * [Quickstart (scikit-learn)](https:/
-/github.com/adap/flower/tree/main/examples/sklearn-logreg-mnist) * [Quickstart
-(TFLite on Android)](https://github.com/adap/flower/tree/main/examples/android)
-Other [examples](https://github.com/adap/flower/tree/main/examples): *
-[Raspberry Pi & Nvidia Jetson Tutorial](https://github.com/adap/flower/tree/
-main/examples/embedded_devices) * [Android & TFLite](https://github.com/adap/
-flower/tree/main/examples/android) * [PyTorch: From Centralized to Federated]
-(https://github.com/adap/flower/tree/main/examples/
+fedavg_mnist) * [FedProx](https://arxiv.org/abs/1812.06127): * [MNIST](https://
+github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/
+fedprox_mnist) * [FedBN: Federated Learning on non-IID Features via Local Batch
+Normalization](https://arxiv.org/abs/2102.07623): * [Convergence Rate](https://
+github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/fedbn/
+convergence_rate) * [Adaptive Federated Optimization](https://arxiv.org/abs/
+2003.00295): * [CIFAR-10/100](https://github.com/adap/flower/tree/main/
+baselines/flwr_baselines/publications/adaptive_federated_optimization) Check
+the Flower documentation to learn more: [Using Baselines](https://flower.dev/
+docs/using-baselines.html) The Flower community loves contributions! Make your
+work more visible and enable others to build on it by contributing it as a
+baseline: [Contributing Baselines](https://flower.dev/docs/contributing-
+baselines.html) ## Flower Usage Examples Several code examples show different
+usage scenarios of Flower (in combination with popular machine learning
+frameworks such as PyTorch or TensorFlow). Quickstart examples: * [Quickstart
+(TensorFlow)](https://github.com/adap/flower/tree/main/examples/
+quickstart_tensorflow) * [Quickstart (PyTorch)](https://github.com/adap/flower/
+tree/main/examples/quickstart_pytorch) * [Quickstart (Hugging Face)](https://
+github.com/adap/flower/tree/main/examples/quickstart_huggingface) * [Quickstart
+(PyTorch Lightning)](https://github.com/adap/flower/tree/main/examples/
+quickstart_pytorch_lightning) * [Quickstart (fastai)](https://github.com/adap/
+flower/tree/main/examples/quickstart_fastai) * [Quickstart (Pandas)](https://
+github.com/adap/flower/tree/main/examples/quickstart_pandas) * [Quickstart
+(MXNet)](https://github.com/adap/flower/tree/main/examples/quickstart_mxnet) *
+[Quickstart (JAX)](https://github.com/adap/flower/tree/main/examples/
+quickstart_jax) * [Quickstart (scikit-learn)](https://github.com/adap/flower/
+tree/main/examples/sklearn-logreg-mnist) * [Quickstart (TFLite on Android)]
+(https://github.com/adap/flower/tree/main/examples/android) Other [examples]
+(https://github.com/adap/flower/tree/main/examples): * [Raspberry Pi & Nvidia
+Jetson Tutorial](https://github.com/adap/flower/tree/main/examples/
+embedded_devices) * [Android & TFLite](https://github.com/adap/flower/tree/
+main/examples/android) * [PyTorch: From Centralized to Federated](https://
+github.com/adap/flower/tree/main/examples/
 pytorch_from_centralized_to_federated) * [MXNet: From Centralized to Federated]
 (https://github.com/adap/flower/tree/main/examples/
 mxnet_from_centralized_to_federated) * [Advanced Flower with TensorFlow/Keras]
 (https://github.com/adap/flower/tree/main/examples/advanced_tensorflow) *
 [Advanced Flower with PyTorch](https://github.com/adap/flower/tree/main/
 examples/advanced_pytorch) * Single-Machine Simulation of Federated Learning
 Systems ([PyTorch](https://github.com/adap/flower/tree/main/examples/
@@ -144,12 +152,14 @@
 examples/simulation_tensorflow)) ## Community Flower is built by a wonderful
 community of researchers and engineers. [Join Slack](https://flower.dev/join-
 slack) to meet them, [contributions](#contributing-to-flower) are welcome.
 [https://contrib.rocks/image?repo=adap/flower] ## Citation If you publish work
 that uses Flower, please cite Flower as follows: ```bibtex @article
 {beutel2020flower, title={Flower: A Friendly Federated Learning Research
 Framework}, author={Beutel, Daniel J and Topal, Taner and Mathur, Akhil and
-Qiu, Xinchi and Parcollet, Titouan and Lane, Nicholas D}, journal={arXiv
-preprint arXiv:2007.14390}, year={2020} } ``` Please also consider adding your
-publication to the list of Flower-based publications in the docs, just open a
-Pull Request. ## Contributing to Flower We welcome contributions. Please see
-[CONTRIBUTING.md](CONTRIBUTING.md) to get started!
+Qiu, Xinchi and Fernandez-Marques, Javier and Gao, Yan and Sani, Lorenzo and
+Kwing, Hei Li and Parcollet, Titouan and GusmÃ£o, Pedro PB de and Lane,
+Nicholas D}, journal={arXiv preprint arXiv:2007.14390}, year={2020} } ```
+Please also consider adding your publication to the list of Flower-based
+publications in the docs, just open a Pull Request. ## Contributing to Flower
+We welcome contributions. Please see [CONTRIBUTING.md](CONTRIBUTING.md) to get
+started!
```

