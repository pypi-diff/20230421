# Comparing `tmp/sphere_base-0.1.1.tar.gz` & `tmp/sphere_base-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphere_base-0.1.1.tar", last modified: Sun Apr 16 15:11:20 2023, max compression
+gzip compressed data, was "sphere_base-0.1.2.tar", last modified: Fri Apr 21 08:51:17 2023, max compression
```

## Comparing `sphere_base-0.1.1.tar` & `sphere_base-0.1.2.tar`

### file list

```diff
@@ -1,155 +1,176 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 15:11:20.799001 sphere_base-0.1.1/
--rw-rw-rw-   0        0        0      978 2023-04-16 07:19:30.000000 sphere_base-0.1.1/HISTORY.rst
--rw-rw-rw-   0        0        0     1105 2023-04-16 08:54:46.000000 sphere_base-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      252 2023-03-15 14:22:33.000000 sphere_base-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1968 2023-04-16 15:11:20.799001 sphere_base-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1074 2023-04-16 15:08:33.000000 sphere_base-0.1.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-16 15:11:20.578988 sphere_base-0.1.1/docs/
--rw-rw-rw-   0        0        0      638 2023-03-15 17:55:12.000000 sphere_base-0.1.1/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-04-16 15:11:20.542986 sphere_base-0.1.1/docs/build/
-drwxrwxrwx   0        0        0        0 2023-04-16 15:11:20.542986 sphere_base-0.1.1/docs/build/html/
-drwxrwxrwx   0        0        0        0 2023-04-16 15:11:20.583988 sphere_base-0.1.1/docs/build/html/_static/
--rw-rw-rw-   0        0        0      286 2023-03-15 17:53:40.000000 sphere_base-0.1.1/docs/build/html/_static/file.png
--rw-rw-rw-   0        0        0       90 2023-03-15 17:53:40.000000 sphere_base-0.1.1/docs/build/html/_static/minus.png
--rw-rw-rw-   0        0        0       90 2023-03-15 17:53:40.000000 sphere_base-0.1.1/docs/build/html/_static/plus.png
--rwxrwxrwx   0        0        0      804 2023-03-15 17:55:12.000000 sphere_base-0.1.1/docs/make.bat
-drwxrwxrwx   0        0        0        0 2023-04-16 15:11:20.586988 sphere_base-0.1.1/docs/source/
--rw-rw-rw-   0        0        0     1175 2023-03-16 20:29:33.000000 sphere_base-0.1.1/docs/source/conf.py
--rw-rw-rw-   0        0        0      489 2023-03-16 21:15:47.000000 sphere_base-0.1.1/docs/source/index.rst
-drwxrwxrwx   0        0        0        0 2023-04-16 15:11:20.688994 sphere_base-0.1.1/docs/source/rst/
--rw-rw-rw-   0        0        0      163 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.model.mesh.rst
--rw-rw-rw-   0        0        0      166 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.model.model.rst
--rw-rw-rw-   0        0        0      169 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.model.models.rst
--rw-rw-rw-   0        0        0      200 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.model.obj_file_loader.rst
--rw-rw-rw-   0        0        0      369 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.model.rst
--rw-rw-rw-   0        0        0      196 2023-03-16 21:18:48.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.rst
--rw-rw-rw-   0        0        0      780 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.shader.rst
--rw-rw-rw-   0        0        0      200 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.shader.uv_base_shader.rst
--rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.shader.uv_circle_shader.rst
--rw-rw-rw-   0        0        0      203 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.shader.uv_cross_shader.rst
--rw-rw-rw-   0        0        0      209 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.shader.uv_default_shader.rst
--rw-rw-rw-   0        0        0      200 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.shader.uv_flat_shader.rst
--rw-rw-rw-   0        0        0      223 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.shader.uv_holo_sphere_shader.rst
--rw-rw-rw-   0        0        0      200 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.shader.uv_node_shader.rst
--rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.shader.uv_skybox_shader.rst
--rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.shader.uv_socket_shader.rst
--rw-rw-rw-   0        0        0      223 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.shader.uv_sphere_edge_shader.rst
--rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.shader.uv_sphere_shader.rst
--rw-rw-rw-   0        0        0      226 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.shader.uv_sphere_small_shader.rst
--rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.shader.uv_square_shader.rst
--rw-rw-rw-   0        0        0      602 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_overlay.rst
--rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_overlay.sov_conf.rst
--rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_overlay.sov_edge.rst
--rw-rw-rw-   0        0        0      212 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_overlay.sov_sphere.rst
--rw-rw-rw-   0        0        0      246 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_overlay.sov_sphere_node_base.rst
--rw-rw-rw-   0        0        0      223 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_overlay.sov_uv_widget.rst
--rw-rw-rw-   0        0        0      273 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_overlay.sphere_nodes.edge_sphere_item.rst
--rw-rw-rw-   0        0        0      273 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_overlay.sphere_nodes.item_sphere_node.rst
--rw-rw-rw-   0        0        0      279 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_overlay.sphere_nodes.person_sphere_node.rst
--rw-rw-rw-   0        0        0      502 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_overlay.sphere_nodes.rst
--rw-rw-rw-   0        0        0     1563 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_universe_base.rst
--rw-rw-rw-   0        0        0      226 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_universe_base.suv_calc.rst
--rw-rw-rw-   0        0        0      223 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_universe_base.suv_cam.rst
--rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_universe_base.suv_cam_movement.rst
--rw-rw-rw-   0        0        0      241 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_universe_base.suv_clipboard.rst
--rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_universe_base.suv_config.rst
--rw-rw-rw-   0        0        0      241 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_universe_base.suv_constants.rst
--rw-rw-rw-   0        0        0      243 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_universe_base.suv_edge_drag.rst
--rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_disc.rst
--rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_edge.rst
--rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_item.rst
--rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_node.rst
--rw-rw-rw-   0        0        0      258 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_socket.rst
--rw-rw-rw-   0        0        0      235 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_universe_base.suv_history.rst
--rw-rw-rw-   0        0        0      243 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_universe_base.suv_mouse_ray.rst
--rw-rw-rw-   0        0        0      226 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_universe_base.suv_node.rst
--rw-rw-rw-   0        0        0      249 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_universe_base.suv_rubber_band.rst
--rw-rw-rw-   0        0        0      250 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_universe_base.suv_serializable.rst
--rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_universe_base.suv_skybox.rst
--rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_universe_base.suv_socket.rst
--rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_universe_base.suv_sphere.rst
--rw-rw-rw-   0        0        0      249 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_universe_base.suv_sphere_edge.rst
--rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_universe_base.suv_surface_edge.rst
--rw-rw-rw-   0        0        0      238 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_universe_base.suv_universe.rst
--rw-rw-rw-   0        0        0      229 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_universe_base.suv_utils.rst
--rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_universe_base.suv_widget.rst
--rw-rw-rw-   0        0        0      127 2023-03-15 17:49:53.000000 sphere_base-0.1.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-16 15:11:20.799001 sphere_base-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1781 2023-04-16 15:10:58.000000 sphere_base-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-16 15:11:20.700995 sphere_base-0.1.1/sphere_base/
--rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.1/sphere_base/__init__.py
--rw-rw-rw-   0        0        0     8514 2023-04-14 08:27:37.000000 sphere_base-0.1.1/sphere_base/calc.py
--rw-rw-rw-   0        0        0     6909 2023-04-15 10:13:03.000000 sphere_base-0.1.1/sphere_base/clipboard.py
--rw-rw-rw-   0        0        0     5078 2023-04-14 08:50:15.000000 sphere_base-0.1.1/sphere_base/config.py
--rw-rw-rw-   0        0        0     5372 2023-04-15 11:21:35.000000 sphere_base-0.1.1/sphere_base/constants.py
-drwxrwxrwx   0        0        0        0 2023-04-16 15:11:20.720996 sphere_base-0.1.1/sphere_base/edge/
--rw-rw-rw-   0        0        0        0 2023-03-30 07:32:40.000000 sphere_base-0.1.1/sphere_base/edge/__init__.py
--rw-rw-rw-   0        0        0     6609 2023-04-14 08:50:15.000000 sphere_base-0.1.1/sphere_base/edge/edge_drag.py
--rw-rw-rw-   0        0        0     4771 2023-04-14 17:26:15.000000 sphere_base-0.1.1/sphere_base/edge/graphic_edge.py
--rw-rw-rw-   0        0        0      365 2023-04-15 20:38:35.000000 sphere_base-0.1.1/sphere_base/edge/graphic_line.py
--rw-rw-rw-   0        0        0     1859 2023-04-04 08:07:28.000000 sphere_base-0.1.1/sphere_base/edge/inter_sphere_edge.py
--rw-rw-rw-   0        0        0    14064 2023-04-15 09:49:56.000000 sphere_base-0.1.1/sphere_base/edge/surface_edge.py
--rw-rw-rw-   0        0        0     9835 2023-04-08 12:55:07.000000 sphere_base-0.1.1/sphere_base/history.py
-drwxrwxrwx   0        0        0        0 2023-04-16 15:11:20.726997 sphere_base-0.1.1/sphere_base/model/
--rw-rw-rw-   0        0        0      258 2021-03-02 15:14:54.000000 sphere_base-0.1.1/sphere_base/model/__init__.py
--rw-rw-rw-   0        0        0     4398 2023-04-04 14:50:05.000000 sphere_base-0.1.1/sphere_base/model/mesh.py
--rw-rw-rw-   0        0        0     6060 2023-04-11 18:27:52.000000 sphere_base-0.1.1/sphere_base/model/model.py
--rw-rw-rw-   0        0        0     3318 2023-04-04 11:04:51.000000 sphere_base-0.1.1/sphere_base/model/models.py
--rw-rw-rw-   0        0        0    23013 2023-04-07 13:30:04.000000 sphere_base-0.1.1/sphere_base/model/obj_file_loader.py
-drwxrwxrwx   0        0        0        0 2023-04-16 15:11:20.734997 sphere_base-0.1.1/sphere_base/node/
--rw-rw-rw-   0        0        0        0 2023-03-30 07:35:09.000000 sphere_base-0.1.1/sphere_base/node/__init__.py
--rw-rw-rw-   0        0        0     8018 2023-04-03 06:31:17.000000 sphere_base-0.1.1/sphere_base/node/graphic_disc.py
--rw-rw-rw-   0        0        0     2676 2023-04-03 06:31:17.000000 sphere_base-0.1.1/sphere_base/node/graphic_node.py
--rw-rw-rw-   0        0        0     2449 2023-04-03 06:31:16.000000 sphere_base-0.1.1/sphere_base/node/graphic_socket.py
--rw-rw-rw-   0        0        0    13284 2023-04-14 09:24:59.000000 sphere_base-0.1.1/sphere_base/node/node.py
--rw-rw-rw-   0        0        0     8797 2023-04-13 12:16:43.000000 sphere_base-0.1.1/sphere_base/node/socket.py
--rw-rw-rw-   0        0        0     1737 2023-03-30 07:13:13.000000 sphere_base-0.1.1/sphere_base/serializable.py
-drwxrwxrwx   0        0        0        0 2023-04-16 15:11:20.770999 sphere_base-0.1.1/sphere_base/shader/
--rw-rw-rw-   0        0        0      258 2021-03-02 15:14:54.000000 sphere_base-0.1.1/sphere_base/shader/__init__.py
--rw-rw-rw-   0        0        0    10547 2023-04-14 08:50:15.000000 sphere_base-0.1.1/sphere_base/shader/base_shader.py
--rw-rw-rw-   0        0        0     1956 2023-03-30 12:23:24.000000 sphere_base-0.1.1/sphere_base/shader/circle_shader.py
--rw-rw-rw-   0        0        0     1946 2023-03-30 12:23:24.000000 sphere_base-0.1.1/sphere_base/shader/cross_shader.py
--rw-rw-rw-   0        0        0      572 2023-03-30 09:23:40.000000 sphere_base-0.1.1/sphere_base/shader/default_shader.py
--rw-rw-rw-   0        0        0     1174 2023-04-15 09:19:58.000000 sphere_base-0.1.1/sphere_base/shader/edge_shader.py
--rw-rw-rw-   0        0        0      886 2023-03-30 12:22:23.000000 sphere_base-0.1.1/sphere_base/shader/flat_shader.py
--rw-rw-rw-   0        0        0     1447 2023-03-30 12:22:23.000000 sphere_base-0.1.1/sphere_base/shader/holo_sphere_shader.py
--rw-rw-rw-   0        0        0     1160 2023-03-30 12:22:23.000000 sphere_base-0.1.1/sphere_base/shader/node_shader.py
--rw-rw-rw-   0        0        0     2150 2023-03-30 12:20:38.000000 sphere_base-0.1.1/sphere_base/shader/skybox_shader.py
--rw-rw-rw-   0        0        0     1238 2023-03-30 12:20:38.000000 sphere_base-0.1.1/sphere_base/shader/socket_shader.py
--rw-rw-rw-   0        0        0     3109 2023-03-31 17:56:46.000000 sphere_base-0.1.1/sphere_base/shader/sphere_edge_shader.py
--rw-rw-rw-   0        0        0     1631 2023-03-30 12:18:39.000000 sphere_base-0.1.1/sphere_base/shader/sphere_shader.py
--rw-rw-rw-   0        0        0     1232 2023-03-30 12:18:13.000000 sphere_base-0.1.1/sphere_base/shader/sphere_small_shader.py
--rw-rw-rw-   0        0        0     1808 2023-03-30 12:18:13.000000 sphere_base-0.1.1/sphere_base/shader/square_shader.py
-drwxrwxrwx   0        0        0        0 2023-04-16 15:11:20.773999 sphere_base-0.1.1/sphere_base/sphere/
--rw-rw-rw-   0        0        0        0 2023-03-28 18:59:07.000000 sphere_base-0.1.1/sphere_base/sphere/__init__.py
--rw-rw-rw-   0        0        0    28219 2023-04-16 07:14:28.000000 sphere_base-0.1.1/sphere_base/sphere/sphere.py
-drwxrwxrwx   0        0        0        0 2023-04-16 15:11:20.779999 sphere_base-0.1.1/sphere_base/sphere_overlay/
--rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.1/sphere_base/sphere_overlay/__init__.py
--rw-rw-rw-   0        0        0     1875 2023-03-28 18:59:36.000000 sphere_base-0.1.1/sphere_base/sphere_overlay/sov_conf.py
--rw-rw-rw-   0        0        0     2468 2023-04-13 17:50:12.000000 sphere_base-0.1.1/sphere_base/sphere_overlay/sov_sphere.py
--rw-rw-rw-   0        0        0     1598 2023-04-13 12:14:08.000000 sphere_base-0.1.1/sphere_base/sphere_overlay/sov_sphere_node_base.py
-drwxrwxrwx   0        0        0        0 2023-04-16 15:11:20.785000 sphere_base-0.1.1/sphere_base/sphere_overlay/sphere_nodes/
--rw-rw-rw-   0        0        0      248 2021-03-02 15:18:12.000000 sphere_base-0.1.1/sphere_base/sphere_overlay/sphere_nodes/__init__.py
--rw-rw-rw-   0        0        0      460 2023-04-04 13:53:39.000000 sphere_base-0.1.1/sphere_base/sphere_overlay/sphere_nodes/edge_sphere_item.py
--rw-rw-rw-   0        0        0     1084 2023-04-13 12:16:43.000000 sphere_base-0.1.1/sphere_base/sphere_overlay/sphere_nodes/item_sphere_node.py
--rw-rw-rw-   0        0        0     1002 2023-04-13 12:14:08.000000 sphere_base-0.1.1/sphere_base/sphere_overlay/sphere_nodes/person_sphere_node.py
-drwxrwxrwx   0        0        0        0 2023-04-16 15:11:20.796000 sphere_base-0.1.1/sphere_base/sphere_universe_base/
--rw-rw-rw-   0        0        0       23 2021-03-11 14:37:00.000000 sphere_base-0.1.1/sphere_base/sphere_universe_base/__init__.py
--rw-rw-rw-   0        0        0     7829 2023-04-15 12:02:34.000000 sphere_base-0.1.1/sphere_base/sphere_universe_base/suv_cam.py
--rw-rw-rw-   0        0        0     3434 2023-04-15 11:53:42.000000 sphere_base-0.1.1/sphere_base/sphere_universe_base/suv_cam_movement.py
--rw-rw-rw-   0        0        0      365 2023-03-28 18:59:36.000000 sphere_base-0.1.1/sphere_base/sphere_universe_base/suv_graphic_item.py
--rw-rw-rw-   0        0        0    15874 2023-04-14 08:50:15.000000 sphere_base-0.1.1/sphere_base/sphere_universe_base/suv_mouse_ray.py
--rw-rw-rw-   0        0        0     7211 2023-04-14 09:13:08.000000 sphere_base-0.1.1/sphere_base/sphere_universe_base/suv_rubber_band.py
--rw-rw-rw-   0        0        0     5392 2023-03-28 18:59:36.000000 sphere_base-0.1.1/sphere_base/sphere_universe_base/suv_skybox.py
--rw-rw-rw-   0        0        0    14026 2023-04-14 08:50:15.000000 sphere_base-0.1.1/sphere_base/sphere_universe_base/suv_universe.py
--rw-rw-rw-   0        0        0    17879 2023-04-16 07:15:30.000000 sphere_base-0.1.1/sphere_base/sphere_universe_base/suv_widget.py
--rw-rw-rw-   0        0        0     1494 2023-03-30 07:18:00.000000 sphere_base-0.1.1/sphere_base/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-16 15:11:20.711995 sphere_base-0.1.1/sphere_base.egg-info/
--rw-rw-rw-   0        0        0     1968 2023-04-16 15:11:20.000000 sphere_base-0.1.1/sphere_base.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6024 2023-04-16 15:11:20.000000 sphere_base-0.1.1/sphere_base.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 15:11:20.000000 sphere_base-0.1.1/sphere_base.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-16 07:34:46.000000 sphere_base-0.1.1/sphere_base.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      119 2023-04-16 15:11:20.000000 sphere_base-0.1.1/sphere_base.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-16 15:11:20.000000 sphere_base-0.1.1/sphere_base.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-16 15:11:20.797001 sphere_base-0.1.1/tests/
--rw-rw-rw-   0        0        0      530 2023-03-15 14:00:41.000000 sphere_base-0.1.1/tests/test_000_import.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:51:17.418788 sphere_base-0.1.2/
+-rw-rw-rw-   0        0        0      978 2023-04-16 07:19:30.000000 sphere_base-0.1.2/HISTORY.rst
+-rw-rw-rw-   0        0        0     1105 2023-04-16 08:54:46.000000 sphere_base-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      252 2023-03-15 14:22:33.000000 sphere_base-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1987 2023-04-21 08:51:17.417788 sphere_base-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1205 2023-04-21 08:51:12.000000 sphere_base-0.1.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-21 08:51:16.950761 sphere_base-0.1.2/docs/
+-rw-rw-rw-   0        0        0      638 2023-03-15 17:55:12.000000 sphere_base-0.1.2/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-04-21 08:51:16.934760 sphere_base-0.1.2/docs/build/
+drwxrwxrwx   0        0        0        0 2023-04-21 08:51:16.935761 sphere_base-0.1.2/docs/build/html/
+drwxrwxrwx   0        0        0        0 2023-04-21 08:51:16.954762 sphere_base-0.1.2/docs/build/html/_static/
+-rw-rw-rw-   0        0        0      286 2023-03-15 17:53:40.000000 sphere_base-0.1.2/docs/build/html/_static/file.png
+-rw-rw-rw-   0        0        0       90 2023-03-15 17:53:40.000000 sphere_base-0.1.2/docs/build/html/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2023-03-15 17:53:40.000000 sphere_base-0.1.2/docs/build/html/_static/plus.png
+-rwxrwxrwx   0        0        0      804 2023-03-15 17:55:12.000000 sphere_base-0.1.2/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-04-21 08:51:16.957762 sphere_base-0.1.2/docs/source/
+-rw-rw-rw-   0        0        0     1175 2023-03-16 20:29:33.000000 sphere_base-0.1.2/docs/source/conf.py
+-rw-rw-rw-   0        0        0      489 2023-03-16 21:15:47.000000 sphere_base-0.1.2/docs/source/index.rst
+drwxrwxrwx   0        0        0        0 2023-04-21 08:51:17.077769 sphere_base-0.1.2/docs/source/rst/
+-rw-rw-rw-   0        0        0      163 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.model.mesh.rst
+-rw-rw-rw-   0        0        0      166 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.model.model.rst
+-rw-rw-rw-   0        0        0      169 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.model.models.rst
+-rw-rw-rw-   0        0        0      200 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.model.obj_file_loader.rst
+-rw-rw-rw-   0        0        0      369 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.model.rst
+-rw-rw-rw-   0        0        0      196 2023-03-16 21:18:48.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.rst
+-rw-rw-rw-   0        0        0      780 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.shader.rst
+-rw-rw-rw-   0        0        0      200 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.shader.uv_base_shader.rst
+-rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.shader.uv_circle_shader.rst
+-rw-rw-rw-   0        0        0      203 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.shader.uv_cross_shader.rst
+-rw-rw-rw-   0        0        0      209 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.shader.uv_default_shader.rst
+-rw-rw-rw-   0        0        0      200 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.shader.uv_flat_shader.rst
+-rw-rw-rw-   0        0        0      223 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.shader.uv_holo_sphere_shader.rst
+-rw-rw-rw-   0        0        0      200 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.shader.uv_node_shader.rst
+-rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.shader.uv_skybox_shader.rst
+-rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.shader.uv_socket_shader.rst
+-rw-rw-rw-   0        0        0      223 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.shader.uv_sphere_edge_shader.rst
+-rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.shader.uv_sphere_shader.rst
+-rw-rw-rw-   0        0        0      226 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.shader.uv_sphere_small_shader.rst
+-rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.shader.uv_square_shader.rst
+-rw-rw-rw-   0        0        0      602 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_overlay.rst
+-rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_overlay.sov_conf.rst
+-rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_overlay.sov_edge.rst
+-rw-rw-rw-   0        0        0      212 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_overlay.sov_sphere.rst
+-rw-rw-rw-   0        0        0      246 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_overlay.sov_sphere_node_base.rst
+-rw-rw-rw-   0        0        0      223 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_overlay.sov_uv_widget.rst
+-rw-rw-rw-   0        0        0      273 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_overlay.sphere_nodes.edge_sphere_item.rst
+-rw-rw-rw-   0        0        0      273 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_overlay.sphere_nodes.item_sphere_node.rst
+-rw-rw-rw-   0        0        0      279 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_overlay.sphere_nodes.person_sphere_node.rst
+-rw-rw-rw-   0        0        0      502 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_overlay.sphere_nodes.rst
+-rw-rw-rw-   0        0        0     1563 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_universe_base.rst
+-rw-rw-rw-   0        0        0      226 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_universe_base.suv_calc.rst
+-rw-rw-rw-   0        0        0      223 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_universe_base.suv_cam.rst
+-rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_universe_base.suv_cam_movement.rst
+-rw-rw-rw-   0        0        0      241 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_universe_base.suv_clipboard.rst
+-rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_universe_base.suv_config.rst
+-rw-rw-rw-   0        0        0      241 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_universe_base.suv_constants.rst
+-rw-rw-rw-   0        0        0      243 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_universe_base.suv_edge_drag.rst
+-rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_disc.rst
+-rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_edge.rst
+-rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_item.rst
+-rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_node.rst
+-rw-rw-rw-   0        0        0      258 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_socket.rst
+-rw-rw-rw-   0        0        0      235 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_universe_base.suv_history.rst
+-rw-rw-rw-   0        0        0      243 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_universe_base.suv_mouse_ray.rst
+-rw-rw-rw-   0        0        0      226 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_universe_base.suv_node.rst
+-rw-rw-rw-   0        0        0      249 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_universe_base.suv_rubber_band.rst
+-rw-rw-rw-   0        0        0      250 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_universe_base.suv_serializable.rst
+-rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_universe_base.suv_skybox.rst
+-rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_universe_base.suv_socket.rst
+-rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_universe_base.suv_sphere.rst
+-rw-rw-rw-   0        0        0      249 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_universe_base.suv_sphere_edge.rst
+-rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_universe_base.suv_surface_edge.rst
+-rw-rw-rw-   0        0        0      238 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_universe_base.suv_universe.rst
+-rw-rw-rw-   0        0        0      229 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_universe_base.suv_utils.rst
+-rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_universe_base.suv_widget.rst
+-rw-rw-rw-   0        0        0      127 2023-03-15 17:49:53.000000 sphere_base-0.1.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 08:51:17.418788 sphere_base-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1574 2023-04-21 08:10:33.000000 sphere_base-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:51:17.085769 sphere_base-0.1.2/sphere_base/
+-rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.2/sphere_base/__init__.py
+-rw-rw-rw-   0        0        0     8512 2023-04-20 14:05:18.000000 sphere_base-0.1.2/sphere_base/calc.py
+-rw-rw-rw-   0        0        0     6909 2023-04-15 10:13:03.000000 sphere_base-0.1.2/sphere_base/clipboard.py
+-rw-rw-rw-   0        0        0     5078 2023-04-14 08:50:15.000000 sphere_base-0.1.2/sphere_base/config.py
+-rw-rw-rw-   0        0        0     4839 2023-04-20 17:12:04.000000 sphere_base-0.1.2/sphere_base/constants.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:51:17.181775 sphere_base-0.1.2/sphere_base/edge/
+-rw-rw-rw-   0        0        0        0 2023-03-30 07:32:40.000000 sphere_base-0.1.2/sphere_base/edge/__init__.py
+-rw-rw-rw-   0        0        0     7711 2023-04-20 09:15:29.000000 sphere_base-0.1.2/sphere_base/edge/edge_drag.py
+-rw-rw-rw-   0        0        0     4592 2023-04-20 07:51:22.000000 sphere_base-0.1.2/sphere_base/edge/graphic_edge.py
+-rw-rw-rw-   0        0        0      809 2023-04-19 12:36:22.000000 sphere_base-0.1.2/sphere_base/edge/graphic_line.py
+-rw-rw-rw-   0        0        0     1859 2023-04-04 08:07:28.000000 sphere_base-0.1.2/sphere_base/edge/inter_sphere_edge.py
+-rw-rw-rw-   0        0        0    14119 2023-04-20 17:33:34.000000 sphere_base-0.1.2/sphere_base/edge/surface_edge.py
+-rw-rw-rw-   0        0        0     9835 2023-04-08 12:55:07.000000 sphere_base-0.1.2/sphere_base/history.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:51:17.239778 sphere_base-0.1.2/sphere_base/model/
+-rw-rw-rw-   0        0        0      258 2021-03-02 15:14:54.000000 sphere_base-0.1.2/sphere_base/model/__init__.py
+-rw-rw-rw-   0        0        0     4197 2023-04-20 17:16:58.000000 sphere_base-0.1.2/sphere_base/model/mesh.py
+-rw-rw-rw-   0        0        0     6393 2023-04-20 17:27:51.000000 sphere_base-0.1.2/sphere_base/model/model.py
+-rw-rw-rw-   0        0        0     3318 2023-04-04 11:04:51.000000 sphere_base-0.1.2/sphere_base/model/models.py
+-rw-rw-rw-   0        0        0    23063 2023-04-21 06:52:17.000000 sphere_base-0.1.2/sphere_base/model/obj_file_loader.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:51:17.241778 sphere_base-0.1.2/sphere_base/model/resources/
+-rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.2/sphere_base/model/resources/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:51:17.242778 sphere_base-0.1.2/sphere_base/model/resources/icons/
+-rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.2/sphere_base/model/resources/icons/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:51:17.244778 sphere_base-0.1.2/sphere_base/model/resources/images/
+-rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.2/sphere_base/model/resources/images/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:51:17.245778 sphere_base-0.1.2/sphere_base/model/resources/meshes/
+-rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.2/sphere_base/model/resources/meshes/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:51:17.246778 sphere_base-0.1.2/sphere_base/model/resources/shaders/
+-rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.2/sphere_base/model/resources/shaders/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:51:17.247779 sphere_base-0.1.2/sphere_base/model/resources/sphere_textures/
+-rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.2/sphere_base/model/resources/sphere_textures/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:51:17.248778 sphere_base-0.1.2/sphere_base/model/resources/textures/
+-rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.2/sphere_base/model/resources/textures/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:51:17.260779 sphere_base-0.1.2/sphere_base/node/
+-rw-rw-rw-   0        0        0        0 2023-03-30 07:35:09.000000 sphere_base-0.1.2/sphere_base/node/__init__.py
+-rw-rw-rw-   0        0        0     8018 2023-04-03 06:31:17.000000 sphere_base-0.1.2/sphere_base/node/graphic_disc.py
+-rw-rw-rw-   0        0        0     2676 2023-04-03 06:31:17.000000 sphere_base-0.1.2/sphere_base/node/graphic_node.py
+-rw-rw-rw-   0        0        0     2449 2023-04-03 06:31:16.000000 sphere_base-0.1.2/sphere_base/node/graphic_socket.py
+-rw-rw-rw-   0        0        0    13282 2023-04-20 17:22:13.000000 sphere_base-0.1.2/sphere_base/node/node.py
+-rw-rw-rw-   0        0        0     8797 2023-04-13 12:16:43.000000 sphere_base-0.1.2/sphere_base/node/socket.py
+-rw-rw-rw-   0        0        0     1737 2023-03-30 07:13:13.000000 sphere_base-0.1.2/sphere_base/serializable.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:51:17.344784 sphere_base-0.1.2/sphere_base/shader/
+-rw-rw-rw-   0        0        0      258 2021-03-02 15:14:54.000000 sphere_base-0.1.2/sphere_base/shader/__init__.py
+-rw-rw-rw-   0        0        0     9085 2023-04-20 17:12:04.000000 sphere_base-0.1.2/sphere_base/shader/base_shader.py
+-rw-rw-rw-   0        0        0     1979 2023-04-20 17:16:57.000000 sphere_base-0.1.2/sphere_base/shader/circle_shader.py
+-rw-rw-rw-   0        0        0     1969 2023-04-20 17:16:57.000000 sphere_base-0.1.2/sphere_base/shader/cross_shader.py
+-rw-rw-rw-   0        0        0      572 2023-03-30 09:23:40.000000 sphere_base-0.1.2/sphere_base/shader/default_shader.py
+-rw-rw-rw-   0        0        0     2235 2023-04-20 09:28:14.000000 sphere_base-0.1.2/sphere_base/shader/drag_edge_shader.py
+-rw-rw-rw-   0        0        0     1164 2023-04-20 17:31:03.000000 sphere_base-0.1.2/sphere_base/shader/edge_shader.py
+-rw-rw-rw-   0        0        0      909 2023-04-20 17:16:58.000000 sphere_base-0.1.2/sphere_base/shader/flat_shader.py
+-rw-rw-rw-   0        0        0     1467 2023-04-20 17:16:57.000000 sphere_base-0.1.2/sphere_base/shader/holo_sphere_shader.py
+-rw-rw-rw-   0        0        0     1166 2023-04-20 17:16:57.000000 sphere_base-0.1.2/sphere_base/shader/node_shader.py
+-rw-rw-rw-   0        0        0     2150 2023-04-20 17:12:04.000000 sphere_base-0.1.2/sphere_base/shader/skybox_shader.py
+-rw-rw-rw-   0        0        0     1261 2023-04-20 17:16:58.000000 sphere_base-0.1.2/sphere_base/shader/socket_shader.py
+-rw-rw-rw-   0        0        0     3117 2023-04-20 17:31:03.000000 sphere_base-0.1.2/sphere_base/shader/sphere_edge_shader.py
+-rw-rw-rw-   0        0        0     1668 2023-04-20 17:16:58.000000 sphere_base-0.1.2/sphere_base/shader/sphere_shader.py
+-rw-rw-rw-   0        0        0     1254 2023-04-20 17:16:58.000000 sphere_base-0.1.2/sphere_base/shader/sphere_small_shader.py
+-rw-rw-rw-   0        0        0     1845 2023-04-20 17:16:58.000000 sphere_base-0.1.2/sphere_base/shader/square_shader.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:51:17.347784 sphere_base-0.1.2/sphere_base/sphere/
+-rw-rw-rw-   0        0        0        0 2023-03-28 18:59:07.000000 sphere_base-0.1.2/sphere_base/sphere/__init__.py
+-rw-rw-rw-   0        0        0    28884 2023-04-21 06:53:52.000000 sphere_base-0.1.2/sphere_base/sphere/sphere.py
+-rw-rw-rw-   0        0        0     6068 2023-04-21 07:05:58.000000 sphere_base-0.1.2/sphere_base/sphere/sphere_lines.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:51:17.399787 sphere_base-0.1.2/sphere_base/sphere_overlay/
+-rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.2/sphere_base/sphere_overlay/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:51:17.400787 sphere_base-0.1.2/sphere_base/sphere_overlay/icons/
+-rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.2/sphere_base/sphere_overlay/icons/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:51:17.402787 sphere_base-0.1.2/sphere_base/sphere_overlay/qss/
+-rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.2/sphere_base/sphere_overlay/qss/__init__.py
+-rw-rw-rw-   0        0        0    30464 2021-01-18 11:54:48.000000 sphere_base-0.1.2/sphere_base/sphere_overlay/qss/nodeeditor_dark_resources.py
+-rw-rw-rw-   0        0        0     1875 2023-03-28 18:59:36.000000 sphere_base-0.1.2/sphere_base/sphere_overlay/sov_conf.py
+-rw-rw-rw-   0        0        0     2161 2023-04-20 13:43:23.000000 sphere_base-0.1.2/sphere_base/sphere_overlay/sov_sphere.py
+-rw-rw-rw-   0        0        0     1598 2023-04-13 12:14:08.000000 sphere_base-0.1.2/sphere_base/sphere_overlay/sov_sphere_node_base.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:51:17.406787 sphere_base-0.1.2/sphere_base/sphere_overlay/sphere_nodes/
+-rw-rw-rw-   0        0        0      248 2021-03-02 15:18:12.000000 sphere_base-0.1.2/sphere_base/sphere_overlay/sphere_nodes/__init__.py
+-rw-rw-rw-   0        0        0      460 2023-04-04 13:53:39.000000 sphere_base-0.1.2/sphere_base/sphere_overlay/sphere_nodes/edge_sphere_item.py
+-rw-rw-rw-   0        0        0     1084 2023-04-13 12:16:43.000000 sphere_base-0.1.2/sphere_base/sphere_overlay/sphere_nodes/item_sphere_node.py
+-rw-rw-rw-   0        0        0     1002 2023-04-13 12:14:08.000000 sphere_base-0.1.2/sphere_base/sphere_overlay/sphere_nodes/person_sphere_node.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:51:17.415788 sphere_base-0.1.2/sphere_base/sphere_universe_base/
+-rw-rw-rw-   0        0        0       23 2021-03-11 14:37:00.000000 sphere_base-0.1.2/sphere_base/sphere_universe_base/__init__.py
+-rw-rw-rw-   0        0        0     7829 2023-04-15 12:02:34.000000 sphere_base-0.1.2/sphere_base/sphere_universe_base/suv_cam.py
+-rw-rw-rw-   0        0        0     3434 2023-04-15 11:53:42.000000 sphere_base-0.1.2/sphere_base/sphere_universe_base/suv_cam_movement.py
+-rw-rw-rw-   0        0        0      365 2023-03-28 18:59:36.000000 sphere_base-0.1.2/sphere_base/sphere_universe_base/suv_graphic_item.py
+-rw-rw-rw-   0        0        0    15874 2023-04-14 08:50:15.000000 sphere_base-0.1.2/sphere_base/sphere_universe_base/suv_mouse_ray.py
+-rw-rw-rw-   0        0        0     7211 2023-04-14 09:13:08.000000 sphere_base-0.1.2/sphere_base/sphere_universe_base/suv_rubber_band.py
+-rw-rw-rw-   0        0        0     5392 2023-03-28 18:59:36.000000 sphere_base-0.1.2/sphere_base/sphere_universe_base/suv_skybox.py
+-rw-rw-rw-   0        0        0    14026 2023-04-14 08:50:15.000000 sphere_base-0.1.2/sphere_base/sphere_universe_base/suv_universe.py
+-rw-rw-rw-   0        0        0    17954 2023-04-20 15:39:40.000000 sphere_base-0.1.2/sphere_base/sphere_universe_base/suv_widget.py
+-rw-rw-rw-   0        0        0     1494 2023-03-30 07:18:00.000000 sphere_base-0.1.2/sphere_base/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:51:17.148773 sphere_base-0.1.2/sphere_base.egg-info/
+-rw-rw-rw-   0        0        0     1987 2023-04-21 08:51:16.000000 sphere_base-0.1.2/sphere_base.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6579 2023-04-21 08:51:16.000000 sphere_base-0.1.2/sphere_base.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 08:51:16.000000 sphere_base-0.1.2/sphere_base.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-16 07:34:46.000000 sphere_base-0.1.2/sphere_base.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      119 2023-04-21 08:51:16.000000 sphere_base-0.1.2/sphere_base.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-21 08:51:16.000000 sphere_base-0.1.2/sphere_base.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 08:51:17.416788 sphere_base-0.1.2/tests/
+-rw-rw-rw-   0        0        0      530 2023-03-15 14:00:41.000000 sphere_base-0.1.2/tests/test_000_import.py
```

### Comparing `sphere_base-0.1.1/HISTORY.rst` & `sphere_base-0.1.2/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.1/LICENSE` & `sphere_base-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.1/PKG-INFO` & `sphere_base-0.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: sphere_base
-Version: 0.1.1
-Summary: The library was created to be used as a building block for applications were informationshould appear on the surface of a sphere. It allows for creating spheres with nodesand edges that can be dragged on its surface. Nodes and edges can be placed and removed from the sphere surface. 
+Version: 0.1.2
+Summary: library for applications were information should appear on the surface of a sphere. It allows for creating spheres with nodes and edges that can be dragged on its surface. 
 Home-page: https://github.com/rboltze/spherebase
 Author: Richard Boltze
 Author-email: rboltze@protonmail.com
 License: MIT license
 Keywords: sphere_base
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -20,48 +20,59 @@
 Sphere Base
 ############
 
 Introduction
 =============
 
 This library was created as a building block for use in applications were information should be displayed as nodes or
-labels on a sphere. These nodes are interactive so they can be moved by dragging and connecting them to other nodes.
+labels on a sphere. These nodes are interactive so they can be moved by dragging and can be connected to other nodes.
 
-This package is created in python using a pyqt5 window.
 
-* Development Status :: 4 - Beta
+* Development Status: 4 - Beta
 * Free software: MIT license
 
 
 Features
 =========
 
 - Customizable spheres with textures and colors
 - Nodes, sockets and edges can be dragged over the surface of the sphere
 - Support for undo/redo, cut and paste using serialization
 - Hovering effects, dragging nodes, cutting edges
+- Background skybox image can be changed
+- Sphere color and texture can be changed
 - Example on how the library can be implemented
 
+
 Requirements
 =============
 
+This package is created in python using a pyqt5 window.
+
 - Python 3.x
 - PyOpenGL
 - PyQt5
+- pyperclip
+- pybullet
+- Pillow
+- numpy
 
 
 Supported Environment
 ======================
 
 * Windows (Win32, x64)
 
 
 The library is available from PyPI
 
-    $ pip install sphere-base==0.0.1
+    $ pip install sphere-base
+
+
+
 
 
 Or download the source code from github
 
     git clone https://github.com/rboltze/sphere_base.git
```

### Comparing `sphere_base-0.1.1/README.rst` & `sphere_base-0.1.2/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,59 @@
 Sphere Base
 ############
 
 Introduction
 =============
 
 This library was created as a building block for use in applications were information should be displayed as nodes or
-labels on a sphere. These nodes are interactive so they can be moved by dragging and connecting them to other nodes.
+labels on a sphere. These nodes are interactive so they can be moved by dragging and can be connected to other nodes.
 
-This package is created in python using a pyqt5 window.
 
-* Development Status :: 4 - Beta
+* Development Status: 4 - Beta
 * Free software: MIT license
 
 
 Features
 =========
 
 - Customizable spheres with textures and colors
 - Nodes, sockets and edges can be dragged over the surface of the sphere
 - Support for undo/redo, cut and paste using serialization
 - Hovering effects, dragging nodes, cutting edges
+- Background skybox image can be changed
+- Sphere color and texture can be changed
 - Example on how the library can be implemented
 
+
 Requirements
 =============
 
+This package is created in python using a pyqt5 window.
+
 - Python 3.x
 - PyOpenGL
 - PyQt5
+- pyperclip
+- pybullet
+- Pillow
+- numpy
 
 
 Supported Environment
 ======================
 
 * Windows (Win32, x64)
 
 
 The library is available from PyPI
 
-    $ pip install sphere-base==0.0.1
+    $ pip install sphere-base
+
+
+
 
 
 Or download the source code from github
 
     git clone https://github.com/rboltze/sphere_base.git
```

### Comparing `sphere_base-0.1.1/docs/Makefile` & `sphere_base-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.1/docs/make.bat` & `sphere_base-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.1/docs/source/conf.py` & `sphere_base-0.1.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.1/docs/source/rst/sphere_base.shader.rst` & `sphere_base-0.1.2/docs/source/rst/sphere_base.shader.rst`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_overlay.rst` & `sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_overlay.rst`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_universe_base.rst` & `sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_universe_base.rst`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.1/setup.py` & `sphere_base-0.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,26 +26,24 @@
         'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
     ],
-    description="The library was created to be used as a building block for applications were information"
-                "should appear on the surface of a sphere. It allows for creating spheres with nodes"
-                "and edges that can be dragged on its surface. Nodes and edges can be placed and removed "
-                "from the sphere surface. \n"
-                "This library is written in Python, PyOpenGL and PyQT5",
+    description="library for applications were information "
+                "should appear on the surface of a sphere. It allows for creating spheres with nodes "
+                "and edges that can be dragged on its surface. ",
     install_requires=requirements,
     license="MIT license",
     long_description=readme,
     include_package_data=True,
     keywords='sphere_base',
     name='sphere_base',
     packages=find_packages(include=['sphere_base*'], exclude=['examples*', 'test*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/rboltze/spherebase',
-    version='0.1.1',
+    version='0.1.2',
     zip_safe=False,
 )
```

### Comparing `sphere_base-0.1.1/sphere_base/calc.py` & `sphere_base-0.1.2/sphere_base/calc.py`

 * *Files 0% similar despite different names*

```diff
@@ -165,15 +165,14 @@
                 p1 = quaternion.normalize(p1)
                 p2 = vector.normalize(Vector3([collision_point]))  # The position of the point in world space
 
                 x1, x2 = p1[0], p2[0]
                 y1, y2 = p1[1], p2[1]
                 z1, z2 = p1[2], p2[2]
 
-
                 pitch = math.asin(x2) - math.acos(z1)
                 # and then over the x axis (yaw)
                 yaw = math.atan2(z2, y2)
 
                 # Correct the rotation with the default sphere position with the default camera direction
                 pitch_rad = -pitch + ((math.pi / 180) * 90)
                 yaw_rad = yaw
```

### Comparing `sphere_base-0.1.1/sphere_base/clipboard.py` & `sphere_base-0.1.2/sphere_base/clipboard.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.1/sphere_base/config.py` & `sphere_base-0.1.2/sphere_base/config.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.1/sphere_base/edge/edge_drag.py` & `sphere_base-0.1.2/sphere_base/edge/edge_drag.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 
 """
 
 from pyrr import quaternion
 from sphere_base.node.socket import *
 from sphere_base.edge.graphic_edge import GraphicEdge
 from sphere_base.shader.sphere_shader import SphereShader
+from sphere_base.model.model import Model
+from sphere_base.utils import dump_exception
 
 
 class EdgeDrag:
 
     GraphicsEdge_class = GraphicEdge
     Shader_class = SphereShader
 
@@ -28,15 +30,15 @@
 
         :param sphere: This class is instantiated from the :class:`~sphere_iot.uv_sphere.Sphere`
         :type sphere: :class:`~sphere_iot.uv_sphere.Sphere`
 
         :Instance Attributes:
 
         - **gr_edge** - Instance of :class:`~sphere_iot.uv_edge.SphereSurfaceEdge`
-        - **calc** - Instance of :class:`~sphere_iot.uv_calc.UvCalc` from universe
+        - **calc** - Instance of :class:`~sphere_iot.uv_calc.UvCalc` from universe.
 
         :Instance Variables:
 
         - **uv** - reference to :class:`~sphere_iot.uv_universe.Universe`
         - **sphere_base** - reference to :class:`~sphere_iot.uv_sphere.Sphere`
         - **config** - reference to :class:`~sphere_iot.uv_config.UvConfig`
         - **shader** - reference to :class:`~sphere_iot.shader.uv_base_shader.BaseShader`
@@ -48,33 +50,55 @@
 
         : Properties:
             - **dragging** - property flag indicating whether the edge being dragged
 
         """
         self.sphere = sphere
         self.config = sphere.config
-        self._init_variables()
 
-    def _init_variables(self):
         self.uv = self.sphere.uv
-        self.shader = self.sphere.shader
-        # self.shader = self.__class__.Shader_class(self)
 
         self.radius = self.sphere.radius
         self.start_socket = None
         self.xyz = None
         self.pos_orientation_offset = None
         self._dragging = False
 
         self.unit_length = 0.04
         self.pos_array = []
 
         self.gr_edge = self.__class__.GraphicsEdge_class(self)
+        self.model = self.set_up_model('drag_edge')
         self.calc = Calc()
 
+    def set_up_model(self, model_name):
+        shader, vertex_shader, fragment_shader, geometry_shader = None, None, None, None
+
+        # get the shaders for the edge
+        for _name in MODELS.keys():
+            if _name == model_name:
+                shader = MODELS[_name]["shader"]
+                vertex_shader = MODELS[_name]["vertex_shader"]
+                fragment_shader = MODELS[_name]["fragment_shader"]
+                geometry_shader = MODELS[_name]["geometry_shader"]
+                geometry_shader = None if geometry_shader == "none" else geometry_shader
+
+        # create a model for the edge
+        model = Model(
+                      models=self.uv.models,
+                      model_id=0,
+                      model_name=model_name,
+                      obj_file="",
+                      shader=shader,
+                      vertex_shader=vertex_shader,
+                      fragment_shader=fragment_shader,
+                      geometry_shader=geometry_shader)
+
+        return model
+
     def _init_start_dragging(self, start_socket: 'Socket'):
         # dragging start point is the start socket
         self.start_socket = start_socket
         self.xyz = start_socket.xyz  # position of the mouse at start
         self.pos_orientation_offset = self.start_socket.node.pos_orientation_offset
 
     def _stop_dragging(self):
@@ -94,15 +118,15 @@
         return self._dragging
 
     @dragging.setter
     def dragging(self, value: bool):
         if not self._dragging and value:
             self._dragging = value
 
-    def drag(self, start_socket: 'socket', dragging: bool, mouse_ray_collision_point=None):
+    def drag(self, start_socket, dragging: bool, mouse_ray_collision_point=None):
         """
         Dragging an edge
 
         :param start_socket:
         :type start_socket: :class:`~sphere_iot.uv_socket.Socket`
         :param mouse_ray_collision_point: mouse x-offset
         :type mouse_ray_collision_point: ``float``
@@ -180,9 +204,12 @@
         return self.gr_edge.get_position(self.pos_orientation_offset, self.sphere.radius)
 
     def draw(self):
         """
         Drawing the edge with dotted lines.
 
         """
-        if self._dragging:
-            self.shader.draw_edge(self.pos_array, width=2, color=[0, 0, 0, 1], dotted=True)
+        try:
+            if self._dragging:
+                self.model.shader.draw_edge(self.pos_array, width=2, color=[0, 0, 0, 1], dotted=True)
+        except Exception as e:
+            dump_exception(e)
```

### Comparing `sphere_base-0.1.1/sphere_base/edge/graphic_edge.py` & `sphere_base-0.1.2/sphere_base/edge/graphic_edge.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,35 +32,29 @@
             - **calc** - instance of :class:`~sphere_iot.uv_calc.UvCalc`
 
         """
         self.edge = parent
         self.sphere = parent.sphere
         self.calc = self.__class__.calc_class()
 
-        self._init_variables()
-        self._init_flags()
-        self._init_assets()
-
-    def _init_flags(self):
-        self._hover = False
-
-    def _init_variables(self):
         self._selected = False
         self._current_color = None
 
         self.unit_length = 0.05
         self.color = [0, 0, 0, .5]
+        self._hover = False
+        self._init_assets()
 
     def _init_assets(self):
         """Initialize ``QObjects`` like ``QColor``, ``QPen`` and ``QBrush``"""
         self.default_color = [0, 0, 0, .5]  # black
         self.selected_color = [0.9, 0.0, 0.0, 0.4]
         self.hover_color = [191, 255, 0, 1]
 
-    def count_vertices(self, start_xyz: 'Vector3', end_xyz: 'Vector3', radius: float, unit_length: float):
+    def count_vertices(self, start_xyz, end_xyz, radius: float, unit_length: float):
         """
         Returns the number of vertices on the edge.
 
         :param start_xyz: start position
         :type start_xyz: ``Vector3``
         :param end_xyz: end position
         :type end_xyz: ``Vector3``
@@ -71,30 +65,31 @@
         :returns: ``int`` number of edge elements
 
         """
         # shortest distance over the surface of the globe between start socket and edge-end
         length = self.calc.get_distance_on_sphere(end_xyz, start_xyz, radius)
         return int(math.ceil(length / unit_length))
 
-    def get_position(self, pos_orientation_offset: 'Quaternion', radius=None) -> 'Vector3':
+    def get_position(self, pos_orientation_offset, radius=None):
         """
         Returns xyz vector based on degree offset (position orientation offset)
 
         :param pos_orientation_offset: degree offset from the zero-position of the ``Sphere``.
         :param pos_orientation_offset: ``Quaternion``
+        :param radius:
         :returns: ``Vector3`` xyz-position
 
         """
         cumulative_orientation = self.get_cumulative_rotation(pos_orientation_offset)
 
         # get the position of the edge vertex on the sphere_base, calculated from the cumulative rotation
         xyz = self.calc.move_to_position(cumulative_orientation, self.sphere)
         return xyz
 
-    def get_cumulative_rotation(self, pos_orientation_offset: 'Quaternion') -> 'Quaternion':
+    def get_cumulative_rotation(self, pos_orientation_offset):
         """
         Returns the cumulative rotation of the pos_orientation_offset with the sphere rotation.
 
         :param pos_orientation_offset: degree offset from the zero-position of the ``Sphere``.
         :type pos_orientation_offset: ``Quaternion``
         :returns: ``Quaternion`` cumulative offset
         """
```

### Comparing `sphere_base-0.1.1/sphere_base/edge/inter_sphere_edge.py` & `sphere_base-0.1.2/sphere_base/edge/inter_sphere_edge.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.1/sphere_base/edge/surface_edge.py` & `sphere_base-0.1.2/sphere_base/edge/surface_edge.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,20 +84,21 @@
         self.start_socket = socket_start if socket_start else None
         self.end_socket = socket_end if socket_end else None
         self.xyz, self.pos_orientation_offset = None, None
         self.collision_object_id = None
         self.vert = []  # vertices needed for pybullet mouse ray
         self.serialized_detail_scene = None
         self._edge_moved = False
+        self.line_width = 2
         self.scale = [1.0, 1.0, 1.0]
         self.color = self.gr_edge.color
         self.edge_type = 0
         self.orientation = self.sphere.orientation
         self._new_edge = True
-        self.model = self.set_up_model('edge1')
+        self.model = self.set_up_model('edge')
 
         self.mesh = self.model.meshes[0]
         self.mesh_id = self.mesh.mesh_id
 
         self.model.name = 'edge_' + str(self.mesh_id)
 
         self.radius = self.sphere.radius  # - 0.01
@@ -112,15 +113,15 @@
             if _name == model_name:
                 shader = MODELS[_name]["shader"]
                 vertex_shader = MODELS[_name]["vertex_shader"]
                 fragment_shader = MODELS[_name]["fragment_shader"]
                 geometry_shader = MODELS[_name]["geometry_shader"]
                 geometry_shader = None if geometry_shader == "none" else geometry_shader
 
-        # create a model for this edge
+        # create a model for the edge
         model = Model(
                       models=self.uv.models,
                       model_id=0,
                       model_name=model_name,
                       obj_file="",
                       shader=shader,
                       vertex_shader=vertex_shader,
@@ -345,15 +346,15 @@
             self.sphere.uv.mouse_ray.delete_collision_object(self)
 
     def draw(self):
         """
         Renders the edge.
         """
         try:
-            self.model.draw(self, color=self.color)
+            self.model.draw(self, color=self.color, line_width=self.line_width)
         except Exception as e:
             dump_exception(e)
 
     def serialize(self):
         return OrderedDict([
             ('id', self.id),
             ('type', self.type),
```

### Comparing `sphere_base-0.1.1/sphere_base/history.py` & `sphere_base-0.1.2/sphere_base/history.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.1/sphere_base/model/mesh.py` & `sphere_base-0.1.2/sphere_base/model/mesh.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         :return:
         """
         self.vertices = None
         self.indices = None
         self.buffer = None
 
     def draw(self, shader: 'Shader', model_id: int, position: 'Vector3', orientation: 'Quaternion', scale: list = None,
-             texture_id: int = 0, color: list = None, switch: int = 0):
+             texture_id: int = 0, color: list = None, switch: int = 0, line_width=1):
         """
         Sending the ``Mesh`` with all the parameters to the dedicated shader.
 
         :param shader: Each ``Model`` gets its own ``Shader`` allocated.
         :type shader: :class:`~sphere_iot.shader.uv_base_shader.BaseShader`.
         :param model_id: The id of :class:`~sphere_iot.uv_models.Model` this ``Mesh`` is on.
         :type model_id: ``int``
@@ -89,21 +89,12 @@
                 print("indices_len", self.indices_len)
                 print("position", position)
                 print("orientation", orientation)
                 print("scale", scale)
                 print("texture_id", texture_id, "\n")
 
         try:
-            shader.draw(
-                         object_index=model_id,
-                         object_type=self.model.type,
-                         mesh_index=self.mesh_id,
-                         indices_len=self.indices_len,
-                         position=position,
-                         orientation=orientation,
-                         scale=scale,
-                         texture_id=texture_id,
-                         color=color,
-                         switch=switch
-                         )
+            shader.draw(object_index=model_id, object_type=self.model.type, mesh_index=self.mesh_id,
+                        indices_len=self.indices_len, position=position, orientation=orientation, scale=scale,
+                        texture_id=texture_id, color=color, switch=switch, line_width=line_width)
         except Exception as e:
             dump_exception(e)
```

### Comparing `sphere_base-0.1.1/sphere_base/model/model.py` & `sphere_base-0.1.2/sphere_base/model/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,19 +11,21 @@
 from sphere_base.shader.circle_shader import CircleShader
 from sphere_base.shader.square_shader import SquareShader
 from sphere_base.shader.sphere_edge_shader import SphereEdgeShader
 from sphere_base.shader.cross_shader import CrossShader
 from sphere_base.shader.holo_sphere_shader import HoloSphereShader
 from sphere_base.shader.sphere_small_shader import SphereSmallShader
 from sphere_base.shader.edge_shader import EdgeShader
+from sphere_base.shader.drag_edge_shader import DragEdgeShader
 # -----------------------------------------------------------------------
 
 from sphere_base.sphere_universe_base.suv_graphic_item import GraphicItem
 from sphere_base.model.mesh import Mesh
 from sphere_base.model.obj_file_loader import ObjectFileLoader
+from sphere_base.utils import dump_exception
 import pathlib
 
 DEBUG = True
 
 
 class Model(GraphicItem):
     Mesh_class = Mesh
@@ -97,15 +99,15 @@
 
     def get_number_of_meshes_in_model(self) -> int:
         """
         Returns the number of ``Meshes`` in this ``Model``
         """
         return len(self.meshes)
 
-    def draw(self, parent, texture_id=0, color=None, switch=0, scale=None):
+    def draw(self, parent, texture_id=0, color=None, switch=0, scale=None, line_width=1):
         """
         Draw all ``Meshes`` for this ``Model``.
 
         :param parent: Parent object where this model was created.
         :param texture_id: Id of the ``Texture`` that needs to be applied.
         :type texture_id: ``int``
         :param color: color array rgb with alpha value
@@ -114,32 +116,36 @@
         :type switch: ``int``
         :param scale: ``list`` used for scaling the model
         :type scale:   ``list``
 
         """
 
         # draws all meshes
-        color = color if color else [0.0, 0.0, 0.0, 0.5]
-        for mesh in self.meshes:
-            mesh.draw(self.shader,
-                      model_id=self.model_id,
-                      position=parent.xyz,
-                      orientation=parent.orientation,
-                      scale=scale if scale else parent.scale,
-                      texture_id=texture_id,
-                      color=color,
-                      switch=switch
-                      )
+        try:
+            color = color if color else [0.0, 0.0, 0.0, 0.5]
+            for mesh in self.meshes:
+                mesh.draw(self.shader,
+                          model_id=self.model_id,
+                          position=parent.xyz,
+                          orientation=parent.orientation,
+                          scale=scale if scale else parent.scale,
+                          texture_id=texture_id,
+                          color=color,
+                          switch=switch,
+                          line_width=line_width)
+        except Exception as e:
+            dump_exception(e)
 
 # Do not remove these!!!
 # from sphere_base.shader.uv_skybox_shader import SkyboxShader
 # from sphere_base.shader.uv_sphere_shader import SphereShader
 # from sphere_base.shader.uv_node_shader import NodeShader
 # from sphere_base.shader.uv_socket_shader import SocketShader
 # from sphere_base.shader.uv_flat_shader import FlatShader
 # from sphere_base.shader.uv_default_shader import DefaultShader
 # from sphere_base.shader.uv_circle_shader import CircleShader
 # from sphere_base.shader.uv_square_shader import SquareShader
 # from sphere_base.shader.uv_sphere_edge_shader import SphereEdgeShader
 # from sphere_base.shader.uv_cross_shader import CrossShader
 # from sphere_base.shader.uv_holo_sphere_shader import HoloSphereShader
 # from sphere_base.shader.uv_sphere_small_shader import SphereSmallShader
+# from sphere_base.shader.drag_edge_shader import DragEdgeShader
```

### Comparing `sphere_base-0.1.1/sphere_base/model/models.py` & `sphere_base-0.1.2/sphere_base/model/models.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.1/sphere_base/model/obj_file_loader.py` & `sphere_base-0.1.2/sphere_base/model/obj_file_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,14 +140,16 @@
 
     @staticmethod
     def search_data(data_values, val_list, skip, data_type):
         # appends each data value found in the data value line to the val_list
         for d in data_values:
             if d == skip:
                 continue
+            elif d == '':
+                d = 0
             if data_type == 'float':
                 val_list.append(float(d))
             elif data_type == 'int':
                 val_list.append(int(d) - 1)
         return val_list
 
     @staticmethod
```

### Comparing `sphere_base-0.1.1/sphere_base/node/graphic_disc.py` & `sphere_base-0.1.2/sphere_base/node/graphic_disc.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.1/sphere_base/node/graphic_node.py` & `sphere_base-0.1.2/sphere_base/node/graphic_node.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.1/sphere_base/node/graphic_socket.py` & `sphere_base-0.1.2/sphere_base/node/graphic_socket.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.1/sphere_base/node/node.py` & `sphere_base-0.1.2/sphere_base/node/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
             - **serialized_detail_scene** - contains the ``json`` data of the detail node editor for this node.
             - **xyz** - ``Vector`` location of the ``node``.
 
         """
 
         super().__init__(node_type)
 
-        self.node_type_name = "node"
+        self.node_type_name = 'node'
         self.sphere = target_sphere
         self.config = self.sphere.config
         self.calc = self.sphere.calc
         self.node_disc = self.sphere.uv.models.get_model('node')
         self.circle = self.sphere.uv.models.get_model('circle')
         self.ray = self.sphere.uv.mouse_ray
 
@@ -214,15 +214,14 @@
         normal = self.calc.get_item_direction_pointing_outwards(self, self.sphere)
         return normal
 
     def update_position(self):
         """
         update the position of the node_disc on the sphere_base. Calculate the position and the direction.
         """
-
         self.xyz = self.get_position()
         self.orientation = self.get_orientation()
         self.socket.update_position()
 
         return self.xyz
 
     def update_collision_object(self):
```

### Comparing `sphere_base-0.1.1/sphere_base/node/socket.py` & `sphere_base-0.1.2/sphere_base/node/socket.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.1/sphere_base/serializable.py` & `sphere_base-0.1.2/sphere_base/serializable.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.1/sphere_base/shader/base_shader.py` & `sphere_base-0.1.2/sphere_base/shader/base_shader.py`

 * *Files 5% similar despite different names*

```diff
@@ -205,35 +205,32 @@
         if scale is None:
             scale = Vector3([1.0, 1.0, 1.0])
         else:
             scale = Vector3(scale)
 
         return matrix44.create_from_scale(scale)
 
-    def draw(self, object_index: int = 0, object_type: str = "", mesh_index: int = 0, indices_len=0,
-             position: 'Vector3' = None, orientation: 'Quaternion' = None,
-             scale: 'Vector3' = None, texture_id: int = 0, color: 'Vector4' = None,
-             switch: int = 0, ):
+    def draw(self, object_index: int = 0, object_type: str = "", mesh_index: int = 0, indices_len=0, position=None,
+             orientation=None, scale: 'Vector3' = None, texture_id: int = 0, color=None, switch: int = 0, line_width=1):
 
         """
 
         Needs to be extended
 
         Rendering and preparing the OpenGL shader
 
+        :param line_width:
         :param object_index: ID of the object
         :type object_index: ``int``
         :param object_type: Object type name
         :type object_type: ``str``
         :param mesh_index: ID of the Mesh
         :type mesh_index: ``int``
         :param indices_len: length of Indices
         :type indices_len: ``int``
-        :param vertices: List of vertex coordinates
-        :type indices: ``list``
         :param position: Position of the object
         :type position: ``Vector3``
         :param orientation: Orientation of the object
         :type orientation: ``Quaternion``
         :param scale: object scaling factor
         :type scale: ``Vector3``
         :param texture_id: ID of the texture to apply
@@ -273,52 +270,14 @@
         tm = matrix44.multiply(sm, rm)
         glUniformMatrix4fv(self.transform_loc, 1, GL_FALSE, tm)
 
     def draw_edge(self, points, width=1.5, color=None, dotted=False, switch=0):
         """
         Drawing edges. Using direct Open GL
 
-        :param points: list of Vector3 points positions
-        :type points: ``list``
-        :param width: width of the line
-        :type width: ``float``
-        :param color: color of the line
-        :type color: ``Vector4``
-        :param dotted: is the line dotted
-        :type dotted: ``bool``
-        :param switch: OpenGL switch
-        :type switch: ``int``
-
         .. Warning::
 
             This method is using obsolete direct OpenGL instead of modern OpenGL.
             This needs to be updated in a future iteration.
 
         """
-        # TODO: still needed do not remove yet
-        # drawing lines
-        glUseProgram(self.shader_id)  # using the standard shader
-        glUniform1i(self.switcher_loc, 3)  # switch to use fragment and vertex shader for lines
-        glLineWidth(width)
-
-        if color:
-            # enable blending
-            # glEnable(GL_BLEND)
-            glUniform4f(self.a_color, *color)
-            # glBlendFunc(GL_SRC_ALPHA, GL_ONE_MINUS_SRC_ALPHA)
-            glEnable(GL_LINE_SMOOTH)
-            glHint(GL_LINE_SMOOTH_HINT, GL_NICEST)
-
-        if dotted:
-            # dotted line for dragging
-            glLineStipple(4, 0xAAAA)
-            glEnable(GL_LINE_STIPPLE)
-        else:
-            # reset to normal
-            glDisable(GL_LINE_STIPPLE)
-
-        glBegin(GL_LINE_STRIP)
-        for point in points:
-            glVertex3f(point[0], point[1], point[2])
-        glEnd()
-        glDisable(GL_LINE_STIPPLE)  # just in case ....
-        glLineWidth(1)
+        return NotImplemented
```

### Comparing `sphere_base-0.1.1/sphere_base/shader/circle_shader.py` & `sphere_base-0.1.2/sphere_base/shader/circle_shader.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,21 +33,20 @@
             - **scale** - scaling of the circle
 
         """
 
         self.line_width = 1
         self.scale = [1.0, 1.0, 1.0]
 
-    def draw(self, object_index=0, object_type="", mesh_index=0, indices_len=0,
-             position=None, orientation=None, scale=None,
-             texture_id=0, color=None, switch: int = 0):
+    def draw(self, object_index=0, object_type="", mesh_index=0, indices_len=0, position=None, orientation=None,
+             scale=None, texture_id=0, color=None, switch: int = 0, line_width=1):
 
         super().draw(object_index=object_index, object_type=object_type, mesh_index=mesh_index, indices_len=indices_len,
-                     position=position, orientation=orientation, scale=scale, texture_id=texture_id,
-                     color=color, switch=switch)
+                     position=position, orientation=orientation, scale=scale, texture_id=texture_id, color=color,
+                     switch=switch, line_width=line_width)
 
         glLineWidth(self.line_width)
 
         rm = matrix44.create_from_inverse_of_quaternion(orientation)
         sm = self.create_scale_matrix(scale)
 
         # combined transformation matrix
```

### Comparing `sphere_base-0.1.1/sphere_base/shader/cross_shader.py` & `sphere_base-0.1.2/sphere_base/shader/cross_shader.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,21 +32,20 @@
             - **scale** - scaling of the circle
 
         """
 
         self.line_width = 1
         self.scale = [1.0, 1.0, 1.0]
 
-    def draw(self, object_index=0, object_type="", mesh_index=0, indices_len=0,
-             position=None, orientation=None, scale=None,
-             texture_id=0, color=None, switch=0):
+    def draw(self, object_index=0, object_type="", mesh_index=0, indices_len=0, position=None, orientation=None,
+             scale=None, texture_id=0, color=None, switch=0, line_width=1):
 
         super().draw(object_index=object_index, object_type=object_type, mesh_index=mesh_index, indices_len=indices_len,
-                     position=position, orientation=orientation, scale=scale, texture_id=texture_id,
-                     color=color, switch=switch)
+                     position=position, orientation=orientation, scale=scale, texture_id=texture_id, color=color,
+                     switch=switch, line_width=line_width)
 
         glLineWidth(self.line_width)
 
         rm = matrix44.create_from_inverse_of_quaternion(orientation)
         sm = self.create_scale_matrix(scale)
 
         # combined transformation matrix
```

### Comparing `sphere_base-0.1.1/sphere_base/shader/default_shader.py` & `sphere_base-0.1.2/sphere_base/shader/default_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.1/sphere_base/shader/edge_shader.py` & `sphere_base-0.1.2/sphere_base/shader/edge_shader.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,31 +3,28 @@
 """
 Dynamic shader. This is the dynamic shader class. It allows for dynamic shading lines and objects
 
 
 """
 
 from OpenGL.GL import *
-from pyrr import Vector3
 from sphere_base.shader.base_shader import BaseShader
 
 
 class EdgeShader(BaseShader):
 
-    def draw(self, object_index: int = 0, object_type: str = "", mesh_index: int = 0, indices_len=0,
-             position=None, orientation=None,
-             scale=None, texture_id: int = 0, color=None,
-             switch: int = 0, ):
+    def draw(self, object_index: int = 0, object_type: str = "", mesh_index: int = 0, indices_len=0, position=None,
+             orientation=None, scale=None, texture_id: int = 0, color=None, switch: int = 0, line_width=1):
 
         super().draw(object_index=object_index, object_type=object_type, mesh_index=mesh_index, indices_len=indices_len,
-                     position=position, orientation=orientation, scale=scale, texture_id=texture_id,
-                     color=color, switch=switch)
+                     position=position, orientation=orientation, scale=scale, texture_id=texture_id, color=color,
+                     switch=switch, line_width=line_width)
 
         glUniform4f(self.a_color, *color)
-        glLineWidth(2)
+        glLineWidth(line_width)
         glEnable(GL_CULL_FACE)
         glEnable(GL_POLYGON_SMOOTH)
         glEnable(GL_LINE_SMOOTH)
 
         glDrawElements(GL_LINE_STRIP, indices_len, GL_UNSIGNED_INT, ctypes.c_void_p(0))
 
         glDisable(GL_LINE_SMOOTH)
```

### Comparing `sphere_base-0.1.1/sphere_base/shader/flat_shader.py` & `sphere_base-0.1.2/sphere_base/shader/sphere_small_shader.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,35 @@
 # -*- coding: utf-8 -*-
 
+"""
+This class contains the class that colors the small overview spheres. It inherits from the base shader class.
+
+"""
 
 from OpenGL.GL import *
 from OpenGL.GLU import *
 from sphere_base.shader.base_shader import BaseShader
 
 
-class FlatShader(BaseShader):
+class SphereSmallShader(BaseShader):
 
-    def draw(self, object_index=0, object_type="", mesh_index=0, indices_len=0,
-             position=None, orientation=None, scale=None, texture_id=0,
-             color=None, switch=0):
+    def _init_locations(self):
+        """
+        Initiates the OpenGL locations
+
+        """
+        super()._init_locations()
+        self.switcher_loc = glGetUniformLocation(self.shader_id, "switcher")
 
-        scale = [scale[0] * .97, scale[1] * .97, scale[2]]
+    def draw(self, object_index=0, object_type="", mesh_index=0, indices_len=0, position=None, orientation=None,
+             scale=None, texture_id=0, color=None, switch=0, line_width=1):
 
         super().draw(object_index=object_index, object_type=object_type, mesh_index=mesh_index, indices_len=indices_len,
-                     position=position, orientation=orientation, scale=scale, texture_id=texture_id,
-                     color=color, switch=switch)
+                     position=position, orientation=orientation, scale=scale, texture_id=texture_id, color=color,
+                     switch=switch, line_width=line_width)
 
-        if object_type == "rubber_band":
-            glUniform4f(self.a_color, *color)
+        glUniform1i(self.switcher_loc, 2)
 
+        glUniform4f(self.a_color, *color)
+        glEnable(GL_CULL_FACE)
         glDrawElements(GL_TRIANGLES, indices_len * 3, GL_UNSIGNED_INT, ctypes.c_void_p(0))
+        glDisable(GL_CULL_FACE)
```

### Comparing `sphere_base-0.1.1/sphere_base/shader/holo_sphere_shader.py` & `sphere_base-0.1.2/sphere_base/shader/node_shader.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,41 +3,30 @@
 """
 Node shader module. This module contains the Node shader class which inherits from the base shader class.
 It is used to render nodes
 
 """
 
 from OpenGL.GL import *
+from OpenGL.GLU import *
 from sphere_base.shader.base_shader import BaseShader
 
 
-class HoloSphereShader(BaseShader):
+class NodeShader(BaseShader):
 
     def _init_locations(self):
         """
         Initiates the OpenGL locations
 
         """
         super()._init_locations()
         self.switcher_loc = glGetUniformLocation(self.shader_id, "switcher")
 
-    def draw(self, object_index=0, object_type="", mesh_index=0, indices_len=0,
-             position=None, orientation=None, scale=None, texture_id=0, texture_file="", color=None, switch=0):
+    def draw(self, object_index=0, object_type="", mesh_index=0, indices_len=0, position=None, orientation=None,
+             scale=None, texture_id=0, color=None, switch=0, line_width=1):
 
         super().draw(object_index=object_index, object_type=object_type, mesh_index=mesh_index, indices_len=indices_len,
-                     position=position, orientation=orientation, scale=scale, texture_id=texture_id,
-                     color=color, switch=switch)
+                     position=position, orientation=orientation, scale=scale, texture_id=texture_id, color=color,
+                     switch=switch, line_width=line_width)
 
         glUniform1i(self.switcher_loc, switch)
-        glUniform4f(self.a_color, *color)
-
-        # One way to draw with indexes
-        glEnable(GL_CULL_FACE)
         glDrawElements(GL_TRIANGLES, indices_len * 3, GL_UNSIGNED_INT, ctypes.c_void_p(0))
-
-        # alternative possibility drawing arrays.....
-        # glDrawArrays(GL_TRIANGLES, 0, len(vertices))
-        glDisable(GL_CULL_FACE)
-        glStencilFunc(GL_ALWAYS, object_index, -1)
-
-
-
```

### Comparing `sphere_base-0.1.1/sphere_base/shader/node_shader.py` & `sphere_base-0.1.2/sphere_base/shader/flat_shader.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,23 @@
 # -*- coding: utf-8 -*-
 
-"""
-Node shader module. This module contains the Node shader class which inherits from the base shader class.
-It is used to render nodes
-
-"""
 
 from OpenGL.GL import *
 from OpenGL.GLU import *
 from sphere_base.shader.base_shader import BaseShader
 
 
-class NodeShader(BaseShader):
+class FlatShader(BaseShader):
+
+    def draw(self, object_index=0, object_type="", mesh_index=0, indices_len=0, position=None, orientation=None,
+             scale=None, texture_id=0, color=None, switch=0, line_width=1):
 
-    def _init_locations(self):
-        """
-        Initiates the OpenGL locations
-
-        """
-        super()._init_locations()
-        self.switcher_loc = glGetUniformLocation(self.shader_id, "switcher")
-
-    def draw(self, object_index=0, object_type="", mesh_index=0, indices_len=0,
-             position=None, orientation=None, scale=None, texture_id=0, texture_file="",
-             color=None, switch=0):
+        scale = [scale[0] * .97, scale[1] * .97, scale[2]]
 
         super().draw(object_index=object_index, object_type=object_type, mesh_index=mesh_index, indices_len=indices_len,
-                     position=position, orientation=orientation, scale=scale, texture_id=texture_id,
-                     color=color, switch=switch)
+                     position=position, orientation=orientation, scale=scale, texture_id=texture_id, color=color,
+                     switch=switch, line_width=line_width)
+
+        if object_type == "rubber_band":
+            glUniform4f(self.a_color, *color)
 
-        glUniform1i(self.switcher_loc, switch)
         glDrawElements(GL_TRIANGLES, indices_len * 3, GL_UNSIGNED_INT, ctypes.c_void_p(0))
```

### Comparing `sphere_base-0.1.1/sphere_base/shader/skybox_shader.py` & `sphere_base-0.1.2/sphere_base/shader/skybox_shader.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,17 +40,16 @@
 
         glTexParameteri(GL_TEXTURE_CUBE_MAP, GL_TEXTURE_MIN_FILTER, GL_LINEAR)
         glTexParameteri(GL_TEXTURE_CUBE_MAP, GL_TEXTURE_MAG_FILTER, GL_LINEAR)
         glTexParameteri(GL_TEXTURE_CUBE_MAP, GL_TEXTURE_WRAP_S, GL_CLAMP_TO_EDGE)
         glTexParameteri(GL_TEXTURE_CUBE_MAP, GL_TEXTURE_WRAP_T, GL_CLAMP_TO_EDGE)
         glTexParameteri(GL_TEXTURE_CUBE_MAP, GL_TEXTURE_WRAP_R, GL_CLAMP_TO_EDGE)
 
-    def draw(self, object_index=0, object_type="", mesh_index=0, indices_len=0,
-             position=None, orientation=None, scale=None, texture_id=0,
-             color=None, switch=0):
+    def draw(self, object_index=0, object_type="", mesh_index=0, indices_len=0, position=None, orientation=None,
+             scale=None, texture_id=0, color=None, switch=0, line_width=1):
 
         glUseProgram(self.shader_id)
         # glUniformMatrix4fv(self.view_loc, 1, GL_FALSE, self.config.view_loc)
 
         glBindVertexArray(self.config.VAO[mesh_index])
 
         obj_pos = matrix44.create_from_translation(Vector3(self.config.uv.cam.xyz))
```

### Comparing `sphere_base-0.1.1/sphere_base/shader/socket_shader.py` & `sphere_base-0.1.2/sphere_base/shader/socket_shader.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,21 +17,20 @@
         """
         Initiates the OpenGL locations
 
         """
         super()._init_locations()
         self.switcher_loc = glGetUniformLocation(self.shader_id, "switcher")
 
-    def draw(self, object_index=0, object_type="", mesh_index=0, indices_len=0,
-             position=None, orientation=None, scale=None, texture_id=0,
-             color=None, switch=0):
+    def draw(self, object_index=0, object_type="", mesh_index=0, indices_len=0, position=None, orientation=None,
+             scale=None, texture_id=0, color=None, switch=0, line_width=1):
 
         super().draw(object_index=object_index, object_type=object_type, mesh_index=mesh_index, indices_len=indices_len,
-                     position=position, orientation=orientation, scale=scale, texture_id=texture_id,
-                     color=color, switch=switch)
+                     position=position, orientation=orientation, scale=scale, texture_id=texture_id, color=color,
+                     switch=switch, line_width=line_width)
 
         # switch = SHADER_SWITCH[object_type]
         glUniform1i(self.switcher_loc, 2)
 
         glUniform4f(self.a_color, *color)
 
         glDrawElements(GL_TRIANGLES, indices_len * 3, GL_UNSIGNED_INT, ctypes.c_void_p(0))
```

### Comparing `sphere_base-0.1.1/sphere_base/shader/sphere_edge_shader.py` & `sphere_base-0.1.2/sphere_base/shader/sphere_edge_shader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 """
 Sphere edge shader module. This module contains the edge shader class which inherits from the base shader class.
 It is used to render edges between spheres.
 
-It works different than the other shaders as it does not use indices.
+It works different from the other shaders as it does not use indices.
 
     - Each shader instance holds one edge
 
 
 """
 
 from OpenGL.GL import *
@@ -18,28 +18,27 @@
 
 
 class SphereEdgeShader(BaseShader):
     def __init__(self, parent, vertex_shader=None, fragment_shader=None, geometry_shader=None):
         super().__init__(parent, vertex_shader=vertex_shader, fragment_shader=fragment_shader,
                          geometry_shader=geometry_shader)
 
-
     def _init_locations(self):
         """
         Initiates the OpenGL locations
 
         """
         super()._init_locations()
         self.switcher_loc = glGetUniformLocation(self.shader_id, "switcher")
         self.vertices = []
         self.buffer = np.array(self.vertices, dtype=np.float32)
         self.vertices = np.array(self.vertices, dtype=np.float32)
 
-    def draw(self, object_index=0, object_type="", mesh_index=0, indices_len=0, position=None,
-             orientation=None, scale=None, texture_id=0, color=None, switch=0):
+    def draw(self, object_index=0, object_type="", mesh_index=0, indices_len=0, position=None, orientation=None,
+             scale=None, texture_id=0, color=None, switch=0, line_width=1):
 
         print("mesh_index", self.vertices)
         color = [0, 0, 0, 1]
 
         print("----------------- variables for drawing -----------------")
         print("object_index", object_index)
         print("object_type", object_type)
@@ -62,16 +61,14 @@
         #              scale=scale,
         #              texture_id=texture_id,
         #              color=color,
         #              switch=switch)
 
         # ------------------------------
 
-
-
         glBindVertexArray(self.mesh_index)
 
         glBindBuffer(GL_ARRAY_BUFFER, self.buffer_id)
         glBufferData(GL_ARRAY_BUFFER, len(self.vertices), self.vertices, GL_STATIC_DRAW)
 
         # print(mesh_index, self.vertices)
```

### Comparing `sphere_base-0.1.1/sphere_base/shader/sphere_shader.py` & `sphere_base-0.1.2/sphere_base/shader/holo_sphere_shader.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,47 +1,43 @@
 # -*- coding: utf-8 -*-
 
 """
-Sphere shader module. This module contains the Sphere shader class which inherits from the base shader class.
-It is used to render Sphere
+Node shader module. This module contains the Node shader class which inherits from the base shader class.
+It is used to render nodes
 
 """
 
 from OpenGL.GL import *
-from OpenGL.GLU import *
 from sphere_base.shader.base_shader import BaseShader
 
-from sphere_base.constants import *
 
+class HoloSphereShader(BaseShader):
 
-class SphereShader(BaseShader):
     def _init_locations(self):
         """
         Initiates the OpenGL locations
 
         """
         super()._init_locations()
-        self.light_id = glGetUniformLocation(self.shader_id, "LightPosition_world_space")
         self.switcher_loc = glGetUniformLocation(self.shader_id, "switcher")
 
-    def set_buffer_bits(self):
-        super().set_buffer_bits()
-
-    def draw(self, object_index=0, object_type="", mesh_index=0, indices_len=0, position=None,
-             orientation=None, scale=None, texture_id=0, color=None, switch=0):
+    def draw(self, object_index=0, object_type="", mesh_index=0, indices_len=0, position=None, orientation=None,
+             scale=None, texture_id=0, color=None, switch=0, line_width=1):
 
         super().draw(object_index=object_index, object_type=object_type, mesh_index=mesh_index, indices_len=indices_len,
-                     position=position, orientation=orientation, scale=scale, texture_id=texture_id,
-                     color=color, switch=switch)
+                     position=position, orientation=orientation, scale=scale, texture_id=texture_id, color=color,
+                     switch=switch, line_width=line_width)
 
-        # switch between shaders per object_type
-        switch = SHADER_SWITCH[object_type]
         glUniform1i(self.switcher_loc, switch)
+        glUniform4f(self.a_color, *color)
 
-        # Using element arrays
+        # One way to draw with indexes
+        glEnable(GL_CULL_FACE)
         glDrawElements(GL_TRIANGLES, indices_len * 3, GL_UNSIGNED_INT, ctypes.c_void_p(0))
 
         # alternative possibility drawing arrays.....
         # glDrawArrays(GL_TRIANGLES, 0, len(vertices))
-
+        glDisable(GL_CULL_FACE)
         glStencilFunc(GL_ALWAYS, object_index, -1)
 
+
+
```

### Comparing `sphere_base-0.1.1/sphere_base/shader/sphere_small_shader.py` & `sphere_base-0.1.2/sphere_base/shader/sphere_shader.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,47 @@
 # -*- coding: utf-8 -*-
 
 """
-This class contains the class that colors the small overview spheres. It inherits from the base shader class.
+Sphere shader module. This module contains the Sphere shader class which inherits from the base shader class.
+It is used to render Sphere
 
 """
 
 from OpenGL.GL import *
 from OpenGL.GLU import *
 from sphere_base.shader.base_shader import BaseShader
 
+from sphere_base.constants import *
 
-class SphereSmallShader(BaseShader):
 
+class SphereShader(BaseShader):
     def _init_locations(self):
         """
         Initiates the OpenGL locations
 
         """
         super()._init_locations()
+        self.light_id = glGetUniformLocation(self.shader_id, "LightPosition_world_space")
         self.switcher_loc = glGetUniformLocation(self.shader_id, "switcher")
 
-    def draw(self, object_index=0, object_type="", mesh_index=0, indices_len=0, vertices=None, position=None,
-             orientation=None, scale=None, texture_id=0, color=None, switch=0):
+    def set_buffer_bits(self):
+        super().set_buffer_bits()
+
+    def draw(self, object_index=0, object_type="", mesh_index=0, indices_len=0, position=None, orientation=None,
+             scale=None, texture_id=0, color=None, switch=0, line_width=1):
 
         super().draw(object_index=object_index, object_type=object_type, mesh_index=mesh_index, indices_len=indices_len,
-                     position=position, orientation=orientation, scale=scale, texture_id=texture_id,
-                     color=color, switch=switch)
+                     position=position, orientation=orientation, scale=scale, texture_id=texture_id, color=color,
+                     switch=switch, line_width=line_width)
 
-        glUniform1i(self.switcher_loc, 2)
+        # switch between shaders per object_type
+        switch = SHADER_SWITCH[object_type]
+        glUniform1i(self.switcher_loc, switch)
 
-        glUniform4f(self.a_color, *color)
-        glEnable(GL_CULL_FACE)
+        # Using element arrays
         glDrawElements(GL_TRIANGLES, indices_len * 3, GL_UNSIGNED_INT, ctypes.c_void_p(0))
-        glDisable(GL_CULL_FACE)
+
+        # alternative possibility drawing arrays.....
+        # glDrawArrays(GL_TRIANGLES, 0, len(vertices))
+
+        glStencilFunc(GL_ALWAYS, object_index, -1)
+
```

### Comparing `sphere_base-0.1.1/sphere_base/shader/square_shader.py` & `sphere_base-0.1.2/sphere_base/shader/square_shader.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,20 +27,20 @@
         Adds a scale location to the geometric shader to. This scale is the fraction used to
         correctly scale the border box of size 1 by 1
 
         """
         super()._init_locations()
         self.scale_loc = glGetUniformLocation(self.shader_id, "scale")
 
-    def draw(self, object_index=0, object_type="", mesh_index=0, indices_len=0, position=None,
-             orientation=None, scale=None, texture_id=0, color=None, switch=0):
+    def draw(self, object_index=0, object_type="", mesh_index=0, indices_len=0, position=None, orientation=None,
+             scale=None, texture_id=0, color=None, switch=0, line_width=1):
 
         super().draw(object_index=object_index, object_type=object_type, mesh_index=mesh_index, indices_len=indices_len,
-                     position=position, orientation=orientation, scale=scale, texture_id=texture_id,
-                     color=color, switch=switch)
+                     position=position, orientation=orientation, scale=scale, texture_id=texture_id, color=color,
+                     switch=switch, line_width=line_width)
 
         glLineWidth(self.line_width)
         glUniform3f(self.scale_loc, *scale)  # sending the size of the box to the geometric shader
 
         glDrawElements(GL_POINTS, indices_len * 3, GL_UNSIGNED_INT, ctypes.c_void_p(0))
         glStencilFunc(GL_ALWAYS, object_index, -1)
         glLineWidth(1)
```

### Comparing `sphere_base-0.1.1/sphere_base/sphere/sphere.py` & `sphere_base-0.1.2/sphere_base/sphere/sphere.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from random import *
 from sphere_base.serializable import Serializable
 from sphere_base.utils import dump_exception
 from collections import OrderedDict
 from sphere_base.node.node import Node
 from sphere_base.edge.edge_drag import EdgeDrag
 from sphere_base.edge.surface_edge import SurfaceEdge
+from sphere_base.sphere.sphere_lines import SphereLines
 from sphere_base.history import History
 from pyrr import quaternion
 from math import pi
 from sphere_base.calc import Calc
 from sphere_base.constants import *
 import numpy as np
 import pyperclip
@@ -95,15 +96,15 @@
         self.start_socket = None
         self._hovered_item = None
         self.animation = 0  # rotation speed
         self.node_class_selector = None
 
         self.selected_item = None
         self._last_selected_items = None
-        # self.last_collision_point = None
+
         self.items = []
         self.items_selected = []
         self.items_deselected = []
         self._selection_changed_listeners = []
         self._items_deselected_listeners = []
         self._has_been_modified_listeners = []
 
@@ -119,14 +120,19 @@
 
         self.xyz = position if position else ([randint(-25, 25), randint(-25, 25), randint(-25, 25)])
         self.texture_id = texture_id if texture_id or texture_id == 0 else randint(1, 5)
 
         self.collision_shape_id = self.uv.mouse_ray.get_collision_shape(self)
         self.collision_object_id = self.uv.mouse_ray.create_collision_object(self)
 
+        self.sphere_lines_mayor = SphereLines(self, 20, 20, 0, [0.5, 0, 0, 0.05], 4)  # red lines
+        self.sphere_lines_minor = SphereLines(self, 40, 40, 0, [0.3, 0.3, 0.5, 0.1], 3)  # blue lines
+        self.sphere_lines_micro = SphereLines(self, 100, 100, 0, [0, 0, 0, 0.1], 1)  # black lines
+        self.sphere_lines_nano = SphereLines(self, 200, 200, 0, [0, 0, 0, 0.03], 1, 7)  # close distance only
+
         # for testing purposes a number of random nodes can be created
         # self.create_test_node(NUMBER_OF_TEST_NODES)
 
         # add the sphere_base to the universe
         self.uv.add_sphere(self)
         self.history.store_initial_history_stamp()
 
@@ -398,15 +404,15 @@
 
             This method only explicitly instructs nodes to update themselves.
             updating nodes will trickle down, causing the connected node socket and connected edges to update as well.
         """
 
         # update orientation of all nodes on sphere_base
         for item in self.items:
-            if item.type == "node":
+            if item.type in ('node', 'sphere_lines'):
                 # updating the node trickles down to updating sockets and edges"
                 item.update_position()
 
     def rotate_sphere(self, offset_degrees: int):
         """
         Rotating the sphere_base over the y-axis as per the offset_degrees.
 
@@ -539,19 +545,21 @@
             self._hovered_item.set_hovered(False)
             self._hovered_item = None
 
         if hovered_item and hovered_item != self.id:
             for item in self.items:
                 if item.id == hovered_item:
                     # set hover
-                    item.set_hovered(True)
-                    self._hovered_item = item
+                    if item.type in ('node', 'socket', 'edge'):
+                        item.set_hovered(True)
+                        self._hovered_item = item
                 else:
                     # remove hover
-                    item.set_hovered(False)
+                    if item.type in ('node', 'socket', 'edge'):
+                        item.set_hovered(False)
 
         return self._hovered_item
 
     def edit_cut(self):
         """
         Cut _selected sphere_base items to clipboard
         """
@@ -633,20 +641,22 @@
         """
         Render the sphere_base and all the items on it.
         """
 
         if self.animation != 0:
             self.rotate_sphere(self.animation)
 
-        self.model.draw(self, texture_id=self.texture_id,  color=self.color)
+        self.model.draw(self, texture_id=self.texture_id, color=self.color)
         for item in self.items:
             if item.type == "node":
                 item.draw()
             elif item.type == "edge":
                 item.draw()
+            elif item.type == "sphere_lines":
+                item.draw()
 
         if self.edge_drag.dragging:
             self.edge_drag.draw()
 
     def serialize(self):
         nodes, edges = [], []
         for item in self.items:
```

### Comparing `sphere_base-0.1.1/sphere_base/sphere_overlay/sov_conf.py` & `sphere_base-0.1.2/sphere_base/sphere_overlay/sov_conf.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.1/sphere_base/sphere_overlay/sov_sphere.py` & `sphere_base-0.1.2/sphere_base/sphere_overlay/sov_sphere.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,60 +17,52 @@
     def __init__(self, universe, position=None, texture_id=None):
         super().__init__(universe, position, texture_id)
 
         self.set_node_class_selector(self.get_node_class_from_data)
         self._close_event_listeners = []
         self.billboard_id = random.randint(30, 31)
 
-
     def get_model(self):
-        # self.cube = self.uv.models.get_model('cube') #model in the middle of the globe
-        self.model_h = self.uv.models.get_model('holo_sphere')
-        self.model = self.uv.models.get_model('sphere_base')
-        self.shader = self.model.shader
+        self.model = self.uv.models.get_model('holo_sphere')
 
     def get_node_class_from_data(self, data):
         if 'op_code' not in data:
             return self.Node
         return get_class_from_type(data['op_code'], SPHERE_NODE_EDITOR)
 
     def create_new_node(self, node_type=0, mouse_ray_collision_point=None):
-        # create new node at the mouse pointer
+        node = None
 
         # calculate the cumulative angle based on the mouse position
         orientation = self.calc.find_angle(mouse_ray_collision_point, self.orientation)
 
-        # create new node at the cumulative angle
-
         try:
 
             if node_type:
-
                 node = get_class_from_type(node_type, SPHERE_NODE_EDITOR)(self, orientation_offset=orientation)
             else:
                 node = self.Node(self, orientation)
 
         except Exception as e:
             dump_exception(e)
 
         self.history.store_history("node created", True)
         return node
 
-    def draw(self):
-        """
-        Render the sphere_base and all the items on it.
-        """
-
-        if self.animation != 0:
-            self.rotate_sphere(self.animation)
-
-        # self.cube.draw(self, self.billboard_id, scale=[0.5, 0.5, 0.5])
-        self.model_h.draw(self, texture_id=self.texture_id, color=self.color)
-
-        for item in self.items:
-            if item.type == "node":
-                item.draw()
-            elif item.type == "edge":
-                item.draw()
-
-        if self.edge_drag.dragging:
-            self.edge_drag.draw()
+    # def draw(self):
+    #     """
+    #     Render the sphere_base and all the items on it.
+    #     """
+    #
+    #     if self.animation != 0:
+    #         self.rotate_sphere(self.animation)
+    #
+    #     self.model.draw(self, texture_id=self.texture_id, color=self.color)
+    #
+    #     for item in self.items:
+    #         if item.type == "node":
+    #             item.draw()
+    #         elif item.type == "edge":
+    #             item.draw()
+    #
+    #     if self.edge_drag.dragging:
+    #         self.edge_drag.draw()
```

### Comparing `sphere_base-0.1.1/sphere_base/sphere_overlay/sov_sphere_node_base.py` & `sphere_base-0.1.2/sphere_base/sphere_overlay/sov_sphere_node_base.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.1/sphere_base/sphere_overlay/sphere_nodes/item_sphere_node.py` & `sphere_base-0.1.2/sphere_base/sphere_overlay/sphere_nodes/item_sphere_node.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.1/sphere_base/sphere_overlay/sphere_nodes/person_sphere_node.py` & `sphere_base-0.1.2/sphere_base/sphere_overlay/sphere_nodes/person_sphere_node.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.1/sphere_base/sphere_universe_base/suv_cam.py` & `sphere_base-0.1.2/sphere_base/sphere_universe_base/suv_cam.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.1/sphere_base/sphere_universe_base/suv_cam_movement.py` & `sphere_base-0.1.2/sphere_base/sphere_universe_base/suv_cam_movement.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.1/sphere_base/sphere_universe_base/suv_mouse_ray.py` & `sphere_base-0.1.2/sphere_base/sphere_universe_base/suv_mouse_ray.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.1/sphere_base/sphere_universe_base/suv_rubber_band.py` & `sphere_base-0.1.2/sphere_base/sphere_universe_base/suv_rubber_band.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.1/sphere_base/sphere_universe_base/suv_skybox.py` & `sphere_base-0.1.2/sphere_base/sphere_universe_base/suv_skybox.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.1/sphere_base/sphere_universe_base/suv_universe.py` & `sphere_base-0.1.2/sphere_base/sphere_universe_base/suv_universe.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.1/sphere_base/sphere_universe_base/suv_widget.py` & `sphere_base-0.1.2/sphere_base/sphere_universe_base/suv_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -233,15 +233,16 @@
                         # if edge does not already exist, create it
                         self.uv.target_sphere.create_edge(item.socket)
             except Exception as e:
                 dump_exception(e)
 
         if self._middle_mouse_button_down:
             for item in self.uv.target_sphere.items:
-                item.update_collision_object()
+                if item.type in ('sphere', 'edge', 'node', 'socket'):
+                    item.update_collision_object()
 
         self._reset_mouse()
 
     def mouseMoveEvent(self, event: 'event'):
         """
         Handles mouse release event
```

### Comparing `sphere_base-0.1.1/sphere_base/utils.py` & `sphere_base-0.1.2/sphere_base/utils.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.1/sphere_base.egg-info/PKG-INFO` & `sphere_base-0.1.2/sphere_base.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: sphere-base
-Version: 0.1.1
-Summary: The library was created to be used as a building block for applications were informationshould appear on the surface of a sphere. It allows for creating spheres with nodesand edges that can be dragged on its surface. Nodes and edges can be placed and removed from the sphere surface. 
+Version: 0.1.2
+Summary: library for applications were information should appear on the surface of a sphere. It allows for creating spheres with nodes and edges that can be dragged on its surface. 
 Home-page: https://github.com/rboltze/spherebase
 Author: Richard Boltze
 Author-email: rboltze@protonmail.com
 License: MIT license
 Keywords: sphere_base
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -20,48 +20,59 @@
 Sphere Base
 ############
 
 Introduction
 =============
 
 This library was created as a building block for use in applications were information should be displayed as nodes or
-labels on a sphere. These nodes are interactive so they can be moved by dragging and connecting them to other nodes.
+labels on a sphere. These nodes are interactive so they can be moved by dragging and can be connected to other nodes.
 
-This package is created in python using a pyqt5 window.
 
-* Development Status :: 4 - Beta
+* Development Status: 4 - Beta
 * Free software: MIT license
 
 
 Features
 =========
 
 - Customizable spheres with textures and colors
 - Nodes, sockets and edges can be dragged over the surface of the sphere
 - Support for undo/redo, cut and paste using serialization
 - Hovering effects, dragging nodes, cutting edges
+- Background skybox image can be changed
+- Sphere color and texture can be changed
 - Example on how the library can be implemented
 
+
 Requirements
 =============
 
+This package is created in python using a pyqt5 window.
+
 - Python 3.x
 - PyOpenGL
 - PyQt5
+- pyperclip
+- pybullet
+- Pillow
+- numpy
 
 
 Supported Environment
 ======================
 
 * Windows (Win32, x64)
 
 
 The library is available from PyPI
 
-    $ pip install sphere-base==0.0.1
+    $ pip install sphere-base
+
+
+
 
 
 Or download the source code from github
 
     git clone https://github.com/rboltze/sphere_base.git
```

### Comparing `sphere_base-0.1.1/sphere_base.egg-info/SOURCES.txt` & `sphere_base-0.1.2/sphere_base.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -88,41 +88,53 @@
 sphere_base/edge/inter_sphere_edge.py
 sphere_base/edge/surface_edge.py
 sphere_base/model/__init__.py
 sphere_base/model/mesh.py
 sphere_base/model/model.py
 sphere_base/model/models.py
 sphere_base/model/obj_file_loader.py
+sphere_base/model/resources/__init__.py
+sphere_base/model/resources/icons/__init__.py
+sphere_base/model/resources/images/__init__.py
+sphere_base/model/resources/meshes/__init__.py
+sphere_base/model/resources/shaders/__init__.py
+sphere_base/model/resources/sphere_textures/__init__.py
+sphere_base/model/resources/textures/__init__.py
 sphere_base/node/__init__.py
 sphere_base/node/graphic_disc.py
 sphere_base/node/graphic_node.py
 sphere_base/node/graphic_socket.py
 sphere_base/node/node.py
 sphere_base/node/socket.py
 sphere_base/shader/__init__.py
 sphere_base/shader/base_shader.py
 sphere_base/shader/circle_shader.py
 sphere_base/shader/cross_shader.py
 sphere_base/shader/default_shader.py
+sphere_base/shader/drag_edge_shader.py
 sphere_base/shader/edge_shader.py
 sphere_base/shader/flat_shader.py
 sphere_base/shader/holo_sphere_shader.py
 sphere_base/shader/node_shader.py
 sphere_base/shader/skybox_shader.py
 sphere_base/shader/socket_shader.py
 sphere_base/shader/sphere_edge_shader.py
 sphere_base/shader/sphere_shader.py
 sphere_base/shader/sphere_small_shader.py
 sphere_base/shader/square_shader.py
 sphere_base/sphere/__init__.py
 sphere_base/sphere/sphere.py
+sphere_base/sphere/sphere_lines.py
 sphere_base/sphere_overlay/__init__.py
 sphere_base/sphere_overlay/sov_conf.py
 sphere_base/sphere_overlay/sov_sphere.py
 sphere_base/sphere_overlay/sov_sphere_node_base.py
+sphere_base/sphere_overlay/icons/__init__.py
+sphere_base/sphere_overlay/qss/__init__.py
+sphere_base/sphere_overlay/qss/nodeeditor_dark_resources.py
 sphere_base/sphere_overlay/sphere_nodes/__init__.py
 sphere_base/sphere_overlay/sphere_nodes/edge_sphere_item.py
 sphere_base/sphere_overlay/sphere_nodes/item_sphere_node.py
 sphere_base/sphere_overlay/sphere_nodes/person_sphere_node.py
 sphere_base/sphere_universe_base/__init__.py
 sphere_base/sphere_universe_base/suv_cam.py
 sphere_base/sphere_universe_base/suv_cam_movement.py
```

### Comparing `sphere_base-0.1.1/tests/test_000_import.py` & `sphere_base-0.1.2/tests/test_000_import.py`

 * *Files identical despite different names*

