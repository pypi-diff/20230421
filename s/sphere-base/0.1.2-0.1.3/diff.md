# Comparing `tmp/sphere_base-0.1.2.tar.gz` & `tmp/sphere_base-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphere_base-0.1.2.tar", last modified: Fri Apr 21 08:51:17 2023, max compression
+gzip compressed data, was "sphere_base-0.1.3.tar", last modified: Fri Apr 21 09:00:59 2023, max compression
```

## Comparing `sphere_base-0.1.2.tar` & `sphere_base-0.1.3.tar`

### file list

```diff
@@ -1,176 +1,180 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 08:51:17.418788 sphere_base-0.1.2/
--rw-rw-rw-   0        0        0      978 2023-04-16 07:19:30.000000 sphere_base-0.1.2/HISTORY.rst
--rw-rw-rw-   0        0        0     1105 2023-04-16 08:54:46.000000 sphere_base-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      252 2023-03-15 14:22:33.000000 sphere_base-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1987 2023-04-21 08:51:17.417788 sphere_base-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1205 2023-04-21 08:51:12.000000 sphere_base-0.1.2/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-21 08:51:16.950761 sphere_base-0.1.2/docs/
--rw-rw-rw-   0        0        0      638 2023-03-15 17:55:12.000000 sphere_base-0.1.2/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-04-21 08:51:16.934760 sphere_base-0.1.2/docs/build/
-drwxrwxrwx   0        0        0        0 2023-04-21 08:51:16.935761 sphere_base-0.1.2/docs/build/html/
-drwxrwxrwx   0        0        0        0 2023-04-21 08:51:16.954762 sphere_base-0.1.2/docs/build/html/_static/
--rw-rw-rw-   0        0        0      286 2023-03-15 17:53:40.000000 sphere_base-0.1.2/docs/build/html/_static/file.png
--rw-rw-rw-   0        0        0       90 2023-03-15 17:53:40.000000 sphere_base-0.1.2/docs/build/html/_static/minus.png
--rw-rw-rw-   0        0        0       90 2023-03-15 17:53:40.000000 sphere_base-0.1.2/docs/build/html/_static/plus.png
--rwxrwxrwx   0        0        0      804 2023-03-15 17:55:12.000000 sphere_base-0.1.2/docs/make.bat
-drwxrwxrwx   0        0        0        0 2023-04-21 08:51:16.957762 sphere_base-0.1.2/docs/source/
--rw-rw-rw-   0        0        0     1175 2023-03-16 20:29:33.000000 sphere_base-0.1.2/docs/source/conf.py
--rw-rw-rw-   0        0        0      489 2023-03-16 21:15:47.000000 sphere_base-0.1.2/docs/source/index.rst
-drwxrwxrwx   0        0        0        0 2023-04-21 08:51:17.077769 sphere_base-0.1.2/docs/source/rst/
--rw-rw-rw-   0        0        0      163 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.model.mesh.rst
--rw-rw-rw-   0        0        0      166 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.model.model.rst
--rw-rw-rw-   0        0        0      169 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.model.models.rst
--rw-rw-rw-   0        0        0      200 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.model.obj_file_loader.rst
--rw-rw-rw-   0        0        0      369 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.model.rst
--rw-rw-rw-   0        0        0      196 2023-03-16 21:18:48.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.rst
--rw-rw-rw-   0        0        0      780 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.shader.rst
--rw-rw-rw-   0        0        0      200 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.shader.uv_base_shader.rst
--rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.shader.uv_circle_shader.rst
--rw-rw-rw-   0        0        0      203 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.shader.uv_cross_shader.rst
--rw-rw-rw-   0        0        0      209 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.shader.uv_default_shader.rst
--rw-rw-rw-   0        0        0      200 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.shader.uv_flat_shader.rst
--rw-rw-rw-   0        0        0      223 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.shader.uv_holo_sphere_shader.rst
--rw-rw-rw-   0        0        0      200 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.shader.uv_node_shader.rst
--rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.shader.uv_skybox_shader.rst
--rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.shader.uv_socket_shader.rst
--rw-rw-rw-   0        0        0      223 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.shader.uv_sphere_edge_shader.rst
--rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.shader.uv_sphere_shader.rst
--rw-rw-rw-   0        0        0      226 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.shader.uv_sphere_small_shader.rst
--rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.shader.uv_square_shader.rst
--rw-rw-rw-   0        0        0      602 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_overlay.rst
--rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_overlay.sov_conf.rst
--rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_overlay.sov_edge.rst
--rw-rw-rw-   0        0        0      212 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_overlay.sov_sphere.rst
--rw-rw-rw-   0        0        0      246 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_overlay.sov_sphere_node_base.rst
--rw-rw-rw-   0        0        0      223 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_overlay.sov_uv_widget.rst
--rw-rw-rw-   0        0        0      273 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_overlay.sphere_nodes.edge_sphere_item.rst
--rw-rw-rw-   0        0        0      273 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_overlay.sphere_nodes.item_sphere_node.rst
--rw-rw-rw-   0        0        0      279 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_overlay.sphere_nodes.person_sphere_node.rst
--rw-rw-rw-   0        0        0      502 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_overlay.sphere_nodes.rst
--rw-rw-rw-   0        0        0     1563 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_universe_base.rst
--rw-rw-rw-   0        0        0      226 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_universe_base.suv_calc.rst
--rw-rw-rw-   0        0        0      223 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_universe_base.suv_cam.rst
--rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_universe_base.suv_cam_movement.rst
--rw-rw-rw-   0        0        0      241 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_universe_base.suv_clipboard.rst
--rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_universe_base.suv_config.rst
--rw-rw-rw-   0        0        0      241 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_universe_base.suv_constants.rst
--rw-rw-rw-   0        0        0      243 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_universe_base.suv_edge_drag.rst
--rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_disc.rst
--rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_edge.rst
--rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_item.rst
--rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_node.rst
--rw-rw-rw-   0        0        0      258 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_socket.rst
--rw-rw-rw-   0        0        0      235 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_universe_base.suv_history.rst
--rw-rw-rw-   0        0        0      243 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_universe_base.suv_mouse_ray.rst
--rw-rw-rw-   0        0        0      226 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_universe_base.suv_node.rst
--rw-rw-rw-   0        0        0      249 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_universe_base.suv_rubber_band.rst
--rw-rw-rw-   0        0        0      250 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_universe_base.suv_serializable.rst
--rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_universe_base.suv_skybox.rst
--rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_universe_base.suv_socket.rst
--rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_universe_base.suv_sphere.rst
--rw-rw-rw-   0        0        0      249 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_universe_base.suv_sphere_edge.rst
--rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_universe_base.suv_surface_edge.rst
--rw-rw-rw-   0        0        0      238 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_universe_base.suv_universe.rst
--rw-rw-rw-   0        0        0      229 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_universe_base.suv_utils.rst
--rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_universe_base.suv_widget.rst
--rw-rw-rw-   0        0        0      127 2023-03-15 17:49:53.000000 sphere_base-0.1.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 08:51:17.418788 sphere_base-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1574 2023-04-21 08:10:33.000000 sphere_base-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:51:17.085769 sphere_base-0.1.2/sphere_base/
--rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.2/sphere_base/__init__.py
--rw-rw-rw-   0        0        0     8512 2023-04-20 14:05:18.000000 sphere_base-0.1.2/sphere_base/calc.py
--rw-rw-rw-   0        0        0     6909 2023-04-15 10:13:03.000000 sphere_base-0.1.2/sphere_base/clipboard.py
--rw-rw-rw-   0        0        0     5078 2023-04-14 08:50:15.000000 sphere_base-0.1.2/sphere_base/config.py
--rw-rw-rw-   0        0        0     4839 2023-04-20 17:12:04.000000 sphere_base-0.1.2/sphere_base/constants.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:51:17.181775 sphere_base-0.1.2/sphere_base/edge/
--rw-rw-rw-   0        0        0        0 2023-03-30 07:32:40.000000 sphere_base-0.1.2/sphere_base/edge/__init__.py
--rw-rw-rw-   0        0        0     7711 2023-04-20 09:15:29.000000 sphere_base-0.1.2/sphere_base/edge/edge_drag.py
--rw-rw-rw-   0        0        0     4592 2023-04-20 07:51:22.000000 sphere_base-0.1.2/sphere_base/edge/graphic_edge.py
--rw-rw-rw-   0        0        0      809 2023-04-19 12:36:22.000000 sphere_base-0.1.2/sphere_base/edge/graphic_line.py
--rw-rw-rw-   0        0        0     1859 2023-04-04 08:07:28.000000 sphere_base-0.1.2/sphere_base/edge/inter_sphere_edge.py
--rw-rw-rw-   0        0        0    14119 2023-04-20 17:33:34.000000 sphere_base-0.1.2/sphere_base/edge/surface_edge.py
--rw-rw-rw-   0        0        0     9835 2023-04-08 12:55:07.000000 sphere_base-0.1.2/sphere_base/history.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:51:17.239778 sphere_base-0.1.2/sphere_base/model/
--rw-rw-rw-   0        0        0      258 2021-03-02 15:14:54.000000 sphere_base-0.1.2/sphere_base/model/__init__.py
--rw-rw-rw-   0        0        0     4197 2023-04-20 17:16:58.000000 sphere_base-0.1.2/sphere_base/model/mesh.py
--rw-rw-rw-   0        0        0     6393 2023-04-20 17:27:51.000000 sphere_base-0.1.2/sphere_base/model/model.py
--rw-rw-rw-   0        0        0     3318 2023-04-04 11:04:51.000000 sphere_base-0.1.2/sphere_base/model/models.py
--rw-rw-rw-   0        0        0    23063 2023-04-21 06:52:17.000000 sphere_base-0.1.2/sphere_base/model/obj_file_loader.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:51:17.241778 sphere_base-0.1.2/sphere_base/model/resources/
--rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.2/sphere_base/model/resources/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:51:17.242778 sphere_base-0.1.2/sphere_base/model/resources/icons/
--rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.2/sphere_base/model/resources/icons/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:51:17.244778 sphere_base-0.1.2/sphere_base/model/resources/images/
--rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.2/sphere_base/model/resources/images/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:51:17.245778 sphere_base-0.1.2/sphere_base/model/resources/meshes/
--rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.2/sphere_base/model/resources/meshes/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:51:17.246778 sphere_base-0.1.2/sphere_base/model/resources/shaders/
--rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.2/sphere_base/model/resources/shaders/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:51:17.247779 sphere_base-0.1.2/sphere_base/model/resources/sphere_textures/
--rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.2/sphere_base/model/resources/sphere_textures/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:51:17.248778 sphere_base-0.1.2/sphere_base/model/resources/textures/
--rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.2/sphere_base/model/resources/textures/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:51:17.260779 sphere_base-0.1.2/sphere_base/node/
--rw-rw-rw-   0        0        0        0 2023-03-30 07:35:09.000000 sphere_base-0.1.2/sphere_base/node/__init__.py
--rw-rw-rw-   0        0        0     8018 2023-04-03 06:31:17.000000 sphere_base-0.1.2/sphere_base/node/graphic_disc.py
--rw-rw-rw-   0        0        0     2676 2023-04-03 06:31:17.000000 sphere_base-0.1.2/sphere_base/node/graphic_node.py
--rw-rw-rw-   0        0        0     2449 2023-04-03 06:31:16.000000 sphere_base-0.1.2/sphere_base/node/graphic_socket.py
--rw-rw-rw-   0        0        0    13282 2023-04-20 17:22:13.000000 sphere_base-0.1.2/sphere_base/node/node.py
--rw-rw-rw-   0        0        0     8797 2023-04-13 12:16:43.000000 sphere_base-0.1.2/sphere_base/node/socket.py
--rw-rw-rw-   0        0        0     1737 2023-03-30 07:13:13.000000 sphere_base-0.1.2/sphere_base/serializable.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:51:17.344784 sphere_base-0.1.2/sphere_base/shader/
--rw-rw-rw-   0        0        0      258 2021-03-02 15:14:54.000000 sphere_base-0.1.2/sphere_base/shader/__init__.py
--rw-rw-rw-   0        0        0     9085 2023-04-20 17:12:04.000000 sphere_base-0.1.2/sphere_base/shader/base_shader.py
--rw-rw-rw-   0        0        0     1979 2023-04-20 17:16:57.000000 sphere_base-0.1.2/sphere_base/shader/circle_shader.py
--rw-rw-rw-   0        0        0     1969 2023-04-20 17:16:57.000000 sphere_base-0.1.2/sphere_base/shader/cross_shader.py
--rw-rw-rw-   0        0        0      572 2023-03-30 09:23:40.000000 sphere_base-0.1.2/sphere_base/shader/default_shader.py
--rw-rw-rw-   0        0        0     2235 2023-04-20 09:28:14.000000 sphere_base-0.1.2/sphere_base/shader/drag_edge_shader.py
--rw-rw-rw-   0        0        0     1164 2023-04-20 17:31:03.000000 sphere_base-0.1.2/sphere_base/shader/edge_shader.py
--rw-rw-rw-   0        0        0      909 2023-04-20 17:16:58.000000 sphere_base-0.1.2/sphere_base/shader/flat_shader.py
--rw-rw-rw-   0        0        0     1467 2023-04-20 17:16:57.000000 sphere_base-0.1.2/sphere_base/shader/holo_sphere_shader.py
--rw-rw-rw-   0        0        0     1166 2023-04-20 17:16:57.000000 sphere_base-0.1.2/sphere_base/shader/node_shader.py
--rw-rw-rw-   0        0        0     2150 2023-04-20 17:12:04.000000 sphere_base-0.1.2/sphere_base/shader/skybox_shader.py
--rw-rw-rw-   0        0        0     1261 2023-04-20 17:16:58.000000 sphere_base-0.1.2/sphere_base/shader/socket_shader.py
--rw-rw-rw-   0        0        0     3117 2023-04-20 17:31:03.000000 sphere_base-0.1.2/sphere_base/shader/sphere_edge_shader.py
--rw-rw-rw-   0        0        0     1668 2023-04-20 17:16:58.000000 sphere_base-0.1.2/sphere_base/shader/sphere_shader.py
--rw-rw-rw-   0        0        0     1254 2023-04-20 17:16:58.000000 sphere_base-0.1.2/sphere_base/shader/sphere_small_shader.py
--rw-rw-rw-   0        0        0     1845 2023-04-20 17:16:58.000000 sphere_base-0.1.2/sphere_base/shader/square_shader.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:51:17.347784 sphere_base-0.1.2/sphere_base/sphere/
--rw-rw-rw-   0        0        0        0 2023-03-28 18:59:07.000000 sphere_base-0.1.2/sphere_base/sphere/__init__.py
--rw-rw-rw-   0        0        0    28884 2023-04-21 06:53:52.000000 sphere_base-0.1.2/sphere_base/sphere/sphere.py
--rw-rw-rw-   0        0        0     6068 2023-04-21 07:05:58.000000 sphere_base-0.1.2/sphere_base/sphere/sphere_lines.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:51:17.399787 sphere_base-0.1.2/sphere_base/sphere_overlay/
--rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.2/sphere_base/sphere_overlay/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:51:17.400787 sphere_base-0.1.2/sphere_base/sphere_overlay/icons/
--rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.2/sphere_base/sphere_overlay/icons/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:51:17.402787 sphere_base-0.1.2/sphere_base/sphere_overlay/qss/
--rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.2/sphere_base/sphere_overlay/qss/__init__.py
--rw-rw-rw-   0        0        0    30464 2021-01-18 11:54:48.000000 sphere_base-0.1.2/sphere_base/sphere_overlay/qss/nodeeditor_dark_resources.py
--rw-rw-rw-   0        0        0     1875 2023-03-28 18:59:36.000000 sphere_base-0.1.2/sphere_base/sphere_overlay/sov_conf.py
--rw-rw-rw-   0        0        0     2161 2023-04-20 13:43:23.000000 sphere_base-0.1.2/sphere_base/sphere_overlay/sov_sphere.py
--rw-rw-rw-   0        0        0     1598 2023-04-13 12:14:08.000000 sphere_base-0.1.2/sphere_base/sphere_overlay/sov_sphere_node_base.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:51:17.406787 sphere_base-0.1.2/sphere_base/sphere_overlay/sphere_nodes/
--rw-rw-rw-   0        0        0      248 2021-03-02 15:18:12.000000 sphere_base-0.1.2/sphere_base/sphere_overlay/sphere_nodes/__init__.py
--rw-rw-rw-   0        0        0      460 2023-04-04 13:53:39.000000 sphere_base-0.1.2/sphere_base/sphere_overlay/sphere_nodes/edge_sphere_item.py
--rw-rw-rw-   0        0        0     1084 2023-04-13 12:16:43.000000 sphere_base-0.1.2/sphere_base/sphere_overlay/sphere_nodes/item_sphere_node.py
--rw-rw-rw-   0        0        0     1002 2023-04-13 12:14:08.000000 sphere_base-0.1.2/sphere_base/sphere_overlay/sphere_nodes/person_sphere_node.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:51:17.415788 sphere_base-0.1.2/sphere_base/sphere_universe_base/
--rw-rw-rw-   0        0        0       23 2021-03-11 14:37:00.000000 sphere_base-0.1.2/sphere_base/sphere_universe_base/__init__.py
--rw-rw-rw-   0        0        0     7829 2023-04-15 12:02:34.000000 sphere_base-0.1.2/sphere_base/sphere_universe_base/suv_cam.py
--rw-rw-rw-   0        0        0     3434 2023-04-15 11:53:42.000000 sphere_base-0.1.2/sphere_base/sphere_universe_base/suv_cam_movement.py
--rw-rw-rw-   0        0        0      365 2023-03-28 18:59:36.000000 sphere_base-0.1.2/sphere_base/sphere_universe_base/suv_graphic_item.py
--rw-rw-rw-   0        0        0    15874 2023-04-14 08:50:15.000000 sphere_base-0.1.2/sphere_base/sphere_universe_base/suv_mouse_ray.py
--rw-rw-rw-   0        0        0     7211 2023-04-14 09:13:08.000000 sphere_base-0.1.2/sphere_base/sphere_universe_base/suv_rubber_band.py
--rw-rw-rw-   0        0        0     5392 2023-03-28 18:59:36.000000 sphere_base-0.1.2/sphere_base/sphere_universe_base/suv_skybox.py
--rw-rw-rw-   0        0        0    14026 2023-04-14 08:50:15.000000 sphere_base-0.1.2/sphere_base/sphere_universe_base/suv_universe.py
--rw-rw-rw-   0        0        0    17954 2023-04-20 15:39:40.000000 sphere_base-0.1.2/sphere_base/sphere_universe_base/suv_widget.py
--rw-rw-rw-   0        0        0     1494 2023-03-30 07:18:00.000000 sphere_base-0.1.2/sphere_base/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:51:17.148773 sphere_base-0.1.2/sphere_base.egg-info/
--rw-rw-rw-   0        0        0     1987 2023-04-21 08:51:16.000000 sphere_base-0.1.2/sphere_base.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6579 2023-04-21 08:51:16.000000 sphere_base-0.1.2/sphere_base.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 08:51:16.000000 sphere_base-0.1.2/sphere_base.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-16 07:34:46.000000 sphere_base-0.1.2/sphere_base.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      119 2023-04-21 08:51:16.000000 sphere_base-0.1.2/sphere_base.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-21 08:51:16.000000 sphere_base-0.1.2/sphere_base.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-21 08:51:17.416788 sphere_base-0.1.2/tests/
--rw-rw-rw-   0        0        0      530 2023-03-15 14:00:41.000000 sphere_base-0.1.2/tests/test_000_import.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:00:59.511082 sphere_base-0.1.3/
+-rw-rw-rw-   0        0        0      978 2023-04-16 07:19:30.000000 sphere_base-0.1.3/HISTORY.rst
+-rw-rw-rw-   0        0        0     1105 2023-04-16 08:54:46.000000 sphere_base-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      252 2023-03-15 14:22:33.000000 sphere_base-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1987 2023-04-21 09:00:59.510082 sphere_base-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1205 2023-04-21 08:51:12.000000 sphere_base-0.1.3/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-21 09:00:59.286069 sphere_base-0.1.3/docs/
+-rw-rw-rw-   0        0        0      638 2023-03-15 17:55:12.000000 sphere_base-0.1.3/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-04-21 09:00:59.241067 sphere_base-0.1.3/docs/build/
+drwxrwxrwx   0        0        0        0 2023-04-21 09:00:59.241067 sphere_base-0.1.3/docs/build/html/
+drwxrwxrwx   0        0        0        0 2023-04-21 09:00:59.290069 sphere_base-0.1.3/docs/build/html/_static/
+-rw-rw-rw-   0        0        0      286 2023-03-15 17:53:40.000000 sphere_base-0.1.3/docs/build/html/_static/file.png
+-rw-rw-rw-   0        0        0       90 2023-03-15 17:53:40.000000 sphere_base-0.1.3/docs/build/html/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2023-03-15 17:53:40.000000 sphere_base-0.1.3/docs/build/html/_static/plus.png
+-rwxrwxrwx   0        0        0      804 2023-03-15 17:55:12.000000 sphere_base-0.1.3/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-04-21 09:00:59.293069 sphere_base-0.1.3/docs/source/
+-rw-rw-rw-   0        0        0     1175 2023-03-16 20:29:33.000000 sphere_base-0.1.3/docs/source/conf.py
+-rw-rw-rw-   0        0        0      489 2023-03-16 21:15:47.000000 sphere_base-0.1.3/docs/source/index.rst
+drwxrwxrwx   0        0        0        0 2023-04-21 09:00:59.364074 sphere_base-0.1.3/docs/source/rst/
+-rw-rw-rw-   0        0        0      163 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.model.mesh.rst
+-rw-rw-rw-   0        0        0      166 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.model.model.rst
+-rw-rw-rw-   0        0        0      169 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.model.models.rst
+-rw-rw-rw-   0        0        0      200 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.model.obj_file_loader.rst
+-rw-rw-rw-   0        0        0      369 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.model.rst
+-rw-rw-rw-   0        0        0      196 2023-03-16 21:18:48.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.rst
+-rw-rw-rw-   0        0        0      780 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.shader.rst
+-rw-rw-rw-   0        0        0      200 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.shader.uv_base_shader.rst
+-rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.shader.uv_circle_shader.rst
+-rw-rw-rw-   0        0        0      203 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.shader.uv_cross_shader.rst
+-rw-rw-rw-   0        0        0      209 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.shader.uv_default_shader.rst
+-rw-rw-rw-   0        0        0      200 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.shader.uv_flat_shader.rst
+-rw-rw-rw-   0        0        0      223 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.shader.uv_holo_sphere_shader.rst
+-rw-rw-rw-   0        0        0      200 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.shader.uv_node_shader.rst
+-rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.shader.uv_skybox_shader.rst
+-rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.shader.uv_socket_shader.rst
+-rw-rw-rw-   0        0        0      223 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.shader.uv_sphere_edge_shader.rst
+-rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.shader.uv_sphere_shader.rst
+-rw-rw-rw-   0        0        0      226 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.shader.uv_sphere_small_shader.rst
+-rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.shader.uv_square_shader.rst
+-rw-rw-rw-   0        0        0      602 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_overlay.rst
+-rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_overlay.sov_conf.rst
+-rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_overlay.sov_edge.rst
+-rw-rw-rw-   0        0        0      212 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_overlay.sov_sphere.rst
+-rw-rw-rw-   0        0        0      246 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_overlay.sov_sphere_node_base.rst
+-rw-rw-rw-   0        0        0      223 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_overlay.sov_uv_widget.rst
+-rw-rw-rw-   0        0        0      273 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_overlay.sphere_nodes.edge_sphere_item.rst
+-rw-rw-rw-   0        0        0      273 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_overlay.sphere_nodes.item_sphere_node.rst
+-rw-rw-rw-   0        0        0      279 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_overlay.sphere_nodes.person_sphere_node.rst
+-rw-rw-rw-   0        0        0      502 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_overlay.sphere_nodes.rst
+-rw-rw-rw-   0        0        0     1563 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_universe_base.rst
+-rw-rw-rw-   0        0        0      226 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_universe_base.suv_calc.rst
+-rw-rw-rw-   0        0        0      223 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_universe_base.suv_cam.rst
+-rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_universe_base.suv_cam_movement.rst
+-rw-rw-rw-   0        0        0      241 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_universe_base.suv_clipboard.rst
+-rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_universe_base.suv_config.rst
+-rw-rw-rw-   0        0        0      241 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_universe_base.suv_constants.rst
+-rw-rw-rw-   0        0        0      243 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_universe_base.suv_edge_drag.rst
+-rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_disc.rst
+-rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_edge.rst
+-rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_item.rst
+-rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_node.rst
+-rw-rw-rw-   0        0        0      258 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_socket.rst
+-rw-rw-rw-   0        0        0      235 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_universe_base.suv_history.rst
+-rw-rw-rw-   0        0        0      243 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_universe_base.suv_mouse_ray.rst
+-rw-rw-rw-   0        0        0      226 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_universe_base.suv_node.rst
+-rw-rw-rw-   0        0        0      249 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_universe_base.suv_rubber_band.rst
+-rw-rw-rw-   0        0        0      250 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_universe_base.suv_serializable.rst
+-rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_universe_base.suv_skybox.rst
+-rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_universe_base.suv_socket.rst
+-rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_universe_base.suv_sphere.rst
+-rw-rw-rw-   0        0        0      249 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_universe_base.suv_sphere_edge.rst
+-rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_universe_base.suv_surface_edge.rst
+-rw-rw-rw-   0        0        0      238 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_universe_base.suv_universe.rst
+-rw-rw-rw-   0        0        0      229 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_universe_base.suv_utils.rst
+-rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_universe_base.suv_widget.rst
+-rw-rw-rw-   0        0        0      127 2023-03-15 17:49:53.000000 sphere_base-0.1.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 09:00:59.511082 sphere_base-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1574 2023-04-21 09:00:50.000000 sphere_base-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:00:59.372074 sphere_base-0.1.3/sphere_base/
+-rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.3/sphere_base/__init__.py
+-rw-rw-rw-   0        0        0     8512 2023-04-20 14:05:18.000000 sphere_base-0.1.3/sphere_base/calc.py
+-rw-rw-rw-   0        0        0     6909 2023-04-15 10:13:03.000000 sphere_base-0.1.3/sphere_base/clipboard.py
+-rw-rw-rw-   0        0        0     5078 2023-04-14 08:50:15.000000 sphere_base-0.1.3/sphere_base/config.py
+-rw-rw-rw-   0        0        0     4839 2023-04-20 17:12:04.000000 sphere_base-0.1.3/sphere_base/constants.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:00:59.435078 sphere_base-0.1.3/sphere_base/edge/
+-rw-rw-rw-   0        0        0        0 2023-03-30 07:32:40.000000 sphere_base-0.1.3/sphere_base/edge/__init__.py
+-rw-rw-rw-   0        0        0     7711 2023-04-20 09:15:29.000000 sphere_base-0.1.3/sphere_base/edge/edge_drag.py
+-rw-rw-rw-   0        0        0     4592 2023-04-20 07:51:22.000000 sphere_base-0.1.3/sphere_base/edge/graphic_edge.py
+-rw-rw-rw-   0        0        0      809 2023-04-19 12:36:22.000000 sphere_base-0.1.3/sphere_base/edge/graphic_line.py
+-rw-rw-rw-   0        0        0     1859 2023-04-04 08:07:28.000000 sphere_base-0.1.3/sphere_base/edge/inter_sphere_edge.py
+-rw-rw-rw-   0        0        0    14119 2023-04-20 17:33:34.000000 sphere_base-0.1.3/sphere_base/edge/surface_edge.py
+-rw-rw-rw-   0        0        0     9835 2023-04-08 12:55:07.000000 sphere_base-0.1.3/sphere_base/history.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:00:59.441078 sphere_base-0.1.3/sphere_base/model/
+-rw-rw-rw-   0        0        0      258 2021-03-02 15:14:54.000000 sphere_base-0.1.3/sphere_base/model/__init__.py
+-rw-rw-rw-   0        0        0     4197 2023-04-20 17:16:58.000000 sphere_base-0.1.3/sphere_base/model/mesh.py
+-rw-rw-rw-   0        0        0     6393 2023-04-20 17:27:51.000000 sphere_base-0.1.3/sphere_base/model/model.py
+-rw-rw-rw-   0        0        0     3318 2023-04-04 11:04:51.000000 sphere_base-0.1.3/sphere_base/model/models.py
+-rw-rw-rw-   0        0        0    23063 2023-04-21 06:52:17.000000 sphere_base-0.1.3/sphere_base/model/obj_file_loader.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:00:59.442078 sphere_base-0.1.3/sphere_base/model/resources/
+-rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.3/sphere_base/model/resources/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:00:59.443078 sphere_base-0.1.3/sphere_base/model/resources/icons/
+-rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.3/sphere_base/model/resources/icons/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:00:59.444078 sphere_base-0.1.3/sphere_base/model/resources/images/
+-rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.3/sphere_base/model/resources/images/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:00:59.445078 sphere_base-0.1.3/sphere_base/model/resources/meshes/
+-rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.3/sphere_base/model/resources/meshes/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:00:59.446078 sphere_base-0.1.3/sphere_base/model/resources/shaders/
+-rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.3/sphere_base/model/resources/shaders/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:00:59.448078 sphere_base-0.1.3/sphere_base/model/resources/sphere_textures/
+-rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.3/sphere_base/model/resources/sphere_textures/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:00:59.449078 sphere_base-0.1.3/sphere_base/model/resources/textures/
+-rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.3/sphere_base/model/resources/textures/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:00:59.450079 sphere_base-0.1.3/sphere_base/model/resources/textures/skybox/
+-rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.3/sphere_base/model/resources/textures/skybox/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:00:59.451079 sphere_base-0.1.3/sphere_base/model/resources/textures/skybox/blue1/
+-rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.3/sphere_base/model/resources/textures/skybox/blue1/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:00:59.459079 sphere_base-0.1.3/sphere_base/node/
+-rw-rw-rw-   0        0        0        0 2023-03-30 07:35:09.000000 sphere_base-0.1.3/sphere_base/node/__init__.py
+-rw-rw-rw-   0        0        0     8018 2023-04-03 06:31:17.000000 sphere_base-0.1.3/sphere_base/node/graphic_disc.py
+-rw-rw-rw-   0        0        0     2676 2023-04-03 06:31:17.000000 sphere_base-0.1.3/sphere_base/node/graphic_node.py
+-rw-rw-rw-   0        0        0     2449 2023-04-03 06:31:16.000000 sphere_base-0.1.3/sphere_base/node/graphic_socket.py
+-rw-rw-rw-   0        0        0    13282 2023-04-20 17:22:13.000000 sphere_base-0.1.3/sphere_base/node/node.py
+-rw-rw-rw-   0        0        0     8797 2023-04-13 12:16:43.000000 sphere_base-0.1.3/sphere_base/node/socket.py
+-rw-rw-rw-   0        0        0     1737 2023-03-30 07:13:13.000000 sphere_base-0.1.3/sphere_base/serializable.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:00:59.477080 sphere_base-0.1.3/sphere_base/shader/
+-rw-rw-rw-   0        0        0      258 2021-03-02 15:14:54.000000 sphere_base-0.1.3/sphere_base/shader/__init__.py
+-rw-rw-rw-   0        0        0     9085 2023-04-20 17:12:04.000000 sphere_base-0.1.3/sphere_base/shader/base_shader.py
+-rw-rw-rw-   0        0        0     1979 2023-04-20 17:16:57.000000 sphere_base-0.1.3/sphere_base/shader/circle_shader.py
+-rw-rw-rw-   0        0        0     1969 2023-04-20 17:16:57.000000 sphere_base-0.1.3/sphere_base/shader/cross_shader.py
+-rw-rw-rw-   0        0        0      572 2023-03-30 09:23:40.000000 sphere_base-0.1.3/sphere_base/shader/default_shader.py
+-rw-rw-rw-   0        0        0     2235 2023-04-20 09:28:14.000000 sphere_base-0.1.3/sphere_base/shader/drag_edge_shader.py
+-rw-rw-rw-   0        0        0     1164 2023-04-20 17:31:03.000000 sphere_base-0.1.3/sphere_base/shader/edge_shader.py
+-rw-rw-rw-   0        0        0      909 2023-04-20 17:16:58.000000 sphere_base-0.1.3/sphere_base/shader/flat_shader.py
+-rw-rw-rw-   0        0        0     1467 2023-04-20 17:16:57.000000 sphere_base-0.1.3/sphere_base/shader/holo_sphere_shader.py
+-rw-rw-rw-   0        0        0     1166 2023-04-20 17:16:57.000000 sphere_base-0.1.3/sphere_base/shader/node_shader.py
+-rw-rw-rw-   0        0        0     2150 2023-04-20 17:12:04.000000 sphere_base-0.1.3/sphere_base/shader/skybox_shader.py
+-rw-rw-rw-   0        0        0     1261 2023-04-20 17:16:58.000000 sphere_base-0.1.3/sphere_base/shader/socket_shader.py
+-rw-rw-rw-   0        0        0     3117 2023-04-20 17:31:03.000000 sphere_base-0.1.3/sphere_base/shader/sphere_edge_shader.py
+-rw-rw-rw-   0        0        0     1668 2023-04-20 17:16:58.000000 sphere_base-0.1.3/sphere_base/shader/sphere_shader.py
+-rw-rw-rw-   0        0        0     1254 2023-04-20 17:16:58.000000 sphere_base-0.1.3/sphere_base/shader/sphere_small_shader.py
+-rw-rw-rw-   0        0        0     1845 2023-04-20 17:16:58.000000 sphere_base-0.1.3/sphere_base/shader/square_shader.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:00:59.482080 sphere_base-0.1.3/sphere_base/sphere/
+-rw-rw-rw-   0        0        0        0 2023-03-28 18:59:07.000000 sphere_base-0.1.3/sphere_base/sphere/__init__.py
+-rw-rw-rw-   0        0        0    28884 2023-04-21 06:53:52.000000 sphere_base-0.1.3/sphere_base/sphere/sphere.py
+-rw-rw-rw-   0        0        0     6068 2023-04-21 07:05:58.000000 sphere_base-0.1.3/sphere_base/sphere/sphere_lines.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:00:59.488081 sphere_base-0.1.3/sphere_base/sphere_overlay/
+-rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.3/sphere_base/sphere_overlay/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:00:59.489081 sphere_base-0.1.3/sphere_base/sphere_overlay/icons/
+-rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.3/sphere_base/sphere_overlay/icons/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:00:59.492081 sphere_base-0.1.3/sphere_base/sphere_overlay/qss/
+-rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.3/sphere_base/sphere_overlay/qss/__init__.py
+-rw-rw-rw-   0        0        0    30464 2021-01-18 11:54:48.000000 sphere_base-0.1.3/sphere_base/sphere_overlay/qss/nodeeditor_dark_resources.py
+-rw-rw-rw-   0        0        0     1875 2023-03-28 18:59:36.000000 sphere_base-0.1.3/sphere_base/sphere_overlay/sov_conf.py
+-rw-rw-rw-   0        0        0     2161 2023-04-20 13:43:23.000000 sphere_base-0.1.3/sphere_base/sphere_overlay/sov_sphere.py
+-rw-rw-rw-   0        0        0     1598 2023-04-13 12:14:08.000000 sphere_base-0.1.3/sphere_base/sphere_overlay/sov_sphere_node_base.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:00:59.497081 sphere_base-0.1.3/sphere_base/sphere_overlay/sphere_nodes/
+-rw-rw-rw-   0        0        0      248 2021-03-02 15:18:12.000000 sphere_base-0.1.3/sphere_base/sphere_overlay/sphere_nodes/__init__.py
+-rw-rw-rw-   0        0        0      460 2023-04-04 13:53:39.000000 sphere_base-0.1.3/sphere_base/sphere_overlay/sphere_nodes/edge_sphere_item.py
+-rw-rw-rw-   0        0        0     1084 2023-04-13 12:16:43.000000 sphere_base-0.1.3/sphere_base/sphere_overlay/sphere_nodes/item_sphere_node.py
+-rw-rw-rw-   0        0        0     1002 2023-04-13 12:14:08.000000 sphere_base-0.1.3/sphere_base/sphere_overlay/sphere_nodes/person_sphere_node.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:00:59.508082 sphere_base-0.1.3/sphere_base/sphere_universe_base/
+-rw-rw-rw-   0        0        0       23 2021-03-11 14:37:00.000000 sphere_base-0.1.3/sphere_base/sphere_universe_base/__init__.py
+-rw-rw-rw-   0        0        0     7829 2023-04-15 12:02:34.000000 sphere_base-0.1.3/sphere_base/sphere_universe_base/suv_cam.py
+-rw-rw-rw-   0        0        0     3434 2023-04-15 11:53:42.000000 sphere_base-0.1.3/sphere_base/sphere_universe_base/suv_cam_movement.py
+-rw-rw-rw-   0        0        0      365 2023-03-28 18:59:36.000000 sphere_base-0.1.3/sphere_base/sphere_universe_base/suv_graphic_item.py
+-rw-rw-rw-   0        0        0    15874 2023-04-14 08:50:15.000000 sphere_base-0.1.3/sphere_base/sphere_universe_base/suv_mouse_ray.py
+-rw-rw-rw-   0        0        0     7211 2023-04-14 09:13:08.000000 sphere_base-0.1.3/sphere_base/sphere_universe_base/suv_rubber_band.py
+-rw-rw-rw-   0        0        0     5392 2023-03-28 18:59:36.000000 sphere_base-0.1.3/sphere_base/sphere_universe_base/suv_skybox.py
+-rw-rw-rw-   0        0        0    14026 2023-04-14 08:50:15.000000 sphere_base-0.1.3/sphere_base/sphere_universe_base/suv_universe.py
+-rw-rw-rw-   0        0        0    17954 2023-04-20 15:39:40.000000 sphere_base-0.1.3/sphere_base/sphere_universe_base/suv_widget.py
+-rw-rw-rw-   0        0        0     1494 2023-03-30 07:18:00.000000 sphere_base-0.1.3/sphere_base/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:00:59.394075 sphere_base-0.1.3/sphere_base.egg-info/
+-rw-rw-rw-   0        0        0     1987 2023-04-21 09:00:59.000000 sphere_base-0.1.3/sphere_base.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6697 2023-04-21 09:00:59.000000 sphere_base-0.1.3/sphere_base.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 09:00:59.000000 sphere_base-0.1.3/sphere_base.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-16 07:34:46.000000 sphere_base-0.1.3/sphere_base.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      119 2023-04-21 09:00:59.000000 sphere_base-0.1.3/sphere_base.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-21 09:00:59.000000 sphere_base-0.1.3/sphere_base.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 09:00:59.509082 sphere_base-0.1.3/tests/
+-rw-rw-rw-   0        0        0      530 2023-03-15 14:00:41.000000 sphere_base-0.1.3/tests/test_000_import.py
```

### Comparing `sphere_base-0.1.2/HISTORY.rst` & `sphere_base-0.1.3/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.2/LICENSE` & `sphere_base-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.2/PKG-INFO` & `sphere_base-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphere_base
-Version: 0.1.2
+Version: 0.1.3
 Summary: library for applications were information should appear on the surface of a sphere. It allows for creating spheres with nodes and edges that can be dragged on its surface. 
 Home-page: https://github.com/rboltze/spherebase
 Author: Richard Boltze
 Author-email: rboltze@protonmail.com
 License: MIT license
 Keywords: sphere_base
 Classifier: Development Status :: 4 - Beta
```

### Comparing `sphere_base-0.1.2/README.rst` & `sphere_base-0.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.2/docs/Makefile` & `sphere_base-0.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.2/docs/make.bat` & `sphere_base-0.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.2/docs/source/conf.py` & `sphere_base-0.1.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.2/docs/source/rst/sphere_base.shader.rst` & `sphere_base-0.1.3/docs/source/rst/sphere_base.shader.rst`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_overlay.rst` & `sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_overlay.rst`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.2/docs/source/rst/sphere_base.sphere_universe_base.rst` & `sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_universe_base.rst`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.2/setup.py` & `sphere_base-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,10 +40,10 @@
     keywords='sphere_base',
     name='sphere_base',
     packages=find_packages(include=['sphere_base*'], exclude=['examples*', 'test*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/rboltze/spherebase',
-    version='0.1.2',
+    version='0.1.3',
     zip_safe=False,
 )
```

### Comparing `sphere_base-0.1.2/sphere_base/calc.py` & `sphere_base-0.1.3/sphere_base/calc.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.2/sphere_base/clipboard.py` & `sphere_base-0.1.3/sphere_base/clipboard.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.2/sphere_base/config.py` & `sphere_base-0.1.3/sphere_base/config.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.2/sphere_base/constants.py` & `sphere_base-0.1.3/sphere_base/constants.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.2/sphere_base/edge/edge_drag.py` & `sphere_base-0.1.3/sphere_base/edge/edge_drag.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.2/sphere_base/edge/graphic_edge.py` & `sphere_base-0.1.3/sphere_base/edge/graphic_edge.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.2/sphere_base/edge/graphic_line.py` & `sphere_base-0.1.3/sphere_base/edge/graphic_line.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.2/sphere_base/edge/inter_sphere_edge.py` & `sphere_base-0.1.3/sphere_base/edge/inter_sphere_edge.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.2/sphere_base/edge/surface_edge.py` & `sphere_base-0.1.3/sphere_base/edge/surface_edge.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.2/sphere_base/history.py` & `sphere_base-0.1.3/sphere_base/history.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.2/sphere_base/model/mesh.py` & `sphere_base-0.1.3/sphere_base/model/mesh.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.2/sphere_base/model/model.py` & `sphere_base-0.1.3/sphere_base/model/model.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.2/sphere_base/model/models.py` & `sphere_base-0.1.3/sphere_base/model/models.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.2/sphere_base/model/obj_file_loader.py` & `sphere_base-0.1.3/sphere_base/model/obj_file_loader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.2/sphere_base/node/graphic_disc.py` & `sphere_base-0.1.3/sphere_base/node/graphic_disc.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.2/sphere_base/node/graphic_node.py` & `sphere_base-0.1.3/sphere_base/node/graphic_node.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.2/sphere_base/node/graphic_socket.py` & `sphere_base-0.1.3/sphere_base/node/graphic_socket.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.2/sphere_base/node/node.py` & `sphere_base-0.1.3/sphere_base/node/node.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.2/sphere_base/node/socket.py` & `sphere_base-0.1.3/sphere_base/node/socket.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.2/sphere_base/serializable.py` & `sphere_base-0.1.3/sphere_base/serializable.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.2/sphere_base/shader/base_shader.py` & `sphere_base-0.1.3/sphere_base/shader/base_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.2/sphere_base/shader/circle_shader.py` & `sphere_base-0.1.3/sphere_base/shader/circle_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.2/sphere_base/shader/cross_shader.py` & `sphere_base-0.1.3/sphere_base/shader/cross_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.2/sphere_base/shader/default_shader.py` & `sphere_base-0.1.3/sphere_base/shader/default_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.2/sphere_base/shader/drag_edge_shader.py` & `sphere_base-0.1.3/sphere_base/shader/drag_edge_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.2/sphere_base/shader/edge_shader.py` & `sphere_base-0.1.3/sphere_base/shader/edge_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.2/sphere_base/shader/flat_shader.py` & `sphere_base-0.1.3/sphere_base/shader/flat_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.2/sphere_base/shader/holo_sphere_shader.py` & `sphere_base-0.1.3/sphere_base/shader/holo_sphere_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.2/sphere_base/shader/node_shader.py` & `sphere_base-0.1.3/sphere_base/shader/node_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.2/sphere_base/shader/skybox_shader.py` & `sphere_base-0.1.3/sphere_base/shader/skybox_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.2/sphere_base/shader/socket_shader.py` & `sphere_base-0.1.3/sphere_base/shader/socket_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.2/sphere_base/shader/sphere_edge_shader.py` & `sphere_base-0.1.3/sphere_base/shader/sphere_edge_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.2/sphere_base/shader/sphere_shader.py` & `sphere_base-0.1.3/sphere_base/shader/sphere_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.2/sphere_base/shader/sphere_small_shader.py` & `sphere_base-0.1.3/sphere_base/shader/sphere_small_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.2/sphere_base/shader/square_shader.py` & `sphere_base-0.1.3/sphere_base/shader/square_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.2/sphere_base/sphere/sphere.py` & `sphere_base-0.1.3/sphere_base/sphere/sphere.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.2/sphere_base/sphere/sphere_lines.py` & `sphere_base-0.1.3/sphere_base/sphere/sphere_lines.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.2/sphere_base/sphere_overlay/qss/nodeeditor_dark_resources.py` & `sphere_base-0.1.3/sphere_base/sphere_overlay/qss/nodeeditor_dark_resources.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.2/sphere_base/sphere_overlay/sov_conf.py` & `sphere_base-0.1.3/sphere_base/sphere_overlay/sov_conf.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.2/sphere_base/sphere_overlay/sov_sphere.py` & `sphere_base-0.1.3/sphere_base/sphere_overlay/sov_sphere.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.2/sphere_base/sphere_overlay/sov_sphere_node_base.py` & `sphere_base-0.1.3/sphere_base/sphere_overlay/sov_sphere_node_base.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.2/sphere_base/sphere_overlay/sphere_nodes/item_sphere_node.py` & `sphere_base-0.1.3/sphere_base/sphere_overlay/sphere_nodes/item_sphere_node.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.2/sphere_base/sphere_overlay/sphere_nodes/person_sphere_node.py` & `sphere_base-0.1.3/sphere_base/sphere_overlay/sphere_nodes/person_sphere_node.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.2/sphere_base/sphere_universe_base/suv_cam.py` & `sphere_base-0.1.3/sphere_base/sphere_universe_base/suv_cam.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.2/sphere_base/sphere_universe_base/suv_cam_movement.py` & `sphere_base-0.1.3/sphere_base/sphere_universe_base/suv_cam_movement.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.2/sphere_base/sphere_universe_base/suv_mouse_ray.py` & `sphere_base-0.1.3/sphere_base/sphere_universe_base/suv_mouse_ray.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.2/sphere_base/sphere_universe_base/suv_rubber_band.py` & `sphere_base-0.1.3/sphere_base/sphere_universe_base/suv_rubber_band.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.2/sphere_base/sphere_universe_base/suv_skybox.py` & `sphere_base-0.1.3/sphere_base/sphere_universe_base/suv_skybox.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.2/sphere_base/sphere_universe_base/suv_universe.py` & `sphere_base-0.1.3/sphere_base/sphere_universe_base/suv_universe.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.2/sphere_base/sphere_universe_base/suv_widget.py` & `sphere_base-0.1.3/sphere_base/sphere_universe_base/suv_widget.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.2/sphere_base/utils.py` & `sphere_base-0.1.3/sphere_base/utils.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.2/sphere_base.egg-info/PKG-INFO` & `sphere_base-0.1.3/sphere_base.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphere-base
-Version: 0.1.2
+Version: 0.1.3
 Summary: library for applications were information should appear on the surface of a sphere. It allows for creating spheres with nodes and edges that can be dragged on its surface. 
 Home-page: https://github.com/rboltze/spherebase
 Author: Richard Boltze
 Author-email: rboltze@protonmail.com
 License: MIT license
 Keywords: sphere_base
 Classifier: Development Status :: 4 - Beta
```

### Comparing `sphere_base-0.1.2/sphere_base.egg-info/SOURCES.txt` & `sphere_base-0.1.3/sphere_base.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -95,14 +95,16 @@
 sphere_base/model/resources/__init__.py
 sphere_base/model/resources/icons/__init__.py
 sphere_base/model/resources/images/__init__.py
 sphere_base/model/resources/meshes/__init__.py
 sphere_base/model/resources/shaders/__init__.py
 sphere_base/model/resources/sphere_textures/__init__.py
 sphere_base/model/resources/textures/__init__.py
+sphere_base/model/resources/textures/skybox/__init__.py
+sphere_base/model/resources/textures/skybox/blue1/__init__.py
 sphere_base/node/__init__.py
 sphere_base/node/graphic_disc.py
 sphere_base/node/graphic_node.py
 sphere_base/node/graphic_socket.py
 sphere_base/node/node.py
 sphere_base/node/socket.py
 sphere_base/shader/__init__.py
```

### Comparing `sphere_base-0.1.2/tests/test_000_import.py` & `sphere_base-0.1.3/tests/test_000_import.py`

 * *Files identical despite different names*

